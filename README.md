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
Go ahead and login into the osTicket Admin Panel.  When you pull up the Panel you will see tickets for admin/ helpdesk user interface (UI), that reflects the tickets that are created by the end User. 

-Now, we will Configure Roles.

Roles are the permissions granted to Agents per department that they have access to. You are able to check/ uncheck agents gevin that role in association with a department. An unlimited number of roles can be created and assigned to agents with access to various departments. 

1. Admin Panel -> Agents -> Roles
2. Supreme Admin

![image](https://github.com/emodjeska/post-install-config/assets/143763072/fac4319b-c177-4338-af1c-8f94a00c0730)


For example, select add new role. Then create a "Supreme Admin Role" This role will be the overall Administrator for our example. So go to Permissions and enable "supreme Admin" to have every possible permission available.

-Configuring Departments.

Tickets are routed though departments in the help desk in osTicket, so they have many setting that you can set for each department. These allow you or your comapny to create a system that works for you.

1. In the Admin Panel -> Agents-> Departments
2. System Administators
3. Leave the remaining fields set as default and simply look around and see what settings there are to chose from.

  ![image](https://github.com/emodjeska/post-install-config/assets/143763072/3c99382a-3a93-4cfb-a0f4-2703761ea8cf)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/47e8117d-e85d-4bf7-98c1-82c58e6fa15b)


-Team allow you to pull Agents and group them into projects and organize them to handle a specific issue or user via a help desk topic or ticket filter.

1. Admin Panel -> Agents -> Teams
2. Level l support
3. Level 2 support

![image](https://github.com/emodjeska/post-install-config/assets/143763072/7166f914-97e4-4088-bcde-f40f6cc82ad9)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/6de59e53-24ad-4590-89a9-c3a91516f206)


Agents are allowed onto the sytem with the intent to resolve and respond to tickets. When you add an agent to the help desk, you will need to assign a primary department and give a primary role for the tickets and tasks routed to that department.

Admin Panel -> Agents -> Add New
1. Jane 
2. John

![image](https://github.com/emodjeska/post-install-config/assets/143763072/e05925bb-d059-4e97-9341-0a439a35bfdc)

Users (customers) are able to create an account to log in and  create tickets, or check on the status of their ticket.

Agent Panel -> Users -> Add New
1. karen
2. Ken

![image](https://github.com/emodjeska/post-install-config/assets/143763072/7107ed5f-72ab-4bc6-abfd-9cbbeb441be1)

SLA Plans or Service level Agreements, provide a length of time in which the help desk Administator expects tickets to be closed. You are able to create any SLA plans you would like.

Admin Panel -> Manage -> SLA

1. Sev-A (1 hour, 24/7)
2. Sev- B (4 hours, 24/7)
3. Sev-C (8 hours, business hours)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/bf2a9c78-58f8-4b75-85a2-0e26960c8344)

![image](https://github.com/emodjeska/post-install-config/assets/143763072/8fc84ad6-02fa-43ad-b98f-41c0d675ff7d)

Lastly, We will be Configuring Help Topics. Help Topics serve to streamline the expirience for the end-user to make sure the ticket has the proper assignment and prompt response to ticket. Create as many Help Topics as needed.

Admin Panel -> Manage -> Help Topics

1. Bussiness Critical Outage
2. Personal Computer Issues
3. Equipment Request
4. Password Reset

![image](https://github.com/emodjeska/post-install-config/assets/143763072/17ea0bef-c0d4-4721-8891-7367181729c4)

