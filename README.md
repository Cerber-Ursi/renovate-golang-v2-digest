# 37132

## Context

There's a dependency on a package which uses separate brance for `v2`; this dependency refers to specific commit via digest.

## Current behavior

Renovate tries to update dependency to the latest digest in the `master` branch, leading to broken `go.mod` file.

## Expected behavior

Renovate either updates to the lates digest in `v2` branch, or skips update entirely until a new tagged version is released.

## Link to the Renovate Discussion

[Discussion 37132](https://github.com/renovatebot/renovate/discussions/37132)
