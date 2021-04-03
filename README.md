# docker-test-github-actions

[![github-actions](https://github.com/leojonathanoh/docker-test-github-actions/workflows/ci-master-pr/badge.svg)](https://github.com/leojonathanoh/docker-test-github-actions/actions)
[![github-tag](https://img.shields.io/github/tag/leojonathanoh/docker-test-github-actions)](https://github.com/leojonathanoh/docker-test-github-actions/releases/)
[![docker-image-size](https://img.shields.io/docker/image-size/leojonathanoh/docker-test-github-actions/latest)](https://hub.docker.com/r/leojonathanoh/docker-test-github-actions)

Example repository with CalVer (date-based) release workflow.

## Github Workflows

### Build

Trigger: `git push origin master` or PR

- `ci-master-pr`: CI on `master` and PRs.

### Releases

#### CalVer (date-based) releases

Trigger: `git checkout release && git merge --no-ff master`.

- `ci-release`: CI on `release`. Resolves the next tag in CalVer format `YYYYMMDD.<MINOR>.<PATCH>`, creates the release, and publishes release notes.

## Useful links

- [CalVer releases](https://github.com/release-drafter/release-drafter/issues/315)
