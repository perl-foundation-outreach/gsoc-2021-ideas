# Automated Rakudo Star Builds

## Description

Rakudo Star is currently build by hand on every release. This, in conjuction
with a maintainer that doesn't use every OS in existence, causes targets other
than GNU+Linux to be left behind. By leveraging automated builds, whether it be
through GitHub, GitLab, SourceHut or anything else, support for other systems
can be improved and kept up to date much easier.

## Expected Outcomes

- On a push to master, automatically build a distribution tarball for:
  - FreeBSD
  - GNU+Linux (glibc)
  - (nonGNU+)Linux (musl)
  - MacOS
  - OpenBSD
  - Windows
  - NetBSD

Support for each single platform can be seen as a milestone to achieve.

## Required Skills

- Bash
- Git
- GitHub Actions (or equivalent skills on any other platform)
- Familiarity with build tooling of the required platforms

## Rating

Medium

## Possible Mentors

- @tyil
