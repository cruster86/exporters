<details><summary>Состав проекта:</summary>

    .
    ├── README.md
    ├── deploy
    │   └── helm
    │       └── charts
    │           ├── prometheus-elasticsearch-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   ├── prod
    │           │   │   │   ├── corp.yaml
    │           │   │   │   ├── cpm.yaml
    │           │   │   │   ├── sirius.yaml
    │           │   │   │   └── univ.yaml
    │           │   │   └── stage
    │           │   │       └── cpm-dev.yaml
    │           │   ├── templates
    │           │   │   ├── _helpers.tpl
    │           │   │   ├── cert-secret.yaml
    │           │   │   ├── deployment.yaml
    │           │   │   ├── podsecuritypolicies.yaml
    │           │   │   ├── prometheusrule.yaml
    │           │   │   ├── role.yaml
    │           │   │   ├── rolebinding.yaml
    │           │   │   ├── secret.yaml
    │           │   │   ├── service.yaml
    │           │   │   ├── serviceaccount.yaml
    │           │   │   └── servicemonitor.yaml
    │           │   └── values.yaml
    │           ├── prometheus-ngenix-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   └── prod
    │           │   │       ├── corp.yaml
    │           │   │       ├── cpm.yaml
    │           │   │       ├── sirius.yaml
    │           │   │       └── univ.yaml
    │           │   ├── templates
    │           │   │   ├── _helpers.tpl
    │           │   │   ├── deployment.yml
    │           │   │   ├── service.yml
    │           │   │   └── servicemonitor.yml
    │           │   └── values.yaml
    │           ├── prometheus-postgres-exporter
    │           │   ├── Chart.yaml
    │           │   ├── conf
    │           │   │   ├── prod
    │           │   │   │   ├── corp.yaml
    │           │   │   │   ├── cpm.yaml
    │           │   │   │   ├── sirius.yaml
    │           │   │   │   └── univ.yaml
    │           │   │   └── stage
    │           │   │       ├── sirius.yaml
    │           │   │       └── univ.yaml
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
    │               ├── Chart.yaml
    │               ├── conf
    │               │   ├── prod
    │               │   │   ├── corp.yaml
    │               │   │   ├── cpm.yaml
    │               │   │   └── univ.yaml
    │               │   └── stage
    │               │       ├── sirius.yaml
    │               │       └── univ.yaml
    │               ├── templates
    │               │   ├── _helpers.tpl
    │               │   ├── deployment.yaml
    │               │   ├── podsecuritypolicy.yaml
    │               │   ├── prometheusrule.yaml
    │               │   ├── role.yaml
    │               │   ├── rolebinding.yaml
    │               │   ├── service.yaml
    │               │   ├── serviceaccount.yaml
    │               │   └── servicemonitor.yaml
    │               └── values.yaml
    └── scripts
        └── helm_deploy_and_wait.sh
</details>

<details><summary>Настройки:</summary>

  - Версии образов:
    - prometheus-postgres-exporter: v0.9.0
    - prometheus-redis-exporter: v1.45.0
    - prometheus-elasticsearch-exporter: v1.5.0
    - prometheus-ngenix-exporter: v0.15 (latest)

  - Общий неймспейс: prometheus-exporters
  - Настройка параметров: `deploy/helm/charts/${CHART_NAME}/conf/${CI_ENVIRONMENT_SLUG}/${CLUSTER_NAME}.yaml`
</details>
