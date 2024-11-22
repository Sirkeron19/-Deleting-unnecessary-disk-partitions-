<h1>Wiping Unnecessary Disk Partitions using Disk Management and Windows PowerShell<h1>

 ### [YouTube Demonstration](https://www.youtube.com/watch?v=Up68ykJCKn4)

<h2>Description</h2>
This repository provides a guide and set of instructions for removing unnecessary disk partitions on a Windows system. It outlines how to manage disk partitions both using the built-in Disk Management tool and the Windows PowerShell command line.


<h2>Languages and Utilities Used</h2>

- <b>DiskManagement</b>
- <b>PowerShell</b> 
- <b>Diskpart</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (21H2)

<h2>The Problem</h2>

![Screenshot 2024-11-21 172250](https://github.com/user-attachments/assets/5b833d56-df25-4338-99a8-c56255de7afc)
<p align="center">
Launch the Disk Management: <br/>

![Screenshot 2024-11-21 172325](https://github.com/user-attachments/assets/73711c28-0e35-4064-8115-25e650c87279)

<img width="960" alt="Screenshot_1" src="https://github.com/user-attachments/assets/385e3fbe-9fc0-4ade-8e3b-cc9cd2e56a3e">

<p align="center">  
You Can See Disk 1 has 3 partitions with its own Drive Letter

<p align="center">
We want to clean this entire drive erasing all those partitions

<h2>Program walk-through:</h2>

<p align="center">
Launch Windows Powershell

![Screenshot 2024-11-21 172817](https://github.com/user-attachments/assets/e01106db-1a8e-4bd8-a922-a4b2566ed4a8)

<p align="center">
Right click it and run it in adminstrator mode

![Screenshot 2024-11-21 173608](https://github.com/user-attachments/assets/c2ffdd96-a8e4-4869-bdb5-7c29aae84dad)

<p align="center">
<img width="673" alt="Screenshot_2" src="https://github.com/user-attachments/assets/7a82e42c-d392-40c7-9ac5-3cb85b14e96a">

<p align="center">
type "diskpart
  
<p align="center">
<img width="671" alt="Screenshot_3" src="https://github.com/user-attachments/assets/4d192c76-92d8-4fe4-89ef-0077d0939b95">

<p align="center">
Now we need to see the disk that has the issue

<p align="center">  
Type "list disk"

<p align="center">
<img width="672" alt="Screenshot_4" src="https://github.com/user-attachments/assets/bc933d14-50f6-4eaa-ab99-972f4995b53d">

<p align="center">
<img width="669" alt="Screenshot_5" src="https://github.com/user-attachments/assets/a0293154-ed49-4eb9-adab-e649dc2b032f">

<p align="center">
You can now see all disk that on pc (in my case my issue is with disk 1)

<p align="center">
Now we need to select that disk

<p align="center">
type select disk 1 

<p align="center">
(make sure to use the number that's assocated with your disk you having a problem with

<p align="center">
<img width="672" alt="Screenshot_6" src="https://github.com/user-attachments/assets/2781f8ee-d40d-40db-af53-f5b6102db69f">

<p align="center">
<img width="670" alt="Screenshot_7" src="https://github.com/user-attachments/assets/313fe99c-e4eb-463e-bbab-2272383f81de">

<p align="center">
Now all we have to do now is type the word "clean"

<p align="center">
<img width="671" alt="Screenshot_8" src="https://github.com/user-attachments/assets/c17a6788-38f9-4162-bb8c-f3e21b697829">

<p align="center">
<img width="960" alt="Screenshot_9" src="https://github.com/user-attachments/assets/0986cae8-1e43-4345-ba0d-1a8c709db6b2">

<p align="center">
And as you can see! Our issue is now solved

<p align="center">
in windows explorer it shows only 2 drives

<p align="center">
And in Disk Management

<p align="center">
<img width="560" alt="Screenshot_10" src="https://github.com/user-attachments/assets/06b90338-baa0-4ac3-a36c-450f98d41f3f">

<p align="center">
It shows Disk 1 with all available space































