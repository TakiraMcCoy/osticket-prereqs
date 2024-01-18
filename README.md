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

- Windows 10</b> (22H2)

<h2>List of Prerequisites</h2>

- PHP Manager for IIS
- Rewrite Module 
- PHP 7.3.8
- VC_redist.x86.exe
- MySQL 5.5.62
- OsTicket
- HeidiSQL

<h2>Video Demonstration</h2>

- ### (https://youtu.be/aok12l0Ssxg)

<h2>Installation Steps</h2>
<img width="863" alt="Screen Shot 2024-01-17 at 11 02 58 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/ad1385ca-8799-4e58-89e3-bf0166e9238f">
<img width="618" alt="Screen Shot 2024-01-17 at 11 03 25 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e21637ca-503c-4d6d-a106-1fed71b1689b">
<img width="563" alt="Screen Shot 2024-01-17 at 11 04 04 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/f3be7d92-da24-4c83-b40a-d3b8ca8adb9f">


<img width="563" alt="Screen Shot 2024-01-17 at 11 04 04 PM" <img width="605" alt="Screen Shot 2024-01-17 at 11 04 40 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e83574c8-b9ab-4c3e-8997-6fa1f985101e">
<img width="511" alt="Screen Shot 2024-01-17 at 11 05 15 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/d04644b1-c613-4b4c-87c5-210adfff6c3f">
<img width="609" alt="Screen Shot 2024-01-17 at 11 07 51 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/4510c595-627a-4904-907a-3d316861c906">
<img width="581" alt="Screen Shot 2024-01-17 at 11 08 56 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/9c33c172-036e-4c65-8489-b28fb1abecf2">
<img width="581" alt="Screen Shot 2024-01-17 at 11 10 05 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/bc0fb47d-4863-4042-8f0a-4d1286c82255">
<img width="598" alt="Screen Shot 2024-01-17 at 11 11 37 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/a6d92b8e-3e0a-408d-987a-68ea88261ba6">
<img width="599" alt="Screen Shot 2024-01-17 at 11 12 43 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/a1bdbfcf-c3ed-4b64-b928-bbd4af51ac8c">
<img width="408" alt="Screen Shot 2024-01-17 at 11 14 42 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e54173fd-6d93-4d52-ae5b-8278f2692220">
<img width="287" alt="Screen Shot 2024-01-17 at 11 15 26 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/5a63efb8-8046-4d56-8070-a6e4cc90525c">
<img width="545" alt="Screen Shot 2024-01-17 at 11 16 09 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/cf2ab6ba-a208-4d89-8661-ce74b21fd4a2">
<img width="343" alt="Screen Shot 2024-01-17 at 11 16 52 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/3d1e64fc-6faa-4801-8a48-cfa34289c8ac">



Step 1:

Setup the virtual machine in Azure by first creating a resouce group.


Name the resouce group and select the region.


Then create the first Virtual machine within the this RG.


It should be a Windows 10 computer with 2-4 Virtual CPUs.


Create the user name and password for loging into this VM.


When creating the VM, under the networking tab, allow the Virtual Network (Vnet) to generate before continuing.


Then go on to create the 2nd virtual machine following the same steps for VM1 but this will be an Ubuntu computer.


In the Resource group tab select Vm1 to retrive the public IP address and copy it.

Search Remote desktop in the windows search bar.


When remote desktop is launched paste the public Ip address and login with the username and password created in the virtual machine setup.

<img width="243" alt="Screen Shot 2024-01-17 at 11 19 45 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/cd7fa8ab-960e-45b4-bd31-4782bd29d361">
<img width="354" alt="Screen Shot 2024-01-17 at 11 20 12 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/5df27984-411d-4952-9034-51a8bb253f69">
<img width="430" alt="Screen Shot 2024-01-17 at 11 21 20 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/f54cc4be-4948-4136-8bf3-4998318cb5cb">
<img width="372" alt="Screen Shot 2024-01-17 at 11 21 40 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/8bdd1764-e77b-45d2-b050-f674be67529f">
<img width="356" alt="Screen Shot 2024-01-17 at 11 22 43 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/ec67cfa5-f8d4-4920-9993-c4189b520443">
<img width="356" alt="Screen Shot 2024-01-17 at 11 24 35 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/603dd5f6-d9c7-43ab-9e71-ed99742a2ae7">
<img width="356" alt="Screen Shot 2024-01-17 at 11 24 51 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/80168da8-d95c-4de5-a5f1-387fa0e570a1">



