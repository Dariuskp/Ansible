
 ⚙️ Ansible Automation Lab

> Centralized repo for reusable Ansible playbooks, roles, and automation tasks focused on DevOps, CloudOps, and Infrastructure as Code (IaC).

---

📦 Repo Overview

This repository is a collection of Ansible automation content curated and created by [Darius Powell](https://github.com/Dariuskp). It includes playbooks, inventories, and reusable roles to automate:

- Patch Management 
- Configuration management
- CloudOps tasks
- Security hardening
- Server tasks

---

🧰 Tech Stack

- **Automation Tool:** Ansible
- **Languages:** YAML, Bash
- **OS Support:** Ubuntu, CentOS, Redhat, AlmaLinux

---

---

🚀 Getting Started

### Prerequisites

- Ansible installed (`pip install ansible`)
- SSH access to target nodes
- Inventory configured under `inventories/hosts.ini`

---

```

---

🔐 Security Hardening Features

The `harden.yml` playbook includes:

- Disabling root SSH
- Enforcing SSH key auth
- Setting up auditd
- UFW or firewalld configuration
- Installing OS updates

---

📦 Supported Roles

| Role   | Description                   |
|--------|-------------------------------|
| nginx  | Install and configure NGINX   |
| docker | Setup Docker and Docker Compose |
| users  | Create secure admin users     |

---

🔄 CI/CD Integration

You can integrate this repo with:

- GitHub Actions
- Jenkins
- GitLab CI
- Terraform for provisioning, Ansible for config

---

🌍 Use Cases

- Internal DevSecOps environments
- Chaos-ready automation (resilient provisioning)
- Infrastructure compliance bootstrapping

---

🧠 About

Created and maintained by Darius Powell
