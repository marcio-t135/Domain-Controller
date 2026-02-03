# Windows Server: Active Directory Domain Controller Implementation

## Objective
The objective of this project was to implement and configure a complete network infrastructure for the company XPFO within a virtualized environment using VirtualBox. The project focused on the role of a systems administrator, establishing  Windows and Linux clients integrated into a managed domain. I did this project with the objective of refreshing knowladge of operationg systems such as windows and linux because its a very fundamental knowladge.

### Skills Learned

- Active Directory Administration: Installation and promotion of Windows Server 2019 as Domain Controller.
- Network Services Management: Configuration of DHCP for dynamic IP assignment and DNS for name resolution.
- File System Resilience: Implementation of DFS Namespaces and DFS Replication for centralized and redundant storage.
- Identity & Access Control: Organizing users into Organizational Units (OUs) and applying Group Policy Objects (GPOs).
- Security Auditing: Setting up event logs for failed login attempts and file manipulation.
- Automated Software Deployment: Distributing software packages across the domain via GPO

### Tools Used

- VirtualBox: Used for creating the virtual lab environment.
- Windows Server 2019: Operating system used for both the primary Domain Controller (DC-01) and the File Server (DFS-01).
- Active Directory Domain Services (AD-DS): For centralized management of users, groups, and permissions.
- Distributed File System (DFS): To manage shared folders and replication.
- GPO (Group Policy Object): To enforce security rules and environment settings.
- Linux & Windows Clients: Workstations used to validate domain connectivity and policies.

## Steps
Infrastucture and system Design and Planning.

<img width="632" height="700" alt="image" src="https://github.com/user-attachments/assets/18143548-d49b-4a2d-a269-794e5145fdb3" />

*Ref 1: Network Diagram*

## Services especifications

| VM Name | CPU | RAM | Disk | Operating System | Installed Services |
| :--- | :---: | :---: | :---: | :--- | :--- |
| **Windows_Server_DC** | 2 | 4GB | 40GB | Windows Server 2019 | Active Directory (AD-DS), DNS, DHCP  |
| **Windows_Server_DFS** | 2 | 4GB | 35GB | Windows Server 2019 | DFS Namespace, DFS Replication |
| **CLIENTE_LINUX** | 2 | 2GB | 25GB | Ubuntu Desktop 22.04.1 | Domain Connectivity & Integration Tests  |
| **CLIENTE_WINDOWS** | 2 | 2GB | 25GB | Windows Client* | Domain Connectivity & GPO Validation  |

## Documentation

<a href="https://github.com/marcio-t135/Enterprise-Network-Design-and-Implementation-Cisco-Packet-Tracer-/blob/main/Enterprise%20Network.pdf">Cisco packet tracer lab</a> 


