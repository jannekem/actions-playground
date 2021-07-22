# Actions Playground

This repository is meant for testing different GitHub Actions workflows. I feature these examples on my [YouTube channel](https://www.youtube.com/channel/UCg_e3UBPs-BxPo_jVg1gGOQ) and [on my blog](https://www.pakstech.com/).

I aim to create practical examples for people who are just getting started with GitHub Actions and are in need of some inspiration.

If you have a cool workflow in mind then feel free to open a pull request and I might even do a video about it!

## Current workflows

Here are the workwlows that are currently configured.

### PR Labeler

The pull request labeler workflow in [.github/workflows/pr-labels.yml](.github/workflows/pr-labels.yml) assigns labels to pull requests based on the edited file types and directories.


### First interaction

When someone opens a pull request or a new issue for the first time in this repository they are greeted by the first interaction action located in [.github/workflows/first-interaction.yml](.github/workflows/first-interaction.yml).

### Stale issues

If there are issues that are have not been resolved and have been open for a long time they will be marked as stale and eventually closed automatically. The workflow is located in [.github/workflows/stale.yml](.github/workflows/stale.yml).

### Black

Pull requests are checked with the [Black](https://github.com/psf/black) code formatter to verify that all committed Python code is formatted properly. The workflow can be found from [.github/workflows/black.yml](.github/workflows/black.yml).

### Flake8

Flake8 is a Python linter. The [.github/workflows/flake8.yml](.github/workflows/flake8.yml) workflow verifies that all pull requests pass the check.

### Unittest

The repository contains a super simple Python unit test that always passes. The [.github/workflows/unittest.yml](.github/workflows/unittest.yml) is the workwflow that runs that check against all push events.

### I like pizza

When someone comments a pull request or an issue with "I like pizza", the workflow in [.github/workflows/like-pizza.yml](.github/workflows/like-pizza.yml) will react to the comment with a thumbs up emoji. This demonstrates how you can use the `issue_comment` event.

## Contributing

1. Have an idea for a cool workflow
2. Fork the repository
3. Implement and test your workflow
4. Describe it shortly in the README
5. Open a pull request
