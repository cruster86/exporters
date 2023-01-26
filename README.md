<details><summary>Состав проекта:</summary>

    .
    ├── README.md
    ├── deploy
    │   └── helm
    │       └── charts
    │           ├── prometheus-elasticsearch-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   ├── corp-prod.yaml
    │           │   │   ├── cpm-dev-stage.yaml
    │           │   │   ├── cpm-prod.yaml
    │           │   │   ├── sirius-prod.yaml
    │           │   │   └── univ-prod.yaml
    │           │   ├── templates
    │           │   │   ├── _helpers.tpl
    │           │   │   ├── cert-secret.yaml
    │           │   │   ├── deployment.yaml
    │           │   │   ├── podsecuritypolicies.yaml
    │           │   │   ├── prometheusrule.yaml
    │           │   │   ├── role.yaml
    │           │   │   ├── rolebinding.yaml
    │           │   │   ├── service.yaml
    │           │   │   ├── serviceaccount.yaml
    │           │   │   └── servicemonitor.yaml
    │           │   └── values.yaml
    │           ├── prometheus-ngenix-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   ├── corp-prod.yaml
    │           │   │   ├── cpm-prod.yaml
    │           │   │   ├── sirius-prod.yaml
    │           │   │   └── univ-prod.yaml
    │           │   ├── templates
    │           │   │   ├── _helpers.tpl
    │           │   │   ├── deployment.yml
    │           │   │   ├── service.yml
    │           │   │   └── servicemonitor.yml
    │           │   └── values.yaml
    │           ├── prometheus-postgres-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   ├── corp-prod.yaml
    │           │   │   ├── cpm-dev-stage.yaml
    │           │   │   ├── cpm-prod.yaml
    │           │   │   ├── sirius-prod.yaml
    │           │   │   ├── sirius-stage.yaml
    │           │   │   ├── univ-prod.yaml
    │           │   │   └── univ-stage.yaml
    │           │   ├── templates
    │           │   │   ├── _helpers.tpl
    │           │   │   ├── configmap.yaml
    │           │   │   ├── deployment.yaml
    │           │   │   ├── networkpolicy.yaml
    │           │   │   ├── pdb.yaml
    │           │   │   ├── podsecuritypolicy.yaml
    │           │   │   ├── prometheusrule.yaml
    │           │   │   ├── role.yaml
    │           │   │   ├── rolebinding.yaml
    │           │   │   ├── secrets.yaml
    │           │   │   ├── service.yaml
    │           │   │   ├── serviceaccount.yaml
    │           │   │   └── servicemonitor.yaml
    │           │   └── values.yaml
    │           └── prometheus-redis-exporter
    │               ├── Chart.yaml
    │               ├── conf
    │               │   ├── corp-prod.yaml
    │               │   ├── univ-prod.yaml
    │               │   └── univ-stage.yaml
    │               ├── templates
    │               │   ├── _helpers.tpl
    │               │   ├── deployment.yaml
    │               │   ├── podsecuritypolicy.yaml
    │               │   ├── prometheusrule.yaml
    │               │   ├── role.yaml
    │               │   ├── rolebinding.yaml
    │               │   ├── service.yaml
    │               │   ├── serviceaccount.yaml
    │               │   └── servicemonitor.yaml
    │               └── values.yaml
    └── scripts
        └── helm_deploy_and_wait.sh
</details>

<details><summary>Настройки:</summary>

  - Настройка параметров: `deploy/helm/charts/${CHART_NAME}/conf/${CLUSTER_NAME}-${CI_ENVIRONMENT_SLUG}.yaml`
</details>
