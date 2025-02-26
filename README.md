<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Basic Configuration Tools</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Assign Roles
- Create Departments
- Edit Help Topics
- Assign Agents to a Team
- Establish SLA Parameters

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/6bllQ0y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing all the proper software, we can now access the osTicket web server we created and log in to the admin account. The admin account has the ability to manage agents, set up different configuration protocols, as well as a slew of other administrative tools.
</p>
<br />

<p>
<img src="https://i.imgur.com/fm4DMmc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Firstly, let's go over the agents tab and the different roles that can be assigned and created on this page. On this page, we can see some preset roles like “View Only” or “Expanded Access,” which we can assign to agents and departments on the network because we are currently in an admin account. For example, we could edit the Expanded Access role to have the ability to not only view tickets but also edit the SLA or due date. Not only that, but the admin can also create new roles within osTicket. I recommend creating an “All Access” role just so we can fully test all the capabilities an agent will have within most ticketing software. When creating the All Access role, make sure to checkmark all the permissions in the tickets tab so that our agent account has no restrictions.
</p>
<br />

<p>
<img src="https://i.imgur.com/Xwp07nN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Another important property of the admin account is the ability to add new departments and manage the agents and permissions assigned to them. This is done so that when a ticket is created, it can be seen by the people in the department that can best help with resolving the issue at hand. If a ticket requires resources from different departments, you can form a team that would have agents from different departments assigned to one ticket. In osTicket, this is done by the admin's account and clicking on “Add New Team” when looking through the agents tab on the top bar. Now that we have a department and a team created, we can add a new agent to the system and then assign that agent to the team and department we created. When adding an agent, you're going to need the full name and email of the agent. Next, you can assign them a username, and the agent will be prompted to create a password the next time they sign in to their account. When adding an agent, you can also immediately assign them to any team or department you need to as the admin. For now, let's assign this agent to the department with All Access permissions and the Online Banking team.
</p>
<br />

<p>
<img src="https://i.imgur.com/VQG5lXV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Admins can also give the end user the ability to create tickets and assign labels to those tickets so that the agent can better identify the issue. We can add help topics through the manage tab of osTicket, and we can create common categories to help the end user correctly identify the type of issue at hand. If the end user can correctly categorize the issue in the ticket request, it can help speed up the assignment process of a ticket. For example, I created a topic called "Password Reset" so that if the end user chooses that topic, it can automatically be directed to the support department.
</p>
<br />

<p>
<img src="https://i.imgur.com/AVWLoFO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lastly, admins can set SLA parameters (Service Level Agreement) so that the agent working on the ticket can determine how severe the issue is. For now, let's open the manage tab, click on SLA, and create a new SLA plan. From here, we can create an SLA plan called "Sev-A," and we can set a grace period of 4 hours, meaning the ticket needs to be worked on within 4 hours of being posted. From here, we can create a Sev-B and Sev-C SLA plan that allows for a larger response window, meaning they have less direct impact on the success/security of the business.
</p>
<br />
