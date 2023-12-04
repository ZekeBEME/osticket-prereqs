<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Instal/Enable Internet Information Services (IIS) with CGI and Common HTTP Features
- IIS Management Console
- PHP
- HeidiSQL
- OS Ticket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/u3qy6aw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a Resource Group and a Windows 10 Virtual Machine(VM). When creating the VM, allow it to create a new Virtual Network (Vnet)
</p>
<br />

<p>
<img src="https://i.imgur.com/kNUF0bd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install/Enable IIS in Windows with CGI, Common HTTP Features, and IIS Management Console.
</p>
<br />

<p>
<img src="https://i.imgur.com/V3LtLPo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Instal PHP Manager for IIS, Rewrite Module, and PHP 7.3.8. Create the directory C:\PHP and unzip PHP 7.3.8 into it.
</p>
<br />

<p>
<img src="https://i.imgur.com/DpuJp2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an Admin and Register PHP from within IIS. Restart the IIS then install osTicket v1.15.8. Within the osTicket file extract and copy the "upload" folder to c:\inetpub\wwwroot. Now rename the "upload" file to "osTicket"
</p>
<br />

<p>
<img src="https://i.imgur.com/DYtP59p.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart IIS again. Now click "Browse*:80". Observe that some extensions are not enabled. Go to osTicket PHP Manager and enable extensions php_imap.dll, php_intl.dll, and php_opcache.dll. Refresh the osTicket site and check the extension changes
</p>
<br />

<p>
<img src="https://i.imgur.com/DpuJp2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DpuJp2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DpuJp2V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
