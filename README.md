# gh-release-install-action

```yaml
jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - uses: jooola/gh-release-install-action@main
        with:
          repository: mvdan/sh
          asset: shfmt_{tag}_linux_amd64
          destination: /usr/local/bin/shfmt

      - run: shfmt --version
```
