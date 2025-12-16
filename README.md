LAN and Internet Connectivity Setup for a Residential Home Using Cisco Packet Tracer

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

illustrates the type of network Annie’s home has:
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
<img width="723" height="160" alt="image" src="https://github.com/user-attachments/assets/f0035f82-1382-40b8-a69d-6f3ac5635e91" />


 
<img width="940" height="487" alt="image" src="https://github.com/user-attachments/assets/a9938a1e-49c4-479d-973a-22325bc2f637" />
<img width="940" height="460" alt="image" src="https://github.com/user-attachments/assets/38a7d96b-02cb-4e77-b546-2248ac393604" />
<img width="940" height="460" alt="image" src="https://github.com/user-attachments/assets/d05dc5d8-012a-4dd6-813e-893c422c86d3" />


Select Coaxial Cable (coax0).
Drag from Modem port 0 → Cable Splitter coax2.
<img width="710" height="156" alt="image" src="https://github.com/user-attachments/assets/12af6532-11e4-42d0-a808-ab5c72b7e70b" />
<img width="940" height="481" alt="image" src="https://github.com/user-attachments/assets/b08d492b-7d36-4456-8f32-eb41607e58bb" />
<img width="940" height="470" alt="image" src="https://github.com/user-attachments/assets/ac7b7d61-43ca-443f-bb50-4ad5281ac920" />


Testing the TV

Once the connections have been made, we will test the TV by clicking on it and turning it ON. This will confirm that the TV is successfully receiving the Internet signal from the cable splitter.
TV turned ON, confirming connectivity.
<img width="940" height="993" alt="image" src="https://github.com/user-attachments/assets/95657eac-15d8-4a5a-9802-c2e9c4473ab9" />

 
Connecting the Office PC

Next, we will proceed to establish network connectivity for the Office PC. To do this, we will use the coaxial cable as we did for the TV connection.

Connections:

1. Click on the coaxial cable and then click on the modem.
<img width="710" height="156" alt="image" src="https://github.com/user-attachments/assets/ad71fd20-7e7a-45d9-8e4a-0d3d8dc905c5" />
 

2. Connect Modem port 1 → Router Internet port.
 <img width="764" height="600" alt="image" src="https://github.com/user-attachments/assets/9d4eca27-9b55-4c72-a719-818601d0f532" />
<img width="739" height="484" alt="image" src="https://github.com/user-attachments/assets/6c023c95-5d14-4927-b1d6-c6d16f68a67c" />
<img width="921" height="651" alt="image" src="https://github.com/user-attachments/assets/a64da141-4e4c-4421-b502-8365ce7cc3c2" />


Task 2
Connecting the Office Desktop and Configuring IP
As per the setup completed in Task 1, the next step is to establish network connectivity for the Office Desktop
Step 1: Connecting the Office Desktop
1.	Select a copper cable (straight-through) from the cable menu.
 <img width="739" height="140" alt="image" src="https://github.com/user-attachments/assets/608d4353-2276-4d4d-92eb-45ba19439a47" />

2. Click and drag from Office PC FastEthernet0 → Router GigabitEthernet1.
<img width="940" height="568" alt="image" src="https://github.com/user-attachments/assets/ad59e3f4-94af-4791-8d55-bc61e2d4eec6" />
<img width="940" height="568" alt="image" src="https://github.com/user-attachments/assets/31778361-c80a-484d-97e0-e652c97dab74" />
<img width="788" height="519" alt="image" src="https://github.com/user-attachments/assets/2bd7d4c2-7317-43d8-9f1f-aa7bba135a97" />

Step 2: Configuring IP for Office Desktop
1. Click on Office PC → Configuration window opens.
2. Go to IP Configuration → Change from Static to DHCP.
3. The DHCP server automatically assigns an IP address; in this case, it is 192.168.0.1.

 <img width="573" height="391" alt="image" src="https://github.com/user-attachments/assets/a2eec2c6-f1f6-4b54-9351-476af30dec8d" />
 <img width="573" height="391" alt="image" src="https://github.com/user-attachments/assets/9033b483-05c2-4616-8edf-18e1c44ec3a7" />
 <img width="235" height="240" alt="image" src="https://github.com/user-attachments/assets/103b2816-d4f2-467d-b23f-c7d48b749344" />
 <img width="235" height="240" alt="image" src="https://github.com/user-
  attachments/assets/ba04e0a5-30af-4ca9-a3c9-7a946106b8f9" />
<img width="630" height="306" alt="image" src="https://github.com/user-attachments/assets/f6e9a7e2-4fdd-444b-ac42-6e361cfb5d29" />

Step 3: Testing Connectivity
1. Close the configuration window and return to the Home Page.
2. Open the Web Browser on the Office PC.
3. Type in the IP address of the router: 192.168.0.1.
4. A login window appears; enter the default username and password:
Username: admin
Password: admin
<img width="206" height="203" alt="image" src="https://github.com/user-attachments/assets/51a85530-4ce1-4c73-af49-bd6adcbc42ce" />
<img width="206" height="203" alt="image" src="https://github.com/user-attachments/assets/acfd1780-88ae-4bcd-9635-01ccaeef8ba0" />

Step 4: Configuring Router Settings
1. Navigate to Administration → Change the router password to mypassword1.
2. To verify, close the session and log in again using the updated password.
<img width="940" height="871" alt="image" src="https://github.com/user-attachments/assets/29b72942-984e-4c20-af33-13d76226f5d9" />

