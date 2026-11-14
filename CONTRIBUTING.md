# Contributing to paper-now

Paper Now is a Jekyll-based format for developing and displaying journal articles in GitHub. Read the [README](README.md) and distinguish changes to the publishing template from changes to an individual article.

## Before you start

Search existing issues and pull requests before starting, and discuss substantial changes or new dependencies in an issue. Use an issue template when one is offered. For a bug, include the affected commit or version, environment, a minimal reproduction, and expected versus observed behavior; remove sensitive information from logs and screenshots.

## Development and validation

The existing [serve.sh](serve.sh) script starts the local preview with:

```sh
bundle exec jekyll serve --config _config.yml --baseurl ''
```

Prepare a compatible Ruby/Bundler environment using [Gemfile](Gemfile) before previewing. Record any dependency or build failure; the Gemfile resolves GitHub Pages version information externally. A local preview does not require publishing or changing Pages settings.

For template changes, check headings, navigation, figures, tables, references, and links in the rendered article. For manuscript changes, keep claims traceable to cited sources and preserve author attribution. Include small shareable examples and record any accessibility or layout checks. Avoid committing generated outputs or large data files unless they are an intentional part of the contribution.

## Pull requests

Work on a focused branch from the current default branch. Open a pull request explaining the problem, the resulting behavior, and any compatibility or data-format changes. Link the relevant issue and complete any existing PR template.

Add focused regression coverage for changed behavior and update affected examples or documentation. Describe the checks actually run, their results, and any checks you could not run. For documentation-only changes, verify links, examples, and rendered formatting. Use the repository's existing checks and review/merge process; preserve required checks and resolve actionable feedback without weakening the checks.

## Security and sensitive information

Follow the [account security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Report vulnerabilities privately through the repository's **Report a vulnerability** option if available; otherwise request a private reporting contact without posting exploit details. Never include credentials, personal information, restricted datasets, or confidential records in issues, commits, fixtures, or diagnostic output.

## Licensing and conduct

The repository's [license](LICENSE) continues to apply. Be respectful and constructive, and follow the [account code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md). Preserve attribution and third-party notices. Contribute only material you are entitled to share; resolve unclear permissions before adding third-party content. This guide does not change licensing terms or introduce a CLA or DCO requirement.

## References

- [GitHub contribution guideline conventions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)
- [OpenSSF contribution and quality criteria](https://www.bestpractices.dev/en/criteria)
