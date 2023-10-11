# Bootstrap via ArgoCD

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
