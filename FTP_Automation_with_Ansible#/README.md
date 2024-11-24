# 🛠️ Automating FTP Client and Server Setup with Ansible

This project automates the deployment and configuration of FTP clients and servers using **Ansible**. It consists of three modular playbooks, each with a specific role, ensuring a clean and efficient setup for FTP infrastructures.

---

## 📋 Playbooks Overview

### 1️⃣ **Client Setup Playbook**
- Ensures the lftp package is installed on systems designated as FTP clients.
- Verifies the presence of the software and installs it if missing.
- Guarantees all client systems are consistent and ready for file transfers.

### 2️⃣ **Server Setup and Configuration Playbook**
- Installs and configures the vsftpd service on systems that act as FTP servers.
- Manages the configuration file to ensure secure and reliable operation.
- Provides flexibility for tailoring the server to your specific requirements.

### 3️⃣ **Site Playbook (site.yml)**
- Orchestrates the execution of both the **Client Setup** and **Server Setup** playbooks.
- Simplifies deployment by enabling a single command to configure both clients and servers.
