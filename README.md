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

- Create an Azure Virtual Machine Windows 10, 4 vCPUs
- Install / Enable IIS in Windows WITH CGI
- Create the directory C:\PHP
- Register PHP from within IIS
- Install osTicket v1.15.8

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/lebpTzf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create an Azure virtual machine using windows 10. After created, copy the public IP address from your virtual machine. Open microsoft remote desktop and paste the IP address into the add new pc section. You then connect to the pc and log in with the username and password you used to create the virtual machine.
</p>
<br />

<p>
<img src="https://i.imgur.com/OKImj8w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Head to the pc's control panel and click programs. Press turn windows features on or off. Find internet information services and turn them on. Expand IIS, woldwide web, and application developer. Under application developer you should see CGI and you want to click the square to install. Last you wanna download PHP manager and the rewrite module.
</p>
<br />

<p>
<img src="https://i.imgur.com/bUfgbvZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>       
Create a new foler in the root of the C drive and name it PHP. Then download PHP and extract the contents in the new PHP folder. You want to download C++ redistributable since PHP requires it. Download and install MySqL server. Inside MySQL you want to set up and remember your root password. This is used to setup a database to store the users, tickets, etc.
</p>
<br />                                                                                                                                                  <p>       
<p>
<img src="https://i.imgur.com/3qV73bC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>       
Find the IIS app and before opening right click on it,and click run as admin. Double click PHP manager and register new PHP version. Then go head to the C drive, PHP, and click PHP-CGI.
</p>
<br />  
<p>
<img src="https://i.imgur.com/IlEPLmM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is the final screen you should have after completely setting up OsTicket on the pc. There are multiple steps to get here which includes enabling multiple extentions in PHP manager, Disable inheritence and giving everyone permission inside of osticket. The last istallation you will need to do is HeidiSQL. After a few clean up procedures, you now have a fully working OsTicketing system.
</p>
<br />
