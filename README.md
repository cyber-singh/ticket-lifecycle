<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle Examples</h1>

This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. This tutorial assumes you have completed both the <a href= "https://github.com/cyber-singh/osticket-prereqs"> installation </a> and <a href = "https://github.com/cyber-singh/post-install-config">configuration</a> of osTicket

</br>

<p>
<h2>Environments and Technologies Used</h2>

 - **Microsoft Azure (Virtual Machines/Compute)**
 - **Remote Desktop**
 - **Internet Information Services (IIS)**
 - **osTicket**
  
   </p>

</br>

<h2>Operating System Used</h2>

 - **Windows 10**

</br>

<p>
  <h2>Ticket Lifecycle Stages</h2>

**1. Intake**  
**2. Assignment & Communication**   
**3. Working the Issue**   
**4. Resolution**  
    </p>

</br>

<p>
<h2>Lifecycle Stages</h2>

<h3>Intake</h3>

 - **From the End User's Perspective (Karen Karen):** Karen initiates the ticket creation process by accessing **osTicket's local host site**. She provides her details and selects a relevant **Help Topic**.  

   <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/e34eb6f7-1bc9-47ad-af5a-577f1a5296f4"/>
   </p>

</br>

<p>
  
 - **End User's Action:** Subsequently, the **End User (Karen Karen)** provides detailed information about the issue by composing a ticket through the **Issue Summary**. This includes specifying a subject and furnishing details related to the ticket, resembling the process of composing an email.

 - **Ticket Creation Example:** In this instance, **Karen** initiates the ticket creation process under the Help Topic category of a **Business Critical Outage**, a configuration we set up in **osTicket**. **Karen** articulates the issue, elucidating that the **Mobile Banking Application** is encountering a **404 error**.

   <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/ca9e6496-5f95-4708-87db-7de83e851b1a"/>
   </p>

</br>

<p>
  
 - **Ticket Assignment:** After **Karen** creates the ticket, it is directed to Agent **Jane Doe**, designated as the **Supreme Admin** with the ability to monitor all incoming tickets, as configured in the tutorial. **Jane Doe** reviews the ticket through the local Help Desk Login Interface.

 - **Ticket Priorities:** It's important to note that **Priorities** haven't been assigned for other incoming tickets, like **Ticket #951342**, where end user **Ken** is seeking an upgrade to Adobe Reader. The tutorial suggests the necessity to set **SLA plans** for these tickets, hence why they currently fall under the **"Normal"** priority state.
 
    <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/a04d0885-6d48-4f9f-a600-4a23eef184b7"/>
    </p>
    
****

<p>  
<h3>Assignment & Communication</h3>  
<br>  

- **Ticket Assignment:** The **Business Critical Outage** ticket, **Numbered 282733**, created by **Karen**, is now assigned to Agent **Jane Doe**. From Jane's perspective, the picture illustrates how the ticket appears when initially viewed.

- **Communication via Ticket Thread:** Within the ticket page, Agent Jane Doe can communicate with the End User, Karen, through the **Ticket Thread** located at the bottom of the page.
 
    <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/7e14f2ab-cab9-4d4a-84c2-960e0410030e"/>
    </p>

</br>

<p>
  
- **Setting Ticket Priority:** To adjust the priority of the ticket, click on the link next to **"Priority"**. You can choose from options such as **Low**, **Normal**, **High**, or **Emergency**.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/1c8fe483-5ff2-4205-84f9-fb9b96f221a9"/>

<br>
  
- **Assigning the Ticket:** Click on the greyed-out link --**Unassigned**-- next to **"Assigned To"**. Here, you can assign the ticket to a **Team** or specific **Agents**. Keep in mind that if assigned to an Agent outside of Agent **Jane's Department**, it won't appear in their feed.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/565c86b4-31cc-4e88-9e83-aa4e7d222bc2"/>

</br>

- **Setting SLA Plan:** Navigate to the link next to **"SLA Plan"**. Change it from the **Default SLA** to one of the SLA Plans configured earlier. For the **Business Critical Outage** ticket, set it to **SEV-A**.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/22b50dd2-777b-4917-b252-747807a132cd"/>

</br>

- **Adjusting Department:** Click on the link next to **"Department"** to modify it. Change it from **Support** to **System Administrators** for this Business Critical Outage ticket.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/5f2608bd-9b16-4b31-b0bd-9d340cb2c1f2"/>

</br>

- **Updating Ticket Thread:** The Ticket Thread is automatically updated when changes are made to the ticket.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/4e5aca49-6acb-4813-8455-593b3744ba70"/>

</br>

- **Agent Communication:** The **Agent** can use the **Ticket Thread** to send messages to the **End User**, providing updates on the ticket. Additionally, the Agent can adjust the ticket **Status** as needed, with the current status being left as **"Open"** while the issue is being addressed.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/17b4e37e-3ebd-430b-91c7-1fd88e321074"/>
  </p>

****  

<p>
<h3>Working the Issue and Resolution</h3>  

- **Issue Resolution:** After addressing the problem through departmental assignment and communication with the End User, the critical banking outage in our **Hypothetical scenario** has been **successfully resolved**, courtesy of the **System Engineering team**. The **Agent** must now inform the **End User** about the **Resolution** using the **Ticket Thread**. Furthermore, the Agent should update the ticket **status** from **"Open"** to **"Resolved"**. Once the reply is posted, the ticket is marked as **"Closed"**.

  <img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/f9ea5d54-2498-49b9-943d-b044c2ecbd02"/>

</br>

- **Ticket Closure and Archiving:** Closed tickets are archived and can be accessed under the **"Closed"** section in the **Tickets** tab. This serves as a valuable resource for **Agents** to enhance their expertise by studying the information and status of past tickets. Analyzing closed tickets contributes to continuous improvement in managing and resolving similar issues in the future.
</p>

****

<h3>Conclusion:</h3>  

 - **Congratulations!** You've successfully navigated the intricate stages of osTicket, from its installation and configuration to the practical handling of tickets in a simulated environment. This tutorial has equipped you with the essential skills to manage the complete lifecycle of a ticket, ensuring efficient issue resolution and user communication.

 - Thank you for embarking on this osTicket journey with **[ME](https://www.linkedin.com/in/cybersingh)**. ***Happy ticketing!***

