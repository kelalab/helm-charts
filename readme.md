# Helm charts by Kelalab

Using this repository:
```
helm repo add kelalab https://kelalab.github.io/helm-charts/
```

## Updating repository

### 1. Check charts that you want to add
```
helm lint chart-sources/*
```
### 2. Creating chart packages from those local charts
```
helm package chart-sources/*
```
### 3a. Creating index.yaml (only in case of must, otherwise look to 3b)
```
helm repo index --url https://kelalab.github.io/helm-charts .
```
### 3b. Updating index.yaml with a new chart package
```
helm repo index --url https://kelalab.github.io/helm-charts --merge index.yaml .
```
