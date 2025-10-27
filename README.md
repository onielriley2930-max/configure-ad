<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Active Directory
- Azure (Cloud)to create Virtual Machines.
- Microsoft Data center (host)
- Step 4

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://imgur.com/CvkJpC3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Active Directory is like a digital phonebook and security guard for computers in a company or school.
It helps keep track of people, computers, and what they’re allowed to do on the network.

So instead of every computer trying to remember every person, Active Directory is the “brain” that remembers it all. So When a company moves to the cloud (like Microsoft Azure), instead of keeping everything stored on physical servers in the office, they use Microsoft’s data centers to host their network.

This means the “brain” of Active Directory — the system that stores all users, passwords, and permissions — now lives online instead of on a local server.

That cloud version of Active Directory is called:

 Azure Active Directory (Azure AD)
</p>
<br />

<p>
<img src="https://imgur.com/xp8xmcq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Next is the cloud. The cloud is just someone else’s powerful computer (server) that you rent space or services from over the internet.

So instead of storing user accounts, passwords, and files on a physical server in your office,
you let Microsoft’s Azure servers handle it all safely online.

</p>
<br />

<p>
<img src="https://imgur.com/v1jV50a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/tOxEc11.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
</p>
<p>
 How to Install Active Directory in Azure (Simple Steps)

 Step 1: Sign in to Azure
		Go to portal.azure.com
		Log in with your Microsoft account
		Make sure you have an active subscription



 Step 2: Create a Virtual Machine (VM)
	1.	Click Create a resource → Virtual Machine
	2.	Choose:
		Windows Server 2022 (or 2019)
		Name it something like ADServer
		Allow RDP (port 3389) so you can log in
	3.	Click Review + Create → Create

This gives you a computer in the cloud.



 Step 3: Connect to the VM
		When it’s done, go to the VM page
		Click Connect → RDP
		Download and open the file
		Log in with the username and password you created

Now you’re inside your Windows Server.



 Step 4: Install Active Directory
		Open Server Manager (it opens automatically)
		Click Add Roles and Features
		Choose Active Directory Domain Services (AD DS)
		Click Next → Install



 Step 5: Set Up the Domain
		After install, click Promote this server to a domain controller
		Choose Add a new forest
		Type your domain name (like mycompany.local)
		Click Next → Install

The server will restart — that’s normal!



 Step 6: You Now Have Active Directory!
		Log back in using:.
</p>
<br />
