# Contributing <!-- omit in toc -->

First of all, thanks for thinking of contributing to this project! 👏

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

As a contributor, here are the guidelines we would like you to follow:

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Code of Conduct](#code-of-conduct)
- [How can I contribute?](#how-can-i-contribute)
  - [Give Feedback on Issues](#give-feedback-on-issues)
  - [Fix bugs and implement features](#fix-bugs-and-implement-features)
- [Using the issue tracker](#using-the-issue-tracker)
  - [Bug report](#bug-report)
  - [Feature request](#feature-request)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Style Guides](#style-guides)
  - [Commit Messages](#commit-messages)

We also recommend that you read [How to Contribute to Open Source](https://opensource.guide/how-to-contribute).

## Code of Conduct

Please note that this project have a [code of conduct](CODE_OF_CONDUCT.md), please follow it in all your interactions with the project.

## How can I contribute?

### Give Feedback on Issues

Some issues are created without information requested in the [Bug report guideline](#bug-report). Help make them easier to resolve by adding any relevant information.

Issues with the **`enhancement`** label are meant to discuss the implementation of new features. Participating in the discussion is a good opportunity to get involved and influence our future direction.

### Fix bugs and implement features

Confirmed bugs and ready-to-implement features are marked with the **`help wanted`** label. Post a comment on an issue to indicate you would like to work on it and to request help from the **maintainers** and the **community**.

## Using the issue tracker

The issue tracker is the channel for [bug reports](#bug-report), [features requests](#feature-request) and [submitting pull requests](#submitting-a-pull-request) only.

Before opening an issue or a Pull Request, please use the **GitHub issue search** to make sure the bug or feature request hasn't been already reported or fixed.

### Bug report

A good bug report shouldn't leave others needing to chase you for more information. Please try to be as detailed as possible in your report and fill the information requested in the **Bug report template**.

### Feature request

Feature requests are welcome, but take a moment to find out whether your idea fits with the scope and aims of the project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Please provide as much detail and context as possible and fill the information requested in the **Feature request template**.

## Submitting a Pull Request

Good pull requests, whether patches, improvements, or new features, are a fantastic help. They should remain focused in scope and avoid containing unrelated commits.

**Please ask first** before embarking on any significant pull requests (e.g. implementing features, refactoring code), otherwise you risk spending a lot of time working on something that the project's developers might not want to merge into the project.

If you have never created a pull request before, welcome 🎉 😄. [Here is a great tutorial](https://opensource.guide/how-to-contribute/#opening-a-pull-request) on how to send one. 😃

This is our preferred process for opening a PR on GitHub:

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request

## Style Guides

### Commit Messages

This project uses the [conventional commit](https://www.conventionalcommits.org) for your commit messages. This format is used to generate changelogs and ensures consistency and better filtering.

Each commit message consists of a **header**, a **body** and a **footer**. The header has a special format that includes a **type**, a **scope** and a **subject**:

```commit
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and the **scope** of the header is optional.

The **footer** can contain a [closing reference to an issue](https://help.github.com/articles/closing-issues-via-commit-messages).

**Revert**

If the commit reverts a previous commit, it should begin with `revert: `, followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>.`, where the hash is the SHA of the commit being reverted.


**Type**

Must be one of the following:

| Type           | Description                                                                                                  |
| -------------- | ------------------------------------------------------------------------------------------------------------ |
| **`build`**    | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm).         |
| **`chore`**    | Used when changes are about organization, not about logic.                                                   |
| **`ci`**       | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs). |
| **`docs`**     | Documentation only changes.                                                                                  |
| **`feat`**     | A new feature.                                                                                               |
| **`fix`**      | A bug fix.                                                                                                   |
| **`perf`**     | A code change that improves performance.                                                                     |
| **`refactor`** | A code change that neither fixes a bug nor adds a feature.                                                   |
| **`revert`**   | Reverts a previous commit.                                                                                   |
| **`style`**    | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).      |
| **`test`**     | Adding missing tests or correcting existing tests.                                                           |

**Subject**

The subject contains succinct description of the change:
- use the imperative, present tense: "change" not "changed" nor "changes"
- don't capitalize first letter
- no dot (.) at the end

**Body**
Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

**Footer**
The footer should contain any information about **Breaking Changes** and is also the place to reference GitHub issues that this commit **Closes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

**Examples**

```commit
fix(pencil): stop graphite breaking when too much pressure applied
```

```commit
feat(pencil): add 'graphiteWidth' option

Fix #42
```

```commit
perf(pencil): remove graphiteWidth option

BREAKING CHANGE: The graphiteWidth option has been removed.

The default graphite width of 10mm is always used for performance reasons.
```