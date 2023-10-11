# Build Helm Chart Repository

### Requisite
- Preparing a Helm Chart source

### Layout of repository

```
helm-packages/
  |
  |- index.yaml
  |
  |- handson-0.1.0.tgz
```

### Hosting Chart Repository
- Reference: https://helm.sh/docs/topics/chart_repository/#github-pages-example

### Store charts in your chart repository

```sh
git clone https://github.com/USERNAME/REPOSITORY_NAME.git
git checkout main
helm package path/to/helm-chart-source-directory
helm repo index . --url https://USERNAME.github.io/REPOSITORY_NAME
```