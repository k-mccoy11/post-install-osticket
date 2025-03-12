<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align= "center">osTicket Configuration & User Management</h1>
<p></p>This tutorial explains how to set up osTicket after installation to expedite ticket handling, including establishing user roles, departments, teams, agents, and support topics. This tutorial will create a Supreme Administrator role with full access, along with two agents (employees) and their assigned departments. We will also set up teams for agents and clients accessing the help desk system. Finally, we will configure SLA plans and create a help topic for "Accessing Clients' Credentials", specifically for situations where clients experience credential issues. <br /> </p>

<h2 align= "center" > Access URLs </h2>

<ul>
<li><a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login </a> </li>
<li><a href="http://localhost/osTicket">End User Portal</a></li>
</ul>

<h2 align= "center" > Key Configurations </h2>
<ul>
<li>Agent Panel vs. Admin Panel </li>
<li>User & Access Management </li>
<li>Ticket Submission Rules </li>
  <li>Configure Agents & Users</li>
  <li>SLA (Service Level Agreements)</li>
  <li>Help Topics for Ticket Categorization</li>
</ul>

<p>
In the previous project, we set up the osTicket system from scratch. Refer to the previous project for detailed instructions on the installation requirements needed for this tutorial.
</p>

<h3 > Agent Panel vs. Admin Panel </h3>
<p>The Admin Panel is used for system configuration and settings, while the Agent Panel is designed for handling support tickets and customer interactions.
<p>
<img src="https://github.com/user-attachments/assets/28bce924-c465-4e10-8215-d2b5f99a85b3"/>
</p>
<h6> The previous picture shows the layout of the Agent Panel. Click Admin Panel to configure settings.</h6>
<h3>User & Access Management</h3>
<ul>
  <p>
<img src="https://github.com/user-attachments/assets/78a653df-7be9-4537-9352-f0842af6472f"/>
</p>
<li><b>Configure Roles (Permission grouping) → Admin Panel → Agents → Roles</b></li>
  <p>
  <img src="https://github.com/user-attachments/assets/3237077b-d89a-4534-b676-b419cd5afa31">
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/2e0fe76a-8931-4546-b008-561fc2acdadd">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/d1dec94e-10a1-4bb8-9aa7-0484171ac009">
</p>
<li>Configure Departments (Ticket Visibility) →<b> Admin Panel → Agents → Departments</b>
</li>
 <p>
   The System Administrators department is where Supreme Admins will be assigned. Additional configurations, including SLAs, managers, and email settings, can be managed within the department's tab.
 </p>
 <p>
  <img src="https://github.com/user-attachments/assets/3f2673f8-5cba-4d7d-8e43-e40e6b38a358">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/4b69f85d-27be-487c-9e89-7f069022e04d">
</p>
  <li>Configure Teams (Cross-department collaboration) → <b>Admin Panel → Agents → Teams</b></li>
<p>Teams enable you to bring together agents from different departments, allowing you to form a specialized group. For example, you can create a help topic related to logging into Apple products and assign it to a team of agents who specialize in supporting Apple products.</p>
<p>
  <img src="https://github.com/user-attachments/assets/5965261f-ad32-4055-98bf-e36168adb51f">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/4e6204d2-f2ce-49dd-b64a-9313b1fab5b8">
</p>
<h3>Configure Agents & Users</h3>
<p>Now that we have created a new team, we will configure a setting that allows anyone to submit tickets. Navigate to <b>Admin Panel → Settings → User Settings</b> to enable this option.</p>
<p>
<img src="https://github.com/user-attachments/assets/1a75f71c-60ea-4921-b88d-e279042846ca"/>
</p>
  <h6>Registration Required: Leave uncheck</h6>
  <p> Agents are the helpdesk employees responsible for resolving tickets. Each agent is assigned a primary department and a primary role for handling tickets within that department. Additionally, agents can be granted access to multiple departments and can have different roles based on the department they are working in.</p>
<p>
<img src="https://github.com/user-attachments/assets/0b631003-3a85-4e3c-b996-ce8c3c415b57">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/83c21544-f0d8-4dae-99cf-77e87128c819">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/ab4f5101-27a5-46d0-88e2-fed48a23e5a8">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/d8b14c4c-7c6e-4391-8f07-0b9e6bc0a060">
</p>
  <p>
  <img src="https://github.com/user-attachments/assets/1cd9d387-6d90-44bc-a395-d3b7c5465ae3">
</p>
<p>
  <img src="https://github.com/user-attachments/assets/00df4b5d-8c88-4835-a044-f12d476258e9">
</p>
<h6>Complete this process for each agent, choosing different departments and teams.</h6>

<p>Users are customers who submit tickets when they encounter issues. Each user is identified by their email address. To create a new user, navigate to <b>Agent Panel → Users → User Directory → Add New.</b>/</p>

<h5>In Agent Panel<p>
<img src="https://github.com/user-attachments/assets/d5bdb88b-7c02-4570-9487-e68c8462faca"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/a29bbe91-a3ba-437e-be0a-49e1955a6510"/>
</p>
  </ul>

<h3>SLA (Service Level Agreements)</h3>
<p>SLA plans define the timeframe within which the help desk is expected to resolve a ticket. To create an SLA plan, navigate to <b>Admin Panel → Manage → SLA Plans.</b> Each SLA includes a schedule and a designated grace period. </p>
<br />

<h5>In the Admin Panel</h5>
<p>
  <img src="https://github.com/user-attachments/assets/91f31460-d98a-4ba5-acd2-32eb54285528">
</p>
<p>
<img src="https://github.com/user-attachments/assets/3b9865e6-55cc-4ce2-a58c-9c80ee554acc"/>
</p>
<p>
<img src="https://github.com/user-attachments/assets/86fae277-ada5-4d87-834d-86817362e893"/>
</p>
<h6>Create Sev-A and Sev-B with 24/7 schedule.</h6>

<h3>Help Topics for Ticket Categorization</h3>
<p>Help topics help users organize their tickets.<b>Admin Panel → Manage → Help Topics</b></p>
Examples:
  <ul>
<li>Business Critical Outage</li>
<p>
<img src="https://github.com/user-attachments/assets/7575082b-e5c1-4fc8-834b-22c2e92095ee">
</p>
<p>
<img src="https://github.com/user-attachments/assets/c9acff6d-45cb-4f4a-8065-ede71a0b5b1c"></p>
<p>
<img src="https://github.com/user-attachments/assets/7bde745e-96cd-4900-93df-0ff7b51299e2"></p>
<li>Password Reset</li>
<p>
<img src="https://github.com/user-attachments/assets/2472d303-0e28-4956-9d88-7f306092b9fc"></p>
<p>
<img src="https://github.com/user-attachments/assets/6fa48f97-72ee-4f86-8ca5-fb614dbb0a44"></p>
    <p>
<img src="https://github.com/user-attachments/assets/47d10a3d-c3a0-4cbb-8ad6-a89c8524243b"></p>
    <h6>Update: Report a Problem" department to "Support". </h6>
</ul>
