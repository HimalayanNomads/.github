# Contributing to Himalayan Nomads

Thanks for helping out. This guide applies to every repository in the organization. When a project has its own `CONTRIBUTING.md`, read that too: it covers setup, tests and conventions for that codebase, and it takes precedence over this page.

Everyone taking part is expected to follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## Ways to contribute

- Report bugs.
- Suggest features and improvements.
- Write or improve documentation.
- Submit bug fixes or new features.
- Test releases and share feedback.

Looking for a place to start? Try issues labeled `good first issue` or `help wanted`. Comment on an issue before you start so two people don't work on the same thing.

Security problems don't go in public issues. See [SECURITY.md](SECURITY.md).

## Reporting bugs

Search open and closed issues first. If nobody has reported it yet, open a new issue and include:

- What you did, what you expected and what happened instead.
- Your OS and the project version (or commit).
- Error messages and logs, if any.
- A screenshot or recording, if the bug is visible.

## Suggesting features

Open an issue and describe the problem before the solution: what you were trying to do and what got in the way. Wait for a maintainer to agree on the direction before you start a large change.

## Making a change

Only maintainers push to the organization's repositories. Every change goes through a fork and a pull request:

1. Fork the repository, clone your fork and add the original as `upstream`:

   ```sh
   git clone https://github.com/<your-username>/<repository>.git
   cd <repository>
   git remote add upstream https://github.com/HimalayanNomads/<repository>.git
   ```

2. Create a branch from an up-to-date `main`, one branch per change:

   ```sh
   git fetch upstream
   git checkout -b fix/short-name upstream/main   # or feat/, docs/
   ```

3. Keep one change per pull request, and update the docs in the same pull request when behavior changes.
4. Write commit messages as a short imperative sentence that says what changes.
5. Run the project's build and tests before you push.
6. Push the branch to your fork and open a pull request. Link the issue it resolves (`Closes #12`), describe what changed and why, and list what you tested.

Maintainers review pull requests and cut releases. A merged pull request ships in the next release.

## License

Each project is licensed as stated in its `LICENSE` file. By opening a pull request, you agree that your contribution is licensed under the same terms as that project.
