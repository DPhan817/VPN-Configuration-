# VPN-Configuration<p align="center">
<img src="https://imgur.com/QYDPM41.png" height="40%" width="60%"/>
</p>

<h1>Observing the Effect of a VPN on IP Addressing</h1>
In this project, the impact of a virtual private network (VPN) on IP address will be observed. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines)
-	Remote Desktop
-	ProtonVPN (free version)


<h2>Operating System Used </h2>

- Windows 10 (21H2)

<h2>High-Level Steps</h2>

-	Create a Windows 10 virtual machine in Azure
-	Remote Desktop into the virtual machine
-	Use whatismyipaddress.com to find the IP address and location for the virtual machine
-	Download the free version of ProtonVPN 
-	In ProtonVPN, connect to a server in another country
-	Use whatismyipaddress.com to find the new IP address and location for the virtual machine
-	Browse a webpage to see if there are any changes to the URL or language
-	Delete Resource Groups in Azure


<h2>Summary</h2>

<p>
<img src="https://imgur.com/ZwnmwMj.png" height="70%" width="70%"/> 
</p>
<p>
On your pc type in "free azure account". Click on the link which should say "Create Your Azure Free Account Today". In the webpage, click on the "start free" box. 
 
<p>
<img src="https://imgur.com/hrlVkh2.jpg" height="70%" width="70%"/> 
</p>
<p>
You will be prompted to sign into an existing Microsoft account or to create one (Note: creating an azure account does require the use of a credit card, but will not charge the card unless the free $200 of credit that is applied to the account is exceeded so be sure to have that ready to input.)
</p>
<br />

<p>
<img src="https://imgur.com/2r2x9vk.jpg" height="70%" width="70%"/>
</p>
<p>
After creating your account, go to the Azure portal by typing in portal.azure.com in the search bar. Verify the creation of your new subscription by typing in "subscription" in the Microsoft azure search bar interface. 

<p>
<img src="https://imgur.com/hXloN6k.jpg" height="70%" width="70%"/>
</p>
<p>  
Open another web browser and type in the search bar "whatismyipaddress.com". Take a note of the IP address displayed. (Note: it's important not to share or disclose your public IP address with just anyone because it can expose your location, gain access to your network and devices, as well as make you vulnerable to hackers.
</p>
<br />

<p>
<img src="https://imgur.com/LKzSdDC.jpeg" height="70%" width="70%"/>
</p>
<p>
Go back to the Microsoft Azure interface. Type in "virtual machine" in the Microsoft azure search bar and select the virtual machine icon. This step will require basically just inputting different names or titles and selecting different types of resources. 
</p>
<br />

 - Subscription: (choose subscription you created)
 - Resource Group: (leave unmarked, or create in advance)
 - Virtual machine: (provide a name)
 - Region: select any available region and take note of it (in this demonstration, (Europe) France Central is used)
 - Image: select "Windows 10 pro, version 21H2 - Gen2 (free services eligible)" 
 - Size: (choose an option of your choice for the best performance)
 - Administrator Account: (create a username and password)

<p>
Check the licensing agreement box then click "Review + Create". Once the process is finished validating all the resources, click "Create" to initialize the virtual machine.
</p>
<br />

<p>
<img src="https://imgur.com/H6mxDfP.jpeg" height="70%" width="70%"/>
</p>
<p>
After the virtual machine is created, click on the virtual machine and copy the public IP address of the virtual machine in order to connect to it remotely. Depending on the operating system, open up either "Remote Desktop Connection" (Windows) or in this case, "Microsoft Remote Desktop" (MacOS), and click on "Add PC".
</p>
<br />

<p>
<img src="https://imgur.com/EXx7nb2.png" height="70%" width="70%"/>
</p>
<p>
Input the public IP address of the virtual machine in for the "PC Name" then click "add".
</p>
<br />

<p>
<img src="https://imgur.com/K3TcgcP.jpeg" height="70%" width="70%"/>  
</p>
<p>
Click on the interface of the virtual machine and input the username and password that you used when creating the virtual machine.
</p>
<br />

<p>
<img src="https://imgur.com/UEUFRyX.jpeg" height="70%" width="70%"/>
</p>
<p>
After the connection to the virtual machine is completed, open up the web browser and type in whatismyipaddress.com and take note of the ip that is displayed. 
</p>
<br />

<p>
<img src="https://imgur.com/HMrzsQx.jpg" height="70%" width="70%"/>
</p>
<p>
Open up another tab, and type in protonvpn.com in the browser. Click on create free account and fill out the informatoin to create your account. 
</p>
<br />

<p>
<img src="https://imgur.com/bksha5p.jpg" height="70%" width="70%"/>
</p>
<p>
After creating the Proton VPN account, download the proton vpn client that is necessary for your OS. 
</p>
<br />

<p>
<img src="https://imgur.com/p148AAS.jpg" height="70%" width="70%"/>
</p>
<p>
Once the download is completed, open up the VPN client installer and select all the default options for the proton VPN setup wizard. 
</p>
<br />

<p>
<img src="https://imgur.com/G8v30oe.jpg" height="70%" width="70%"/>
</p>
<p>
Once the installation is completed open up the proton VPN application and login with the same credentials used to create the account. 
</p>
<br />

<p>
<img src="https://imgur.com/crsLB4o.jpg" height="70%" width="70%"/>
</p>
<p>
When you get logged in there will likely only be a few options for VPN servers due to the limited selection of the free account.
</p>

<p>
<img src="https://imgur.com/jA5zMPv.jpg" height="70%" width="70%"/>
</p>
<p>  
Choose any one of the available VPN servers to connect to and allow the connection to build up. In this demonstration, Netherlands is selected. 
</p>  

<p>
<img src="https://imgur.com/9p80LP4.png" height="70%" width="70%"/>
</p>
<p>
Once the connection is completed, refresh the dashboard interface to confirm an established connection, open up a web browser and go to "whatismyipaddress.com" and you'll see that the public ip address of the VM now displays region in which the VPN server is located in. 
</p>
  
In conclusion, a VPN (Virtual Private Network) encrypts your internet connection, hides your IP address, and provides privacy and security by routing your traffic through a remote server. This helps protect your data and anonymity online. While creating a VM similarly acts like a VPN by displaying an IP address where the VM's server is located at when choosing the region. The IP address is getting masked, you can simply open up a web browser and notice that your language has changed into the location servers language. For example- if you were in the Netherlands and searched for yahoo.com. You would see that the webpage is in Dutch. 
</p>
<br />
