# Bootstrap via ArgoCD

## Clone this repository to your own

To ensure working with your settings and ownership, clone this repo to your own github space.

Change the repo settings to your github repo accordingly in file `project.yaml` 

```yaml
...
spec:
  project: default
  source:
    repoURL: [YOUR CLONED OWN GITHuB REPO]
...
```

## Change the eMail Address for the cluster issuer

Change the email address in `2nd-wave/cluster-issuer/cluster-issuer.yaml` to your valid email address

## Check hostnames in ingress definitions

Change the Hostname to your appropriate name in

- bootstrap/kube-prometheus-stack/ingress.yaml
- bootstrap/minio-operator/application.yaml

## Bootstrap the cluster

```bash
kubectl apply -f .
```
