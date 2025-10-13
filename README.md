# Nexus Homelab Automation

[![Nexus-Homelab Ansible](https://github.com/shabhilash/homelab-ansible/actions/workflows/ansible.yml/badge.svg)](https://github.com/shabhilash/homelab-ansible/actions/workflows/ansible.yml)

Centralized infrastructure-as-code for managing homelab servers using Ansible and GitHub Actions (self-hosted runner).

## Overview

Automates provisioning, updates, and configuration of homelab nodes.
Runs safely over passwordless SSH inside a private network (Tailscale).
Designed to be modular and extensible as new roles or services are added.

## Repository Structure

```
.
├── ansible/            # Playbooks, roles, inventory
├── .github/workflows/  # GitHub Actions workflows
└── README.md
```

`ansible/` — main playbooks, modular roles, and inventory.

`workflows/` — workflows that trigger playbooks on the self-hosted runner.

## Getting Started

- Set up a self-hosted runner in your homelab.
- Ensure runner has passwordless SSH to target nodes.
- Ensure Ansible user(`sysadmin`) has passwordless sudo.

Trigger workflows manually or run playbooks locally:

```
ansible-playbook ansible/site.yml -i ansible/inventory/hosts.yml
```

## Notes

- Nodes should be Debian/Ubuntu-based (adjust roles for other OS).
- Roles are modular; new roles can be added without changing existing workflows.
- Workflows can run manually or via schedule once configured.

## Roadmap

- Patch/update roles
- Docker/Docker Compose management
- Terraform provisioning
- Monitoring roles (Prometheus/Grafana)
- Notifications (Discord/email)
