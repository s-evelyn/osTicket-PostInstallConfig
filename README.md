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

- Windows 10</b> (22H2)


<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create a ticket
- Configure Agents
- Configure Users
- Configure SLA
- Configure Helper Topic

<h2>Configuration Steps</h2>


<h4>1. Configure Rules </h4>

- Login to osTicket via Admin user and Password
- Click on Admin Panel (Note that when you go into Admin panel, the Agent Panel option becomes available in the upper right hand corner, and vice-versa)
    - Select Agents -> Roles
    - Create New Role
          
       <img width="50%" hieght ="50%"  alt="Add New Role" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/83c42ba2-9fc0-4d32-a040-73395a3834e3">

    - We are now going to create a Supreme Admin Role
  
       <img width="50%" hieght ="50%"  alt="Add Supreme Admin" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/71552f42-74a3-45f0-afde-fa2a10d37849">
       
    - Click on the Permisssions tab and Enable all Permissions for Tickets, Tasks and Knowledgebase, once complete click Add Role.
      
       <img align = "top" width="32%" hieght ="32%" alt="Sup Admin pt 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/6d404614-3e7a-4e15-9a8e-1140cd33ee29">
  
       <img align = "top" width="32%" hieght ="32%"  alt="Sup Admin pt 3" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/c477bfe0-92d7-459e-96f4-f1d01c04929a">
               
      <img width="32%" hieght ="32%" align = "top"  alt="Sup Admin pt 4" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/8a096fdd-2db2-408d-a3f7-cdde6143e91c">



</p>

<br />

-----------------------------------------------------------------------------------------------------------------------------------------------

<h4>2. Configure Departments</h4>

- In the Admin Panel, Select Agents,and then Departments
  - Create new Department  
     
    <img width="50%" hieght ="50%" align = "top" width="658" alt="Create New Department" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/a3348454-4683-462a-952e-0fc2becc68a5">

  - Create System Administrator Department
        
      <img width="50%" hieght ="50%"  align = "top" alt="Sys Admin Dpt created" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/a5b8865a-73c8-4559-ae91-5a88973e7b26">


----------------------------------------------------------------------------------------------------------------------------------------

<h4>3. Configure Teams</h4>
   
- In the Admin Panel, Select Agents,and then Teams
    - Create New Teams

        <img width="50%" hieght ="50%" alt="Add Teams" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/9bc80ffd-45a4-44a3-837b-220c97883f09">
        
    - Create Team called Level II Support
      
       <img width="50%" hieght ="50%" alt="Level II Support creation Plus add member" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/c5232f89-6b79-4c05-b322-e6d01b0e4ec4">

    - Add a member to that team by select the member tab, and selecting an agent.

        <img width="50%" hieght ="50%" alt="add member to teams" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/2056fc9d-7f2e-403c-a0e0-2b0e37903ab0">

----------------------------------------------------------------------------------------------------------------------------------------------

<h4> 4. Make Sure That Anyone Can Register </h4>

   - Make sure that you are in the Admin Panel
   - Go to Settings, then users and then user settings.
       - Make sure that in the registration required section, the box is NOT checked.
          
          <img width="50%" hieght ="50%" alt="Make sure anyone can register" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/6d4923bc-c83a-4eac-925c-45b5c01b725f">


---------------------------------------------------------------------------------------------------------------------------------------------------

<h4>5. Configure Agents </h4>

   - Make sure that you are in the Admin Panel, select the Agents, and then Agents
   - Click Add New Agent, give your agent a name and an email address
   - Then click on set password

      <img width="50%" hieght ="50%" alt="Set Password for New Agent" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/8881d1be-c444-4e67-9e9d-a42279c3dbc6">


   - For the purpose of this tutorial unclick " Send the agent a password reset". Also unclick  " Require Password Change at next login". Note that this is not best practice when in a work environment, but for the purpose of this tutorial. Type in a password that you can remember, and click Set.
     
      <img width="50%" hieght ="50%" alt="New Agent 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/e9e43040-bff3-4a7e-9bfa-790a2b685ced">
      
   - Next click on the Access tab, and assign your new agent to the System Administrator Department that we created earlier giving them full access. We are also going to give this Agent extended access to the Support department. Click Create once completed
  
     <img width="50%" hieght ="50%" alt="new agent 3" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/4db08ac2-d5b8-4135-823d-ff7ff504d807">
  
     
 -------------------------------------------------------------------------------------------------------------------------------------------------------------------

<h4>6. Configure Users</h4> 

- Navigate to the Agents Panel

  <img width="50%" hieght ="50%" alt="Create User" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/31bbe2e8-328b-43c0-90f0-e9d5ae1a4efa">

    - Click on Users and then User Directory
    - Click on Create a New User
   
      <img width="50%" hieght ="50%" alt="new user 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/97c62ce5-0159-493c-bc01-49119924f43d">
   
    - Put in an email address for the user as well as their full name and click Add User when you are done.
      
        <img width="50%" hieght ="50%" alt="new user 3" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/4bd907d7-8851-401e-95db-9cec4176f8d3">

      ---------------------------------------------------------------------------------------------------------------------------------------------------

<h4>7. Configure SLA (Service Level Agreements) </h4>
    - Navigate to the Admin Panel
    - Click on the Manage tab and then SLA

        <img width="50%" hieght ="50%" alt="add sla 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/6c95474c-77e2-47d4-8b74-c844b3b0019a">

   - In our example we are going to create and SLA titles SEV-A with a Grace period of 1 hour on a 24/7 schedule
     
        <img width="50%" hieght ="50%" alt="Add SLA" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/62a2e423-4e16-49bb-8982-f93a0b3386b8">

   - Create 3 more SLA with the following grace periods and schedules just to practice
       -  Sev-B (4 hours, 24/7)
       -  Sev-C (8 hours, Business Hours)
          
   ----------------------------------------------------------------------------------------------------------------------------------------------------------

<h4> 8. Configure Help Topics </h4>

- Navigate to the Admin Panel, click on the Manage tab and then on Help Topics
- Click on Add New Help Topics

    <img width="50%" hieght ="50%" alt="Add Help Topics" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/b4d0dd33-e444-4f71-a85e-0b0105e614c5">

- Add a Help Topic called Business Critical Outage, Click Add Topic when completed.

    <img width="50%" hieght ="50%" alt="add help topics 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/65eb8b98-d8bd-4b36-a5c9-b691267ef5d2">

- Continue to add the following Help Topics
    - Personal Computer Issues
    - Equipment Request
    - Password Reset


<h2>osTicket Documentation</h2>
If you would like to get more information about the different configuration here are a few links to their documentation:

- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html)
- [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)
- [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html)
- [SLA](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
- [Help Topics](https://docs.osticket.com/en/latest/Admin/Manage/Help%20Topic.html)

