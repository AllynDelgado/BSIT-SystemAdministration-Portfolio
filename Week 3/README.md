# Week 03 – Enterprise Server Deployment and Operating System Installation

**Student:** Allyn Jade L. Delgado  
**Course:** ITEP 414 – System Administration and Maintenance  
**Project:** Week 03 Portfolio  
**Repository:** BSIT-SystemAdministration-Portfolio  

---

## 1. Project Introduction

The Week 03 activity focuses on the deployment of an Ubuntu Server operating system inside a virtual machine. The purpose of the activity is to develop practical knowledge in Linux server installation, basic configuration, system verification, and server administration.

The virtual server will serve as a starting point for future enterprise services. These may include file sharing, remote management, web services, databases, and other internal network applications.

This activity also introduces important concepts related to computer firmware and startup procedures, particularly the differences between BIOS and UEFI and the stages involved when an Ubuntu Server system starts.

---

## 2. Objectives

At the end of this activity, I should be able to:

- Explain the role of an operating system in a server environment.
- Identify the main differences between BIOS and UEFI.
- Describe the basic stages of the computer boot process.
- Compare Ubuntu Server with Windows Server and Rocky Linux.
- Deploy Ubuntu Server using a virtual machine.
- Configure basic server settings.
- Create and use an administrative account.
- Configure SSH for remote administration.
- Test network and server functionality.
- Document the installation and configuration process.
- Organize technical documentation in a professional manner.

---

## 3. Virtual Machine Configuration

The Ubuntu Server virtual machine was configured according to the requirements of the Week 03 activity.

| Component | Configuration |
|---|---|
| Virtual Machine Name | Ubuntu-Server-Week03 |
| Memory | 4 GB RAM |
| Processor | 2 Virtual CPUs |
| Storage | 40 GB |
| Disk Type | VDI/VMDK |
| Network Mode | NAT / Bridged when required |
| Operating System | Ubuntu Server LTS |
| Hostname | `server01` |

These settings provide the virtual machine with enough resources to perform the required server installation and basic administration tasks.

---

## 4. Ubuntu Server Installation

Ubuntu Server was installed as a virtual machine. Before starting the installation, the required memory, processor, storage, and network settings were configured.

During the operating system installation, the English language and appropriate keyboard settings were selected. The network was configured using DHCP so that the server could automatically obtain an IP address from the available network.

The hostname was set to:

`server01`

A regular administrative account was created instead of relying on the root account for normal administration. Disk installation was performed using the guided option to use the available disk space.

OpenSSH Server was selected so that the server could later be administered remotely. After the installation finished, the virtual machine was restarted and the installation media was removed.

---

## 5. Basic Server Configuration

The main server configuration can be summarized as follows:

- **Hostname:** `server01`
- **Network Configuration:** DHCP
- **Storage:** 40 GB
- **Administrative Account:** Configured
- **SSH:** OpenSSH Server enabled
- **Operating System:** Ubuntu Server LTS
- **Additional Software:** Only packages required by the activity

The configuration was kept simple because the purpose of this activity was to establish a functional base server for future administration tasks.

---

## 6. Server Verification

After installation, several Linux commands were used to check whether the server was operating correctly.

### 6.1 Checking the Hostname

Command:

`hostname`

Expected output:

`server01`

This command confirms the identity assigned to the server.

### 6.2 Checking the Network Interface

Command:

`ip addr`

Assigned IP address:

`[ENTER YOUR ACTUAL IP ADDRESS]`

The `ip addr` command displays the available network interfaces and their assigned addresses.

### 6.3 Testing Internet Connectivity

Command:

`ping -c 4 google.com`

Result:

`[ENTER YOUR ACTUAL RESULT]`

A successful response indicates that the server can communicate with an external network.

### 6.4 Updating the System

Commands:

`sudo apt update`

`sudo apt upgrade -y`

Result:

`[ENTER YOUR ACTUAL RESULT]`

Updating the package information and installed packages helps keep the server environment current.

### 6.5 Checking the SSH Service

Command:

`systemctl status ssh`

Expected status:

`active (running)`

The SSH service allows authorized administrators to manage the server through a secure remote connection.

Screenshots of the installation and verification activities should be placed in the appropriate `screenshots/` folder in the repository.

---

## 7. BIOS and UEFI Comparison

BIOS and UEFI are firmware technologies responsible for initializing computer hardware and starting the operating system.

| Category | BIOS | UEFI |
|---|---|---|
| Purpose | Initializes hardware and begins the boot process | Performs hardware initialization and provides a modern boot environment |
| Partitioning | Commonly associated with MBR | Commonly used with GPT |
| Storage Support | More limited with traditional MBR configurations | Better support for large storage devices |
| Security | Provides basic firmware-level controls | Can support features such as Secure Boot |
| Interface | Usually text-based and limited | Can provide a more flexible interface |
| Modern Systems | Mostly found on older or legacy systems | Common on current computers |

UEFI is generally preferred on modern systems because it works well with newer hardware, GPT partitioning, large storage devices, and security features such as Secure Boot.

---

## 8. Ubuntu Server Boot Process

When an Ubuntu Server computer starts, several components work together before the user reaches the login screen.

The general sequence is:

Power On  
↓  
BIOS / UEFI  
↓  
Hardware Initialization  
↓  
Boot Device Selection  
↓  
GRUB Boot Loader  
↓  
Linux Kernel  
↓  
systemd Initialization  
↓  
System Services Start  
↓  
Login Prompt

### Explanation

