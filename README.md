<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket -  Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source helpdesk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure
- Virtual Machine
- osTicket 



<h2>Installation Steps</h2>

<h3>Step 1: Open osTicket and Log In </h3>

- Log in to osTicket using the credentials you created previously

<p align="center">
<img src="https://github.com/user-attachments/assets/ee04f582-5232-4df4-ba21-86067ad5cdd2" height="80%" width="80%" alt="Azure Free Account"/>	


<h3>Step 2: Create Roles </h3>

- Go to the Admin panel 
- Select the Agent tab --> Roles --> Add New Role
- Name: Supreme Admin
- Go to the Permissions tab and check every box under the "Tickets," "Tasks," and "Knowledgebase" sections
- Select Add Role
	
<p align="center">
<img src="https://github.com/user-attachments/assets/6f4cdca3-ba10-4a04-83e8-7e5e394708be" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/7f5e14c0-1a65-40ae-aee3-eafc03d7de8f" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 3: Create Departments</h3>

- Go to the Admin panel
- Select the Agent tab --> Departments --> Add New Department 
- Name: System Administrators
- Select Create Department 


<p align="center">
<img src="https://github.com/user-attachments/assets/bbe11c05-700e-466c-a27d-dff85264bd67" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/0595e30c-afe5-4a7a-8098-6bcc07953741" height="70%" width="70%" alt="Azure Free Services"/>
</p>


<h3>Step 4: Create Teams
</h3>

- Select the Agent tab --> Teams --> Add New Team
- Name: Level II Support 
- Go to the Members tab and select yourself in "Select Agent" dropdown menu
- Select Create Team
	
<p align="center">
<img src="https://github.com/user-attachments/assets/96d16dee-e6de-4bfc-8952-4b7ef2ddb295" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/6c480e2b-e265-40f7-a4ff-5639e6153d12" height="70%" width="70%" alt="Azure Free Services"/>
</p>

<h3>Step 5: Allow Anyone to Create Tickets</h3>

- Select Settings --> User Settings
- Uncheck the following box: 
- Registration Required: Require registration and login to create tickets 
		
<p align="center">
<img src="https://github.com/user-attachments/assets/b54844b2-a3b2-4cdd-9995-da739be3c7ec" height="80%" width="80%" alt="Azure Free Account"/>		


<h3>Step 6: Create Agents</h3>

- Select the Agent tab --> Add New Agents
- Name: Justin Here
- Email : justin.here(@)osticket.com
- Username: justin.here
- Click Set Password and uncheck the box that says "Send the Agent a Password Reset Email"
- Create a password
- Uncheck the box that says "Require Password Change at Next Login"
- Select set
		
<p align="center">
<img src="https://github.com/user-attachments/assets/d6154489-838a-4d2c-a86a-78a8967a39d8" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/32354625-4e24-49e3-a9c9-d1cbbe348d65" height="70%" width="70%" alt="Azure Free Services"/>
</p>

- Select the Access tab 
- Under Primary Department: 
- Select the Department dropdown menu > System Administrators
- Select the Role dropdown menu --> Supreme Admin
- Extended Accesss 
- Select Department --> Support --> Add --> Supreme Admin
- Select Team tab
- Select Team dropdown menu --> Level II Support
- Select Add
- Select Create	

	
<p align="center">
<img src="https://github.com/user-attachments/assets/d94d3529-ce9b-475e-a712-d366d70a7efd" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/ebd5e021-cd44-4e48-8361-143bf3e38efb" width="70%" alt="Azure Free Services"/>
</p>

- Create another agent
- Follow the same steps as above (step 6), except make some changes to the Primary Department
- Select the Department dropdown menu --> Support
- Select the Role dropdown menu --> View Only
- Extended Accesss 
- Select Department --> Support --> Save Changes
		
<p align="center">
<img src="https://github.com/user-attachments/assets/f85bf7f4-3cda-4ff7-877d-2acca91c4465" height="70%" width="70%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/2bd08047-97e9-494a-a06f-33d096f1639c" height="70%" width="70%" alt="Azure Free Services"/>
</p>
 
     

<h3>Step 7: Create Users
</h3>

<p align="center">
<img src="https://github.com/user-attachments/assets/d850a502-f168-4a3d-ad38-369090812b88" height="80%" width="80%" alt="Azure Free Account"/>		
	
- Select the Users tab to create a user
- Email Address: Jason(@)osticket.com
- Full Name: Jason Jason
- Select Add User
	
<p align="center">
<img src="https://github.com/user-attachments/assets/66976565-af3e-4647-a813-050aa057ebf3" height="80%" width="80%" alt="Azure Free Account"/>			
	
- Select the User tab again to create another user
- Email Address: Stephen(@)osticket.com
- Full Name: Stephen Stepehn
- Select Add User

<p align="center">
<img src="https://github.com/user-attachments/assets/6f616138-6615-48c5-b4ac-8c0ff05afb22" height="80%" width="80%" alt="Azure Free Account"/>		

<h3>Step 8:  Create Service Level Agreements (SLA)
</h3>

- We will create three SLAs
- Select the Manage tab --> SLA --> Add New SLA Plan
- Name: SEV-A 			
- Grace Period: 1
- Schedule dropdown menu: 24/7
- Select Add Plan
	
<p align="center">
<img src="https://github.com/user-attachments/assets/372a0e7b-a60b-4805-879e-1f580c3860e9" height="80%" width="80%" alt="Azure Free Account"/> 
<img src="https://github.com/user-attachments/assets/9f42767f-11cf-4879-bdff-c632c5e8d882" height="80%" width="80%" alt="Azure Free Services"/>
</p>

- Name: SEV-B
- Grace Period: 4
- Schedule dropdown menu: 24/7
- Select Add Plan
	
<p align="center">
<img src="https://github.com/user-attachments/assets/e2cbd11b-477c-477c-a8aa-d7c1e5c10962" height="80%" width="80%" alt="Azure Free Account"/>

- Name: SEV-C 
- Grace Period: 8
- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S. Holidays
- Select Add Plan

<p align="center">
<img src="https://github.com/user-attachments/assets/87a0a2b9-57db-446b-abb0-7c00599a7b19" height="80%" width="80%" alt="Azure Free Account"/>



<h3>Step 9:   Create Help Topics
</h3>

- Select the Manage --> Help Topics --> Add New Help Topic
- Business Critical Outage
- Equipment Request
- Password Reset
- Personal Computer Issues
- Select Add Topic for each topic

<p align="center">
<img src="https://github.com/user-attachments/assets/1da0850b-4d6f-40f9-a66b-394a7959f4b5" height="80%" width="80%" alt="Azure Free Account"/>
<img src="https://github.com/user-attachments/assets/e0d98b5a-909d-48c9-aa27-0e41c558b8d0" height="80%" width="80%" alt="Azure Free Account"/>


The post-installation configuration is complete.  This should conclude the lab.


