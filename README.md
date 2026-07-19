# Enterprise Ansible Linux Administration project

## Project Overview

this project demonstrates enterprise Linux server administration using Ansible

the infrastructure consists of four Linux servers managed from one Ansible Control Node

## Architecture

Admin Server (Ansible Control Node)

|
v

Web Server(Apache)

|
v

File Server(NFS)

|
v

Backup Server(Automated Backups)

## Features

-Automated package installation
-Apache Web Server deployment
-NFS File Server configuration
-NFS Client configuration
-Automated Backup Server
-Compressed Backups(.tar.gz)
-Scheduled backups using Cron
-Backup logging
-Git version control

## Technologies Used

-RHEL / Rocky Linux
-Ansible
-Apache HTTP Server
-NFS
-Cron
-Bash
-Git
-GitHub

## Project Structure

enterprise-ansible-project/

|---- ansible.cfg
|---- inventory/
|---- playbooks/
|---- README.md

## Author

Shravani Jadhav
