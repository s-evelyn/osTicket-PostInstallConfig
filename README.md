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

- Configure Roles
- Configure Departments
- Configure Teams
- Allow anyone to create a ticket
- Configure Agents
- Configure Users
- Configure SLA
- Configure Helper Topic

<h2>Configuration Steps</h2>

1. Configure Roles
    - Login to osTicket via Admin user and Password
    - Click on Admin Panel (Note that when you go into Admin panel, the Agent Panel option becomes available in the upper right hand corner, and vice-versa)
    - Select Agents -> Roles
        - Create New Role
          
            <img width="50%" hieght ="50%"  alt="Add New Role" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/83c42ba2-9fc0-4d32-a040-73395a3834e3">

        - We are now going to create a Supreme Admin Role
  
           <img width="50%" hieght ="50%"  alt="Add Supreme Admin" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/71552f42-74a3-45f0-afde-fa2a10d37849">
       
        - Enable all Permissions for Tickets, Tasks and Knowledgebase
      
            <img align = "top" width="32%" hieght ="32%" alt="Sup Admin pt 2" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/6d404614-3e7a-4e15-9a8e-1140cd33ee29">
  
            <img align = "top" width="32%" hieght ="32%"  alt="Sup Admin pt 3" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/c477bfe0-92d7-459e-96f4-f1d01c04929a">
               
            <img width="32%" hieght ="32%" align = "top"  alt="Sup Admin pt 4" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/8a096fdd-2db2-408d-a3f7-cdde6143e91c">



</p>

<br />

-----------------------------------------------------------------------------------------------------------------------------------------------

2. Configure Departments

   - In the Admin Panel, Select Agents,and then Departments
       - Create new Department  
     
      <img width="50%" hieght ="50%" align = "top" width="658" alt="Create New Department" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/a3348454-4683-462a-952e-0fc2becc68a5">

      - Create System Administrator Department
        
          <img width="50%" hieght ="50%"  align = "top" alt="Sys Admin Dpt created" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/a5b8865a-73c8-4559-ae91-5a88973e7b26">


----------------------------------------------------------------------------------------------------------------------------------------

3. Configure Teams
   
- In the Admin Panel, Select Agents,and then Teams
    - Create New Teams

        <img width="50%" hieght ="50%" alt="Add Teams" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/9bc80ffd-45a4-44a3-837b-220c97883f09">
        
    - Create Team called Level II Support
      
       <img width="50%" hieght ="50%" alt="Level II Support creation Plus add member" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/c5232f89-6b79-4c05-b322-e6d01b0e4ec4">

    - Add a member to that team by select the member tab, and selecting an agent.

        <img width="50%" hieght ="50%" alt="add member to teams" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/2056fc9d-7f2e-403c-a0e0-2b0e37903ab0">

----------------------------------------------------------------------------------------------------------------------------------------------

4. Make sure that anyone can register

   - Make sure that you are in the Admin Panel
   - Go to Settings, then users and then user settings.
       - Make sure that in the registration required section, the box is NOT checked.
          
          <img width="50%" hieght ="50%" alt="Make sure anyone can register" src="https://github.com/s-evelyn/osTicket-PostInstallConfig/assets/53543374/6d4923bc-c83a-4eac-925c-45b5c01b725f">


---------------------------------------------------------------------------------------------------------------------------------------------------

5. Configure Agents

   - Make sure that you are in the Admin Panel
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
