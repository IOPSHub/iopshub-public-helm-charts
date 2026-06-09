# iopshub-public-helm-charts

## 🎯 Purpose & Scope
Public Helm Charts for packaging and deploying the PSaux cluster agent to Kubernetes.

## 🛠️ Technology Stack & Key Dependencies
- **Technology**: Kubernetes Helm Charts

## 📂 Directory Structure & Entry Points
- `📄 README.md` - File
- `📂 psauxai-cluster-agent-chart/` - Subdirectory
  - `Chart.yaml` (File)
  - `README.md` (File)
  - `templates` (Subdirectory)
  - `values.yaml` (File)

## 🤖 LLM Code Generation Instructions
- Always validate values.yaml structure and ensure templates use standard Helm functions (`toYaml`, `nindent`).
- Maintain version schema in Chart.yaml strictly during changes.

## 📝 Legacy Context & Specifications

```markdown
# iopshub-public-helm-charts

## Publishing

This repository is set up to automatically package and publish Helm charts on every push to the `main` branch via GitHub Actions. Packaged charts are released and indexed on the `gh-pages` branch so the repository can be used as a Helm chart repo.

Multiple charts are supported: add each chart as its own directory at the repo root (each containing a `Chart.yaml`). Bump the chart `version` in `Chart.yaml` to publish a new release.

Initial setup: ensure GitHub Pages is enabled for this repo and points to the `gh-pages` branch (root directory).

## Usage

Replace `<owner>` and `<repo>` with your GitHub org/user and repository name.
```
