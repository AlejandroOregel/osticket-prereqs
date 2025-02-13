

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
<img src="https://i.imgur.com/HLvn4k0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When you boot up the pc head over to control panel and click on "uninstall a program"
</p>
<br />

<p>
<img src="https://i.imgur.com/E9kpbRc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From there click on "Turn Windows features on or off", proceed to fill in the "Internet Information Services" folder and expand it, from there expand "Application Development Features", then fill in the box that says "CGI"
</p>
<br />

<p>
<img src="https://i.imgur.com/ZqySZI8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once your done with that you can proceed to install all the necessary files for osTicket and some of the dependencies needed to run it.
</p>
<br />

<p>
<img src="https://i.imgur.com/MashtTk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next create a new folder within the C Drive and name it "PHP" Be sure to unzip/extract all of the files within the zipped up php folder into the new and seperate PHP folder to avoid any issues.
</p>
<br />

<p>
<img src="https://i.imgur.com/Pit9lWu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When you encounter the MySQL installation proceed with the Typical setup option 
</p>
<br />

<p>
<img src="https://i.imgur.com/dxSDHsd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continuing within the MySQUL installation be sure to click the Standard Configuration option.
</p>
<br />

<p>
<img src="https://i.imgur.com/balWIp4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an admin, click on the PHP Manager and click Register new PHP version, after that go to the PHP file from earlier and find the file that says "C:\PHP\php-cgi.exe" and register it. After this reload IIS, then continue with the installation process.
</p>
<br />

<p>
<img src="https://i.imgur.com/EXgxK1q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make sure to follow these next steps carefully! Unzip the osTicket file and copy the "upload" folder within it into c:\inetpub\wwwroot" Once you have transferred the upload folder rename the "upload" folder to "osTicket" be sure to name it exactly as shown!
</p>
<br />

<p>
<img src="https://i.imgur.com/rFzfF8z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to IIs, click on sites--> Default--> osTicket, click on PHP Manager, click on Enable or disable an extension, from here enable the follolwing extensions: php_imap.dll, php_intl.dll, php_opcache.dll
  after completing these steps load up the osTicket site within ISS.
</p>
<br />

<p>
<img src="https://i.imgur.com/eQKeUs6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the file "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" to "C:\inetpub\wwwroot\osTicket\include\ost-config.php"
</p>
<br />

<p>
<img src="https://i.imgur.com/jRLhcnG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rightclick the renamed file and click on properties, from there click on security, click on advanced, then disable inheritance and click remove all, after that click on new permissions, type in everyone and apply.
</p>
<br />

<p>
<img src="https://i.imgur.com/5IMr3Vp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within IIS click on the link on the right hand side that says Browse *:80 (http) This should take you to osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/KnODn48.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the following info.
</p>
<br />

<p>
<img src="https://i.imgur.com/5hvuWCY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After filling in your info you should be met with this page, proceed with the link that is listed under your staff control panel and fill in the required info.
</p>
<br />

<p>
<img src="https://i.imgur.com/aOzZtdv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Congratulations you set up and installed osTIcket!
</p>
<br />
