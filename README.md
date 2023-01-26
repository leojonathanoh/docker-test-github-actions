# test-github-actions-calver

[![github-actions](https://github.com/leojonathanoh/test-github-actions-calver/workflows/ci-master-pr/badge.svg)](https://github.com/leojonathanoh/test-github-actions-calver/actions)
[![github-tag](https://img.shields.io/github/tag/leojonathanoh/test-github-actions-calver)](https://github.com/leojonathanoh/test-github-actions-calver/releases/)
[![docker-image-size](https://img.shields.io/docker/image-size/leojonathanoh/test-github-actions-calver/latest)](https://hub.docker.com/r/leojonathanoh/test-github-actions-calver)

Example repository with CalVer (date-based) release workflow.

## Github Workflows

### Build

Trigger: `git push origin master` or PR

- `ci-master-pr`: CI on `master` and PRs. Resolves the next tag in CalVer format `YYYYMMDD.<MINOR>.<PATCH>`, drafts release notes on `master`.

### Releases

#### CalVer (date-based) releases

Trigger: `git checkout release && git merge --no-ff master`.

- `ci-release`: CI on `release`. Resolves the next tag in CalVer format `YYYYMMDD.<MINOR>.<PATCH>`, creates the release, and publishes release notes.

## Useful links

- [CalVer releases](https://github.com/release-drafter/release-drafter/issues/315)
