# Home Lab Infrastructure: Hybrid Linux/Windows Environment

## Project Overview
Designed and deployed a hybrid network environment to simulate enterprise IT infrastructure. This project demonstrates proficiency in Linux system administration, network security, web server deployment, and cross-platform interoperability.

**Tech Stack:**
* **OS:** Ubuntu Linux (Server), Windows 11 (Client)
* **Services:** Apache HTTP Server, Samba (SMB/CIFS), OpenSSH
* **Security:** SSH Key-Based Authentication (Ed25519)
* **Tools:** PowerShell, Nano, Linux CLI




## 1. Secure Remote Administration (SSH)
**Objective:** Replace password-based login with cryptographic key authentication for secure server management.
* Generated Ed25519 key pairs using PowerShell.
* Configured `authorized_keys` on the Linux server.
* Successfully established a password-less remote session.

---![ssh-auth png](https://github.com/user-attachments/assets/8c64edf4-d790-4bc5-8885-8d84d521d4cc)



## 2. Internal Web Server Deployment
**Objective:** Host a custom internal website accessible via mobile and desktop clients.
* Installed and configured **Apache2** on Ubuntu.
* Modified HTML content via command line editors (`nano`).
* Configured local DNS (`hosts` file) to map `www.josh-lab.com` to the server IP.


---<img width="585" height="1266" alt="apache-server" src="https://github.com/user-attachments/assets/6d8593e1-3514-463c-abde-bea5fe643e04" />




## 3. Cross-Platform File Sharing (Samba)
**Objective:** Bridge the gap between Linux and Windows file systems.
* Configured **Samba** to share the `/var/www/html` directory.
* Mapped the network drive in Windows 11.
* Verified "Read/Write" access by creating files on the server directly from Windows Explorer.


---![samba-share png](https://github.com/user-attachments/assets/f60f1d72-94c7-4cda-9e9d-9edefa31f7e5)


## 4. User Account Management
**Objective:** Practice standard SysAdmin onboarding tasks.
* Created new user accounts using `adduser`.
* Verified user creation via the `/etc/passwd` file.
* Managed permissions and sudo group access.


---![user-management](https://github.com/user-attachments/assets/5884d0c4-a79d-46ac-9997-47f5576cc014)

## 5. System Visualization
**Objective:** Displayed comprehensive system hardware and software configuration using command-line utilities.
* Installed **Neofetch** to visualize OS version, Kernel, and Uptime.
* Verified resource usage and shell configuration (Bash).

---![neo-fetch](https://github.com/user-attachments/assets/aca1bbbe-280e-43fe-b39b-2ee5ebecf9cf)

