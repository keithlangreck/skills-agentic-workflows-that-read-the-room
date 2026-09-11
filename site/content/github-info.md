# GitHub Info

## Mona's editorial angle

Mona's website focuses on practical GitHub guidance backed by official references from:

- docs.github.com
- github.blog
- github.blog/changelog

## Current homepage themes

- GitHub collaboration basics: repositories, branches, pull requests, and merges.
- GitHub Copilot as an AI coding assistant across the IDE, CLI, and GitHub.
- GitHub Actions as the automation layer behind repository workflows.
- Recent GitHub Blog and Changelog stories worth watching.

## Recent updates worth watching

- **Refreshed repository pull requests page (public preview)** — a redesigned repo-level PR list with content-assisted filters, advanced search, and a collapsible sidebar, making it faster to triage PRs in busy repos. Source: https://github.blog/changelog/2026-09-10-refreshed-repository-pull-requests-page-in-public-preview
- **Control GitHub Actions cache access with `cache-mode`** — a new setting (read/write/write-only/none) lets workflows apply least-privilege control over the Actions cache, defaulting to read-only for risky triggers like `pull_request_target`. Source: https://github.blog/changelog/2026-09-10-control-github-actions-cache-access-with-cache-mode
- **Block pull requests with exposed secrets from merging** — a new repository ruleset rule stops PRs with unresolved secret scanning alerts from merging, closing a gap left by push protection alone. Source: https://github.blog/changelog/2026-09-09-block-pull-requests-with-exposed-secrets-from-merging
- **Automatic Dependabot access to GitHub-hosted registries** — Dependabot's `GITHUB_TOKEN` can now request read access to `*.pkg.github.com` and `ghcr.io` automatically, removing the need for a manually managed PAT. Source: https://github.blog/changelog/2026-09-08-automatic-dependabot-access-to-github-hosted-registries
- **GitHub CLI: media in issues, pull requests, and comments** — `gh` now supports a repeatable `--attach` flag to upload and embed a local image or video when creating or commenting on issues and PRs from the terminal. Source: https://github.blog/changelog/2026-09-01-github-cli-media-in-issues-pull-requests-and-comments
