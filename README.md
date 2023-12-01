<h1>Active Directory Home Lab</h1>

 
<h2>Description</h2>
This project consists of a guide to creating an Active Directory Home Lab utilizing virtual machines. The focus is on establishing a functional Active Directory environment on a personal computer. These snapshots cover some key components such as deploying Windows Server operating systems, configuring domains, and implementing user accounts. A notable aspect of this project is the integration of PowerShell scripting for efficient automation. I provide a snapshot on utilizing PowerShell to generate and deploy 1,000 users seamlessly on the internal network. This project serves as a resource for someone seeking a brief understanding on Active Directory setup and highlights the key steps, including the role PowerShell has in streamlining administrative tasks within the context of a home lab environment.
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 


<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Oracle Virtual Box</b>

<h2>Program walk-through:</h2>

<p align="center">
Download Virtual Box and Install Windows 10 ISO on the first Virtual Machine (Domain Controller): <br/>
<img src="https://imgur.com/jGnqwdC.png" height="80%" width="80%" alt="Active-Directory-Home-Lab"/>
<br />
<br />
Rename networks on the Domain Controller for Home Internet and Internal Network: <br/>
<img src="https://imgur.com/Qgt46lK.png" height="80%" width="80%" alt="Active-Directory-Home-Lab"/>
<br />
<br />
Assign IP address for Internal Network: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Active Directory on the Domain Controller:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Domain for Active Directory:  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Remote Access so the clients on Internal Network can connect to the internet through the Domain Controller:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Configure NAT:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set DCHP on Domain Controller so when we create our second virtual machine it can automatically get an IP address:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run Powershell script for users on the Active Directory:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create another Virtual Machine to connect Internal Network (CLIENT1), join it to the domain, and log in with one of the user accounts:  <br/>
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
