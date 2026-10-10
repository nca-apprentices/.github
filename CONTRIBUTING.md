# Contributing

These rules hold in every nca-apprentices repository that doesn't bring its
own CONTRIBUTING.md.

## Tools

Each repository pins its tools in `mise.toml`. Install
[mise](https://mise.jdx.dev), then run `mise trust` and `mise install` once in
the repository. `mise tasks` lists what you can run, and CI runs the same
tasks.

## Changes

- A change reaches `main` through a pull request that one other member
  approves. It squash-merges, so the pull request title becomes the commit
  subject.
- Titles and commit subjects follow
  [Conventional Commits](https://www.conventionalcommits.org), such as
  `fix(web): keep the score after a reload`. Use the imperative mood and no
  final period.
- The body says why the change matters. The diff already shows what changed.
- `Closes #<n>` in the pull request body closes the issue it fixes.

## Dependencies

Renovate opens update pull requests on the 1st and 15th of each month, for
releases at least 7 days old. The shared settings live in `default.json` in
nca-apprentices/.github, and a repository adds its own rules in
`.github/renovate.json`.

## Security

Report a vulnerability privately, as [SECURITY.md](SECURITY.md) describes.
