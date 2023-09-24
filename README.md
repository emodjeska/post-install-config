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

- Login to the osTicket Admin Panel
- Configure Roles
- Configure Departments
- Configure Teams
- Configure Help Topics

<h2>Configuration Steps</h2>

Welcome to this tutorial on the post-installation steps for OS Ticket. We will be confinguring OS Ticket as an Admin today.

Go ahead and log into your virtual machine in the Azure Portal. From here, login into the osTicket Admin Panel.  When you pull up the Panel you will see tickets for admin/ helpdesk user interface (UI), that reflects the tickets that are created by the end User. 

Here is a link to login as an Admin.
http://localhost/osTicket/scp/login.php

![image](https://github.com/emodjeska/osticket-prereqs/assets/143763072/a3c390e5-cf94-4d31-a88a-522791f523af)

-Now, we will Configure Roles.

Roles are the permissions granted to Agents per department that they have access to. You are able to assign role permissions by checking/ uncheching them in the "Roles" tab, within a department. An unlimited number of roles can be created and assigned to agents with access to various departments. 

1. Admin Panel -> Agents -> Roles
2. Name The "Role" Supreme Admin.
3. Assign all Permissions to the "Role", so that we have an Admin that is able to do and access everything with OS Ticket.

![image](https://github.com/emodjeska/post-install-config/assets/143763072/bc476e7f-691f-4d57-a3d2-37d0e13ba280)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/0f6df0e4-5bbd-4279-beb2-8e44d4327614)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/6af89808-d311-4db1-8e03-e11307ecc0d0)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/ab6e8015-289e-4d4c-8d5e-7d8b7b116bdb)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/33b0c496-b468-43a0-a0c3-8269d117e07e)

For example, select add new role. Then create a "Supreme Admin Role" This role will be the overall Administrator for our example. So go to Permissions and enable "supreme Admin" to have every possible permission available.

-Configuring Departments

Tickets are routed though departments in the help desk in OS Ticket, so they have many setting that you can set for each department. These allow you or your comapny to create a system that works for you.

1. In the Admin Panel -> Agents-> Departments
2. System Administators
3. Leave the remaining fields set as default and simply look around and see what settings there are to chose from.

![image](https://github.com/emodjeska/post-install-config/assets/143763072/852c63b3-5584-47af-ad63-fd47b0ded126)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/326513ef-88ff-4eb0-ab36-f0d31f494943)

-Configuring Teams

Teams allow you to pull Agents and group them into projects and organize them to handle specific issues or users via a help desk topic or ticket filter.

1. Admin Panel -> Agents -> Teams
2. Level l support
3. Level 2 support

![image](https://github.com/emodjeska/post-install-config/assets/143763072/aac74d91-5384-4d9e-8ff8-7b4adfb71b63)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/26c3b42e-b0d0-4c21-bd99-9a128d0c5e29)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/b719ef84-59fc-47ec-8562-fb2c9d4b0ca1)

-Before we go any further, we have to configure OS Ticket so that anyone may create tickets.

Admin Panel -> Settings -> User Settings -> Check the box next to " Require registration and login to create tickets"

![image](https://github.com/emodjeska/post-install-config/assets/143763072/8e611810-0b8e-4e95-9020-93de22342668)

-Configuring Agents

Agents are allowed onto the sytem with the intent to resolve and respond tickets. When you add an agent to the help desk, you will need to assign a primary department and give a primary role for the tickets and tasks routed to that department.

Admin Panel -> Agents -> Add New
1. Jane Doe
2. John Doe

![image](https://github.com/emodjeska/post-install-config/assets/143763072/712187c0-c010-4d63-bf41-596112d23b66)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/274cc49f-7a2b-4002-97d4-3cec58f7c62d)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/6362ab1b-0db0-4835-818f-76446dfa8ddf)


-Configuring Users

Users (customers) are able to create an account to log in and create tickets, or check on the status of their ticket. An email address will be associated with each user in the ticketing system.

Agent Panel -> Users -> Add New
1. karen
2. Ken

![image](https://github.com/emodjeska/post-install-config/assets/143763072/8fa15a15-2adb-4bfb-ba39-76f92786e3da)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/05a0007f-4e46-48ac-b9c0-300ae146a4d3)

-Configuring SLA

SLA Plans or Service level Agreements, provide a length of time in which the help desk expects tickets to be closed. You are able to create any kind of SLA plans you would like.

Admin Panel -> Manage -> SLA

1. Sev-A (1 hour, 24/7)
2. Sev- B (4 hours, 24/7)
3. Sev-C (8 hours, business hours)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/a6564ea8-bbe6-4b43-be4d-6c165c65af1e)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/8af604f6-fae5-4b90-ae12-cb04ee349862)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/ce6342d5-26c7-4c17-9393-746893278c55)

-Configure Help Topics

Lastly, We will be Configuring Help Topics. Help Topics serve to streamline the expirience for the end-user to make sure the ticket has the proper assignment and prompt response. Create as many Help Topics as needed.

Admin Panel -> Manage -> Help Topics

1. Bussiness Critical Outage
2. Personal Computer Issues
3. Equipment Request
4. Password Reset

![image](https://github.com/emodjeska/post-install-config/assets/143763072/b303e0b5-3683-4e56-95a4-c2b76c95fa3f)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/2fb2bf77-1fa9-49fb-b219-423f631e1902)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/b941c627-ed10-4348-b881-f79abe94716a)


Congradulations, together we have configured OS Ticket.

Thank you for joining me today.
