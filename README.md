# This is CD project for simple GO app deployments using GKE, CloudBuild and ArgoCD

## How to deploy app
   1. You need to deploy cluster via [terraform scripts](https://github.com/dotrashevskyi/terrafrom_gke)
   2. CI part for the app is [here](https://github.com/dotrashevskyi/test-02) Dashboard is [here](https://console.cloud.google.com/cloud-build/dashboard?project=internship-166-375809)
   3. Please deploy ArgoCD using [documentation](https://argo-cd.readthedocs.io/en/stable/getting_started/)

## How deploy the app in declarative way
   1. Please connect to your k8s cluster (in case you didn't connect before)
   2. run `kubectl apply -f application-$env.yaml` - where $env should be specified as 'dev' or 'main' for the corresponding environments