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
<p>Creating a New Role in osTicket

Disclaimer: I am RDP’d into a virtual machine where osTicket is installed.

In this section, I will demonstrate how to create a new role within osTicket.
First, navigate to the Admin Panel, then go to Agents > Roles > Add New Role.
Enter a name for the new role. Next, open the Permissions tab, where you can view and define the specific access levels you want the agent to have.

After configuring the desired permissions for this role, click Add Role.
You have now successfully created a new role within the osTicket database.
To manage existing roles, navigate to Agents > Roles from the Admin Panel. From there, you can edit, update, or remove roles as needed to maintain proper access control.
</p>
<br />

<p>
<img width="805" height="940" alt="image" src="https://github.com/user-attachments/assets/808d6468-b9d3-4a18-93b1-444ed9735911" />
<img width="800" height="460" alt="image" src="https://github.com/user-attachments/assets/869852d1-fba4-43ac-a3c0-d8bde84a84b0" />
</p>
<p>
Creating and Managing Departments in osTicket

In this section, we will add a new department within osTicket.
From the Admin Panel, go to Roles > Departments > Add New Department.
Enter the department’s name, status, and type, then review the available settings to configure what best fits the department’s responsibilities and workflow.

In the Access tab, you can assign agents who will be primary members of the department.
Once all settings are configured, click Create Department. You have now successfully added a new department to the osTicket database.

To manage existing departments, return to Roles > Departments. From there, you can edit, update, or delete departments as needed to keep your organizational structure accurate and up to date.
</p>
<br />

<p><img width="795" height="588" alt="image" src="https://github.com/user-attachments/assets/1cf4e7d2-07fa-4434-986b-04204a8b2592" />
<img width="796" height="365" alt="image" src="https://github.com/user-attachments/assets/e1c65b99-8259-4934-97fc-1987272c0ed7" />
</p>
<p>Creating and Managing Teams in osTicket

In this section, we will add a new team within osTicket.
From the Admin Panel, go to Roles > Teams > Add New Team.
Enter the team’s name, status, and team lead, then review the settings to ensure they align with your organizational structure.

In the Members tab, you can assign agents to the team.
Once all settings are configured, click Create Team. You have now successfully added a new team to the osTicket database.

To manage existing teams, return to Roles > Teams. From there, you can edit, update, or remove teams as needed to maintain accurate team organization within the system. 
</p>
<br />

<p>
<img width="801" height="809" alt="image" src="https://github.com/user-attachments/assets/46434e05-6d1e-4c5e-81e2-c78ecbc13a95" />
<img width="799" height="458" alt="image" src="https://github.com/user-attachments/assets/fdc2f63d-529b-42b5-83aa-e2bd27f53015" />
<img width="803" height="448" alt="image" src="https://github.com/user-attachments/assets/85535faf-682d-4236-b42d-0a1499ffddad" />
<img width="814" height="381" alt="image" src="https://github.com/user-attachments/assets/7cef907f-b8d2-49a2-9bb9-aecc44ef08ef" />

</p>
<p>
Creating and Managing Agents in osTicket

In this section, we will create a new agent within osTicket.
From the Admin Panel, go to Agents > Agents > Create New Agent.
Enter the agent’s name, along with their personal and work information. Create a username, then configure the agent’s status and settings.

In the Access tab, assign the agent to a department and give them a role.
In the Permissions tab, configure specific permissions for the agent based on their responsibilities.
Under the Teams tab, assign the agent to the appropriate team.

Once all information and settings are complete, click Create Now. You have successfully added a new agent to the osTicket database.

To manage existing agents, return to Agents > Agents. From there, you can edit, update, or disable agents as needed to maintain proper access and staff organization within the system.
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

To create a new help topic, go to Manage > Help Topics > Create New Help Topic.
Enter a name for the topic, set its status, and configure the desired settings.

In the New Settings section, you can define which department the ticket will be assigned to, set the priority level, select the SLA plan, and adjust other configurations such as auto-assignment rules or category tags.

To manage existing help topics, navigate to Manage > Help Topics. From there, you can browse, edit, or organize all current help topics as needed.
</p>
<br />
