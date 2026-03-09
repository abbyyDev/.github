# Contributing to AbbyyDev Projects

Thank you for your interest in contributing! We welcome contributions of all kinds — bug fixes, new features, documentation improvements, and more.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [How to Contribute](#how-to-contribute)
- [Pull Request Process](#pull-request-process)
- [Coding Standards](#coding-standards)
- [Reporting Issues](#reporting-issues)

## Code of Conduct

By participating in this project, you agree to abide by our [Code of Conduct](CODE_OF_CONDUCT.md). Please read it before contributing.

## Getting Started

1. **Fork** the repository you want to contribute to.
2. **Clone** your fork locally:
   ```bash
   git clone https://github.com/<your-username>/<repository>.git
   cd <repository>
   ```
3. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Install dependencies** as described in the project's README.

## How to Contribute

### Reporting Bugs

Before creating a bug report, please check existing issues to avoid duplicates. When you create a bug report, include:
- A clear and descriptive title
- Steps to reproduce the problem
- Expected vs. actual behavior
- Environment details (OS, language version, etc.)

Use the [Bug Report template](.github/ISSUE_TEMPLATE/bug_report.md) when opening an issue.

### Suggesting Features

Feature requests are welcome! Use the [Feature Request template](.github/ISSUE_TEMPLATE/feature_request.md) and include:
- A clear description of the problem you're solving
- Your proposed solution
- Any alternatives you've considered

### Submitting Code Changes

1. Ensure your code follows the project's [coding standards](#coding-standards).
2. Add or update tests as appropriate.
3. Update documentation if needed.
4. Commit your changes with a clear, descriptive commit message.

## Pull Request Process

1. **Update the README** or relevant documentation with details of your changes, if applicable.
2. **Ensure all tests pass** before submitting your PR.
3. **Fill out the PR template** completely — incomplete PRs may be delayed.
4. **Request a review** from at least one maintainer.
5. PRs will be merged once approved and all checks pass.

### Commit Message Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short summary>

[optional body]

[optional footer]
```

Types: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

Examples:
- `feat(auth): add OAuth2 login support`
- `fix(api): handle null response from upstream`
- `docs(readme): update installation steps`

## Coding Standards

- Follow the style conventions established in the codebase.
- Write clear, self-documenting code; add comments where logic is non-obvious.
- Ensure new code has adequate test coverage.
- Keep PRs focused — one feature or fix per PR.

## Reporting Issues

If you discover a **security vulnerability**, please do **not** open a public issue. Instead, follow our [Security Policy](SECURITY.md).

For all other issues, use GitHub Issues on the relevant repository and provide as much detail as possible.

---

Thank you for helping make AbbyyDev projects better! 🎉
