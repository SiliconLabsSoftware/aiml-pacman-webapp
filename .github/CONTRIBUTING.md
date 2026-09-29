# Contributing

This repository hosts the GPL v3 Pac-Man web demo for the Silicon Labs AIML BLE
audio classifier sample. It is maintained by the AIML team.

## Community contributions

External contributions are **paused**. The repository is labeled
`community-contributions-paused` on GitHub. Do not open pull requests expecting
merge unless you have agreed with the maintainers in advance.

Silicon Labs employees with access should use the internal process below.

## Code of conduct

Participation is governed by [CODE_OF_CONDUCT.md](../CODE_OF_CONDUCT.md).

## Reporting issues

Use the **Bug report** issue template when reporting problems (browser, board,
BLE connection, and related environment details).

## Changes by maintainers

1. Create a branch from `main`.
2. Make focused changes.
3. **Sign every commit** with GPG. This repository requires verified signatures on
   `main`. See GitHub documentation on
   [signing commits](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits).
4. Open a pull request to `main`.
5. Obtain review from code owners (see [CODEOWNERS](CODEOWNERS)).

### Commit messages

Use clear subjects and bodies. Include a ticket reference when applicable (for
example, `MLSW-11113: ...`).

## Licensing

Contributions to the Pac-Man web application are licensed under the
[GNU General Public License v3.0](../LICENSE) (see the default-license section
in that file).

Third-party code under `js/` retains its original licenses (see file headers).
Prebuilt firmware under `firmware/` is under the Silicon Labs MSLA; see
[firmware/LICENSE](../firmware/LICENSE). Do not contribute firmware changes
under GPL terms unless Legal has approved a different arrangement.
