<img src="https://i.imgur.com/svCFZeT.png" height="40%" width="40%" alt="osticket"/>
<br />
<h1>Configuration of osTicket</h1>


<h2>Description</h2>
In this tutorial, we'll walk through the steps to configure various elements of the osTicket system, such as roles, departments, agents, users, and SLAs, from the perspective of a system administrator. Let's get started!
<br />

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Lab walk-through:</h2>
Firstly we are going to configure Roles - Roles in osTicket define the permissions granted to agents within specific departments. These permissions dictate what actions an agent can take, such as creating, closing, or deleting tickets.<br/>
<br/>Go to your osTicket Admin Panel, then follow the path:
Admin Panel > Agents > Roles > Add New Role<br />
<br /><img src="https://i.imgur.com/araSyVJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />In this example, we're creating a role called "Supreme Admin". This role will have every possible permission granted to it. Make sure to check all permissions to give the agent full access to actions across the departments.<br />
<br /><img src="https://i.imgur.com/cxSZxas.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />
Configuring Departments - 
Departments help organize and categorize tickets within osTicket. Each department can represent a distinct function or team, making it easier to manage tickets based on their specific needs.<br />
<br />Navigate to Departments - go to Admin Panel > Agents > Departments > Add New Department.<br />
<br />For this example, create a department called "SysAdmins". This will be a technical support team that handles system administration-related tickets.<br />
<br /><img src="https://i.imgur.com/fF3ed3k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />Creating Agents - agents are users who are responsible for responding to and resolving tickets within their respective departments. In this step, we'll create two agents.<br />
<br />Go to Admin Panel > Agents > Agents > Add New Agent.<br />
<br />Create two agents: Jon and Jane. For each agent, you'll need to fill out the following basic information: (Name, Email, Username, Password)<br />
<br />After entering the Account details, navigate to the Access tab and assign both Jon and Jane to the "SysAdmins" department we created earlier.<br />
<br /><img src="https://i.imgur.com/uJxxU3d.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />Adding Users - Users are individuals who can create tickets and check the status of existing tickets. In this step, we’ll create a user named Karen.<br />
<br />Go to Admin Panel > Users > User Directory > Add User.<br />
<br />Enter Karen's name and email.<br />
<br /><img src="https://i.imgur.com/BAH04kk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />For lab testing, we need to allow users (like Karen) to create tickets without having to go through registration or login.<br />
<br />Go to Admin Panel > Settings > Users > User Settings.<br />
<br />Uncheck the option that says "Require registration and login to create tickets". This will allow anyone, including non-registered users, to create tickets.<br />
<br /><img src="https://i.imgur.com/pTO0Jng.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />Configuring Service Level Agreements - SLAs define the timeframe in which tickets must be addressed and closed. In this section, we'll create three different SLAs.<br />
<br />Go to Admin Panel > Manage > SLA.<br />
<br />We'll create the following SLAs:<br />
<br />Sev-A (High Priority)
Grace Period: 1 hour
Schedule: 24/7
<br />Sev-B (Medium Priority)
Grace Period: 4 hours
Schedule: 24/7
<br />Sev-C (Low Priority)
Grace Period: 8 hours
Schedule: Business Hours<br />
<br /><img src="https://i.imgur.com/IDH5o3l.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><br />
<br />With these configurations, you've successfully set up roles, departments, agents, users, and SLAs in osTicket. Happy configuring!
