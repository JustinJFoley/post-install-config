<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

1.  Set Up User Roles and Permissions for proper access control.
2.  Configure Departments and Teams for ticket organization.
3.  Allow Ticket Creation by Registered Users Only and adjust registration settings.
4.  Set Up SLA to define response times based on ticket priority.
5.  Create Help Topics to categorize tickets when users submit them.

<h2>Configuration Steps</h2>

    1)    Acknowledge Agent Panel vs. Admin Panel
Understand the distinction between the Agent Panel (for handling tickets) and the Admin Panel (for managing settings and configurations).

    2)    Configure Roles
Go to Admin Panel → Agents → Roles to create roles for different types of users (e.g., Supreme Admin with full permissions).

    3)    Configure Departments
In the Admin Panel → Agents → Departments, create different departments such as SysAdmins and Networking to control ticket visibility for each department.

    4)    Set Up Teams
Under Admin Panel → Agents → Teams, create teams by grouping agents from different departments (e.g., Online Banking team).

    5)    Configure Ticket Creation Settings
Go to Admin Panel → Settings → User Settings, and uncheck "Allow unregistered users to create tickets." Set it to require registration and login before users can create tickets.

    6)    Configure Agents (Workers)
Under Admin Panel → Agents → Add New, add agents like Jane (Dept: SysAdmins) and John (Dept: Support) to manage the tickets.

    7)    Configure Users (Customers)
In the Agent Panel → Users → Add New, add users such as Karen and Ken, who will create and submit tickets.

    8)    Configure SLA (Service Level Agreements)
Go to Admin Panel → Manage → SLA to create different SLA policies:

Sev-A (Grace Period: 1 hour, Schedule: 24/7).

Sev-B (Grace Period: 4 hours, Schedule: 24/7).

Sev-C (Grace Period: 8 hours, Schedule: Business Hours).

    9)    Configure Help Topics
Navigate to Admin Panel → Manage → Help Topics and create predefined topics for users when submitting tickets, such as:

Business Critical Outage, Personal Computer Issues, Equipment Request, Password Reset & Other.
