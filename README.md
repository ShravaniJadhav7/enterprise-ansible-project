# Enterprise Ansible Linux Administration Project

## Project Overview

This project demonstrates Enterprise Linux Server Administration using Ansible in a multi-server environment.

The project automates server configuration, web server deployment, file sharing, and backup management using Ansible playbooks.

It was built on VirtualBox using four Linux virtual machines to simulate a real enterprise infrastructure.

---

# Architecture

```
                   +----------------------+
                   |  Admin Server        |
                   | (Ansible Control)    |
                   +----------+-----------+
                              |
          ------------------------------------------
          |                  |                     |
          |                  |                     |
+----------------+   +----------------+   +----------------+
|  Web Server    |   |  File Server   |   | Backup Server  |
|    Apache      |   |      NFS       |   | Automated      |
|                |   | Shared Storage |   | Backups        |
+----------------+   +----------------+   +----------------+
```

---

# Technologies Used

- Linux (RHEL/CentOS)
- Ansible
- Apache HTTP Server
- NFS
- Bash Shell Scripting
- Cron Jobs
- Git
- GitHub
- VirtualBox

---

# Project Features

- Automated package installation
- Apache Web Server deployment
- NFS Server configuration
- NFS Client configuration
- Automated Backup Server
- Backup logging
- Scheduled Cron jobs
- Compressed backups (.tar.gz)
- Linux administration automation
- Passwordless SSH authentication
- Centralized configuration management using Ansible

---

# Project Structure

```
enterprise-ansible-project/
│
├── ansible.cfg
├── inventory/
│   └── hosts
├── playbooks/
│   ├── apache.yml
│   ├── nfs_server.yml
│   ├── nfs_client.yml
│   ├── backup.yml
│   └── packages.yml
├── README.md
└── .gitignore
```

---

# Servers Used

| Server | Purpose |
|---------|---------|
| admin.example.com | Ansible Control Node |
| web.example.com | Apache Web Server |
| file.example.com | NFS File Server |
| backup.example.com | Automated Backup Server |

---

# Tasks Automated

- Install packages
- Configure Apache
- Configure NFS Server
- Configure NFS Clients
- Mount shared storage
- Create backup directory
- Compress backups
- Configure Cron jobs
- Generate backup logs

---

# Verification Commands

```bash
ansible all -m ping

systemctl status httpd

showmount -e

df -h

crontab -l

ls /backup

cat /var/log/backup.log
```

---

# Future Improvements

- Ansible Roles
- Dynamic Inventory
- Jenkins CI/CD Integration
- Docker Deployment
- Monitoring with Prometheus & Grafana
- Ansible Vault for Secrets Management

---

# Screenshots

Screenshots will be added here:

- Apache Web Page
- Ansible Ping Output
- NFS Shared Directory
- Backup Logs
- Cron Job Configuration

---

# Author

**Shravani Jadhav**

Electronics & Telecommunication Engineering Student

Aspiring Linux System Administrator | RHCSA Certified | Cloud & DevOps Enthusiast

---

⭐ If you found this project helpful, feel free to star the repository.
