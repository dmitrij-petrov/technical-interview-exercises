# Technical Interview Exercises

Technical interview exercises covering infrastructure, automation, and platform engineering tasks.

This repository is a compact interview workspace for evaluating practical engineering judgment across three areas:

- **Terraform** for AWS infrastructure setup
- **Ansible** for host and service configuration
- **Helm** for Kubernetes application packaging

The exercises are intentionally small and focused. They are meant to surface how a candidate reasons about infrastructure, tradeoffs, repeatability, and operational correctness.

## Repository Layout

### `terraform/`
Terraform scenarios for two different interview tracks:

- `terraform/sre/` - infrastructure layout for an SRE-oriented exercise
- `terraform/dba/` - infrastructure layout for a DBA-oriented exercise

Each track includes:

- `provider.tf` - AWS provider configuration
- `variables.tf` - exercise inputs
- `resources.tf` - infrastructure resources
- `terraform.tfvars` - example values

### `ansible/`
Ansible playbooks and roles for host provisioning and service configuration.

Included exercises:

- `nginx.yml` - Nginx deployment playbook
- `k8s.yml` - Kubernetes bootstrap playbook
- `dbms.yml` - database service orchestration

Roles included in the repository:

- `nginx`
- `k8s`
- `postgresql`
- `clickhouse`
- `mongodb`

### `helm/`
Helm chart files for a simple Kubernetes deployment example.

The chart includes:

- `Chart.yaml`
- `values.yaml`
- template manifests for deployment, service, and config maps

## What This Repo Is For

- Assessing infrastructure fundamentals
- Evaluating automation approach and debugging process
- Observing how candidates structure reusable IaC
- Discussing operational concerns such as networking, access, and service bootstrapping
- Reviewing Kubernetes packaging and configuration patterns

## Notes

- The repository is intentionally interview-focused rather than production-complete.
- Treat embedded credentials, keys, and sample tfvars data as placeholders for exercise use only.
- Candidate solutions should be incremental and explained, not just copied into place.

## License

MIT
