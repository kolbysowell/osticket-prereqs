<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket – Post-Install Setup and Configuration</h1>

  
In this walkthrough, I cover the **post-installation setup process** for the open-source helpdesk platform **osTicket**, including how to configure departments, agents, teams, SLAs, and help topics for real-world use.

---

## 🧠 Technologies & Environment

- **Microsoft Azure** (Virtual Machines / Compute Resources)  
- **Remote Desktop Protocol (RDP)**  
- **Internet Information Services (IIS)**  

---

## 💻 Operating System

- **Windows 10 (21H2)**  

---

## 🧩 Prerequisites

Before starting, make sure the following are ready:

- A **Microsoft Azure** environment  
- A **Virtual Machine** with Windows installed  
- A working installation of **osTicket**  



---

## 📘 Helpful References

Explore these links to better understand key osTicket components:

- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)  
- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)  
- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)  
- [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)  
- [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)  
- [Service Level Agreements (SLA)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)  

---

## ⚙️ Step-by-Step Configuration

### Step 1: Log In to osTicket
Open your osTicket URL and sign in using the **admin credentials** you created during installation.  
You should see the main dashboard.

<p align="center">
  <img src="https://i.imgur.com/gAXVBO2.png" width="80%" alt="osTicket login screen"/>
</p>

---

### Step 2: Create Roles
Make sure you’re in the **Admin Panel** (the upper-right toggle should say *Admin*).  
Navigate to **Agents → Roles → Add New Role**.  

Name the role **Supreme Admin**, open the **Permissions** tab, and select every option under *Tickets*, *Tasks*, and *Knowledgebase*.  
Click **Add Role** when finished.

<p align="center">
  <img src="https://i.imgur.com/9tiOON2.png" width="70%" alt="osTicket roles"/>  
  <img src="https://i.imgur.com/CfCzRRk.png" width="70%" alt="osTicket permissions"/>
</p>

---

### Step 3: Add a Department
Still in the **Admin Panel**, go to **Agents → Departments → Add New Department**.  
Name the department **System Administrators**, then click **Create Department**.

<p align="center">
  <img src="https://i.imgur.com/f2uEloL.png" width="70%" alt="osTicket departments"/>  
  <img src="https://i.imgur.com/X2dXwjY.png" width="70%" alt="osTicket create department"/>
</p>

---

### Step 4: Build a Team
Navigate to **Agents → Teams → Add New Team**.  
Name the team **Level II Support**.  

Open the **Members** tab, select yourself under *Select Agent*, and click **Create Team**.

<p align="center">
  <img src="https://i.imgur.com/v6zzN3N.png" width="70%" alt="osTicket teams"/>  
  <img src="https://i.imgur.com/4IieS80.png" width="70%" alt="osTicket add team"/>
</p>

---

### Step 5: Allow Public Ticket Creation
To make osTicket accessible to all users, go to **Settings → User Settings**.  
Ensure **“Registration Required”** is **unchecked** so users can submit tickets without creating an account.

<p align="center">
  <img src="https://i.imgur.com/kcd1jRf.png" width="80%" alt="osTicket user settings"/>
</p>

---

### Step 6: Add Agents
Create a new support agent under **Agents → Add New Agent**.  

Example agent:  
- **Name:** Jane Doe  
- **Email:** jane.doe@osticket.com  
- **Username:** jane.doe  

Click **Set Password**, uncheck *Send Password Reset Email*, choose your own password, and uncheck *Require Password Change at Next Login*.  

<p align="center">
  <img src="https://i.imgur.com/fTvI0Ru.png" width="70%" alt="osTicket agent setup"/>  
  <img src="https://i.imgur.com/6OU5KqX.png" width="70%" alt="osTicket agent credentials"/>
</p>

Under the **Access** tab:  
- Primary Department: *System Administrators*  
- Role: *Supreme Admin*  
- Extended Access: Add *Support* → *Supreme Admin*  

Under the **Teams** tab:  
- Team: *Level II Support* → Add  

Click **Create** to save the agent.

<p align="center">
  <img src="https://i.imgur.com/HPSPHNU.png" width="70%" alt="osTicket agent access"/>  
  <img src="https://i.imgur.com/hotx1wo.png" width="70%" alt="osTicket team membership"/>
</p>

You can repeat the process to add another agent (for example, *John Doe*) with limited access:
- Department: *Support*  
- Role: *View Only*  

<p align="center">
  <img src="https://i.imgur.com/qQ8ckBr.png" width="70%" alt="osTicket view only agent"/>  
  <img src="https://i.imgur.com/KVPsUb4.png" width="70%" alt="osTicket support agent"/>
</p>

---

### Step 7: Add Users
Users represent your end customers or employees.

Navigate to **Users → Add New User** and enter:

1. **Email:** karen@osticket.com  
   **Name:** Karen Karen  
2. **Email:** ken@osticket.com  
   **Name:** Ken Ken  

<p align="center">
  <img src="https://i.imgur.com/UUqCK1d.png" width="80%" alt="osTicket users"/>  
  <img src="https://i.imgur.com/wpTn12W.png" width="80%" alt="osTicket add user"/>  
  <img src="https://i.imgur.com/EXyy5Gq.png" width="80%" alt="osTicket user directory"/>
</p>

---

### Step 8: Configure SLA Plans
Define Service Level Agreements to manage response times.

Go to **Manage → SLA → Add New SLA Plan** and create the following:

| Name | Grace Period | Schedule |
|------|---------------|-----------|
| **SEV-A** | 1 hour | 24/7 |
| **SEV-B** | 4 hours | 24/7 |
| **SEV-C** | 8 hours | Mon–Fri 8AM–5PM (U.S. Holidays) |

<p align="center">
  <img src="https://i.imgur.com/fMR4yMR.png" width="80%" alt="osTicket SLA"/>  
  <img src="https://i.imgur.com/3tQnihq.png" width="80%" alt="osTicket SLA setup"/>  
  <img src="https://i.imgur.com/pAbQPEP.png" width="80%" alt="osTicket SEV-B"/>  
  <img src="https://i.imgur.com/5cgn0oz.png" width="80%" alt="osTicket SEV-C"/>
</p>

---

### Step 9: Add Help Topics
Go to **Manage → Help Topics → Add New Help Topic** and create:

- Business Critical Outage  
- Personal Computer Issues  
- Equipment Request  
- Password Reset  

<p align="center">
  <img src="https://i.imgur.com/uFmSyqK.png" width="80%" alt="osTicket help topics"/>
</p>

---

## 🎉 Completion

Congratulations! 🎊  
You’ve successfully completed the **post-installation configuration** of osTicket.  
Your environment now includes working roles, departments, teams, agents, users, SLAs, and help topics — all ready for ticket creation and management.  

Next up: [**Part 3 – Ticket Lifecycle: Intake Through Resolution**](https://github.com/RoslyndWilliams/osTicket--Ticket-Lifecycle)

---

**Author:** Kolby Sowell  
**Project Type:** IT Help Desk / System Administration Portfolio Project  
**Platform:** osTicket (Open Source Helpdesk Ticketing System)
