# Ansible Monitoring

Ansible playbooks for deploying Prometheus and Grafana stack in Kubernetes.

## Prerequisites
- Ansible 2.14+
- kubectl configured
- Helm 3+
- Kubernetes cluster (Docker Desktop)

## Usage
```bash
ansible-playbook -i inventory.ini monitoring-setup.yaml

## Access

```bash
kubectl port-forward svc/prometheus-grafana 3000:80 -n monitoring
kubectl port-forward svc/prometheus-kube-prometheus-prometheus 9090:9090 -n monitoring
