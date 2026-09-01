---
name: update-github-info
on:
  schedule: daily
  workflow_dispatch:
permissions: read-all
tools:
  edit: true
  web-fetch: {}
  github:
    toolsets:
      - repos
network:
  allowed:
    - github.blog
    - github.com
    - awesome-copilot.github.com
safe-outputs:
  create-pull-request:
    title-prefix: "[github-info] "
    draft: true
    max: 1
---

# Update GitHub Info

Refresh the GitHub information used by Mona's website.

1. Use GitHub repository API tools to read `notes/mona-notes.md` and `site/content/github-info.md`.
2. Use `web-fetch` to read https://github.blog/latest/, https://github.blog/changelog/, and https://awesome-copilot.github.com/workflows/.
3. Select a small set of recent, practical updates that help developers learn GitHub faster. Keep summaries short, include each official source URL, and preserve the existing Markdown structure unless a small adjustment improves it.
4. Use the `edit` tool to update only `site/content/github-info.md`.
5. Use the `create-pull-request` safe output to open one draft pull request for Mona to review. Include a concise summary of the refreshed updates and source URLs in the pull request body.

Do not write directly to the default branch. Do not modify files other than `site/content/github-info.md`.