Step 2:
Enable Internet Informations Services(IIS).

In the vitual machine right click the windows icon/run/type control.

In the "control panel" window select "programs" and "turn windows features on and off".

The window that opens will allow you to enable and install feautures.


<img width="427" alt="Screen Shot 2024-01-17 at 11 26 35 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/d5fe7377-d7d4-432b-b66a-74747ef485e7">
<img width="322" alt="Screen Shot 2024-01-17 at 11 27 11 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/f27085a0-a902-47d5-937f-92f9f7a0ae07">
<img width="314" alt="Screen Shot 2024-01-17 at 11 28 05 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/d7c08eab-e1cf-4500-9dd1-ef111d06cd68">
<img width="376" alt="Screen Shot 2024-01-17 at 11 28 45 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/2bfca96d-b154-4f6d-80b9-e974bac804a5">


Step 3:
Download and install all prerequisites  


<img width="568" alt="Screen Shot 2024-01-17 at 11 30 50 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/f339366a-17cc-4d31-967a-afab77d9cf75">
<img width="196" alt="Screen Shot 2024-01-17 at 11 31 42 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/0889c6b4-2e57-4080-9774-803eccbca7a5">
<img width="307" alt="Screen Shot 2024-01-17 at 11 32 10 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/d9ce921c-fe55-4cf6-8c9d-e55fff1cd309">
<img width="604" alt="Screen Shot 2024-01-17 at 11 33 54 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/cd4339e4-c740-4814-91cd-a3004eec85d7">


Step 4:
Create "PHP" folder in (C:) and extract  PHP 7.3.8 into it.






<img width="572" alt="Screen Shot 2024-01-17 at 11 34 41 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/45e97df6-5f0f-4c56-af4b-125247d83657">
<img width="837" alt="Screen Shot 2024-01-17 at 11 35 18 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/105249cb-45a7-4888-95bd-ea3533ebb8a3">
<img width="837" alt="Screen Shot 2024-01-17 at 11 35 30 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/153197e5-3270-4fec-95b1-a57a2fe73d99">
<img width="698" alt="Screen Shot 2024-01-17 at 11 36 34 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/72bb263b-8807-45c9-acbf-690fe322c63e">
<img width="464" alt="Screen Shot 2024-01-17 at 11 36 54 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/f70dac06-0d47-4c70-9740-6fff7dcb0764">
<img width="187" alt="Screen Shot 2024-01-17 at 11 37 59 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/9d522a9c-e9ee-4071-8682-730c4dacf436">
<img width="177" alt="Screen Shot 2024-01-17 at 11 38 20 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/ea9fdb22-96a0-4e66-9d3e-7e2017f0bcdb">



Step 5:
Launch IIS/Select PHP Manager/Register new PHP version.

select the "PHP" folder created and open "php-cgi" to register "PHP Manager".


Restart "IIS".



<img width="728" alt="Screen Shot 2024-01-17 at 11 39 21 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/139af6a7-5040-4424-9365-f201c8f84ee0">
<img width="728" alt="Screen Shot 2024-01-17 at 11 40 12 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/6096cb3b-a4e7-4e42-a695-386f66e6eafd">
<img width="138" alt="Screen Shot 2024-01-17 at 11 41 39 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/8e836c17-f4f9-48c8-9ec7-9a4fb88948ed">
<img width="170" alt="Screen Shot 2024-01-17 at 11 42 03 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e8ebb5d8-89f5-4b9c-a1ad-e245e997be8e">
<img width="145" alt="Screen Shot 2024-01-17 at 11 42 40 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e351de8b-5f43-423d-856c-120199820929">
<img width="174" alt="Screen Shot 2024-01-17 at 11 43 25 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/90777a10-4190-434c-aff1-4816e7178371">
<img width="695" alt="Screen Shot 2024-01-17 at 11 43 50 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/1b3ef89f-5eeb-423b-95dd-caa8f973039f">



Step 6:
Open the "osTicket folder" and copy the "upload folder" into th"wwwroot" folder.

