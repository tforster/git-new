# Contributing <!-- omit in toc -->

_A step-by-step guide for project installation, development and contribution._

- [Getting Started](#getting-started)
- [Code of Conduct](#code-of-conduct)
- [Development](#development)
- [Versioning](#versioning)

## Getting Started

Before starting, [ensure a ticket](https://dev.azure.com/techsmarts/TechSmarts/_boards/board/t/TechSmarts%20Team/Backlog%20items) exists for the work that is to be done.

Please see the notes on [Prerequisites](README.md#prerequisites), [Installation](README.md#installation) and [Usage](README.md#usage).

## Code of Conduct

You must adhere to the [**Code of Conduct**](CODE_OF_CONDUCT.md) specified in this project. Please review [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md) in full.

## Development

1. Create the new branch, prefixing it with the zero padded issue number:

   ```sh
   git checkout -b 0000-short-name
   ```

2. Update the version number with `patch`, `minor` or `major`, following [SemVer](https://semver.org/):

   ```sh
   npm run bump patch
   ```

3. Update the [`CHANGELOG.md`](CHANGELOG.md) with the appropriate release notes:

   ```md
   `vM.m.p` **Short Title For Changes** (YYYY-MM-DD)

   - Description of changes made in this version.
   - Additional noteworthy changes to be mentioned.
   - [#0nnn The ticket title](https://ticket-link)
   ```

4. Stage the modified / added / removed files which are to be committed:

   ```sh
   git add --all
   ```

5. Optionally view the status to ensure the correct files are staged for commit:

   ```sh
   git status
   ```

6. Optionally view the commit differences to ensure all changes are present:

   ```sh
   git diff --cached
   ```

7. Commit the changes, prefixing the message with the zero padded issue number:

   ```sh
   git commit --message "#0000 Created the example commit message"
   ```

8. Push the new branch to the project repository, while setting remote tracking:

   ```sh
   git push origin 0000-short-name --set-upstream
   ```

9. Submit the changes by [creating a pull request](https://github.com/tforster/git-new/compare).

## Versioning

This project uses **Semantic Versioning 2.0.0**. Please see [SemVer](https://semver.org/) to read the specification.
