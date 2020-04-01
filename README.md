# helm charts list
## cmak
Helm chart for [yahoo/CMAK](https://github.com/yahoo/CMAK) ,Cluster Manager for Apache Kafka, previously known as Kafka Manager.  
Please look at [nacos/README](cmak/README.md).

## nacos
Helm chart for [nacos](https://github.com/nacos-group/nacos-docker).  
Please look at [nacos/README](nacos/README.md).

## How to install these charts
Find the repository you want to use under / directory and enter below command:
```
helm repo add scott-wong https://scott-wong.kubesphere.io/charts
helm search repo scott-wong
```

## Update to repo(private)
1. 打包
```
helm lint --strict nacos
helm lint --strict cmak
helm package nacos
helm package cmak
# 添加描述性文件
helm repo index --url https://scott-wong.github.io/charts .
```
2. 上传包到https://scott-wong.github.io/charts
```
cp *.tgz ../gh-pages/public/charts
cp index.yaml ../gh-pages/public/charts
cd ../gh-pages/public
git add .
git commit -m "update helm charts."
git push
```
