
 ⚙️ Ansible Automation Lab

> Centralized repo for reusable Ansible playbooks, roles, and automation tasks focused on DevOps, CloudOps, and Infrastructure as Code (IaC).

---

📦 Repo Overview

This repository is a collection of Ansible automation content curated and created by [Darius Powell](https://github.com/Dariuskp). It includes playbooks, inventories, and reusable roles to automate:

- Server provisioning
- Configuration management
- CloudOps tasks
- Security hardening
- Application deployment

---

🧰 Tech Stack

- **Automation Tool:** Ansible
- **Languages:** YAML, Bash
- **OS Support:** Ubuntu, CentOS, Amazon Linux
- **Clouds:** AWS (EC2), Local VM (via Vagrant or SSH)

---

📁 Structure

```
Ansible/
├── inventories/             # Inventory files for staging, prod, etc.
│   └── hosts.ini
├── playbooks/               # Main automation logic
│   ├── provision.yml
│   ├── deploy_app.yml
│   └── harden.yml
├── roles/                   # Reusable role definitions
│   ├── nginx/
│   ├── docker/
│   └── users/
├── group_vars/              # Group-level variables
├── host_vars/               # Host-level variables
├── ansible.cfg              # Ansible configuration file
└── README.md                # Repo documentation
```

---

🚀 Getting Started

### Prerequisites

- Ansible installed (`pip install ansible`)
- SSH access to target nodes
- Inventory configured under `inventories/hosts.ini`

---

### Example: Provision a Server

```bash
ansible-playbook -i inventories/hosts.ini playbooks/provision.yml
```

### Example: Harden a Node

```bash
ansible-playbook -i inventories/hosts.ini playbooks/harden.yml
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

- Cloud provisioning for EC2
- Internal DevSecOps environments
- Chaos-ready automation (resilient provisioning)
- Infrastructure compliance bootstrapping

---

🧠 About

Created and maintained by Darius Powell
