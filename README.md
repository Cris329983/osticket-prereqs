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
<img src="https://github.com/user-attachments/assets/02f099fa-686c-4959-aaff-5be05b927bb5" />

</p>
<p>
Before installing osTicket, the web server (IIS) needs to know how to process PHP scripts. Since osTicket is written in PHP, you must register PHP with IIS using the PHP Manager tool.

Open IIS Manager and go to PHP Manager.

You will see a warning that “PHP is not enabled.” Click Register new PHP version.

Browse to the folder where PHP is installed (e.g., C:\PHP).

Select the php-cgi.exe file – this is the FastCGI executable that allows IIS to handle PHP requests.

Click Open to register it.

After this step, IIS will be able to process PHP files, which is required for running the osTicket installer and application.
</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/29b10a6f-507e-4096-89ff-937b2f6f8262" />


</p>
<p>
After downloading the osTicket package (ZIP file), the next step is to extract the contents so they can be copied to the web server directory.

Locate the downloaded osTicket ZIP file.

Right-click the file and select Extract All… (or use the built-in extraction tool as shown).

Choose a destination folder where the files will be extracted (in this example: Desktop\osTicket-Installation-Files\osTicket-v1.15).

Make sure “Show extracted files when complete” is checked to confirm extraction was successful.

Click Extract.

This step prepares the installation files so they can be moved into the IIS web server’s root directory (usually C:\inetpub\wwwroot) for setup. Without extraction, IIS won’t be able to read or run the osTicket installer.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/26a4b028-ed80-4f17-83d3-25573315ac02" />


</p>
<p>
Once the osTicket installation files have been extracted, they need to be placed into the IIS web root directory so the web server can host the application.

Navigate to the IIS root folder: C:\inetpub\wwwroot.

Copy the extracted osTicket files into a new folder named osTicket inside wwwroot.

This creates the path: C:\inetpub\wwwroot\osTicket.

The wwwroot folder is the default location where IIS looks for websites and web applications.

After this step, IIS will be able to recognize osTicket as a web application and serve it through the browser.

This step is crucial because it deploys osTicket to the web server, making it accessible through http://localhost/osTicket (or the server’s IP/domain)
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/7672afa6-b226-4577-93f0-fc16f1e5ee88" />



</p>
<p>
This is the PHP Extensions configuration panel within the Internet Information Services (IIS) Manager on a Windows Server environment. The selected site, osTicket, is part of the Default Web Site under the IIS instance named OSTICKET11.

The panel displays a list of PHP extensions that are currently enabled or disabled for the osTicket web application. These extensions are crucial for osTicket's core functionality, such as database interaction, image processing, internationalization, and web service communication.

Enabled Extensions Include:

php_curl.dll – Enables support for making HTTP requests.

php_gd2.dll – Supports image manipulation (required for CAPTCHA and image processing).

php_gettext.dll – Provides localization and translation support.

php_image.dll – Handles image data functions.

php_intl.dll – Provides internationalization support.

php_mbstring.dll – Required for multibyte string processing.

php_mysql.dll – Allows osTicket to connect to MySQL databases.

php_opcache.dll – Improves PHP performance by caching bytecode.

php_openssl.dll – Enables secure data transmission using SSL.

php_soap.dll – Supports SOAP-based web services.

php_xmlrpc.dll – Provides XML-RPC protocol support.

This configuration ensures that the osTicket application will have the necessary backend support during and after installation, promoting stability and full feature availability.
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

