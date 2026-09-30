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
<img src="https://imgur.com/a/JBTIZp0" height="80%" width="80%" alt=/>
<br />
<br />
Select the disk:  <br/>
<img src="https://imgur.com/a/JBTIZp0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
