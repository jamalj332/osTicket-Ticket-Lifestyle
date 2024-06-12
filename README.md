<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket.<br />


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

Intake

We'll start by creating some tickets through the Users created during the last tutorial (Karen and Ken).

1. Go to the End User osTicket URL: http://localhost/osTicket/

2. Open a new ticket

3. Create a few tickets using the examples provided below.
<img width="420" alt="1 business outage ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/e50c92a6-ed6d-447f-840e-ede9db39ccf9">
<img width="421" alt="2 accounting dept ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/4a08483d-5d27-4ba1-a3e2-38d987245a85">
<img width="418" alt="3 general inquiry ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/f0103f00-10fb-4337-8f78-2eef84b83c88">

Assignment and communication

1. Go to the Admin/Agent login page for osTicket: http://localhost/osTicket/scp/login.php

2. Log in as Jane Doe (jane.doe / Password1)

3. You'll notice when we log in as Jane, we are not able to see tickets. We'll have to go back and make some changes to her Agent permissions/settings.
<img width="479" alt="1 jane log in permissions not set" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/c9d06832-9934-4598-ab78-01a232a7e34f">

4. Log in as your main admin account

5. The tickets are visible to the main admin account (while under the Agent panel). Let's make some changes so Jane can view the tickets.
<img width="479" alt="2 tickets visible as admin" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/d54e8bc0-30df-4cc3-82e8-7affcdfb99e1">

6. Go to the Admin Panel -> Agents -> Jane Doe

7. Under the Access tab, set the Extended Access to the Support dept. Click 'Add' then set the role to Supreme Admin. Save changes.
<img width="480" alt="3 jane permissions" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/dd15eb4c-1eb1-42ab-bb23-a76715f7d8cd">

8. While here, let's also change John's role, because we left him as view-only in the last tutorial. Go to Admin Panel -> Agents -> Departments. Click on the Support dept and go the Access tab. Give John 'All Access'. Save changes.

9. Now log back in as Jane and the tickets will be visible.
<img width="479" alt="4 jane tickets visible" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/f07b7bcc-8e9e-481e-9f1f-052837cd3667">

10. Let's take a look at the Business Critical Outage ticket. As Jane, we can view the ticket as well as make changes, assignments and updates:
    - Change the Priority level to Emergency. Because this is a severe business impacting incident, it should be categorized accordingly. You'll notice that you can add in notes the changes made. This is so you can give reasoning and explanation for yourself or other Agents who may view the ticket in the future.
    - Assign the ticket to yourself (acting as the manager). Tickets with this type of severity level would normally be escalated up to some type of management.
    - Set the SLA Plan to SEV-A. Again, this is a severe, business impacting incedent. The ticket should be resolved ASAP.
    - Set the dept to System Administrators. Let's say that the System Administrator dept is responsible for the mobile banking platform. Therefore, that dept is best equipped for handling this type of issue.
    - Notice for each change made, there's a ticket thread that keeps a list of any changes made as well as the notes written for each change.
    - Post a reply with an update for the ticket status. This will be visible by the customer and provides a level of transparency when it comes to ticket resolution.
    - Go ahead and close the ticket by (Select 'Closed' on the Ticket Status drop down before posting a final response.) The ticket will then appear under the 'Closed' section.
<img width="479" alt="8 snip of all changes made for 1st ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/a0bb926a-567a-4abc-bd32-d63d81c7a823">
   
Working The Issue

1. Next lets take a look at the ticket with the entire acounting dept down. This issue is High priority, due to it affecting an entire department. It's not quite as severe as a business outage. We'll have John handle this ticket. Follow the example below and make necessary changes to the ticket.
<img width="478" alt="9 snip of changes made to secong ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/4f815ae3-50dd-4d01-9535-519317d56f80">

2. Let's look at the inquiry about a hardware refresh. Since this is just an inquiry, its low priorty. But we can go ahead and provide the information needed and resolve the ticket (Select 'Resolved' on the Ticket Status drop down before posting a response.) The ticket will then appear under the 'Closed' section.
<img width="479" alt="10 Hardware refresh" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/1f1e339a-c091-479c-b254-975a6fcf346f">

Resolution

1. We'll log in as John and close the final open ticket. He reinstalled the previous version of the sofware and will research the issue with the new version.
<img width="362" alt="11 closed final ticket" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/5a40983f-cb99-4a6a-b786-7d14fc6b5a9f">

2. You can view other closed tickets (under the 'Closed' section in the 'Ticket' tab) and see how other co-workers worked and resolved previous issues. It also serves as good place for learning possible resolutions for common issues that could appear in the future.
<img width="359" alt="12 closed tab for final note" src="https://github.com/DarianWells/osticket-ticket-lifecycle/assets/132870202/4e733fd5-0ff8-4550-a5c4-1663efd484e0">


That's it for the ticket lifecycle tutorial. Thank you for reading!
