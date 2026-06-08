# Contributing to Pullminder

Thank you for your interest in contributing to Pullminder.

## Repository guide

Pullminder spans two GitHub organizations:

| Organization | Purpose |
|---|---|
| [Upmate](https://github.com/Upmate) | Source code: the [pullminder.com monorepo](https://github.com/Upmate/pullminder.com) contains the API, CLI, web app, and shared libraries. |
| [pullminder](https://github.com/pullminder) | Distribution: npm, Homebrew, GitHub Action, and org-level community health files. |

Code changes belong in the [Upmate/pullminder.com monorepo](https://github.com/Upmate/pullminder.com). The repositories in this organization are distribution channels — they wrap and ship releases built from the monorepo.

## How to contribute

### Code

1. Open an issue in [Upmate/pullminder.com](https://github.com/Upmate/pullminder.com/issues) describing the bug or feature.
2. Fork the monorepo and create a feature branch.
3. Follow the conventional commits format: `type(scope): summary`.
4. Add tests for your changes.
5. Open a pull request against `main`.

### Registry packs

The [official rule pack registry](https://github.com/pullminder/registry) accepts community pack submissions:

1. Read the [pack authoring guide](https://docs.pullminder.com/registry/authoring).
2. Submit your pack as a pull request to [pullminder/registry](https://github.com/pullminder/registry).
3. Include a `pack.yaml` and `pack.schema.json` that pass AJV validation.

### Documentation

Documentation lives at [docs.pullminder.com](https://docs.pullminder.com). To suggest improvements, open an issue in [Upmate/pullminder.com](https://github.com/Upmate/pullminder.com/issues) with the `documentation` label.

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.

## License

Pullminder is licensed under the Apache License 2.0. See [LICENSE](LICENSE) for the full text. By contributing, you agree that your contributions will be licensed under the same terms.
