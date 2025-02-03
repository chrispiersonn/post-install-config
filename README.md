<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Create an Azure Virtual Machine Windows 10 
- osTicket Installed

<h2>Configuration Steps</h2>

![image](https://github.com/user-attachments/assets/f144c578-dc29-4722-af7f-8e55112e8a2a)

osTicket Links:

Admin/Analyst [Login Page](http://localhost/osTicket/scp/login.php)

End Users [osTicket URL](http://localhost/osTicket)

<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1) Configure Roles (for grouping permissions)

Admin Panel -> Agents -> Roles

Supreme Admin (All Permissions)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2) Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)

Admin Panel -> Agents -> Departments

SysAdmins
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3) Configure Teams

Admin Panel -> Agents -> Teams (Pull Agents from different Departments)

Online Banking
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4) Allow anyone to create tickets

Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)

Registration Required: Require registration and login to create tickets 
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5) Configure Agents (workers)

Admin Panel -> Agents -> Add New

Jane (Dept: SysAdmins)

John (Dept: Support)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6) Configure Users (customers)

Agent Panel -> Users -> Add New

Karen

Ken
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7) Configure SLA

Admin Panel -> Manage -> SLA

Sev-A (Grace Period: 1 hour, Schedule: 24/7)

Sev-B (Grace Period: 4 hours, Schedule: 24/7)

Sev-C (Grace Period: 8 hours, Business Hours)
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8) Configure Help Topics (For when users create a ticket)

Admin Panel -> Manage -> Help Topics

Business Critical Outage

Personal Computer Issues

Equipment Request

Password Reset

Other
</p>
<br />
