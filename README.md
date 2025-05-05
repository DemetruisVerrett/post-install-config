<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [Clipchamp: How To Configure osTicket, post-installation](https://1drv.ms/v/c/5dac4edc6b620d54/Ed3lenkHFepHmWgKEXFMaL0Bz0z8JcMRWHWfwW97keGueg)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket System

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- osTicketing system Configurations:
  
-Ticket properties

-Agents

-Help Topics

-SLA

-Departments

-Roles/Permissions

-Users/Teams

<h2>Configuration Steps</h2>

<p>
  
![Image](https://github.com/user-attachments/assets/cb635b0f-9d50-48b3-9752-1dc53abf7163)

</p>
<p>
1.Admin/Analyst Login Page:
URL: http://localhost/osTicket/scp/login.php

This is where Admin and Analyst users log in to manage the osTicket system.

2.End Users osTicket URL:

URL: http://localhost/osTicket
This is the URL for end-users to access and submit support tickets.

3.Acknowledge Agent Panel vs Admin Panel:

The Agent Panel allows agents to manage tickets, assign them, and communicate with users.
The Admin Panel gives full access to system settings, configurations, and advanced user management.

4.Configure Roles:

Path: Admin Panel -> Agents -> Roles
You can define different roles for users, such as Supreme Admin, with specific permissions to control who can access certain features or settings.

5.Configure Departments:

Path: Admin Panel -> Agents -> Departments
Departments allow you to define ticket visibility, such as restricting tickets to certain groups like Help Desk, SysAdmins, or Networking.

6.Configure Teams:

Path: Admin Panel -> Agents -> Teams
Teams allow you to group agents from different departments. For example, you can create a Online Banking team, pulling agents from various departments.

7.Allow Anyone to Create Tickets:

Path: Admin Panel -> Settings -> User Settings
UNCHECK the option to allow unregistered users to create tickets. This ensures that users must register and log in to submit tickets.
Registration Required: Enable the "Require registration and login to create tickets" option for more control over who can create tickets.

This setup allows for a flexible and organized ticketing system with clear roles, permissions, and team structures.
</p>
<br />

<p>
  
![Image](https://github.com/user-attachments/assets/873f465c-c968-49c4-8f9c-3f3435bc9c26)

</p>
<p>
1.Configure Agents (Workers):


Path: Admin Panel -> Agents -> Add New
Jane: Assigned to SysAdmins department.
John: Assigned to Support department.

2.Configure Users (Customers):


Path: Agent Panel -> Users -> Add New
Karen and Ken are added as users (customers) in the system.

3.Configure SLA (Service Level Agreements):


Path: Admin Panel -> Manage -> SLA
Sev-A: Grace Period: 1 hour, Schedule: 24/7
Sev-B: Grace Period: 4 hours, Schedule: 24/7
Sev-C: Grace Period: 8 hours, Schedule: Business Hours

4.Configure Help Topics (For when Users Create a Ticket):


Path: Admin Panel -> Manage -> Help Topics
Available help topics for users when submitting a ticket:
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other

This setup helps define your team structure, user roles, SLA response times, and the categories available for users when submitting support tickets.


</p>
<br />
