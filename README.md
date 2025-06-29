<p align="center">

![image](https://github.com/user-attachments/assets/68b61d3f-9575-41c2-80ec-05cbb1f5f5b0)
</p>

<h1>Active Directory - Group Policy Management: Password Policies</h1>
This tutorial outlines how to configure domain-wide password policies using Group Policy Management in Active Directory.<br />

<h2>Why Use Password Policies?</h2>
Implementing password policies in Active Directory is a fundamental step in securing your organization's network. These policies enforce rules such as minimum password length, complexity requirements, and password history, which help:

- Prevent weak or easily guessable passwords

- Reduce the risk of unauthorized access

- Ensure compliance with industry standards or regulatory requirements

- Encourage better user security habits

By centrally managing these settings through Group Policy, administrators can apply consistent security measures across all domain-joined devices.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines – Optional) 
- Remote Desktop (RDP) (Optional) 
- Group Policy Management
- Active Directory

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- A working Domain Controller
- At least one domain-joined client machine.

<h2>Configuration Steps</h2>

<p align="center">
Domain Controller (Log in) -> Server Manager -> Tools -> Group Policy Management 

</p>
<p>

![image](https://github.com/user-attachments/assets/36eab2ae-5384-47de-8bf6-49af6aef959f)

</p>
<br />

<p align="center">
Locate "Default Domain Policy" within the Forest. Then right click it and click edit.

</p>
<p>

![image](https://github.com/user-attachments/assets/eacccd92-6463-42c3-98ae-3febad367ada)

</p>
<br />

<p align="center">
Computer Configuration -> Policies -> Window Setting -> Security Setting -> Account Policies -> Password Policy

</p>
<p>

![image](https://github.com/user-attachments/assets/7dee4c21-72a3-430a-b33a-85efc9777525)
</p>
<br />

<p align="center">
Open Minimum Password length Properties. Adjust password length to 14 characters. Then click OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/be77f35a-5232-48db-8843-087f8f1a00d8)
</p>
<br />

<p align="center">
Open "Password must meet complexity requirements" Properties. Ensure that "Password must meet complexity requirements" is enabled. Then click OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/7bb4895e-ee06-4d2d-b7e1-a1b72998df85)

</p>
<br />

<p align="center">
Open "Maximum password age" Properties. Adjust "Maximum password age" to 30 days if your scenario is a high-security, or legacy-regulated settings. Or you can put 60 days if you are Ideally thinking about typical business environments that maintain good security hygiene but are not bound by strict compliance rules demanding shorter password lifetimes. Then click OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/34df55db-e530-4b24-a4d5-d91cf61a07ca)

</p>
<br />

<p align="center">
Open "Enforce Password History" Properties. Ensure that "Enforce Password History" stays on 24 for the domain controller. Then click OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/30450069-f987-426d-b045-ec04adef3021)

</p>
<br />

<p align="center">
Open "Minimum Password age" Properties. Adjust "Minimum Password age" to 1 day, which usually for most secure environments. Or set it between 2-7 days for high-security or compliance-driven organizations. Then click OK.

</p>
<p>

![image](https://github.com/user-attachments/assets/35391ba1-ae9f-45bc-b08c-bd8265deba90)

</p>
<br />

<p align="center">
Open "Store Passwords using reversible encryption" Properties. Ensure "Store Passwords using reversible encryption" is diabled. It should never be enabled unless application requirements outweights the need to protect password information. Then click OK. So the next time someone changes their password, all of these password requirements must be fulfilled.

</p>
<p>

![image](https://github.com/user-attachments/assets/bdf7366c-0081-4133-aef2-e1aa22c61318)

</p>
<br />

<h3 align="center">Conclusion</h3>

<p align="center">

**Great job!** You've successfully configured domain-wide password policies using Group Policy Management in Active Directory. These settings help enforce strong password standards across your organization, improving overall security posture. Remember to regularly review and update these policies to align with evolving security requirements and organizational needs. Well done on completing this important configuration!</p>

