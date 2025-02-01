# Client/ENV yaml setup steps

## argocd-application
### Copy Src\Container\k8s\argocd\templates\argocd-application\overlays\clientname\envname to Src\Container\k8s\argocd\argocd-application\overlays\{clientname}\{envname}
### Replace all the {{}} except {{TAG}} variable to customize the template, {{TAG}} will be replaced by the release scripts.
### Application source path may be reuqired to change for the cloud and on-prem based on the git hub structure

## Config
### Copy Src\Container\k8s\argocd\templates\config\clientname\envname to Src\Container\k8s\argocd\config\{clientname}\{envname}
### Replace all the {{}} except {{TAG}} variable to customize the template, {{TAG}} will be replaced by the release scripts.
### Repo, branch, Instance ID and K8S Destination may be reuqired to change for the cloud and on-prem in config

## Deployments
### Copy Src\Container\k8s\argocd\templates\deployments\overlays\clientname\envname\config to Src\Container\k8s\argocd\deployments\overlays\{clientname}\{envname}\config
### Replace all the {{}} except {{TAG}} variable to customize the template, {{TAG}} will be replaced by the release scripts.
### Image name, Deployment Instance or host path may be reuqired to change for the cloud and on-prem based on the git hub structure in deployment config

# For further details Link https://hidglobal.atlassian.net/wiki/spaces/QSPMKB/pages/287440903/ArgoCD+Setup+and+SAFE+Deployment