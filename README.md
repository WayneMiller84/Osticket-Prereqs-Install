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

- Create Azure Virtual Machine
- Install / Enable ISS in Windows with CGI
- On osTicket Installer/Prerequisites setup site
- Config File Permission
- Install osTicker in Browser

<h2>Installation Steps</h2>

![osTicket-vm](https://github.com/user-attachments/assets/6902e890-9443-4496-8715-72a4119150da)

Created an Azure Virtual Machine with Windows 10, to log into the VM remote desktop to run the osTicket installion/setup using the IP Address
</p>
<br />

![IIS Manager](https://github.com/user-attachments/assets/689ecda9-a503-4054-95a0-2e84e280db78)

From the “osTicket-Installation-Files” folder, install PHP Manager for IIS, install the Rewrite Module.  From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder, From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe. From the “osTicket-Installation-Files” folder, install MySQL 5.5.62
Launch the Typical Setup, Launch Config Wizard & Standard Config, Open ISS as an Admin, Register PHP within IIS, and reload ISS to Stop and Start the server
</p>
<br />

![osTicket-installer](https://github.com/user-attachments/assets/c71cc936-5260-417d-8640-63ded8facc05)

![Screenshot 2025-02-17 161930](https://github.com/user-attachments/assets/7e7393ea-ef90-4a07-ab77-72d6a059cc55)

![Screenshot 2025-02-17 162702](https://github.com/user-attachments/assets/3a953e33-e9cb-4c7e-ae49-f7b34276b824)

With installing the osTicket v1, some extensions are not enabled which I had to go back into ISS, click sites, default, osTicket, PHP Manager, click “Enable or disable an extension” Enable: php_imap.dll, Enable: php_intl.dll, Enable: php_opcache.dll
Refresh the osTicket site in your browser, observe the changes.  Rename: ost-config.php, 
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, To: C:\inetpub\wwwroot\osTicket\include\ost-config.php
Assign Permissions: ost-config.php, Disable inheritance -> Remove All, New Permissions -> Everyone -> All, Continue Setting up osTicket in the browser. From the “osTicket-Installation-Files” folder, install HeidiSQL (Open Heidi SQL Create a new session, root/root Connect to the session, Create a database called “osTicket”.  Continue Setting up osTicket in the browser, MySQL Database: osTicket
MySQL Username: root, MySQL Password: root, Click “Install Now!”.
and osTicket Installer in the browser is now installed with no errors

</p>
<br />