Restart "IIS".

Select the drop down arrow for "default web site" and select osTicket.

In the right panel select “Browse *:80”. 

This will launch "osTicket installer".






<img width="521" alt="Screen Shot 2024-01-17 at 11 45 27 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/9216f95c-09a0-46f8-ac6e-7a0643ffaca4">
<img width="296" alt="Screen Shot 2024-01-17 at 11 45 52 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/7189f21c-f161-47ec-ac93-bf59d49c56c1">
<img width="429" alt="Screen Shot 2024-01-17 at 11 47 03 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/139fce64-becb-4818-a466-55e1ea9087f5">
<img width="267" alt="Screen Shot 2024-01-17 at 11 47 41 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/e3de262d-d2e6-45fc-9c06-b2571cc412eb">
<img width="353" alt="Screen Shot 2024-01-17 at 11 48 15 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/08af8373-c9fc-4617-8202-37fb1ecd83f7">



<img width="353" alt="Screen Shot 2024-01-17 at 11 48 27 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/86bf085a-3bc5-4ba0-8e62-863f9759cf8e">


Step 7:
Select (C:)/inetpub/wwwroot/osTicket/include.

Rename "ost-sampleconfig.php" to "os-config.php". 

Right click and select properties/security/advanced/disable inheiretance.

Select "Remove all inheireted permissions from this object"/add/select a principle.

Type "everyone"/click "check names"/"ok".

Set permissions to Full control/"ok"/"apply"/"ok".




<img width="562" alt="Screen Shot 2024-01-17 at 11 49 17 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/6848215a-dbd4-4290-928c-9b4f0bb68093">
<img width="562" alt="Screen Shot 2024-01-17 at 11 49 38 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/0a3a0c1b-c83e-45ef-abfa-5ee296203bfb">
<img width="907" alt="Screen Shot 2024-01-17 at 11 50 08 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/839d0566-ef21-41c7-bf86-f7218df9b8a0">
<img width="665" alt="Screen Shot 2024-01-17 at 11 51 11 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/19a386fa-20c7-49ee-af36-859d2420345f">
<img width="664" alt="Screen Shot 2024-01-17 at 11 52 15 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/1f254bc4-d91d-46ce-bb17-2d56a048bf96">

Step 8:
IIS/PHPManger/"enable or disable an extension".

 
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll

Refresh "osTicket installer"/Continue istallation.







<img width="664" alt="Screen Shot 2024-01-17 at 11 54 54 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/23b9ee12-68bf-4240-9ccd-bba146afc7df">
<img width="664" alt="Screen Shot 2024-01-17 at 11 55 21 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/68497e22-b209-4861-825a-63ad39ff150f">
<img width="664" alt="Screen Shot 2024-01-17 at 11 56 10 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/311e8805-cd15-4075-9707-4040aca941c3">
<img width="664" alt="Screen Shot 2024-01-17 at 11 56 40 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/b6ca219e-2c85-4c26-bd25-db7f6424c4cc">
<img width="633" alt="Screen Shot 2024-01-17 at 11 57 22 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/c5f46581-1aba-48db-8c48-3a90ed759167">
<img width="652" alt="Screen Shot 2024-01-17 at 11 58 12 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/02cad3ec-c57d-482a-9bb9-065306765aeb">
<img width="652" alt="Screen Shot 2024-01-17 at 11 58 40 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/97eab39d-dc91-4273-844b-c37c9b6984f2">
<img width="695" alt="Screen Shot 2024-01-17 at 11 59 05 PM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/2290086d-906d-4e4a-a6e1-d132c52e172e">

Step 9:
Install Heidi SQL to complete installtion.
Select "new".


login it with the password created in MySQL and select "open".

Right click "Unnamed"/create new/database/name database "osTicket"/"ok" 

Finish installtion.


Login into osTicket with Username and password created in installer.









<img width="451" alt="Screen Shot 2024-01-18 at 12 00 03 AM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/d52de009-2224-47bf-ba96-5a459466c7d4">
<img width="537" alt="Screen Shot 2024-01-18 at 12 01 09 AM" src="https://github.com/TakiraMcCoy/osticket-prereqs/assets/155402684/cd3cc16d-5d2d-460f-b09e-16173570d9e4">

























