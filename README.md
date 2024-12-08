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

- Windows 10</b> (22H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<p>
Here are the links to the admin and client ends of our osTicket system: 
  
Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

End Users osTicket URL:
http://localhost/osTicket 

  
First thing we need to do is delete the maintenance department as it will interfere with our lab process. To do this, while in the Admin panel, go to Agents > Departments > Check the box next to Maintenance > More > Delete
</p>

![image](https://github.com/user-attachments/assets/46bb06a2-501d-4137-bd12-322d4e62e630)

<p>
Now, we will create a ticket from the perspective of an end user. To do this, visit the support center webpage - http://localhost/osTicket . Just click Open a new ticket. Enter the information for the user we created in the last part of the walkthrough. For this example, we will be making a ticket surrounding a critical system being down. Phone number is not necessary. Then click Create Ticket.
</p>

![image](https://github.com/user-attachments/assets/4c66b46b-e1ee-4b6c-828a-437498e60a61)

<p>
Next, we need to login as an agent to view the ticket. Login as the second agent we created (The one that is not a member of the team we created or the SysAdmin department). Once logged in, you should see the ticket we created as an end user. Now, we are going to inspect the different properties of this ticket, so click on it. 
</p>

![image](https://github.com/user-attachments/assets/b00ead3e-071e-4596-9163-e48f88d059c2)

<p>
You can see that there are several aspects of this ticket we can interact with and change. After reading the details of the ticket, it can be determined that this is a serious issue, so we can elevate the severity of the ticket by changing the SLA to SEV-A. We should also change the help topic from "Report A Problem" to "Report a Problem / Business Critical Outage". 
We can also change the department to Online Banking so that the correct team will be able to work on the problem. Do this in the "Assigned To:" area.
</p>

![image](https://github.com/user-attachments/assets/30ce46a9-72bc-4b96-a4bd-49ef5d26f52d)

<p>
Now, switch over to the other agent account that should be a member of the Online Banking Team. We can write a response to the ticket and pretend like the issue was resolved. Then to finalize the ticket, we can change the Status from Open to Resolved.
</p>

![image](https://github.com/user-attachments/assets/9b601cd3-7743-4758-9675-3fc9b968b146)

<p>
Lets go ahead and make another ticket as an end user with the following description:  accounting department needs adobe upgrade, broken. 
Then, login as your Agent that is not a member of the Online Banking team. 
In this specific ticket, it would be a good idea to reach out to the person who submitted it to get a better grasp of the issue with more detail.   
Change SLA to Sev-B and the Assigned to to the Agent you are logged in as. 
Finally, mark the ticket as resolved.
</p>

![image](https://github.com/user-attachments/assets/567a817f-467b-4f48-9db8-535c6800d9c2)

<p>
Congratulations! You have finished the walkthrough for setting up and eperimenting with osTicket. Feel free to mess around with osTicket as there is a lot more to do. Just make sure that you stop or delete the Azure VM's so that you are not wasting any money!
</p>
