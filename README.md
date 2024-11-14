<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
In this lab, we have already installed osTicket on our VM or local PC. In the next lab, we will set up the osTicket system in the browser so that we can observe the ticket lifecycle. 

<h2>Configuration Steps</h2>

<h3>Step 1: Configure Roles</h3>

We will be making a Supreme Admin to avoid access issues later on for our admin account. To begin this lab, complete the first osTicket lab: https://github.com/brandenoz/osticket-prereqs. 
- From the admin login, click on Admin Panel > Agents > Roles > from here you can view and adjust the various default access levels. 
- Click Add New Role > name it Supreme Admin > Permissions > click on everything in Tickets, Tasks, and Knowledge Base so that this access level can do everything. Click Add Role. 

<h3>Step 2: Create Departments & Teams</h3>

We will not be setting up some departments that would make functional sense in a potential work environment. 
- Go to Agents > Departments > Add New Department > Choose Top-Level Department > Name it SysAdmins.
- Delete the Maintenance department. 
- Go to Teams > Agents > Teams > Add New Team > Name it Online Banking > Create Team. 

<h3>Step 3: Create Agents</h3>

From the Admin Panel, go to Agents, Add New Agent. Consider opening a Windows Notepad note to keep the credentials organized. 
- Fill out the basics for name and email. The email can be made up.
<br>

![1](https://github.com/user-attachments/assets/9ded3524-3971-4e4c-b9e4-d7d4d08e2fe8)


- For the password settings, click Set Password, uncheck “Send the agent a password reset email”. This will open further settings for you to manually assign a password. Also uncheck “Require password change at next login”. Click Set. 
- For Access, add to the SysAdmins department with Supreme Admin access. For Teams, add her to the Online Banking team. 
- Add a new user. John Doe, fake email, username: john, password: Password1 with same password settings. For Access: set department to Support and access to View only.

<h3>Step 4: Create Users</h3>

From the Agent Panel, click on Users, Add User, use karen@lognpacific.com for the email and karen for the full name. Click Add User. 

<h3>Step 5: Create SLAs</h3>

From the Admin Panel, click on Manage, then click SLA. We will create three different SLAs based on level of severity. 
- Click Add New SLA Plan, set the Name to Sev-A, set Grace Period to 1, set the Schedule to 24/7, click Add Plan. 
- Click Add New SLA Plan, set the Name to Sev-B, set Grace Period to 4, set the Schedule to 24/7, click Add Plan. 
- Click Add New SLA Plan, set the Name to Sev-C, set Grace Period to 8, set the Schedule to “Monday - Friday 8am - 5pm with U.S. Holidays”, click Add Plan.

<h3>Step 6: Configure Topics</h3>

Here we will add various help topics for sorting problems into the right categories for ticket lifecycle later on. Add the following help topics: 
- Click on Help Tickets. Click Add New Help Topic. For Topic put Business Critical Outage, for Parent Topic put Report a Problem, click Add Topic. 
- Add new, name it Personal Computer Issues, for the parent topic put Report a Problem, click Add Topic. 
- Add new, name it Equipment Request, parent topic put General Inquiry, click Add Topic. 
- Add new, name it Password Reset, select Report a Problem for the parent. 
- Add new, name it Other, and select General Inquiry for the parent.
<br>

![2](https://github.com/user-attachments/assets/ba7df540-8e84-4d70-add7-bb71c2b5d559)


<h3>Cleaning Up</h3>

Just as with the last lab, I recommend you pause your VM to save on cost if you are not going directly onto the next project which you can find here: https://github.com/brandenoz/ticket-lifecycle.  



