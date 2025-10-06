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

- Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles

- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments

- Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)

- Configure Agents (workers)
Admin Panel -> Agents -> Add New

- Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)



- Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics


<h2>Configuration Steps</h2>

<p>
<img width="1205" height="740" alt="image" src="https://github.com/user-attachments/assets/6390fc04-9b7a-4cd9-9c66-881b3ba5453b" />
  <img width="1187" height="915" alt="image" src="https://github.com/user-attachments/assets/2d30dde4-d9b7-459f-8609-b3154c65c601" />
</p>
<p>
In this section, I will show you how to create a new role within osTicket. We will navigate to the Admin panel and go to Agents > Roles > Add New Role. Now we can name the role. Click the Permissions folder, where you can see and define what access you want the agent to have. Configure what access you would like for this particular role and click Add Role. You have now created a new role within the osTicket database. 
</p>
<br />

<p>
<img width="805" height="940" alt="image" src="https://github.com/user-attachments/assets/808d6468-b9d3-4a18-93b1-444ed9735911" />
<img width="800" height="460" alt="image" src="https://github.com/user-attachments/assets/869852d1-fba4-43ac-a3c0-d8bde84a84b0" />
</p>
<p>
In this section, we are adding a new department. Click Roles> Departments> Add New Department. Here you will add name, status, type, etc. Go through the settings and configure what best suits the department's tasks. In the access folder, you can add agents who are primary members of the department. Click create department. Now you have a new department in the database.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
