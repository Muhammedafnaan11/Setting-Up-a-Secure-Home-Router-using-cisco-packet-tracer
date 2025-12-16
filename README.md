LAN and Internet Connectivity Setup for a Residential Home Using Cisco Packet Tracer


Contents
Introduction	2
Task 1	3
Task 2	10
Task 3	16
Task 4	23
Conclusion	28
















Introduction
Simulation Tool:
Cisco Packet Tracer (to configure devices, assign IP addresses, and verify connectivity).
Overview of the Project
This project consists of a LAN-based network setup with the following devices:
•	Computers
•	Laptops
•	Desktops
•	Routers
•	Modem
•	Cable splitter
•	Internet Service Provider (ISP)
Overview
<img width="879" height="500" alt="image" src="https://github.com/user-attachments/assets/bb381e2e-879e-4e6c-b37c-c3bd3ba9bf65" />

Screenshot 1.1
 
Considering Screenshot 1.1, which illustrates the type of network Annie’s home has:
•	This home contains three rooms: a Bedroom, a Living Room, and an Office Room.
•	Living Room: TV and Laptop
•	Office Room: Modem, Wireless Router, Office Desktop
•	Bedroom: Bedroom PC
•	A Cable Splitter is placed in the middle, acting as a central gateway to establish network connectivity by linking to the Internet Service Provider (ISP).

Task 1
Connecting TV and Modem to the Internet
In order to get started with the network connection, we will first attempt to connect the TV to the Internet. To achieve this, a cable splitter will be used to manage communications between the modem and the TV. The setup works as follows:

•	The modem is connected to the cable splitter to provide Internet access.
•	The TV is connected to the cable splitter to receive the Internet signal and function based on this connection.


Connections:

•	TV port 0 → Cable Splitter port coax0
•	Modem port 0 → Cable Splitter port coax1
Screenshot 1.2
 
Screenshot 1.2: Shows the list of coaxial cables in the bottom menu of Cisco Packet Tracer.

the step-by-step connection process using the coaxial cables, showing the TV and modem being connected to the cable splitter.
 
 
 
Select Coaxial Cable (coax0).
 
Drag from Modem port 0 → Cable Splitter coax2.
 
 
 

Testing the TV

Once the connections have been made, we will test the TV by clicking on it and turning it ON. This will confirm that the TV is successfully receiving the Internet signal from the cable splitter.
TV turned ON, confirming connectivity.
 
Connecting the Office PC

Next, we will proceed to establish network connectivity for the Office PC. To do this, we will use the coaxial cable as we did for the TV connection.

Connections:

1.	Select coaxial cable from the list.
 

2. Click on the coaxial cable and then click on the modem.
 

3. Connect Modem port 1 → Router Internet port.
 
Drag from Modem port 1 → Router Internet port.
 
 

 


Task 2
Connecting the Office Desktop and Configuring IP
As per the setup completed in Task 1, the next step is to establish network connectivity for the Office Desktop
Step 1: Connecting the Office Desktop
1.	Select a copper cable (straight-through) from the cable menu.
 


2. Click and drag from Office PC FastEthernet0 → Router GigabitEthernet1.
 
 
 

Step 2: Configuring IP for Office Desktop

1. Click on Office PC → Configuration window opens.
2. Go to IP Configuration → Change from Static to DHCP.
3. The DHCP server automatically assigns an IP address; in this case, it is 192.168.0.1.

 
 
 
 
 
Step 3: Testing Connectivity
1. Close the configuration window and return to the Home Page.
2. Open the Web Browser on the Office PC.
3. Type in the IP address of the router: 192.168.0.1.
4. A login window appears; enter the default username and password:
Username: admin
Password: admin
 
 
 

Step 4: Configuring Router Settings
1. Navigate to Administration → Change the router password to mypassword1.
2. To verify, close the session and log in again using the updated password.




 
 
 After successfully logging into the router interface and updating the admin password, the next step is to configure the wireless network name (SSID). This step ensures that the wireless network is identifiable and accessible to wireless devices such as laptops
Changing the SSID Name
•	Enable SSID → MyHome

Task 3
 Establishing Wireless Connectivity for the Living Room Laptop
Now that the Office Room devices are successfully connected to the network, the next step is to connect the Laptop in the Living Room to the Internet using a wireless connection.
Step 1: Configuring Wireless Security on the Router
•	From the Office Desktop, open the Web Browser.


•	Type the router IP address: 192.168.0.1.
•	Log in using the updated credentials:
•	Username: admin Password: mypassword1
•	Once logged in, navigate to Wireless Settings.
•	Click on Wireless Security.
•	Under 2.4 GHz Wireless Settings:
•	Enable 2.4 GHz Wireless
•	Set Security Mode to WPA/WPA2 (WPA-Personal)
•	Set Passphrase (Key) to: MyPassphrase1
•	 
•	
•	2. Navigate to Wireless Security Settings
 

Step 3: Connecting the Laptop to the Wireless Network
•	Click on the Laptop in the Living Room.
•	The Laptop Configuration Window opens.
3. Navigate to Desktop.
4. Click on PC Wireless (or Wireless Configuration).
5. Click Connect.
 

 

 
Successfully connected

6. From the available networks, select MyHome.
7. When prompted, enter the passphrase:
MyPassphrase1
8. Click Connect.
 
Successful wireless connection showing link status as Connected.
Step 4: Verifying Internet Connectivity
•	Go to IP Configuration on the laptop.
•	Set IP configuration to DHCP (Automatic).
•	Confirm that an IP address is assigned automatically.
 
DHCP-assigned IP address on the laptop.
4. Open the Web Browser
5. Type 192.168.0.1.
6. Log in using the updated password (mypassword1) to verify connectivity.
 
 

 


Task 4
 Connecting the Bedroom PC to the Network
The final step to establish full network connectivity across all zones of Annie’s home is connecting the Bedroom PC to the wireless router using a wired connection.

Step 1: Selecting the Network Cable
1. From the bottom menu in Cisco Packet Tracer, select Copper Straight-Through cable.
 

Step 2: Establishing the Physical Connection
1. Click on the Bedroom PC.
2. Select its FastEthernet0 port.
3. Click on the Wireless Router.
4. Connect it to the GigabitEthernet2 port on the router.
This creates a wired link between the Bedroom PC and the router.
Drag from Bedroom PC Fast Ethernet → Router Gigabit Ethernet 2

 

 
 

Step 3: Configuring IP Address on Bedroom PC

•	Click on the Bedroom PC.
•	Open the Configuration window.
•	Navigate to IP Configuration.
•	Change the IP assignment from Static to DHCP (Automatic).
•	The system will automatically assign an IP address and default gateway.
 
 


Step 4: Testing Internet Connectivity

1. Open the Web Browser on the Bedroom PC.
2. Enter the router IP address: 192.168.0.1.
3. Log in using the updated credentials:

Username: admin
Password: mypassword1
 
Conclusion
By the end of this project, a Network Engineer gains a strong understanding of the fundamentals of using Cisco Packet Tracer. Cisco Packet Tracer provides a beginner-friendly and simulation-based environment, making it easier to understand real-world networking concepts without physical hardware.

Throughout this project, Cisco Packet Tracer was used to establish a simple and efficient residential LAN network, covering both wired and wireless connectivity. The project offered a hands-on and practical demonstration of configuring devices, assigning IP addresses, enabling wireless security, and testing network connectivity across multiple zones within a home.

This implementation provides a broad understanding of network setup principles, including device interconnection, IP configuration, and basic network security. As a result, I am confident in my ability to design and establish a LAN-based network in any residential environment.

Thank you.

