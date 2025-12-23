# Home Lab Infrastructure: Hybrid Linux/Windows Environment

## Project Overview
Designed and deployed a hybrid network environment to simulate enterprise IT infrastructure. This project demonstrates proficiency in Linux system administration, network security, web server deployment, and cross-platform interoperability.

**Tech Stack:**
* **OS:** Ubuntu Linux (Server), Windows 11 (Client)
* **Services:** Apache HTTP Server, Samba (SMB/CIFS), OpenSSH
* **Security:** SSH Key-Based Authentication (Ed25519)
* **Tools:** PowerShell, Nano, Linux CLI

---

## 1. Secure Remote Administration (SSH)
**Objective:** Replace password-based login with cryptographic key authentication for secure server management.
* Generated Ed25519 key pairs using PowerShell.
* Configured `authorized_keys` on the Linux server.
* Successfully established a password-less remote session.

![SSH Authentication Evidence](ssh-auth.png)

---

## 2. Internal Web Server Deployment
**Objective:** Host a custom internal website accessible via mobile and desktop clients.
* Installed and configured **Apache2** on Ubuntu.
* Modified HTML content via command line editors (`nano`).
* Configured local DNS (`hosts` file) to map `www.josh-lab.com` to the server IP.

![Apache Server Evidence](apache-server.png)

---

## 3. Cross-Platform File Sharing (Samba)
**Objective:** Bridge the gap between Linux and Windows file systems.
* Configured **Samba** to share the `/var/www/html` directory.
* Mapped the network drive in Windows 11.
* Verified "Read/Write" access by creating files on the server directly from Windows Explorer.

![Samba Share Evidence](samba-share.png)

---

## 4. User Account Management
**Objective:** Practice standard SysAdmin onboarding tasks.
* Created new user accounts using `adduser`.
* Verified user creation via the `/etc/passwd` file.
* Managed permissions and sudo group access.

![User Management Evidence](user-management.png)
