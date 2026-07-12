# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

GitHub's special `.github` repository for the [`@perishdev`](https://github.com/perishdev/) organization. It holds **community health files** and the org **profile page** — there is no application code, no build system, and no test suite. Changes here affect how the org appears on GitHub and how repos in the org inherit defaults.

## Layout

- `profile/README.md` — content rendered on the public org profile page at `github.com/perishdev`.
- Community health files (inherited org-wide — see below):
  - `SECURITY.md` — vulnerability reporting via GitHub private advisories; includes an anti-AI-spam clause.
  - `CODE_OF_CONDUCT.md` — Contributor Covenant 2.0; enforcement contact is `hasansezertasan@gmail.com`.
  - `CONTRIBUTING.md` — workflow, branch policy, and naming conventions.
  - `SUPPORT.md` — routes questions → Discussions, bugs → Issues, vulnerabilities → Security.
  - `AI_POLICY.md` — contributor expectations for AI/LLM use (adapted from Astral, MIT-credited).
- `.github/ISSUE_TEMPLATE/` — issue *forms* (`bug.yml`, `feature.yml`, `docs.yml`) + `config.yml` (blank issues disabled).
- `.github/DISCUSSION_TEMPLATE/questions.yml` — structured discussion template.
- `.github/PULL_REQUEST_TEMPLATE.md` — PR template.
- `.github/CODEOWNERS` — global owner is `@perishdev/maintainers`.
- `.github/release.yml` — config for GitHub's auto-generated release notes (categorized, bots excluded).
- `.github/dependabot.yml` — default Dependabot config (pip + github-actions, monthly, targets the default branch).
- `LICENSE`, `README.md` — repo-level metadata.

## Community health files are inherited org-wide

Files like `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SUPPORT.md`, and the issue/PR/discussion templates are inherited by **every** repo in the org that does not define its own copy. Consequences when editing them here:

- A change here silently changes the default for every other perishdev repo. Consider the blast radius.
- Links inside inherited files must be **absolute** `https://github.com/perishdev/...` URLs, not relative paths — relative links break when GitHub renders the file in another repo's context.
- No funding: `FUNDING.yml` is intentionally omitted (org uses GitHub-only channels).

## Ownership

- `@perishdev/maintainers` is the org maintainers team and the global code owner in `CODEOWNERS`. It has `write` access to this repo (required for a team to be a valid code owner). Sole member: `hasansezertasan`.

## Branch policy

Work happens on short-lived branches off `main`, and pull requests target `main` directly:

```
feature/* → main
```

- Open PRs against `main`.
- Branch names follow the Conventional Branch spec (e.g. `feature/…`, `fix/…`, `docs/…`).
- Dependabot targets the default branch (`main`); no `target-branch` override is set.

## Conventions

- Commit messages: Conventional Commits.
- Branch names: Conventional Branch.
- PR titles: Conventional Pull Request action format.
