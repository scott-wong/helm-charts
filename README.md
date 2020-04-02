[![Build Status](https://travis-ci.org/scott-wong/helm-charts.svg?branch=master)](https://travis-ci.org/scott-wong/helm-charts)  
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


## Skipping a travis-ci build
Commit msg like this:  
```
[skip ci] Update README  
```
related to [docs.travis-ci.com](https://docs.travis-ci.com/user/customizing-the-build/#Skipping-a-build)