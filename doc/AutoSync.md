To enable autosync in ArgoCD:

Instal cli argocd tool using: https://argo-cd.readthedocs.io/en/stable/cli_installation/

login into app: `argocd login localhost:8080 --usename admin`
use password: `kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo`

set auto sync: `argocd app set <APPNAME> --sync-policy automated`