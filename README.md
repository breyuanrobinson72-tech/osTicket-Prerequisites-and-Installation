# osTicket-Prerequisites-and-Installation
This repository will demonstrate the process of installing the OS Ticket system on your computer and the prerequisites required for it to function properly. 


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

- OS-Ticket
- Hedi SQL
- CGI
- PHP Manager
- MySQL

<h2>Installation Steps</h2>

<p>
<img width="500" height="314" alt="zipfolder" src="https://github.com/user-attachments/assets/384e2768-484d-4351-b19a-2ec9b97fe698" />
 


</p>
<p>
Gain access to the OS-Ticket zip folder, which is just a folder you can access from the OS-Ticket website, and dump all the needed files into it to get the OS up and running properly. You then want to extract everything from the zip file, creating a new file that will allow your computer to begin extracting the other data within the zipped file.
</p>
<br />

<p>
<img width="1123" height="450" alt="cotrolpanel" src="https://github.com/user-attachments/assets/75a98b8d-1e0d-40d1-8abb-471485ed21ea" />

</p>
<p>
Even though we don't plan to uninstall any programs, you should open the Control Panel in the Windows search and click Uninstall Programs. Once opened, click Turn Windows features on and off. This is where we will introduce the Internet Information System (IIS). There will be a subfile named World Wide Web Services. you will find a subfile under that named Application Development Features. Under that, you will find the CGI tool that the OS-Ticket needs to run. Common Gateway Interface allows certain scripts on the server to be sent back to the browser.
<br />

<p>
<img width="832" height="393" alt="osticketfolder" src="https://github.com/user-attachments/assets/95a9d528-ca11-457a-b035-81104c03a12b" />
</p>
<p>
Return to the OS-Ticket folder that was created after the zipped file was extracted. Here, you want to extract the data from the PHP manager file and the rewrite module file. Inside the same folder, there will be a zipped PHP file you'll want to create your own PHP folder on the \\:C drive, then you can extract the data from the PHP zipped folder and place it there. You'll finally need to open MySQL and install it with a typical setup option and standard configuration. Create a password you'll remember; it will be important later.

</p>
<br />

<p>
  <img width="924" height="408" alt="IIS" src="https://github.com/user-attachments/assets/320c2c91-d891-412d-afde-b95729cf08f0" />
  <img width="617" height="618" alt="CGI" src="https://github.com/user-attachments/assets/94e54011-4a94-45ea-a24c-dda28278a697" />
</p>
<p>
  In the Windows tab, you should be able to find the Internet Information Services, but by typing IIS, you'll want to open this as an admin. Once inside, open the PHP Manager. Register a new PHP and use the PHP CGI file found in the PHP folder we created with the extracted data in it. Run the program on PHP CGI. You will need to start and stop the IIS to update the system.

</p>
<br />

<p>
<img width="1359" height="693" alt="PHP" src="https://github.com/user-attachments/assets/c89f9a2a-7188-481b-a03c-fe6ea05e3221" />  
</p>
<p>
  You should now have almost everything you need to get OS-Ticket up and running; however, there are a few configurations that need to be made for the system to run. You need to go back into IIS and PHP Manager, next You'll want to click Enable and Disable Extensions under the PHP Manager tab. Enable PHP_IMAP.dII, PHP_intl.dII, and PHP_opcache.dII. Stop and start IIS once again to make these updates and browse the OS-Ticket site from inside IIS

</p>
<br />

<p>
  <img width="699" height="344" alt="HEidi" src="https://github.com/user-attachments/assets/fd91794b-e61d-4c90-a842-c62fc3dd167a" />
</p>
<p>
  In the C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php, change ost-sampleconfig to ost-config.php so that the OS-Ticket system can find the file when processing data. You will finally need to install HeidiSQL, create a new session, connect to the session, and create a new database under the name osTicket
</p>
