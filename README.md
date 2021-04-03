# docker-test-github-actions

[![github-actions](https://github.com/leojonathanoh/docker-test-github-actions/workflows/ci-master-pr/badge.svg)](https://github.com/leojonathanoh/docker-test-github-actions/actions)
[![github-tag](https://img.shields.io/github/tag/leojonathanoh/docker-test-github-actions)](https://github.com/leojonathanoh/docker-test-github-actions/releases/)
[![docker-image-size](https://img.shields.io/docker/image-size/leojonathanoh/docker-test-github-actions/latest)](https://hub.docker.com/r/leojonathanoh/docker-test-github-actions)

Example repository with CalVer (date-based) release workflow.

## Workflows

### Build

Trigger: `git push origin push` or PR

- `ci-master-pr`: CI

### Releases

#### date-based releases

Trigger: `git checkout release && git merge --no-ff master`.

- `ci-release`: CI on branch `elease-tags-date`, ends by tagging its `HEAD` in format: `YYYYMMDD.<MINOR>.<PATCH>`, which will be an official release. Creates the release based on tag `YYYYMMDD.<MINOR>.<PATCH>`, publishing release notes.

## Useful links

- [CalVer releases](https://github.com/release-drafter/release-drafter/issues/315)
