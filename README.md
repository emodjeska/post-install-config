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

Roles are the permissions granted to Agents per department that they have access to. You are able to check/ uncheck agents gevin that role in association with a department. an unlimited number of roles can be created and assigned to agents with access to various departments. 

1. Admin Panel -> Agents -> Roles
2. Supreme Admin

![image](https://github.com/emodjeska/post-install-config/assets/143763072/a66e5cc1-6ef7-4111-9316-c258da58c921)

For example, select add new role. Then create a "Supreme Admin Role" This role will be the overall Administrator for our example. So go to Permissions and enable "supreme Admin" to have every possible permission available.

-Configuring Departments.

Tickets are routed though departments in the help desk in osTicket, so they have many setting that you can set for each department. These allow you or your comapny to create a system that works for you.

1. In the Admin panel -> Agents-> Departments
2. System Administators
3. Leave the remaining fields set as default and simply look around and see what settings there are to chose from.

   ![image](https://github.com/emodjeska/post-install-config/assets/143763072/10cb6097-5fa7-413b-a7fd-c5f9e98a2776)

   ![image](https://github.com/emodjeska/post-install-config/assets/143763072/d37b55b0-5eec-4eef-a1e9-dcb124383413)

-Team allow you to pull Agents and group them into projects and organize them to handle a specific issue or user via a help desk topic or ticket filter.

1. Admin panel -> Agents -> Teams
2. Level l support
3. Level 2 support

   ![image](https://github.com/emodjeska/post-install-config/assets/143763072/4052e53e-170b-4bdc-8aa7-50deb3eb18bf)

   ![image](https://github.com/emodjeska/post-install-config/assets/143763072/ecbcb208-7dde-4fbc-9e76-1379eb9acb6b)

   ![image](https://github.com/emodjeska/post-install-config/assets/143763072/519112d6-cb62-4ca6-b1a4-2cf1b0a04991)



