# Helm charts by Kelalab

Using this repository:
```
helm repo add kelalab https://kelalab.github.io/helm-charts/
```

## 1. Check charts
```
helm lint chart-sources/*
```

## 1. Creating chart packages
```
helm package chart-sources/*
```
## 2a. Creating index.yaml
```
helm repo index --url https://kelalab.github.io/helm-charts .
```
## 2b. Updating index.yaml with a new chart package
```
helm repo index --url https://kelalab.github.io/helm-charts --merge index.yaml .
```