<img width="940" height="626" alt="image" src="https://github.com/user-attachments/assets/46a972c5-4888-4cac-9256-9d5925708009" />

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
	<img width="940" height="626" alt="image" src="https://github.com/user-attachments/assets/7d364dea-1a41-4107-a980-af4eac92aed2" />

Step2 Navigate to Wireless Security Settings
<img width="940" height="819" alt="image" src="https://github.com/user-attachments/assets/07301485-df4a-405c-9eec-d00e775ffd99" />

Step 3: Connecting the Laptop to the Wireless Network
•	Click on the Laptop in the Living Room.
•	The Laptop Configuration Window opens.
3. Navigate to Desktop.
4. Click on PC Wireless (or Wireless Configuration).
5. Click Connect.
 
<img width="940" height="710" alt="image" src="https://github.com/user-attachments/assets/5754cdeb-eee6-4ab4-81bb-234052e35f13" />
<img width="650" height="575" alt="image" src="https://github.com/user-attachments/assets/9e61e46f-03a7-41f5-88ed-18cafdee0a18" />
<img width="753" height="581" alt="image" src="https://github.com/user-attachments/assets/cd7de172-3822-4fd3-a134-43ae4860d0f3" />

Successfully connected
6. From the available networks, select MyHome.
7. When prompted, enter the passphrase:
MyPassphrase1
8. Click Connect.
<img width="596" height="460" alt="image" src="https://github.com/user-attachments/assets/df9fb9d5-d30b-4560-a865-7602b282ee36" />
Successful wireless connection showing link status as Connected.

Step 4: Verifying Internet Connectivity
•	Go to IP Configuration on the laptop.
•	Set IP configuration to DHCP (Automatic).
•	Confirm that an IP address is assigned automatically.
<img width="940" height="820" alt="image" src="https://github.com/user-attachments/assets/480b9e8f-2f4b-4da0-8c48-842dbedf8111" />

DHCP-assigned IP address on the laptop.
4. Open the Web Browser
5. Type 192.168.0.1.
6. Log in using the updated password (mypassword1) to verify connectivity.
<img width="940" height="514" alt="image" src="https://github.com/user-attachments/assets/b0b457f4-81e7-495f-bf6d-ba5eb3cfac0c" />
 <img width="940" height="514" alt="image" src="https://github.com/user-attachments/assets/ecabf78d-f298-4940-8fb8-ad14b57e16c3" />
<img width="940" height="940" alt="image" src="https://github.com/user-attachments/assets/e68fb9d5-6512-49cc-b7e3-a80e3bc6491f" />

Task 4
Connecting the Bedroom PC to the Network
The final step to establish full network connectivity across all zones of Annie’s home is connecting the Bedroom PC to the wireless router using a wired connection.

Step 1: Selecting the Network Cable
1. From the bottom menu in Cisco Packet Tracer, select Copper Straight-Through cable.
 
<img width="710" height="156" alt="image" src="https://github.com/user-attachments/assets/8e6950e9-23ca-4894-a703-d3f63eb7bbf2" />

Step 2: Establishing the Physical Connection
1. Click on the Bedroom PC.
2. Select its FastEthernet0 port.
3. Click on the Wireless Router.
4. Connect it to the GigabitEthernet2 port on the router.
This creates a wired link between the Bedroom PC and the router.
Drag from Bedroom PC Fast Ethernet → Router Gigabit Ethernet 2
<img width="940" height="662" alt="image" src="https://github.com/user-attachments/assets/6f506322-e7ed-489d-9593-1b6837921c2e" />
<img width="890" height="826" alt="image" src="https://github.com/user-attachments/assets/b60982f7-3156-4752-857e-a2fd51a4e886" />
<img width="940" height="724" alt="image" src="https://github.com/user-attachments/assets/44a26863-7890-4891-a437-a495920a82a4" />

Step 3: Configuring IP Address on Bedroom PC

•	Click on the Bedroom PC.
•	Open the Configuration window.
•	Navigate to IP Configuration.
•	Change the IP assignment from Static to DHCP (Automatic).
•	The system will automatically assign an IP address and default gateway.
<img width="940" height="847" alt="image" src="https://github.com/user-attachments/assets/f5aa979f-3a0c-4ac4-a054-5c6c16e08982" />
<img width="940" height="266" alt="image" src="https://github.com/user-attachments/assets/8290f839-742d-4324-8bb5-de86d4657335" />

Step 4: Testing Internet Connectivity

1. Open the Web Browser on the Bedroom PC.
2. Enter the router IP address: 192.168.0.1.
3. Log in using the updated credentials:

Username: admin
Password: mypassword1
<img width="940" height="889" alt="image" src="https://github.com/user-attachments/assets/5ea8ff2e-9835-4fe6-8dba-c9c9125f995e" />

Conclusion
By the end of this project, a Network Engineer gains a strong understanding of the fundamentals of using Cisco Packet Tracer. Cisco Packet Tracer provides a beginner-friendly and simulation-based environment, making it easier to understand real-world networking concepts without physical hardware.

Throughout this project, Cisco Packet Tracer was used to establish a simple and efficient residential LAN network, covering both wired and wireless connectivity. The project offered a hands-on and practical demonstration of configuring devices, assigning IP addresses, enabling wireless security, and testing network connectivity across multiple zones within a home.

This implementation provides a broad understanding of network setup principles, including device interconnection, IP configuration, and basic network security. As a result, I am confident in my ability to design and establish a LAN-based network in any residential environment.

Thank you.

