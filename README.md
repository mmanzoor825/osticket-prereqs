<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Oracle VM VirtualBox
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Required Files</h2>

- [Installation Files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)
- [PHP Manager](https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=drive_link)


<h2>Installation Steps</h2>

<p>
<img width="411" alt="image" src="https://github.com/mmanzoor825/osticket-prereqs/assets/138532574/a3550aac-e490-4ba7-98a8-d06a09b3bb8f">

</p>
<p>
First enable IIS with CGI and some other features. Go to Conrol Panel > Programs > Turn Windows features on or off. Enable the features from the image above.
</p>
Next, download and install:

- [PHP Manager](https://drive.google.com/file/d/1RHsNd4eWIOwaNpj3JW4vzzmzNUH86wY_/view?usp=drive_link)
- [Rewrite module](https://drive.google.com/file/d/1tIK9GZBKj1JyUP87eewxgdNqn9pZmVmY/view?usp=drive_link) 
  
  
</p>
<br />

<p>
<img width="500" alt="image" src="https://github.com/mmanzoor825/osticket-prereqs/assets/138532574/f797b460-685a-43fa-b1bf-53075c92b1fa">

</p>
<p>
Create a folder called PHP on the C drive. Next download and install:
  
- [PHP7.3.8](https://drive.google.com/file/d/1snNMtLdCOpMtkCyD4mvl9yOOmvVIp9fP/view?usp=drive_link) - unzip the contents into C:\PHP
- [VC_redist.x86.exe](https://drive.google.com/file/d/1s1OsGF3-ioO0_9LYizPRiVuIkb3lFJgH/view?usp=drive_link)
- [MySQL 5.5.62](https://drive.google.com/file/d/1_OWh9p7VQLcrB0q_V7qT8yHl0xo5gv7z/view?usp=drive_link) - Typical setup > Launch configuration wizard > standard configuration > set a password                                                                                                                                                          
</p>
<br />

<p>
<img width="400" alt="image" src="https://github.com/mmanzoor825/osticket-prereqs/assets/138532574/922aefea-1c78-4530-8884-3a08d4f22a58">
</p>
<p>
Next register PHP from within IIS. Open IIS as administrator and go to PHP Manager. Click register new PHP and enter C:\PHP\php-cgi.exe. Reload IIS.
</p>
<br />

<p>
<img width="500" alt="image" src="https://github.com/mmanzoor825/osticket-prereqs/assets/138532574/155d394e-2611-45e6-8cf7-e8b7a321ecfb">

Install osTicket v1.15.8

- [osTicket](https://drive.google.com/file/d/1VeVXKlzHDRjeaVUL99ptq7qYbrbXdFxJ/view?usp=drive_link)
- Extract and copy “upload” folder to c:\inetpub\wwwroot
- Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
- Reload IIS
- Go to sites > Default > osTicket. On the right click "Browse *.80(http)"
- This webpage will open and show some installation and extensions information.
</p>


<br />

<p>



<br />
