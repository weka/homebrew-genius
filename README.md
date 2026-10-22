# genius Homebrew tap

Homebrew tap for `genius`, the command-line client of Genius, WEKA's Jira ticket analysis
service. The release job of [weka/genius-api](https://github.com/weka/genius-api) writes
`Formula/genius.rb` and the release assets here on every tag; nothing is edited by hand.

## Install

```sh
brew tap weka/genius
brew trust weka/genius
brew install genius
genius version
```

`brew trust` is required once per tap: Homebrew loads a formula from a non-official tap only
after the user trusts the tap. Homebrew picks the build for the machine (macOS Apple silicon or
Intel, Linux amd64 or arm64).

## Upgrade

```sh
brew update
brew upgrade genius
```

## First run

The CLI needs the URL of a Genius deployment and a personal API key. See
[docs/cli.md](https://github.com/weka/genius-api/blob/main/docs/cli.md) in weka/genius-api
(§ Distribution, "First run: log in").
