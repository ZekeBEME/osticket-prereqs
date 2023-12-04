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
<img src="https://i.imgur.com/dceky3U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next rename From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php To: C:\inetpub\wwwroot\osTicket\include\ost-config.php. Assign Permissions to ost-configh.php for everyone

</p>
<br />

<p>
<img src="https://i.imgur.com/Kk7bJc0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue setting up osTicket in the browser, but wait to install. Install HeidiSQL and create a new session with a password you can remember. Connect to the session and create a database called "osTicket".
</p>
<br />

<p>
<img src="https://i.imgur.com/NH4rZGY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now you can finish filling out osTicket in the browser and install now. To check if your installation worked browse to http://localhost/osTicket/scp/login.php and login
</p>
<br />
