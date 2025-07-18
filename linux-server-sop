# Standard Operating Procedure (SOP)  
## Setting Up a Virtual Linux Server for Web Application Testing

---

### Company Information  
**Company Name:** Olajuwon Ltd.  
**Address:** 1234 Tech Lane, Innovation City, 56789  
**Contact:** IT Department — +1 (555) 123-4567  

---

### Revision History  

| Version | Date       | Author           | Description              |
|---------|------------|------------------|--------------------------|
| 1.0     | 2025-07-17 | Olajuwon Abbatty | Initial version          |

---

### Approval Table  

| Version | Date       | Name             | Role               | Signature |
|---------|------------|------------------|--------------------|-----------|
| 1.0     | 2025-07-17 | Olajuwon Abbatty | IT Engineer        |           |
| 1.0     | 2025-07-17 | Jane Doe         | IT Manager         |           |

---

### Purpose  
This document provides a standardized process for setting up a virtual Linux server designed for web application testing. It ensures a reliable, secure, and reproducible environment for developers and testers.

---

### Scope and Objectives  
This SOP is intended for IT staff and DevOps engineers who manage virtual environments and testing infrastructure. It applies whenever a new Linux-based virtual machine is required for testing web apps.

**Objectives include:**  
- Deploying a virtual machine using Ubuntu Server 22.04 LTS  
- Installing and configuring a LAMP stack (Linux, Apache, MySQL, PHP)  
- Enabling network access and applying basic security settings  
- Documenting system configuration for future reference

---

### Accountability Matrix  

| Task                               | Responsible Team        | Approver         |
|------------------------------------|--------------------------|------------------|
| Virtual Machine Creation           | Infrastructure Team      | IT Manager       |
| Linux OS Installation              | System Administrators    | IT Manager       |
| Web Stack Setup                    | DevOps Team              | DevOps Lead      |
| Networking & Security Configuration| Network Security Team    | Security Officer |
| Documentation                      | Documentation Team       | IT Manager       |

---

### Definitions  

| Term     | Description                                              |
|----------|----------------------------------------------------------|
| VM       | Virtual Machine – A software-based simulation of a physical computer |
| OS       | Operating System                                          |
| LAMP     | Software stack consisting of Linux, Apache, MySQL, PHP   |
| SSH      | Secure Shell – A protocol for remote login               |
| UFW      | Uncomplicated Firewall – A firewall management tool for Ubuntu |

---

### Procedure Steps  

**Step 1: Create the Virtual Machine**  
- Open your virtualization platform (e.g., VMware, VirtualBox).  
- Download Ubuntu Server ISO from [Ubuntu Downloads](https://ubuntu.com/download/server)  
- Create a new VM with the following specs:  
  - OS: Ubuntu Server 22.04 LTS  
  - Hostname: `webtest-server`  
  - CPU: 2 cores  
  - RAM: 4 GB  
  - Storage: 20 GB  
- Attach the Ubuntu ISO file and boot the VM.

**Step 2: Install Ubuntu Server**  
- Complete the guided installation process.  
- Set a secure password and enable OpenSSH Server during setup.  
- Configure network settings (DHCP or static IP as required).

**Step 3: Update the System**  
After the OS is installed and running:
sudo apt update && sudo apt upgrade -y

**Step 4: Install LAMP Stack
Install Apache, MySQL, and PHP using:
sudo apt install apache2 mysql-server php libapache2-mod-php php-mysql -y

Enable services to start on boot:
sudo systemctl enable apache2
sudo systemctl enable mysql


**Step 5: Test Web Server
Create a PHP test page:
echo "<?php phpinfo(); ?>" | sudo tee /var/www/html/index.php
Open a browser and navigate to the server’s IP address to verify PHP is working.

Step 6: Secure the Server

Enable the firewall and allow web traffic:
sudo ufw allow 'Apache Full'
sudo ufw enable

Run MySQL's secure installation script:
sudo mysql_secure_installation

Step 7: Document the Setup
Record system specs, network settings, installed software, and admin credentials.
Share documentation with relevant teams for maintenance and support.



Reference Documents
Ubuntu Server Guide
Apache HTTP Server Documentation
MySQL Secure Deployment Guide
Organization’s IT Security Policy

