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
I. Installing VMWare Workstation Pro
  
Navigate to the official VMware Workstation Pro website and download the software from the Broadcom website.

1. Go to the [VMware Workstation Pro download page](https://www.vmware.com/products/desktop-hypervisor.html).
2. Click **Login** in the upper-right corner of the page.
3. If you do not already have a Broadcom account, select **Register** to create one.
4. Complete the registration process and sign in to your Broadcom account.
5. Once signed in, proceed with the download of **VMware Workstation Pro**.
6. After downloading the installer, go ahead and install VMWare Workstation Pro.

<img width="1679" height="864" alt="Broadcom Vmare Screenshot" src="https://github.com/user-attachments/assets/bc475107-106a-4aec-860d-c64ac60aca71" />



II. Creating a new Virtual Machine on VMWare Workstation Pro with Windows Server 2025
ISO
# Installing Windows Server 2025 on VMware Workstation Pro

1. Download the **Windows Server 2025 evaluation ISO** from the Microsoft link below. Complete the registration for the free trial and select **English (United States)** and the **64-bit ISO** edition.

https://info.microsoft.com/ww-landing-evaluate-windows-server-2025.html

2. Open **VMware Workstation Pro** and select **Create a New Virtual Machine**.

3. Select **I will install the operating system later** and click **Next**.

4. Under **Guest Operating System**, select **Microsoft Windows**. From the version dropdown, select **Windows Server 2025** and click **Next**.

5. Enter a name for the virtual machine and select where you want to save it. Click **Next**.

6. Continue through the **Specify Disk Capacity** section and click **Customize Hardware**.

7. Select **CD/DVD (SATA)**. Under **Connection**, select **Use ISO image file**, then click **Browse** and select the Windows Server 2025 ISO downloaded earlier. Click **Close**.

8. Click **Finish** to create the virtual machine.

The Windows Server 2025 virtual machine is now created and ready for installation.





<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
