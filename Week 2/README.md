# ABC Startup Solutions – Enterprise Infrastructure Planning

## Project Overview

This project is the Week 2 Portfolio Project for **ITEP 414 – System Administration and Maintenance**.

The project focuses on creating an **Enterprise Infrastructure Plan** for a newly established software development company called **ABC Startup Solutions**. The company has 20 employees and operates on a single office floor.

The company starts with no computers, server, network, Internet infrastructure, or security policies. As a Junior System Administrator, the goal of this project is to plan the company's IT infrastructure before any equipment is purchased or deployed.

### Project Coverage

- Company profile and organizational structure
- Hardware inventory
- Software inventory
- Network equipment inventory
- Enterprise network topology
- System administration roles
- Infrastructure recommendations
- Security and backup planning
- Personal reflection

---

## Learning Objectives

This project aims to develop the following skills:

- Analyze organizational IT requirements
- Identify hardware, software, and networking requirements
- Prepare professional IT inventories
- Design an enterprise network topology
- Create technical documentation using Markdown
- Understand the responsibilities of System Administrators
- Develop practical infrastructure recommendations
- Improve technical communication and documentation skills

---

## Company Scenario

**ABC Startup Solutions** is a newly established software development company with **20 employees**.

| Department | Employees |
|---|---:|
| Information Technology | 5 |
| Human Resources | 4 |
| Finance | 5 |
| Sales | 6 |
| **Total** | **20** |

The company occupies a single office floor.

### Current Situation

The company currently has:

- No computers
- No server
- No network
- No Internet infrastructure
- No security policies

The purpose of this project is to plan the required IT infrastructure from scratch.

---

## Hardware Inventory

| Hardware | Quantity | Department | Purpose |
|---|---:|---|---|
| Desktop Computers | 15 | HR, Finance, Sales | Office productivity |
| Laptops | 5 | IT | Software development and administration |
| Server | 1 | IT | Centralized services |
| Router | 1 | IT | Internet and network routing |
| Managed Switch | 2 | IT | Network connectivity |
| Network Printer | 1 | Shared | Printing documents |
| UPS | 4 | IT / Shared | Power protection |
| Wireless Access Point | 2 | Shared | Wireless connectivity |
| NAS Storage | 1 | IT | Storage and backup |
| External Backup Drive | 2 | IT | Offline backup |
| Monitors | 20 | All Departments | Employee workstations |

---

## Software Inventory

| Software | Purpose |
|---|---|
| Windows 11 Pro | Operating system |
| Ubuntu Server | Server operating system |
| Microsoft Office | Documents and presentations |
| Visual Studio Code | Software development |
| Git | Source-code version control |
| GitHub Desktop | Git and GitHub management |
| VirtualBox | Virtual machine testing |
| Google Chrome | Web browsing |
| Microsoft Defender | Endpoint protection |
| AnyDesk | Remote technical support |
| 7-Zip | File compression |

---

## Enterprise Network Diagram

### Network Flow

```text
Internet
   |
ISP Modem
   |
Router
   |
Firewall
   |
Core Managed Switch
   |
   +-- Patch Panel
   |
   +-- Server
   |
   +-- NAS Storage
   |
   +-- Network Printer
   |
   +-- Wireless Access Points
   |
   +-- IT Department – 5 Employees
   |
   +-- HR Department – 4 Employees
   |
   +-- Finance Department – 5 Employees
   |
   +-- Sales Department – 6 Employees
```

### Network Diagram

![ABC Startup Solutions Network Diagram](diagrams/ABC-Network-Diagram.png)

The network diagram was created using **Draw.io (diagrams.net)**. It shows the Internet, ISP modem, router, firewall, core switch, patch panel, server, NAS storage, printer, wireless access points, and the four departments.

---

## Technologies Used

```text
Draw.io / diagrams.net
Windows 11 Pro
Ubuntu Server
Microsoft Office
Visual Studio Code
Git
GitHub
GitHub Desktop
VirtualBox
Google Chrome
Microsoft Defender
AnyDesk
7-Zip
CAT6 Ethernet
TCP/IP
VLAN
Firewall
NAS Storage
Network Switches
Wireless Networking
```

---

## Challenges Encountered

One of the challenges in this project was planning an IT infrastructure for a company that starts with no existing technology.

Another challenge was deciding how many computers and devices each department needed. The infrastructure needed to support all 20 employees while also allowing future expansion.

Creating the network diagram was also challenging because the modem, router, firewall, switch, patch panel, server, printer, wireless access points, and departments needed to be connected correctly.

Security and backup planning were also important because the company would handle business, employee, financial, and client information.

---

## Reflection

This project helped me understand why planning is important before setting up an IT infrastructure. I learned that a System Administrator needs to understand the company's needs before buying equipment, installing software, or configuring the network.

I learned how to prepare hardware, software, and network inventories and how to choose equipment based on the needs of each department. I also learned how routers, firewalls, switches, servers, and wireless access points work together.

The network diagram was one of the most challenging parts for me because I needed to organize all the devices into a clear and logical topology. Creating the diagram helped me understand how the different network devices connect and communicate.

Overall, this project helped me improve my planning, documentation, problem-solving, and system administration skills. It also showed me that good planning can help prevent problems, improve security, and make future expansion easier.

---

## References

1. **Laguna State Polytechnic University.** *ITEP 414 – System Administration and Maintenance: Week 2 Portfolio Project – Enterprise Infrastructure Planning for a Startup Company.*

2. **diagrams.net.** *Diagramming and Network Diagram Software.*

3. **Cisco.** *Networking Basics and Network Devices.*

---

## Project Structure

```text
BSIT-SystemAdministration-Portfolio/
│
└── Week02/
    │
    ├── ABC-Network-Diagram
    ├── README.md
    ├── References.pdf
    ├── Week 2 linkedin.png
    ├── Week2.png
```

---

## Author

**Name:** Allyn Jade L. Delgado

**Course:** ITEP 414 – System Administration and Maintenance

**Program:** Bachelor of Science in Information Technology

**Week:** 2

**Project:** Enterprise Infrastructure Planning for a Startup Company
