<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1> Creating Users with PowerShell</h1>
This tutorial outlines steps on how to configure users in PowerShell within Azure Virtual Machines.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2> Configuration Steps</h2>

1. Log into Client-1 as mydomain.com\jane_admin

- Open system properties
- Click “Remote Desktop”
- Allow “domain users” access to the remote desktop
- You can now log into Client-1 as a normal, non-administrative user.

<img width="2559" height="1439" alt="Screenshot 2025-07-21 103404" src="https://github.com/user-attachments/assets/6b2f91cc-3a90-40eb-943d-24d6ea5a8401" />

2. Log in to DC-1 as jane_admin
- Open PowerShell_ise as an administrator
- Create a new File and paste the contents of the script into it

<img width="2559" height="1439" alt="Screenshot 2025-07-21 104533" src="https://github.com/user-attachments/assets/70dc71a0-b2ef-49c6-a4f3-2f7f60e12757" />

3. Run the script and observe the accounts being created
- When finished, open ADUC and observe the accounts in the appropriate OU　(_EMPLOYEES)

  <img width="2559" height="1439" alt="Screenshot 2025-07-21 105018" src="https://github.com/user-attachments/assets/7aef91be-0060-4dd2-8126-e1ce7c125faa" />

4. Attempt to log into Client-1 with one of the accounts (take note of the password in the script)

   - Username: bab.pif
   - Password: Password1
   - We successfully logged in to a client account!

<img width="2559" height="1439" alt="Screenshot 2025-07-21 105751" src="https://github.com/user-attachments/assets/111310fb-ae17-45a0-b735-b4a8f4c0d42c" />

     


