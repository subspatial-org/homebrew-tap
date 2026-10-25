# subspatial Homebrew tap

Homebrew formulae for [subspatial](https://app.subspatial.io).

```sh
brew install subspatial-org/tap/subspatial
```

Then sign in with `subspatial login --api https://app.subspatial.io`. You need a subspatial alpha account (by invitation). Upgrade with `brew upgrade subspatial`.

The formula installs the unsigned pilot builds published on [subspatial-org/data-cli](https://github.com/subspatial-org/data-cli/releases), each pinned by its SHA-256. See that repository for what the pilot supports.

## Updating the formula for a new release

```sh
./update-formula.sh 0.3.0-alpha.3
```

It reads the release's `SHA256SUMS` and rewrites `Formula/subspatial.rb`; commit and push the result.
