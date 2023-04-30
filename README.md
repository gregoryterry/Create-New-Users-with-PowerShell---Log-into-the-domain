# Create-New-Users-with-PowerShell---Log-into-the-domain

<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
<img src="" alt="PowerShell ISE Logo"/>
</p>

<h1>Create several domain users and attempt to log into client GTWS-01 (Azure)</h1>
This tutorial outlines the creation for new users using PowerShell on Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Login to DC01 as an Domain Admin and Open PowerShell ISE as an administrator
- Run the script to create new users
- Open Active Directory Users and Computers to see the new user accounts in the OU
- Using one of the new users, login to Client computer GTWS-01


<h2>Deployment and Configuration Steps</h2>

<h4>Login to DC01 as an Domain Admin and Open PowerShell ISE as an administrator</h4>

<p>On the DC01 desktop > search > PowerShell ISE > Run as Administrtor
p
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<p>I will run this script to create new users in the EMPLOYEES OU
<p>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<p>On DCO1 > Active Directory Users and Computers > Expand the Domain down to EMPLOYEES OU

Here are the new users that were created in the EMPLOYEES OU
<p>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<p>All the accounts are disabled > right-click an account > enable
<p>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>


<h4>Using one of the new users login to Client computer GTWS-01<h/4>

<p>Enter the password
The users is logging on to the domain
<p>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>

<p>Open a command prompt:	cmd
Check to see which user is logged into GTWS-01	“whoami”  and “hostname” to display the computer name
<p>
<img src="" height="70%" width="70%" alt="Disk Sanitization Steps"/>
