# Pre-Commit

Install pre-commit from
[https://pre-commit.com/#install](https://pre-commit.com/#install)

Create a `.pre-commit-config.yaml` file at the root of your repository with the following content:

```yaml
    repos:
      - repo: https://github.com/timcleaver/gitleaks-system-pre-commit-hook
        rev: HEAD
        hooks:
          - id: gitleaks-system
```

Make sure that you have installed [gitleaks](https://github.com/zricethezav/gitleaks) and it
is available on your \$PATH. On macos you can install via `homebrew`:

```sh
brew install gitleaks
```
