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

- Configure Departments 
Admin Panel -> Agents -> Departments

- Configure Teams
Admin Panel -> Agents -> Teams 

- Configure Agents (workers)
Admin Panel -> Agents -> Add New

- Configure SLA
Admin Panel -> Manage -> SLA




- Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics


<h2>Configuration Steps</h2>

<p>
<img width="1205" height="740" alt="image" src="https://github.com/user-attachments/assets/6390fc04-9b7a-4cd9-9c66-881b3ba5453b" />
  <img width="1187" height="915" alt="image" src="https://github.com/user-attachments/assets/2d30dde4-d9b7-459f-8609-b3154c65c601" />
</p>
<p>
**DISCLAMER*I am RDP to a virtual machine in which I have installed osTicket.** In this section, I will show you how to create a new role within osTicket. We will navigate to the Admin panel and go to Agents > Roles > Add New Role. Now we can name the role. Click the Permissions folder, where you can see and define what access you want the agent to have. Configure what access you would like for this particular role and click Add Role. You have now created a new role within the osTicket database. 
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

<p><img width="795" height="588" alt="image" src="https://github.com/user-attachments/assets/1cf4e7d2-07fa-4434-986b-04204a8b2592" />
<img width="796" height="365" alt="image" src="https://github.com/user-attachments/assets/e1c65b99-8259-4934-97fc-1987272c0ed7" />
</p>
<p>
In this section, we are adding a new team. Click Roles> Teams> Add New Team. Here you will add the team name, status, and team lead. In the members folder, you can add members to the team. Click Create Team, and the team is now in the osTicket database. 
</p>
<br />

<p>
<img width="801" height="809" alt="image" src="https://github.com/user-attachments/assets/46434e05-6d1e-4c5e-81e2-c78ecbc13a95" />
<img width="799" height="458" alt="image" src="https://github.com/user-attachments/assets/fdc2f63d-529b-42b5-83aa-e2bd27f53015" />
<img width="803" height="448" alt="image" src="https://github.com/user-attachments/assets/85535faf-682d-4236-b42d-0a1499ffddad" />
<img width="814" height="381" alt="image" src="https://github.com/user-attachments/assets/7cef907f-b8d2-49a2-9bb9-aecc44ef08ef" />

</p>
<p>
In this section, we are creating new agents. Go to Agents> Agents> Create New Agent. Here you will enter their name and other personal/work information. Create a username and configure status and settings. In the access tab, you will assign them to a department and give them a role. In the permissions folder, you can configure different permissions for the user. In the teams tab, you simply assign them to a team. Click Create Now, and the user is in the osTicket database. 
</p>
<br />

<p>
<img width="800" height="572" alt="image" src="https://github.com/user-attachments/assets/b3350b79-968d-423f-93ff-50125f7b7f32" />


In osTicket, go to Manage> SLA. There, you can add a new SLA. You will name the SLA, give it a status, and a grace period. Configure settings according to your company policies on said SLA severity. Click add plan and the SLA is now in the osTicket database. 
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img width="802" height="544" alt="image" src="https://github.com/user-attachments/assets/dd61a36d-4492-486d-b694-6ecdf2c9215e" />
<img width="799" height="527" alt="image" src="https://github.com/user-attachments/assets/2bc53b07-d00c-4554-ac83-e4f1ca222bb1" />
<img width="793" height="429" alt="image" src="https://github.com/user-attachments/assets/ae306aa5-6663-4241-b618-6c05f65ee8b4" />

</p>
<p>
Creating and Managing Help Topics

To create a new help topic:

Navigate to Manage > Help Topics > Create New Help Topic.

Enter a name, set its status, and configure the desired settings.

In the New Settings section, you can customize several options, such as:

The department the ticket will be assigned to

The priority level

The SLA plan

Other relevant ticket handling preferences

To manage existing help topics, simply go to Manage > Help Topics, where you can browse, edit, or organize all your current topics.

Would you like me to make it sound a bit more instructional (like a step-by-step guide for a manual) or formal (for internal documentation or training slides)?
</p>
<br />
