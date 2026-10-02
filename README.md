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

# 1. Installing VMware Workstation Pro  
  
I downloaded and installed VMware Workstation Pro and created a Broadcom account to access the VMware downloads.

Steps:

1. Go to the [VMware Workstation Pro download page](https://www.vmware.com/products/desktop-hypervisor.html).
2. Click **Login** in the upper-right corner of the page.
3. If you do not already have a Broadcom account, select **Register** to create one.
4. Complete the registration process and sign in to your Broadcom account.
5. Once signed in, proceed with the download of **VMware Workstation Pro**.
6. After downloading the installer, go ahead and install VMWare Workstation Pro.

<img width="1679" height="864" alt="Broadcom Vmare Screenshot" src="https://github.com/user-attachments/assets/bc475107-106a-4aec-860d-c64ac60aca71" />



# 2. Creating a new Virtual Machine on VMWare Workstation Pro with Windows Server 2025 ISO

I downloaded the Windows Server 2025 evaluation ISO directly from Microsoft.


1. Download the **Windows Server 2025 evaluation ISO** from the Microsoft link below. Complete the registration for the free trial and select **English (United States)** and the **64-bit ISO** edition.
https://info.microsoft.com/ww-landing-evaluate-windows-server-2025.html

<img width="432" height="453" alt="Microsoft vmare " src="https://github.com/user-attachments/assets/e6fd0c67-480e-42ee-9f5b-ba3ee1d14066" />

3. Open **VMware Workstation Pro** and select **Create a New Virtual Machine**.
4. Select **I will install the operating system later** and click **Next**.

<img width="1529" height="849" alt="Vmware New virtual machine" src="https://github.com/user-attachments/assets/9036ccc3-2dc8-45cd-95f3-fe3f99516458" />
   
5. Under **Guest Operating System**, select **Microsoft Windows**. From the version dropdown, select **Windows Server 2025** and click **Next**.
6. Enter a name for the virtual machine and select where you want to save it. Click **Next**.
7. Continue through the **Specify Disk Capacity** section and click **Customize Hardware**.
8. Select **CD/DVD (SATA)**. Under **Connection**, select **Use ISO image file**, then click **Browse** and select the Windows Server 2025 ISO downloaded earlier. Click **Close**.
9. Click **Finish** to create the virtual machine.

<img width="676" height="595" alt="VM machine created" src="https://github.com/user-attachments/assets/7413109f-1ed0-4ae9-b8bf-8a6418543d44" />

The Windows Server 2025 virtual machine is now created and ready for installation.


# 3. Creating the Virtual Machine


I created a new virtual machine in VMware Workstation Pro and configured it to use the Windows Server 2025 ISO.

Configuration process:

1. Go to the Microsoft Windows Server 2025 evaluation page.
2. Register for the free evaluation.
3. Select:
   - English (United States)
   - ISO download
   - 64-bit
4. Download the Windows Server 2025 ISO.


# 4. Create the Windows Server Virtual Machine
1. Open VMware Workstation Pro.
2. Select Create a New Virtual Machine.
3. Select I will install the operating system later.
4. Select Microsoft Windows.
5. Select Windows Server 2025.
6. Enter a name for the virtual machine.
7. Continue to Specify Disk Capacity.
8. Select Customize Hardware.


Configure the ISO

10. Select New CD/DVD (SATA).
11. Select Use ISO image file.
12. Browse to the Windows Server 2025 ISO.
13. Select Close.
14. Click Finish.
The Windows Server virtual machine is now created.

# 5. Install Windows Server 2025

1. Right-click the virtual machine.
2. Select Power On.
3. Click inside the VM and press a key to start Windows Setup.
4. Select Next on the language screen.
5. Select Install Now.
6. Select: Windows Server 2025 Standard Evaluation (Desktop Experience)
7. Accept the license terms.
8. Select Custom: Install Windows only (advanced).
9. Select the Unallocated Space drive.
10. Click Next.
11. Wait for Windows Server to finish installing.
12. The VM will restart automatically.
13. Create the Administrator password.
14. Log in to Windows Server.

# 6. Install VMware Tools

1. Power on the Windows Server VM.
2. From the VMware menu, select: VM → Install VMware Tools
3. Log in to Windows Server.
4. Open File Explorer.
5. Open This PC.
6. Locate the VMware Tools virtual CD/DVD drive.
7. Open the drive.
8. Run setup.exe.
9. Select Typical installation.
10. Follow the installation prompts.
11. Restart the virtual machine.


# 7. Lab Status

At this point, I have:
1. Installed VMware Workstation Pro
2. Downloaded Windows Server 2025
3. Created a Windows Server 2025 virtual machine
4. Installed Windows Server 2025
5. Created the Administrator account
6. Installed VMware Tools
7. Restarted the Windows Server VM
  
Next: Configure the Windows Server environment for the Active Directory lab.



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
