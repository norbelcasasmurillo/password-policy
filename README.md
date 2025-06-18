<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to create, work, and resolves tickets within osTicket](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>

![image](https://github.com/user-attachments/assets/102870fa-43ca-4c71-a73c-8dbce9327109)
</p>
<p>
Domain Controller -> Server Manager -> Tools -> Group Policy Management 

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/e1ae9225-5f31-4179-b176-5227a4f442f5)


</p>
<p>
Locate "Default Domain Policy" within the Forest. Then right click it and click edit.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/44894f54-01e9-401e-94c0-79d1a3c7cf78)

</p>
<p>
Computer Configuration -> Policies -> Window Setting -> Security Setting -> Account Policies -> Password Policy
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/bc688b31-7d36-4edf-ab4f-bef5ab2a741c)

</p>
<p>
Open Minimum Password length Properties. Adjust password length to 14 characters. Then click OK.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/7bb4895e-ee06-4d2d-b7e1-a1b72998df85)

</p>
<p>
Open "Password must meet complexity requirements" Properties. Ensure that "Password must meet complexity requirements" is enabled. Then click OK.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/486e78b4-257d-4f84-b9cd-811e774c63c3)


</p>
<p>
Open "Maximum password age" Properties. Adjust "Maximum password age" to 30 days if your scenario is a high-security, or legacy-regulated settings. Or you can put 60 days if you are Ideally thinking about typical business environments that maintain good security hygiene but are not bound by strict compliance rules demanding shorter password lifetimes. Then click OK.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/3c639423-8a55-4769-9554-089ba9fc2509)

</p>
<p>
Open "Enforce Password History" Properties. Ensure that "Enforce Password History" stays on 24 for the domain controller. Then click OK.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/2f8c4008-45f7-440a-8ce1-204c1f877d09)


</p>
<p>
Open "Minimum Password age" Properties. Adjust "Minimum Password age" to 1 day, which usually for most secure environments. Or set it between 2-7 days for high-security or compliance-driven organizations. Then click OK.

</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/bdf7366c-0081-4133-aef2-e1aa22c61318)

</p>
<p>
Open "Store Passwords using reversible encryption" Properties. Ensure "Store Passwords using reversible encryption" is diabled. It should never be enabled unless application requirements outweights the need to protect password information. Then click OK. So the next time someone changes their password, all of these password requirements must be fulfilled.

</p>
<br />

