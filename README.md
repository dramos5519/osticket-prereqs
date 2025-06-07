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

- Microsoft Azure/ Create Virtual Machine
- Install OsTicket zip. / Enable IIS in Windows WITH CGI
- Install osTicket v1.15.8
- Assign Permissions
- Install HeidiSQL.


<h2>Installation Steps</h2>

<p>
  <img width="702" alt="image" src="https://github.com/user-attachments/assets/a2c837ec-87b1-45b0-9a14-b9503b95d123" />
<img width="763" alt="image" src="https://github.com/user-attachments/assets/c4ae5140-0343-4426-a22c-4ef5352ccc7e" />


</p>
<p>
Within Microsoft Azure, find a create VM name it osticket-vm, make sure to remember username and password used when creating the osTicket VM, under resource group ex.(osTicket). Under image pick Windows 10.Find a usable VM with more than 2VCPUS,make sure to click the Licensing checkbox when using a Windows VM found at the bottom. Click create and deploy. In Remote Desktop enter your IP that you will find next to your newly made VM the public IP address in Windows. You will then on your VM on Remote Desktop download the OsTicket ticket installation files https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD and unzip them onto your VM desktop. 
</p>
<br />

<p>
  <img width="562" alt="image" src="https://github.com/user-attachments/assets/dc541426-06b6-4b42-bf72-78ea68b2cde0" />
  <img width="565" alt="image" src="https://github.com/user-attachments/assets/62a47e1f-f98a-4d7d-937b-0544a6c68314" />

  
In VM open control panel to enable IIS, go to Programs, (Turn windows features on or off) left side
Check=Internet information Services, expand it click World Wide Web Services click Application Development Features next click the CGI checkbox click OK, it will apply changes.  
</p>
<p>

</p>
<br />

<img width="551" alt="image" src="https://github.com/user-attachments/assets/a66d440e-74b0-4170-8f8a-cce6fc1d7dfa" />
<img width="303" alt="image" src="https://github.com/user-attachments/assets/37f5e83e-36bb-4251-be0b-60b5291a6c74" />


From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)

<img width="302" alt="image" src="https://github.com/user-attachments/assets/d6ad89fb-4e22-4e4d-ae88-ba850f4726c6" />

From the “osTicket-Installation-Files” folder install the Rewrite Module (rewrite_amd64_en-US.msi)

<img width="409" alt="image" src="https://github.com/user-attachments/assets/d0b2ef95-b413-4d54-a59f-27d0528741da" />

Create the directory C:\PHP

<img width="304" alt="image" src="https://github.com/user-attachments/assets/8825453b-d981-4f8e-bbb3-423b58e3f428" />
<img width="380" alt="image" src="https://github.com/user-attachments/assets/4cb3fc94-2fe5-4d96-82dd-813e60d9505e" />



From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder

<img width="304" alt="image" src="https://github.com/user-attachments/assets/17f1d708-95f6-45ff-b2b6-42b8f1cc9674" />

From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.

<img width="306" alt="image" src="https://github.com/user-attachments/assets/58e696d1-6891-41a6-a6c1-97624153913e" />

From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

<img width="305" alt="image" src="https://github.com/user-attachments/assets/65a5f6be-d112-4c4b-953f-92a01e4d7df4" />

Typical Setup ->

<img width="305" alt="image" src="https://github.com/user-attachments/assets/c0391e37-c0aa-4562-9717-e3766464b008" />

Launch Configuration Wizard (after install) ->
Standard Configuration ->

<img width="305" alt="image" src="https://github.com/user-attachments/assets/c03b3823-7136-41da-a10d-b32d54e1743d" />

Username: root
Password: root

<img width="485" alt="image" src="https://github.com/user-attachments/assets/4079c33d-0abd-4167-baa6-acb327a40949" />

Open IIS as an Admin

<img width="444" alt="image" src="https://github.com/user-attachments/assets/6d2dbbfa-f7d3-4501-9495-7d645e2dcd9f" />

<img width="439" alt="image" src="https://github.com/user-attachments/assets/f5445138-3c6b-406f-8a5f-9cdeb6102c5d" />

<img width="424" alt="image" src="https://github.com/user-attachments/assets/58aacae1-166b-4f98-8802-823193e3d243" />



Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)

<img width="432" alt="image" src="https://github.com/user-attachments/assets/7e68b79a-8bdb-4d8e-88dd-7e46467947a7" />
<img width="425" alt="image" src="https://github.com/user-attachments/assets/ce21a6bd-fb80-4aa7-840d-06830dc06786" />


Reload IIS (Open IIS, Stop and Start the server)

<img width="482" alt="image" src="https://github.com/user-attachments/assets/feafd462-c726-43ec-8470-09cf087e31b0" />

Install osTicket v1.15.8

<img width="410" alt="image" src="https://github.com/user-attachments/assets/fa36a2fb-6155-40ee-832c-d05fc3669579" />
<img width="409" alt="image" src="https://github.com/user-attachments/assets/d9b2ddd0-4e4c-4579-bf56-29b0628d0ed9" />


From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”

<img width="422" alt="image" src="https://github.com/user-attachments/assets/bb6e16b4-4159-49cf-880a-72d885131332" />
<img width="422" alt="image" src="https://github.com/user-attachments/assets/92443937-4d8b-442c-95f4-564d8e29c3ce" />


Reload IIS (Open IIS, Stop and Start the server)

Go to sites -> Default -> osTicket
On the right, click “Browse *:80”

Note that some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browser, observe the changes

Rename: ost-config.php
From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

Assign Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All

Continue Setting up osTicket in the browser (click Continue)
Name Helpdesk
Default email (receives email from customers)

From the “osTicket-Installation-Files” folder, install HeidiSQL.
Open Heidi SQL
Create a new session, root/root
Connect to the session
Create a database called “osTicket”

Continue Setting up osTicket in the browser
MySQL Database: osTicket
MySQL Username: root
MySQL Password: root
Click “Install Now!”

Congratulations, hopefully it is installed with no errors!
Browse to your help desk login page: http://localhost/osTicket/scp/login.php

End Users osTicket URL:
http://localhost/osTicket/ 

Clean up
Delete: C:\inetpub\wwwroot\osTicket\setup
Set Permissions to “Read” only: C:\inetpub\wwwroot\osTicket\include\ost-config.php

<br />
