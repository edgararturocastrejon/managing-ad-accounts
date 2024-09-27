<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Enabling and Unlocking Accounts and Resetting Passwords</h1>
In this tutorial, we are dealing with account lockouts, observing logs, enabling and disabling accounts in Microsoft Active Directory. <br />


<h2>Environments and Technologies Used</h2>

- MacBook Pro
- Microsoft Azure (Virtual Machines/Compute)
- Microsoft Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Windows Server 2022

<h2>High-Level Steps</h2>

- Log into DC-1 as Admin
- Configure Group Policy to Lockout the account after 5 attempts:
- Pick a random user account you created previously
- Attempt to log in with it 6 times with a bad password as Client-1
- Lockout account
- Unlock account

<h2>Actions and Observations</h2>

<p>  
  
![Screen Shot 2024-09-26 at 9 38 33 PM](https://github.com/user-attachments/assets/9e3628d9-3555-4350-a935-98f8e1d4e4f0)


</p>
<p>
Get logged into DC-1 
  
</p>
<br />

<p>
  
![Screen Shot 2024-09-27 at 9 51 54 AM](https://github.com/user-attachments/assets/7f6c3d21-d201-415f-b41e-3c4134c227cc)
![Screen Shot 2024-09-26 at 7 36 33 PM](https://github.com/user-attachments/assets/bd768f83-8eda-4782-b594-e8bc18a12c18)
![Screen Shot 2024-09-27 at 9 58 03 AM](https://github.com/user-attachments/assets/7a4060c9-a017-4eeb-b55b-dce3880b9f89)
![Screen Shot 2024-09-27 at 10 00 05 AM](https://github.com/user-attachments/assets/45393860-58f5-4b01-a9f1-04d285356aeb)


</p>
<p>
Configure Group Policy to Lockout the account <p/>
  
<p> Click Start, and type gpmc.msc in the search box, then press Enter. This opens the Group Policy Management Console. <p/>


</p>
<br />

<p>

![Screen Shot 2024-09-27 at 10 20 20 AM](https://github.com/user-attachments/assets/c2e96127-db06-4ee9-94f3-6ca83454ef48)


</p>
<p>
  Pick a random user account you created previously and try to loggin to Client-1
  <p> Attempt to log in with it 5 times with a bad password to lock the account <p/>
    
</p>
<br />

<p>
  
![Screen Shot 2024-09-27 at 10 44 19 AM](https://github.com/user-attachments/assets/53eeaac2-77af-4555-ad5a-3c3214cab9c0)
![Screen Shot 2024-09-27 at 10 39 46 AM](https://github.com/user-attachments/assets/cd2e752f-eca6-4013-97fa-e3c172139f29)
![Screen Shot 2024-09-27 at 10 52 49 AM](https://github.com/user-attachments/assets/a09d5abe-3790-411a-a004-f9f59b646372)

</p>
<p>
Go back to DC-1, head to Active Directory Users and Computers <p/>
    Right click mydomain.com, click on Find... to search for user we locked out
  <p> Double click on user, click on Account, check off the unlock users account, press apply  </p>
        We unlocked the account!
  
</p>
<br />

<p>

![Screen Shot 2024-09-27 at 11 04 36 AM](https://github.com/user-attachments/assets/e78e281d-613c-4076-87c2-bb06e40e9312)
![Screen Shot 2024-09-27 at 11 04 45 AM](https://github.com/user-attachments/assets/3300fa05-dce6-4709-99ea-6cce4eba1e7c)

</p>
<p>
Go to Client-1 and loggin to user <p/>
  We successfully unlocked account!
  <p>------------------------------------------ <p/>
<p> Next, we will Enable and Disable accounts </p>
  
</p>
<br />

<p>

![Screen Shot 2024-09-27 at 10 44 19 AM](https://github.com/user-attachments/assets/53eeaac2-77af-4555-ad5a-3c3214cab9c0)
![Screen Shot 2024-09-27 at 10 39 46 AM](https://github.com/user-attachments/assets/cd2e752f-eca6-4013-97fa-e3c172139f29)
![Screen Shot 2024-09-27 at 11 38 02 AM](https://github.com/user-attachments/assets/804bdece-d4dd-427c-b808-b72f59f0e73a)


</p>
<p>
Go back to DC-1, head to Active Directory Users and Computers <p/>
    Right click mydomain.com, click on Find... to search for user we unlocked, 
  <p> Right click on user -> Disable Account -> Ok </p>
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
