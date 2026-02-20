## Overview
This portfolio demonstrates my hands-on DevOps skills:
- **Ansible automation** for deployment
- **GitLab CI/CD pipeline** for automated self-update
- **Server deployment workflow** using a PHP application

## Tools Used
- Linux (Ububtu)
- Apache / PHP
- Ansible
- GitLab CI/CD
- Git

## Workflow
1. Click “Update” button (simulated)
2. GitLab CI/CD pipeline triggers
3. Ansible playbook updates the application
4. Web service restarts automatically

## How to Run Locally
1. Ensure Apache and PHP installed
2. Run playbook:
```bash
ansible-playbook ansible/update.yml
