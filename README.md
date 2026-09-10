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
