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

<h2>Configuration Steps</h2>

![image](https://github.com/user-attachments/assets/f144c578-dc29-4722-af7f-8e55112e8a2a)

osTicket Links:

Admin/Analyst [Login Page](http://localhost/osTicket/scp/login.php)

End Users [osTicket URL](http://localhost/osTicket)

<br />

![image](https://github.com/user-attachments/assets/ff85c8b0-c096-4bab-aa13-ef1fb20f145a)
<p>
1) Configure Roles (for grouping permissions)

Admin Panel -> Agents -> Roles

Supreme Admin (All Permissions)(Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/89a8ce87-9e8f-4449-86d0-86a2871d0ade)
<p>
2) Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)

Admin Panel -> Agents -> Departments

Create SysAdmins department (Example)

Delete Maintenance department (Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/06097918-c2a6-4394-a90f-0a6307a6e417)
<p>
3) Configure Teams

Admin Panel -> Agents -> Teams (Pull Agents from different Departments)

Online Banking (Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/a19abcce-0489-48eb-9a58-7ea197402a80)
<p>
4) Allow anyone to create tickets

Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)

Registration Required: Require registration and login to create tickets 
</p>
<br />

![image](https://github.com/user-attachments/assets/2cf81b15-788d-44f2-942e-596372387c7d)
<p>
5) Configure Agents (workers)

Admin Panel -> Agents -> Add New

Jane (Dept: SysAdmins)(Example)

John (Dept: Support)(Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/8680d755-0e35-4735-888a-a9d1bfa94eff)
<p>
6) Configure Users (customers)

Agent Panel -> Users -> Add New

Karen (Example)

Ken (Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/23d8bc95-d37c-4e27-8f4c-0a8762f2bd68)
<p>
7) Configure SLA

Admin Panel -> Manage -> SLA

Sev-A (Grace Period: 1 hour, Schedule: 24/7)(Example)

Sev-B (Grace Period: 4 hours, Schedule: 24/7)(Example)

Sev-C (Grace Period: 8 hours, Business Hours)(Example)
</p>
<br />

![image](https://github.com/user-attachments/assets/acfc0a64-5632-486d-a986-57d182756de8)
8) Configure Help Topics (For when users create a ticket)

Admin Panel -> Manage -> Help Topics

Business Critical Outage (Example)

Personal Computer Issues (Example)

Equipment Request (Example)

Password Reset (Example)

Other (Example)
</p>
<br />
