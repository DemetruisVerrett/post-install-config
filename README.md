# osTicket-Post-Installation-and-Configuration
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
These instructions outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)




## **Phase 2: Configuration**
Now that we've installed all components of the osTicket System, the next step is to take osTicket
into its operational stage where it can, and will, handle tickets, user requests, and support staff assignments.

### Set up and Configure Key Components

- Roles: Assign roles to different agents (Admins and Support Staff) to manage access and permissions
- Departments: Create various departments (e.g., IT, Customer Support) to handle tickets based on the various requests
- Teams: Configure teams to handle specific types of support, such as Level I or Level II Support
- Agents (or Workers): Add agents who will manage and resolve the tickets
- Users (i.e., Customers): Add the users who will submit tickets to the help desk
- SLA's (Service Level Agreements): Configure SLA's to ensure timely ticket resolutions based on severity
- Help Desk Topics: Define help topics to categorize tickets based on the issues users may encounter


## Outline

- Configure Roles
  1. Admin Panel -> Agents -> Roles
  2. Assign the "Supreme Admin" role for full Control
 
- Configure Departments
   1. Admin Panel -> Agents -> Departments
   2. Create "System Administrators" department to handle all high-priority system-level issues
 
    
![osTicket 14](https://github.com/user-attachments/assets/1ab71a76-b08a-4b49-adf1-da37f151c151)


- Configure Teams 
  1. Admin Panel -> Agents -> Teams
  2. Set up Level I and Level II support teams to handle different tiers of support requests
 
- Configure Agents (Workers)
  1. Admin Panel -> Agents -> Add New
  2. Add agents like "Jane" and "John" to handle incoming tickets
 
  ![osTicket 15](https://github.com/user-attachments/assets/7ab81c7c-c35b-46c4-bcac-5003a7d96348)


- Configure Users (Customers)
  1. Agent Panel -> Users -> Add New
  2. Add users like "Karen" and "Ken" who will submit tickets
 
  ![osTicket 19](https://github.com/user-attachments/assets/dace0c6b-9473-4b81-ad8d-86a614bd4218)

 
- Configure SLA (Service Level Agreements)

  SLAs define the timeframes in which tickets are to be resolved based on the severity of said issues. Proper monitoring
  and configuration of SLAs will ensure critical issues are prioritized and handled in an efficient manner

![osTicket 20](https://github.com/user-attachments/assets/6e35c262-d9d4-4b14-b88c-e2a7a4210766)


  1. Admin Panel -> Manage -> SLA
  2. Set Up the following SLAs:
     - Sev-A: 1 hour, 24/7 coverage for critical system outages
     - Sev-B: 4 hours, 24/7 coverage for high-priority issues like software failures
     - Sev-C: 8 hours, business hours coverage for less critical issues, sucha as password resets
    
- Configure Help Topics
  Help topics categorize the types of support requests users may submit. Having the proper categorization in place
  will help route tickets to the correct teams and/or department



![osTicket 21](https://github.com/user-attachments/assets/f9495391-22e3-47d8-af88-5c43d20bc636)

  1. Admin Panel -> Manage -> Help Topics
  2. Add common help topics such as:
     - Business Critical Outage
     - Personal Computer Issues
     - Equipment Request
     - Password Reset
    
Summary

We successfully transformed osTicket from it's dormant installation stage into a fully operational help desk that is capable of 
handling real-world support tickets. After configuring all of the key components such as roles, departments, teams, agents, and users, 
we are assured that the system is well-structured for efficient ticket management. Setting up the Service Level Agreements (SLAs) allowed us to prioritize and resolve issues within the appropiate timeframes based on their severity, while the help topics ensured the proper categorization and routing of tickets to the correct teams and departments. 
  
  
