```bash

helm repo list
helm repo update

# See resources created by Helm release

helm get manifest my-release -n namespace
helm get manifest mysql-exporter -n mysql

helm ls -A
helm ls -n monitoring

# Check files installed by chart
helm install --dry-run debug .