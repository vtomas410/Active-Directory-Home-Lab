<h1>Active Directory Home Lab</h1>

<h2>Description</h2>
This project documents the deployment and configuration of a Windows Server Active Directory environment using VMware Workstation Pro.

The goal of this home lab was to simulate a small enterprise IT environment and gain hands-on experience with Windows Server administration, Active Directory Domain Services (AD DS), DNS, user and group management, Group Policy, and Windows client administration.

This project was built as part of my IT/cybersecurity home lab to develop practical skills that are commonly used in Help Desk, System Administration, and Cybersecurity roles.
<br />


<h2>🎯 Objectives</h2>

- <b>Install Windows Server in VMware Workstation Pro</b>
- <b>Configure a virtualized Windows Server environment</b>
- <b>Configure a static IP address</b>
- <b>Install Active Directory Domain Services (AD DS)t</b>
- <b>Promote Windows Server to a Domain Controller</b>
- <b>Configure DNS</b>
- <b>Create an Active Directory domain</b>
- <b>Create organizational units (OUs)t</b>
- <b>Create users and security groups</b>
- <b>Join a Windows client computer to the domain</b>
- <b>Configure Group Policy</b>
- <b>Implement basic security policiest</b>
- <b>Practice common Active Directory administration tasks</b>
- <b>Document the entire deployment process</b>

<h2>🛠️ Technologies & Tools </h2>

- <b>VMware Workstation Pro: Virtualization platform<b>
- <b>Windows Server:	Domain Controller / Server<b>
- <b>Windows 10/11:	Domain client<b>
- <b>Active Directory Domain Services:	Identity and domain management<b>
- <b>DNS:	Name resolution<b>
- <b>Group Policy:	Centralized configuration and security<b>
- <b>PowerShell:	Windows administration<b>

<h2>🖥️ Lab Environment</h2>

              HOME NETWORK
                   │
                   |
            VMware Workstation
                   |
                   |
          ┌────────┴────────┐
          │                 │
        Admin             User01
          │                 │
          └────────┬────────┘
                   │
             Active Directory
                   │
            Tomashomelab.local
        

            
<h2>Program walk-through:</h2>

<p align="center">
 <br/>

---
Steps:
1. [Installing Active Directory](https://github.com/vtomas410/Installing-Active-Directory)
2. [Creating and Setting up GPO](https://github.com/vtomas410/Creating-And-Setting-Up-GPO)
3. [Windows Domain Join Group Policy Testing](https://github.com/vtomas410/Windows-Domain-Join-Group-Policy-Testing)
