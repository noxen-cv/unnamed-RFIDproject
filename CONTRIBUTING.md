# Contributing to unnamed-RFIDproject

Thank you for your interest in contributing to this project! This document outlines the guidelines and rules for contributing.

## Contribution Rules

### Pull Request Requirement

**All changes to the `main` branch must be made through pull requests.** Direct pushes to the `main` branch are not allowed.

This ensures:
- Code review before changes are merged
- Discussion and collaboration on proposed changes
- A clear history of changes and their purposes
- Quality control for the codebase

### How to Contribute

1. **Fork the repository** (if you're an external contributor) or create a new branch from `main`.

2. **Create a feature branch** with a descriptive name:
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes** and commit them with clear, descriptive commit messages.

4. **Push your branch** to the repository:
   ```bash
   git push origin feature/your-feature-name
   ```

5. **Open a Pull Request** against the `main` branch:
   - Provide a clear title and description of your changes
   - Reference any related issues
   - Wait for code review and address any feedback

6. **Merge** only after approval from at least one maintainer.

### Branch Naming Convention

Use descriptive branch names with prefixes:
- `feature/` - for new features
- `bugfix/` - for bug fixes
- `docs/` - for documentation changes
- `refactor/` - for code refactoring

### Commit Messages

Write clear and descriptive commit messages that explain what changes were made and why.

## Setting Up Branch Protection (For Maintainers)

To enforce the pull request requirement, maintainers should configure branch protection rules in GitHub:

1. Go to **Settings** > **Branches**
2. Add a branch protection rule for `main`
3. Enable:
   - "Require a pull request before merging"
   - "Require approvals" (recommended: at least 1)
   - "Dismiss stale pull request approvals when new commits are pushed" (optional)
   - "Require status checks to pass before merging" (if applicable)

## Questions?

If you have any questions about contributing, please open an issue for discussion.