**Power On**  
The computer receives power and begins the startup process.

**BIOS / UEFI**  
The firmware initializes hardware and determines how the system should begin booting.

**Boot Device Selection**  
The firmware identifies the device containing the operating system.

**GRUB**  
GRUB acts as the boot loader and loads the Linux operating system.

**Linux Kernel**  
The kernel takes control of the system and manages hardware and core operating-system functions.

**systemd**  
Ubuntu uses systemd to initialize the system and manage services.

**System Services**  
Required services are started so the server can perform its intended functions.

**Login Prompt**  
Once initialization is complete, the user can log in and begin using the server.

---

## 9. Operating System Comparison

Ubuntu Server, Windows Server, and Rocky Linux are all operating systems that can be used for server environments, but they differ in design and administration.

| Feature | Ubuntu Server | Windows Server | Rocky Linux |
|---|---|---|---|
| Base | Debian-based Linux | Windows NT family | Enterprise Linux compatible |
| Administration | Command line and web-based tools | GUI and PowerShell | Mainly command line |
| Package Management | APT | Windows package/role management tools | DNF |
| Typical Use | Web servers, cloud, development, infrastructure | Microsoft-based enterprise environments | Enterprise Linux servers |
| Licensing | Open source | Commercial licensing | Open source |
| Desktop GUI | Usually not installed by default | Commonly available | Usually server-focused |

Ubuntu Server is useful for learning Linux administration because it provides a lightweight server environment and a large ecosystem of open-source software. Windows Server is especially useful in organizations that depend on Microsoft technologies. Rocky Linux is another Linux option designed for enterprise-style server environments.

---

## 10. Challenges and Solutions

### Challenge 1 – Virtual Machine Configuration

**Problem:**  
The virtual machine required several settings to be configured correctly before the operating system could be installed.

**Solution:**  
The RAM, processor, storage, and network configuration were reviewed before starting the installation.

### Challenge 2 – Server Verification

**Problem:**  
It is necessary to confirm that the newly installed server can communicate with the network and that important services are operating.

**Solution:**  
Linux commands such as `ip addr`, `ping`, and `systemctl status ssh` were used to verify the network connection and SSH service.

If no significant problems were encountered during the actual installation, the following statement may be used:

> No major problems were encountered during the installation and initial configuration of the Ubuntu Server virtual machine.

---

## 11. Reflection

The Week 03 activity gave me a better understanding of how an operating system is deployed and prepared for use as a server. Instead of simply installing an operating system, I learned that a server also needs proper configuration and testing before it can be considered ready for administration.

One of the main skills I developed was creating an Ubuntu Server virtual machine. I learned how the virtual machine's memory, processor, storage, and network settings affect the installation. I also practiced configuring a hostname, creating an administrative account, setting up storage, and enabling SSH.

The verification process was another important part of the activity. Commands such as `hostname`, `ip addr`, `ping`, `apt update`, `apt upgrade`, and `systemctl status ssh` helped me understand how administrators check the condition of a Linux server. These commands provide information about the server identity, network configuration, software packages, and running services.

I also learned more about BIOS and UEFI and their role during startup. Understanding the relationship between firmware, the boot loader, Linux kernel, systemd, and system services made the boot process easier to understand.

Another lesson I gained from this activity was the importance of documentation. Server administrators need accurate records of configurations and procedures so that systems can be maintained or reproduced when necessary.

Overall, this project improved my understanding of Linux server deployment and basic system administration. The skills learned in this activity can be applied to future topics involving virtualization, networking, server management, and enterprise infrastructure.

---

## 12. References

- Laguna State Polytechnic University. *ITEP 414 – System Administration and Maintenance, Week 3 Portfolio Project: Enterprise Server Deployment and Operating System Installation.*
- Ubuntu Server Documentation.
- Oracle VirtualBox Documentation.
- Microsoft Windows Server Documentation.
- Rocky Linux Documentation.

---

## 13. Repository Organization

BSIT-SystemAdministration-Portfolio/
│
└── Week 03/
    ├── screenshots/
    ├── BIOS_vs_UEFI.pdf
    ├── BootProcessFlowchart.pdf
    ├── InstallationGuide.pdf
    ├── ProfessionalInstallationManual.pdf
    ├── references.pdf
    └── README.md

---

## 14. Project Checklist

- [ ] Ubuntu Server installed
- [ ] Virtual machine configured
- [ ] Hostname configured
- [ ] Keyboard settings configured
- [ ] Disk partition configured
- [ ] Administrative account created
- [ ] SSH installed and running
- [ ] Server login verified
- [ ] IP address recorded
- [ ] Internet connectivity tested
- [ ] System packages updated
- [ ] BIOS and UEFI comparison completed
- [ ] Ubuntu boot process documented
- [ ] Boot process flowchart completed
- [ ] Windows Server evaluation completed
- [ ] Ubuntu, Windows Server, and Rocky Linux comparison completed
- [ ] Installation Guide completed
- [ ] Professional Installation Manual completed
- [ ] README.md completed
- [ ] Screenshots organized
- [ ] GitHub repository updated
- [ ] LinkedIn reflection completed

---

## 15. Project Status

The Week 03 portfolio is organized in the GitHub repository under the `Week 03` directory. The current repository includes the Week 03 README and the project documentation structure.

**Repository:**

BSIT-SystemAdministration-Portfolio – Week 03

**Repository Path:**

https://github.com/AllynDelgado/BSIT-SystemAdministration-Portfolio/tree/main/Week%203
