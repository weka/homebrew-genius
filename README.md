# genius Homebrew tap

Homebrew tap for `genius`, the command-line client of Genius (WEKA's Jira ticket analysis service).
The formula and the release assets here are written by the release job of weka/genius-api on every tag.

```sh
brew tap weka/genius
brew trust weka/genius
brew install genius
genius version
```

Upgrade: `brew update && brew upgrade genius`. First run (API key, profile): docs/cli.md in weka/genius-api.
