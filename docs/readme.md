# Helm charts by Kelalab

## 1. Change to docs dir
```
cd docs
```
## 2. Creating chart packages
```
helm package ../chart-sources/*
```
## 3a. Creating index.yaml
```
helm repo index --url https://kelalab.github.io/helm-charts .
```
## 3b. Updating index.yaml
```

```
