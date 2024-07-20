<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Creation of Microsoft Azure Tenant (Organization)
- Active Subscription to Azure
- Creation of a Resource Group
- Virtual Network
- Subnet
- Creation of Virtual Machine (and create osTicket inside of VM)



<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/L3z3dmM.png" height="80%" width="80%" alt="VM Creation Steps"/>
</p>
<p>
In this step, we created an Azure Virtual Machine that runs with Windows 10 OS.  We named the virtual machine VM-osTicket, and set-up a username and password in order to be able to log into it.  
</p>
<br />

<p>
<img src="https://imgur.com/sVS93bb.png" height="80%" width="80%" alt="File(s) Installation Steps"/>
</p>
<p>
Next, we installed and enabled IIS in Windows (with CGI and Common HTTP Features) and IIS Management Console.  Then, we opened a folder that contained osTicket software and other installation files (which are dependecies used to run osTicket).  We used these files to install the osTicket dependencies 1st.  [ List of dependecy files installed in this step: PHP Manager for IIS, Rewrite Module, PHP 7.3.8, VC_redist.x86.exe, MySQL 5.5.62  ]  Afterwards, we opened IIS as an Admin, we registered PHP from within IIS, and we reloaded IIS (which means to open IIS, Stop and Start the server).

  
</p>
<br />

<p>
<img src="https://imgur.com/kiEIHj2.png" height="80%" width="80%" alt="Installing Actual osTicket software"/>
</p>
<p>
In the last steps of the installation process, we installed osTicket, reloaded IIS, and enabled the needed back-end extensions and set configuratons, and installed HeidiSQL from the installation files so that it runs  properly.  Finally, we browsed to the help desk login page @ http://localhost/osTicket/scp/login.php, and we browsed to the end user login page @ http://localhost/osTicket/, to ensure that we set up everything properly and that we can log into both pages in the browser.


</p>
<br />
