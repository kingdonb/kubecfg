# Kubecfg GitHub Action

Usage:

```yaml
    steps:
      - name: Setup kubecfg CLI
        uses: kingdonb/kubecfg/action@main
      - name: Run kubecfg commands
        run: kubecfg version
```

Note that this action can only be used on GitHub **Linux AMD64** runners.
The latest stable version of the `kubecfg` binary is downloaded from
GitHub [releases](https://github.com/bitnami/kubecfg/releases)
and placed at `/usr/local/bin/kubecfg`.

You can download a specific version with:

```yaml
    steps:
      - name: Setup kubecfg CLI
        uses: kingdonb/kubecfg/action@main
        with:
          version: v0.18.0
```

