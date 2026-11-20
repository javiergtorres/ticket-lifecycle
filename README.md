# ticket-lifecycle
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle</h1>
This tutorial outlines a ticket lifecycle from creation to completion on the ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11
- Garuda Linux</b> 

<h2> Objective</h2>

Create a couple of tickets using the User portal inside osTicket as an End User (I’ll pretend to be an End User with a problem).

After the ticket is created I’ll login as a Help Desk technician (IT person). I’ll observe the ticket, triage it, then work it to completion.

<h2> Login to Microsoft Azure, get Windows 11 virtual machine login information</h2>

<p>
<img width="1901" height="930" alt="gettingipaddressfrom-osticket-vm" src="https://github.com/user-attachments/assets/756917c3-13d3-4a5f-8eba-423c52387f46" />

</p>
<p>
First thing, I created a Windows 11 virtual machine in Microsoft Azure. I'll need the public IP address, username, and password of the virtual machine so I can remote desktop in to the virtual machine. You can see the public IP address in the photo.
</p>

<h2>Using RDP (Remote Desktop Protocol) to connect to virtual machine</h2>
<br />

<p>
<img width="1912" height="1080" alt="remotedesktop-loginscreen" src="https://github.com/user-attachments/assets/d573cbe3-5416-4bcc-a0e9-7945908bcba9" />

</p>
<p>
The software I'm using on my laptop is Garuda Linux. Here you can see I'm using Remmina, a Remote Desktop Protocol application, one of the main options for using RDP on Linux. All I need is to punch in the public IP address of the virtual machine, username,and password in the correct fields. From here I'll connect to the Windows 11 virtual machine by pressing the connect button.
</p>
<br />

<h2>Creating a ticket as an End User (Karen)</h2>

<p>
<img width="1826" height="1028" alt="end-user-loginscreen" src="https://github.com/user-attachments/assets/ae10a4af-2901-42a3-acbc-6537d143cf70" />

</p>
<p>
Here you can see the portal screen for an End User. From here click "Open New Ticket".
</p>

<p>
  <img width="1861" height="1038" alt="creating-ticket-as-Karen" src="https://github.com/user-attachments/assets/9253eb1b-6468-4f0c-8827-70adb6f2b837" />

</p>

<p>
  As Karen, I'm filling out my info. Describing the issue as best as I can. After that I'll click "Create Ticket"
</p>

<p>
  <img width="1867" height="1035" alt="Screenshot_20261119_210021" src="https://github.com/user-attachments/assets/335a0868-cf4a-470c-b248-b2ca91f83181" />

</p>

<p>
  Ticket has been created.
</p>

<h2>
  Login as John (Help Desk Technician)
</h2>

<p>
  <img width="1850" height="1041" alt="login-as-John(Agent)" src="https://github.com/user-attachments/assets/bf930edf-0c2d-4b94-a6ec-9fd302739fb9" />

</p>

<p>
  From here, I'll login as John, a Help Desk technician, observe the ticket, and work it to completion
</p>

<p>
  <img width="1860" height="1044" alt="osTicket-homescreen-forJohn" src="https://github.com/user-attachments/assets/2cbc72c5-bba0-47e9-8018-6fab68746c13" />

</p>

<p>
  Here, on the home screen as John, I can see the ticket that Karen has created. I'll click it to open it and observe the ticket
</p>

<p>
  <img width="1868" height="1034" alt="observing-the-ticket-asJohn" src="https://github.com/user-attachments/assets/2e21b81c-f868-412b-bccf-c6ccdf4900a4" />

</p>

<p>
  <img width="1863" height="1044" alt="observing-the-ticket-asJohn2" src="https://github.com/user-attachments/assets/8f1c8d94-a114-4e4c-80ac-b0c5371d3086" />

</p>

<p>
  From here, I contacted Karen, and verified what's going on and the severity of the issue. First thing I'll do is change the priority of the ticket.
</p>

<p>
  <img width="1870" height="1046" alt="changing-priority-of-problem-on-ticket" src="https://github.com/user-attachments/assets/b4d0041e-6e30-4702-ad41-5a062a9de611" />

</p>

<p>
  Next to "Priority", it says "Normal". I clicked that so I can change the priority level to a more urgent level since the entire business system is down. I'll change it to "Emergency" and expalin why. Then I'll click "Update".
</p>

<p>
  <img width="1859" height="1043" alt="changing-the-SLA-plan" src="https://github.com/user-attachments/assets/2b00adeb-c4a8-42d5-bd6b-ae5232e7a463" />

</p>

<p>
  After that, I noticed the SLA plan hasn't been set. I'll set it to: Sev-A. The reason is because this is a business critical issue and needs to be resolved ASAP. 

  For this, next to "SLA Plan", it says "Default SLA". I'll click that, set the SLA Plan to Sev-A and explain why. Then I'll click "Update".
</p>

<p>
  <img width="1865" height="1042" alt="changed-the-help-topic" src="https://github.com/user-attachments/assets/0866e1c6-3453-4d4d-a4b2-d332734b35a5" />

</p>

<p>
  I'll also change the Help Topic from "General Inquiry" to "Business Critical Outage" which is a more appropriate help topic. For that, next to "Help Topic", click "General Inquiry" then a pop up will appear. In the drop-down menu, I chose "Report a problem/business critical outage" and explained why. Then I clicked "Update".
</p>

<p>
  <img width="1870" height="1041" alt="writing-comment-on-ticket" src="https://github.com/user-attachments/assets/b7b2f6ca-44f1-49f7-a93a-c4d76f01e9de" />

</p>

<p>
  From here, I'll also add a comment saying that I'll pass this ticket along to the SysAdmin Department. The scenario is that I'm an entry level Help Desk technician, therefore would not be able to solve this issue and will forward it along to the correct department.
</p>
<br />
