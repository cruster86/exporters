### Структура репозитория

Настройки для кластеров находятся в:

  - `deploy/helm/charts/${CHART_NAME}/conf/${CI_ENVIRONMENT_SLUG}/${CLUSTER_NAME}.yaml`

Конфигурация деплоя находится в: `.gitlab-ci.yaml`

Upstream проекты:

  - https://github.com/prometheus-community/helm-charts/tree/main/charts/prometheus-postgres-exporter
  - https://github.com/prometheus-community/helm-charts/tree/main/charts/prometheus-redis-exporter
  - https://github.com/prometheus-community/helm-charts/tree/main/charts/prometheus-elasticsearch-exporter
  - https://gitlab.sirius.online/cheops-edu/ngenix-client
