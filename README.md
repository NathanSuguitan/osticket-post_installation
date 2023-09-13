<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>


<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Assign Permissions
- Configure Agents
- Configure Users
- Configure SLA's
- Configure Help Topics

<h2>Configuration Steps</h2>

1. Configure Roles <br>
  &nbsp; A. Admin Panel -> Agents -> Roles <br>
  &nbsp; B. Add New Role -> Type "Supreme Admin" -> Checkmark all boxes under "Permissions" (tickets, task, and knowledgebase) -> Add Role


![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/a1e8335f-fec6-4104-b48d-3be35080ba3c)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/01f328fc-c854-45e3-9631-855db36a86a0)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/d14849b5-a7af-4876-a671-13df27e1be69)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/3f7d8cb9-77cd-4d1a-bc88-ee1f861967bb)


2. Configure Departments<br>
    &nbsp; A. Admin Panel -> Agents -> Departments <br>
    &nbsp; &nbsp; B. Add New Department -> Type "System Administrators" -> Create Dept

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/3691ed12-1b97-44dd-ae77-3efa95fe48ca)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/436f51eb-7eb7-4824-b01d-52d993e93ba2)

3. Configure Teams<br>
 &nbsp;  A. Admin Panel -> Agents -> Teams <br>
 &nbsp; &nbsp;  i.  Level I Support <br>
&nbsp; &nbsp; &nbsp;   ii. Add New Team -> Level II Support -> Create Team

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/0180ce6f-1fa2-48e3-bc7d-504d24663392)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/0c146eb5-c3dd-4b80-becb-a174473a0f03)

  4. Allow anyone to Create Tickets <br>
 &nbsp;  A. Admin Panel -> Settings -> Users <br>
  &nbsp; &nbsp; B. Registration Required: Require registration and login to create tickets <br>
    &nbsp; &nbsp; &nbsp; i. Make sure Registration Method says "Public - Anyone Can Register"

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/5d53ba09-0a70-4fed-9fca-d64f6759d522)

5. Configure Agents (workers) <br>
  &nbsp; A. Admin Panel -> Agents -> Add New <br>
 &nbsp; &nbsp;  i. Jane Doe: Add new agent -> Fill out first name, last name, email and username -> Set Password -> Go to Teams -> Choose Support Level -> Add -> Create  <br> 
  &nbsp; &nbsp; &nbsp; ii. !!! Important !!! Be sure to fill out (for the Sys Admin): Extended Access -> Support -> Add -> Select Role -> Supreme Admin -> Create  <br>

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/8652621f-bf22-4f79-b76a-f026a66c3225)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/4f956121-0394-4333-9c18-fd7497624783)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/25593789-7e30-4031-9696-10b0bed5ad5f)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/c851a20c-b39f-46c6-8a97-a9cc71365abe)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/ad94680b-3315-4c19-9ec1-44d3c3cee4c0)

  6. Configure Users (customers)<br>
 &nbsp;  A. Agent Panel -> Users -> Add New <br>
  &nbsp; &nbsp; i. John: New User -> Email, Full Name -> Add User <br> 

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/d4ebe980-0037-4e2c-a75e-4f381419919b)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/7866f4a6-aaf8-4d78-b37d-9bbb65861bef)


7. Configure SLA<br>
  &nbsp; A.Admin Panel -> Manage -> SLA <br>
 &nbsp; &nbsp;  i. Sev-A (1 hour, 24/7): Add New SLA Plan -> Name, Grace Period, Schedule -> Add Plan <br>
 &nbsp; &nbsp; &nbsp;  ii. Sev-B (4 hours, 24/7) <br>
 &nbsp; &nbsp; &nbsp; &nbsp;  iii. Sev-C (8 hours, business hours)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/f90081db-e0e0-4e3d-beb2-b6efa2098429)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/26a0aa4f-968a-4607-862d-c4f2b39c2f58)

8. Configure Help Topics <br>
 &nbsp;  A. Admin Panel -> Manage -> Help Topics <br>
  &nbsp; &nbsp; i. Business Critical Outage: Add New Help Topic -> Topic -> Add Topic <br>
  &nbsp; &nbsp; &nbsp; ii. Personal Computer Issues <br>
  &nbsp; &nbsp; &nbsp; &nbsp; iii. Equipment Request <br>
  &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; iv. Password Reset

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/ca0ff531-7164-44fd-ab01-0d76d44cdc33)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/309e5b5b-932f-4d81-b20d-60b883b8c658)

![image](https://github.com/NathanSuguitan/osticket-post_installation/assets/138082246/c20f22ba-f78d-4356-af01-c81e4c4973a3)


