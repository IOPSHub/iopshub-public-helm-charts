# iopshub-public-helm-charts

## Publishing

This repository is set up to automatically package and publish Helm charts on every push to the `main` branch via GitHub Actions. Packaged charts are released and indexed on the `gh-pages` branch so the repository can be used as a Helm chart repo.

Multiple charts are supported: add each chart as its own directory at the repo root (each containing a `Chart.yaml`). Bump the chart `version` in `Chart.yaml` to publish a new release.

Initial setup: ensure GitHub Pages is enabled for this repo and points to the `gh-pages` branch (root directory).

## Usage

Replace `<owner>` and `<repo>` with your GitHub org/user and repository name.

```
helm repo add iopshub-public https://<owner>.github.io/<repo>
helm repo update

# Example install (replace with your chart and values)
helm install my-release iopshub-public/<chart-name> -n <namespace> --create-namespace
```
