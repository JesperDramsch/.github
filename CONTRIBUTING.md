# Contributing to this Project

First off, thank you for considering contributing to our project! It's people like you that make this project such a great tool.

## Code of Conduct

By participating in this project, you are expected to uphold our Code of Conduct. Please report unacceptable behavior to [maintainer email].

## Getting Started

Contributions are made to this repo via Issues and Pull Requests (PRs).

-   Search existing Issues and PRs before creating your own
-   If you're fixing a bug or adding a feature, please create an Issue first to discuss it

### Development Process

1. Fork the repository
2. Create a new branch:

    ```bash
    git checkout -b feature/your-feature-name
    ```

    or

    ```bash
    git checkout -b fix/your-bug-fix
    ```

3. Set up your development environment:

    ```bash
    uv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    uv pip install -e "."
    pre-commit install
    ```

4. Make your changes and ensure they meet our standards:

    - Write meaningful commit messages
    - Add or update tests as needed
    - Update documentation if required
    - Run tests and linting locally

5. Push to your fork and submit a Pull Request

### Pull Request Process

1. Update the README.md if needed (e.g., new features, changes in requirements)
2. Update the documentation with details of changes
3. Add your changes to the CHANGELOG.md under "Unreleased"
4. The PR title should follow [Conventional Commits](https://www.conventionalcommits.org/):
    ```
    feat: add new feature
    fix: resolve bug
    docs: update documentation
    style: format code
    refactor: restructure code
    test: add tests
    chore: update dependencies
    ```

### Local Development

1. Run tests:

    ```bash
    pytest
    ```

2. Run linting:

    ```bash
    black .
    ruff check .
    ```

3. Run pre-commit hooks:
    ```bash
    pre-commit run --all-files
    ```

## Style Guide

### Code Style

-   We follow PEP 8 guidelines
-   Use Black for code formatting
-   Use type hints for function arguments and return values
-   Write docstrings for all public functions, classes, and modules

### Documentation

-   Use Google-style docstrings
-   Include examples in docstrings where helpful
-   Keep line length to 88 characters (Black default)
-   Document both successful and error cases

### Commit Messages

-   Use the present tense ("add feature" not "added feature")
-   Use the imperative mood ("move cursor to..." not "moves cursor to...")
-   Reference issues and pull requests when relevant
-   Keep first line under 72 characters
-   Describe what and why, not how

### Testing

-   Write unit tests for new features
-   Ensure all tests pass before submitting PRs
-   Aim for high test coverage of new code
-   Include both positive and negative test cases

## Release Process

1. The maintainers will periodically create releases
2. Version numbers follow [Semantic Versioning](https://semver.org/)
3. Each release will be tagged and have a changelog entry
4. PyPI releases are automated via GitHub Actions

## Getting Help

-   Create an Issue for bug reports or feature requests
-   Contact the maintainers for security issues

## Recognition

Contributors will be recognized in:

-   The project's AUTHORS file
-   Release notes when their changes are included

Thank you for contributing to our project! Your efforts help make this tool better for everyone.
