<h1>Adding A DNS Server</h1>


<h2>Description</h2>
In this lab, I learned to add a DNS server. Domain Name Servers are servers on the Internet whose sole function is to resolve human-readable domain names into their computer-readable IP addresses.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 

<h2>Utilities and Language </h2>

- <b>Windows Powershell</b>

<h2>Program walk-through:</h2>

<p align="center">
Right click the Start menu and click Network Connections: <br/>
<img src="https://i.postimg.cc/q7wnL6Ms/Screen-Shot-2022-06-22-at-10-24-01-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
<br />
In the Network Connections Window, Double Click the Ethernet 2 network adapter:  <br/>
<img src="https://i.postimg.cc/Bbmq6Dsv/Screen-Shot-2022-06-22-at-10-26-36-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the Ethernet 2 status dialog box, click Properties: <br/>
<img src="https://i.postimg.cc/8zZNmLrB/Screen-Shot-2022-06-22-at-10-28-49-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>

 
  
  
<br />
In the Ethernet 2 Properties dialog box, under This connection uses the following items, double-click Internet Protocol Version 4 (TCP/IPv4):  <br/>
<img src="https://i.postimg.cc/g0kMWZjJ/Screen-Shot-2022-06-22-at-10-34-11-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the Internet Protocol Version 4 (TCP/IPv4) Properties dialog box, click Use the following IP address and type information:  <br/>
<img src="https://i.postimg.cc/NGJb6MNq/Screen-Shot-2022-06-22-at-10-40-03-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
Click start menu and open Windows Powershell:  <br/>
<img src="https://i.postimg.cc/MTNLYmw4/Screen-Shot-2022-06-22-at-10-43-42-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
   
  
<br />
In the Windows Powershell window, execute the following command to get the IP address of the Ethernet 2 Network: (Get-NetAdapter -Name "Ethernet 2" | Get-NetIPAddress).IPAddress:  <br/>
<img src="https://i.postimg.cc/7P25xP5M/Screen-Shot-2022-06-22-at-10-46-55-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
  
  
  <br />
You will observe the IP address as 135.58.24.17:  <br/>
<img src="https://i.postimg.cc/FzNQcQ4z/Screen-Shot-2022-06-22-at-10-58-53-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
