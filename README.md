# osticket-prereqs

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

- https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD
- install PHP Manager for IIS 
- install the Rewrite Module 
- install VC_redist.x86.exe
- install MySQL 5.5.62
- install  PHP 7.3.8
- install HeidiSQL

<h2>Installation Steps</h2>

<p>
After creating a virtual machine on https://portal.azure.com/
</p>
<br />

![image](https://github.com/user-attachments/assets/f55f0d22-0b8c-40a1-b4ea-c397047c0c33)


<p>
On the right side of the screen, copy the public ip address of the virtual machine.
</p>
<br />

![image](https://github.com/user-attachments/assets/f1ef5f8f-8a87-4bdf-bc51-cdeaef279ac7)

<p>
Open Remote Desktop Connection. Next paste the public ip address of the virtual machine. Now the username of the virtual machine. Click connect.
</p>
<br />

![image](https://github.com/user-attachments/assets/d0183ebe-36a4-49e0-8f44-6fe77e31974c)

<p>
Enter the password of the virtual machine. Click Yes on the warning message to connect to the vm.
</p>
<br />

![image](https://github.com/user-attachments/assets/d43b446d-5714-4b51-9ba8-e9bc63f70b32)
![image](https://github.com/user-attachments/assets/bfaaed3c-3c84-40b1-86a1-887137c352a3)

<p>
Now that you're connected to the vm, within the vm, download the osTicket-Installation-Files.zip and unzip it onto your desktop.
</p>
<br />

![image](https://github.com/user-attachments/assets/4806f58d-86f6-4b0c-9912-a2405d24c97a)

<p>
Go to Control Panel. Click Programs, now Turn Windows features on or off
</p>
<br />

![image](https://github.com/user-attachments/assets/f9873571-0b62-47d6-bb85-a34eeb6f6c42)

<p>
Check and expand the box next to Internet Information Services. Expand World Wide Web Services. Expand Application Development Features now check the box next to CGI and click OK.
</p>
<br />

![Screenshot 2024-12-14 143825](https://github.com/user-attachments/assets/fe453c25-a3e8-48fc-a8fb-49e94752c6f4)

<p>
From the osTicket-Installation-Files folder, install PHP Manager for IIS 
</p>
<br />

![image](https://github.com/user-attachments/assets/220370c1-53b5-49a2-b1c9-18c94d97c92a)

<p>
From the osTicket-Installation-Files folder, install the Rewrite Module 
</p>
<br />

![image](https://github.com/user-attachments/assets/f40b91d3-db7d-4c2b-b094-cd4d1926dfb4)

<p>
Navigate to the C: drive. Create a folder named PHP
</p>
<br />

![Screenshot 2024-12-14 150506](https://github.com/user-attachments/assets/d8dcfac4-777b-43b8-8f0a-669b9d1a7dc4)

<p>
From the osTicket-Installation-Files folder, unzip PHP 7.3.8 into the C:\PHP folder.
</p> 
<br />

![image](https://github.com/user-attachments/assets/b14276f8-a199-480b-b2ec-bb3ff28f1a97)
![image](https://github.com/user-attachments/assets/f659f913-83f7-4bef-88e1-0fac2c96c433)

<p>From the osTicket-Installation-Files folder, install VC_redist.x86.exe.
</p>
<br />

![Screenshot 2024-12-14 160109](https://github.com/user-attachments/assets/8372df56-73db-47c8-afda-8f756097293d)

<p>From the osTicket-Installation-Files folder, install MySQL 5.5.62
</p>
<br />

![Screenshot 2024-12-14 161008](https://github.com/user-attachments/assets/4e298ee9-ee00-4c1a-80d8-42c0c77dd2cb)

<p>Click Typical Setup, then click Finish to launch configuration wizard.
</p>

![Screenshot 2024-12-16 195527](https://github.com/user-attachments/assets/725716dc-91c0-4e05-9e60-c1bd67e4a4fb)

<p>Click Standard Configuration. Then Next, and Next again.
</p>
<br/>

![Screenshot 2024-12-16 202133](https://github.com/user-attachments/assets/b3158a75-b2d3-4f5a-8414-32adb06797ec)

<p>Make a root password, then click Next, now click Execute and Finish.
</p>
<br/>

![image](https://github.com/user-attachments/assets/98487d67-6cc3-4308-90de-e62b6e8bb84b)

<p>Open IIS as an Admin. Click the Start menu, Type IIS. Click Run as administrator
</p>                
<br/>

![Screenshot 2024-12-17 003902](https://github.com/user-attachments/assets/61f3ae36-ff64-40ad-adff-b79d6a8c6031)

<p>Click PHP Manager, now click Register new PHP version.
</p>
<br />

![Screenshot 2024-12-18 132353](https://github.com/user-attachments/assets/adbb6685-d03d-46b1-9818-56debb0f20a9)

<p>Register PHP from within IIS. Browse to the C:\PHP folder. Click on the php-cgi application and select Open.
</p>
<br />

![image](https://github.com/user-attachments/assets/d939c4cf-ec36-4b52-9574-b36b28f03848)

Proceed with OK and now you should see this screen
</p>
<br />

![image](https://github.com/user-attachments/assets/b29d15bb-c615-48a7-ac1f-fcfed8b79aa7)


<p>Reload IIS (Open IIS, Stop and Start the server)
</p>
<br />

<p>On the left side of the screen, click osTicket and right-click and select Stop. Right click again and select Start.
</p>
<br />

![Screenshot 2024-12-18 154520](https://github.com/user-attachments/assets/47b2dde2-5129-417f-97fb-945d9e1a5636)

![image](https://github.com/user-attachments/assets/7ba5e5e2-b0f5-472b-8803-77ed7e34dfc7)

<p>From the osTicket-Installation-Files folder, unzip osTicket-v1.15.8.zip and copy the upload folder into “c:\inetpub\wwwroot”.
</p>
<br />

![Screenshot 2024-12-18 164706](https://github.com/user-attachments/assets/0576b2ce-02a4-4db3-94e4-e5ab0bccbd04)

![Screenshot 2024-12-18 170739](https://github.com/user-attachments/assets/e6540168-c29e-4a23-b7a9-d6f79008ba0a)

<p>Reload IIS (Open IIS, Stop and Start the server). The same steps from earlier, use Run as administrator before opening IIS.
</p>
</br />

<p>Open the arrow under Connections, next to where you refreshed IIS, click the arrow next to Sites, then Default, now osTicket
 </p>
 <br /> 

 ![Screenshot 2024-12-18 191146](https://github.com/user-attachments/assets/6d468166-8088-45db-bd1b-a345e210e862)

 <p>On the right side of the screen, click Browse *:80.
 </p>
 <br />
 
   ![Screenshot 2024-12-18 195332](https://github.com/user-attachments/assets/a9f285c4-acc3-4987-a6dd-80cfc85f45ba)

   You should see a webpage similar to this.
 </p>
 <br />

![image](https://github.com/user-attachments/assets/3e435983-de55-4cc9-bfd0-7a5a9293aefe)

<p>Go back to IIS, Under Connections, make sure the same arrows are opened that we clicked earlier. Go to PHP Manager again. Now click Enable or disable an extension. Now find the following extensions listed below and right-click on them and enable  

Enable: php_imap.dll   <br />
Enable: php_intl.dll   <br />
Enable: php_opcache.dll

![Screenshot 2024-12-18 205422](https://github.com/user-attachments/assets/b2e186dc-6911-49e3-83b4-15558656712b)

Refresh the osTicket site in your browser, observe the changes
</p>

<p> Rename: ost-config.php <br /> from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
<br /> to C:\inetpub\wwwroot\osTicket\include\ost-config.php
</p>

![Screenshot 2024-12-18 210248](https://github.com/user-attachments/assets/c6652867-bb45-4f05-922d-3db8564168c0)

<p>Right-click on the file. Click Properties, click Security, then Advanced 
</p>

![image](https://github.com/user-attachments/assets/b8aa3d81-3956-49bc-a68a-c848557133a8)

<p>At the bottom click Disable Inheritance. Then Remove all inherited permissions. At the bottom click Add. Click Select a principal.
</p>

![Screenshot 2024-12-18 214552](https://github.com/user-attachments/assets/75858c49-16f0-44c7-8ea7-bc6bc013e628)

<p>Type Everyone, and click Check Names, then OK. Select Full control under Basic permissions.
</p>

![Screenshot 2024-12-18 215522](https://github.com/user-attachments/assets/e2d12cdd-bb0d-4b20-91e9-f77174130bc7)

<p>After Click OK. Then at the bottom click Apply and OK 
</p>
<br />

![image](https://github.com/user-attachments/assets/c866a293-5c05-43b8-a2e2-0788f068a898)

<p>Go back to the osTicket Installer Webpage and click Continue.
</p>
<p>Name the Helpdesk
Default email (receives email from customers)
</p>

<p>From the osTicket-Installation-Files folder, install HeidiSQL.
  
Open Heidi SQL.Create a new session by selecting New, 
</p>

<p>User is root <br />
Password is root  <br /></p>

![image](https://github.com/user-attachments/assets/949d2f22-7abd-4c28-a565-6740f30a7f66)
<p>

Connect to the session
Create a database called “osTicket”
</p>

  ![Screenshot 2024-12-19 213314](https://github.com/user-attachments/assets/ecbe2a33-ed8e-425f-92b9-71772be25d4d)

![Screenshot 2024-12-19 213343](https://github.com/user-attachments/assets/c308b9d9-2a7c-4428-9f61-73041916cf55)

<p>After downloading HeidiSQL, complete the database settings for osTicket installer.
</p>
<br /> 

<p>Now click Install Now, and you should see a webpage similar to this</p>

![Screenshot 2024-12-19 213620](https://github.com/user-attachments/assets/21224ee2-121f-448e-a146-20116af0ee4d)
