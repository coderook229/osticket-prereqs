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

- 
- Item 2
- Item 3
- Item 4
- Item 5

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

<p>Make a root password, then click Next, now click Execute and Finish
</p>
<br/>

![image](https://github.com/user-attachments/assets/98487d67-6cc3-4308-90de-e62b6e8bb84b)

<p>Open IIS as an Admin. Click the Start menu, Type IIS. Click Run as administrator
</p>
<br/>

![Screenshot 2024-12-17 003902](https://github.com/user-attachments/assets/61f3ae36-ff64-40ad-adff-b79d6a8c6031)

<p>
lorem
</p>
<br />
