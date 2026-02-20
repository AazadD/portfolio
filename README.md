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
```
## Nginx Reverse Proxy with Domain
- Configured Nginx on Ubuntu to serve applications through a real domain
- Example workflow:
  - Application runs on internal port (e.g., 8081)
  - Nginx listens on port 80/443 and forwards requests from domain `example.com` to the app
- Demonstrates:
  - Domain mapping
  - Reverse proxy setup
  - Real-world server deployment

E.g.
```
server {
    listen 80;
    server_name yourdomain.com;

    location / {
        proxy_pass http://localhost:80;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
    }
}

```
