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


<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/mbJ4MMo.png)" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This first step shows the process of extracting compressed (zipped) files on a Windows 10 system. The extraction path is set to C:\Users\CRIS\Downloads\osTicket-Installation-Files, indicating that I am preparing installation files for osTicket.
</p>
<br />


<img width="591" height="461" alt="image" src="https://github.com/user-attachments/assets/be09d1ba-ebfe-4609-abf8-183720e999c8" />

</p>
<p>
  
Here you can see the Windows Features window, where various optional Windows components can be turned on or off. The highlighted item is Internet Information Services (IIS), which is not currently enabled. This step is part of a pre-installation process to configure system features needed for IT service environments.
</p>
<br />

<img width="842" height="653" alt="image" src="https://github.com/user-attachments/assets/43168038-5387-4b74-8ff6-9b0974bf8808" />

<p>
  
Next is the extraction of a compressed PHP installation file to the directory C:\PHP as part of the osTicket pre-installation setup. This step prepares the PHP runtime environment required for running the osTicket support ticket system on a Windows machine.
</p>
<br />



<p>
<img src=https://i.imgur.com/6w0gfe7.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This screenshot shows the setup of Microsoft Visual C++ Redistributable packages as part of the osTicket helpdesk system deployment on a Windows environment. This step was crucial to enabling proper operation of Apache, PHP extensions, and other backend services needed by osTicket. Verified successful installation and resolved dependency issues to ensure smooth web-based installation and ticket system performance.
</p>
<br />

<p>
<img src=https://i.imgur.com/roh5oJr.png) height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To continue I Successfully created and configured the MySQL database backend for the osTicket ticketing system. Tasks included creating the initial database schema, assigning secure user privileges, and optimizing database performance for reliability and scalability, this was done after other several steps of course.
</p>
<br />  

<p>
<img src=https://i.imgur.com/voIHrAi.png width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Finally after all the other steps here is the final result.
</p>
<br />

