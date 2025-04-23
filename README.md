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

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
