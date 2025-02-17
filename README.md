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

- Windows 11</b> (21H2)

<h2>List of Prerequisites</h2>

- Create Azure Virtual Machine
- Install / Enable ISS in Windows with CGI
- Item 3
- Item 4
- Item 5

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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
