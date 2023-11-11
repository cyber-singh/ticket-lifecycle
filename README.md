<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Ticket Lifecycle Examples</h1>
This tutorial outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system osTicket. This tutorial assumes you have completed both the <a href= "https://github.com/cyber-singh/osticket-prereqs"> installation </a> and <a href = "https://github.com/cyber-singh/post-install-config">configuration</a> of osTicket

</br>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
  <li>osTicket</li>
</ul>

</br>

<h2>Operating Systems Used </h2>
<ul>
  <li>Windows 10</li>
</ul>

</br>

<h2>Ticket Lifecycle Stages</h2>
<ol>
  <li>Intake</li>
  <li>Assignment & Communication</li>
  <li>Working the Issue</li>
  <li>Resolution</li>
</ol>

</br>

<h2>Lifecycle Stages</h2>


<h3>Intake</h3>

<p>
  <ul>
    <li>From the <b>End User's</b> side (Karen Karen), they create a ticket through osTicket's <a href = "http://localhost/osTicket/ ">local host site</a> and fill their information, select a Help Topic</li>
    <ul>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/e34eb6f7-1bc9-47ad-af5a-577f1a5296f4"/>
     
    </ul>
    
    <li>The End User then writes ticket through the <b>Issue Summary</b> and adds a subject and details of the ticket much similar to writing an email</li>
    <ul>
      <li>In this example, Karen creates the ticket under the Help Topic of a Business Critcal Outage (made from our configuration of osTicket) explaining the mobile banking application is suffering a 404 error</li>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/ca9e6496-5f95-4708-87db-7de83e851b1a"/>
    
    </ul>
    <li>Karen then creates the ticket and is sent to <b>Agent</b> Jane Doe (which we've set as Supreme Admin is able to see all incoming tickets in the configuration tutorial) who views it from the <a href = "http://localhost/osTicket/scp/login.php">local help desk login</a></li>
    <ul>
      <li><b>Note</b>: Priorities have not been set for other incoming tickets such as ticket #951342 where end user Ken is requesting an upgrade to Adobe Reader. SLA plans need to be set for these tickets hence why they are all under the priority state of "Normal"</li>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/a04d0885-6d48-4f9f-a600-4a23eef184b7"/>
    
    </ul>
  </ul>
</p>

<h3>Assignment & Communication</h3>

<p>
  <ul>
    <li>The Business Critical Outage ticket by Karen numbered 282733 is assigned to the Agent Jane Doe. From Jane's perspective, this is how the ticket first looks.</li>
    <ul>
      <li>The Agent is able to message the End User through the <b>Ticket Thread</b> located in the bottom of the ticket page</li>
     
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/7e14f2ab-cab9-4d4a-84c2-960e0410030e"/>
    
    </ul>
    <li>By going to the link next to <b>Priority</b>, you are able to set the priority of the ticket to Low, Normal, High, or Emergency</li>
    <ul>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/1c8fe483-5ff2-4205-84f9-fb9b96f221a9"/>
   
    </ul>
    <li>By going to the greyed out link --Unassigned-- next to <b>Assigned to</b>, you can assign the ticket to a Team or Agents. Note if we were to assign it to an Agent outside of Agent Jane's Department, it will not appear in their feed.</li>
    <ul>
    
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/565c86b4-31cc-4e88-9e83-aa4e7d222bc2"/>
  
    </ul>
    <li>By going to the link next to <b>SLA Plan</b> to set the SLA Plan from Default SLA to one our SLA Plans we have created in configuration. For this Business Critical Outage ticket, it'll be set to SEV-A</li>
    <ul>
    
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/22b50dd2-777b-4917-b252-747807a132cd"/>
    
    </ul>
    <li>By going to the link next to <b>Department</b> to set the Department. For this Business Critical Outage ticket, it'll be set from Support to System Administrators</li>
    <ul>
     
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/5f2608bd-9b16-4b31-b0bd-9d340cb2c1f2"/>
    
    </ul>
    <li>The Ticket Thread is updated when we make the changes to ticket</li>
    <ul>
     
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/4e5aca49-6acb-4813-8455-593b3744ba70"/>
    
    </ul>
    <li>The Agent can message the End User through the Ticket Thread to update the User on the ticket as well as set the status of the ticket (which is left as <b>Open</b> since we need to work it out)</li>
    <ul>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/17b4e37e-3ebd-430b-91c7-1fd88e321074"/>
   
    </ul>
  </ul>
</p>

<br />

<h3>Working the Issue and Resolution</h3>

<p>
  <ul>
    <li>Following from our Assignment of Departments and Communication with the End User, the issue in our hypothetical Critical Banking Outage ticket has been resolved thanks to System Engineering. The Agent should now communicate the issue with the End User using the Ticket Thread and set the status of the ticket from Open to <b>Resolved</b>. Upon posting the Reply, the ticket is <b>Closed</b>.</li>
    <ul>
      
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/f9ea5d54-2498-49b9-943d-b044c2ecbd02"/>
   
    </ul>
    <li>Closed tickets can be found under the Closed section in our Tickets tab, where information and status of the tickets are archived. It is good practice for Agents to study Closed tickets to improve their experience in working with them</li>
    <ul>
    
<img src="https://github.com/cyber-singh/ticket-lifecycle/assets/149118027/0bebfb91-4aad-469e-b3fe-0092ac2ca9b6"/>
  
    </ul>
  </ul>
</p>

<br />
