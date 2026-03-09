# AbbyyDev — Central Configuration

This repository contains central configuration, templates, reusable workflows, and the organization profile README for all [AbbyyDev](https://github.com/abbyyDev) repositories.

## Contents

### 📋 Community Health Files

These files apply as defaults across all AbbyyDev repositories:

| File | Description |
|------|-------------|
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Guidelines for contributing to AbbyyDev projects |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) | Community standards and expectations |
| [`SECURITY.md`](SECURITY.md) | How to report security vulnerabilities |

### 📝 Templates

| Template | Description |
|----------|-------------|
| [`.github/ISSUE_TEMPLATE/bug_report.md`](.github/ISSUE_TEMPLATE/bug_report.md) | Template for reporting bugs |
| [`.github/ISSUE_TEMPLATE/feature_request.md`](.github/ISSUE_TEMPLATE/feature_request.md) | Template for requesting new features |
| [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) | Template for pull requests |

### ⚙️ Reusable Workflows

These workflows can be called from any AbbyyDev repository using `workflow_call`.

| Workflow | Description |
|----------|-------------|
| [`.github/workflows/ci.yml`](.github/workflows/ci.yml) | Reusable CI workflow (lint, build, test) |
| [`.github/workflows/release.yml`](.github/workflows/release.yml) | Reusable release workflow (build, test, publish) |

#### Using a Reusable Workflow

```yaml
# In your repository's .github/workflows/ci.yml
jobs:
  ci:
    uses: abbyyDev/.github/.github/workflows/ci.yml@main
    with:
      node-version: '20'
      lint-command: 'npm run lint'
      test-command: 'npm test'
      build-command: 'npm run build'
```

### 🏢 Organization Profile

[`profile/README.md`](profile/README.md) — Displayed on the [AbbyyDev organization page](https://github.com/abbyyDev).

## About `.github` Repositories

A `.github` repository in a GitHub organization serves as a central place for:

- **Default community health files**: Files like `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `SECURITY.md` here apply to all repositories in the organization that don't have their own.
- **Reusable workflows**: GitHub Actions workflows in `.github/workflows/` can be referenced from other repositories.
- **Organization profile**: `profile/README.md` is shown on the organization's GitHub profile page.

For more information, see [GitHub's documentation on default community health files](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).