# Workflows

Contains the `Github Action` workflow files which should be used from other `Hiconic` repositories.

## How to use

This is standard GitHub mechanism for reusing workflows; e.g. a given repository's `pr.yaml` could look like this:

```
name: Pull Requests

on:
  pull_request:

jobs:
  run:
    uses: hiconic-os/hiconic.ci.workflows/.github/workflows/pr.yaml@main
    secrets: inherit
```