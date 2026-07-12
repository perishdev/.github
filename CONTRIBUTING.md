# Contributing

Thanks for your interest in contributing to a [`@perishdev`](https://github.com/perishdev) project! This guide applies org-wide to any repository that does not provide its own `CONTRIBUTING.md`.

By participating, you agree to abide by our [Code of Conduct](./CODE_OF_CONDUCT.md) and our [AI Policy](./AI_POLICY.md).

## Before you start

- **Search first.** Check [open issues](https://github.com/search?q=org%3Aperishdev+state%3Aopen&type=issues) and [discussions](https://github.com/orgs/perishdev/discussions) before opening something new.
- **Open an issue for non-trivial changes.** For anything beyond a typo or small fix, please open an issue (or discussion) first so we can agree on the approach before you invest time.
- **Questions go to Discussions,** not issues — see [SUPPORT.md](./SUPPORT.md).

## Workflow

1. **Fork** the repository and clone your fork.
2. **Create a branch** off `main` following the [Conventional Branch](https://conventional-branch.github.io/) format, e.g. `feature/add-widget`, `fix/null-pointer`, `docs/clarify-setup`.
3. **Make your changes**, keeping commits focused and atomic.
4. **Commit** using the [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/) spec, e.g. `feat: add widget loader` or `fix: handle empty config`.
5. **Open a pull request against `main`.** Title it using the [Conventional Pull Request](https://github.com/marketplace/actions/conventional-pull-request) format (same prefixes as commits) and fill out the PR template.
6. **Link the issue** your PR addresses (e.g. `Closes #123`).

## Naming conventions

| What             | Convention                                                                                   | Example                       |
| ---------------- | -------------------------------------------------------------------------------------------- | ----------------------------- |
| Commit messages  | [Conventional Commits v1.0.0](https://www.conventionalcommits.org/en/v1.0.0/)                 | `feat: add retry backoff`     |
| Branch names     | [Conventional Branch](https://conventional-branch.github.io/)                                 | `fix/timeout-regression`      |
| Pull request title | [Conventional Pull Request action format](https://github.com/marketplace/actions/conventional-pull-request) | `docs: expand contributing guide` |

## Pull request checklist

- [ ] The branch name, commits, and PR title follow the conventions above.
- [ ] Changes are covered by tests where the project has a test suite.
- [ ] Documentation is updated where relevant.
- [ ] The PR description explains **what** changed and **why**, in your own words.

## A note on AI tooling

We welcome AI-assisted development, but you remain responsible for what you submit. Please read the [AI Policy](./AI_POLICY.md) — in short: a human must understand and stand behind every contribution, and comments to maintainers should be written by you, not generated.

---

Thanks again — every contribution, however small, helps. 🌱
