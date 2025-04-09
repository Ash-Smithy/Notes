# What are Networks?

### Network
    A group of connected devices

### Local Area Network (LAN)
    A network that spans small area, like an office building, a school or a home.

### Wide area Network (WAN)
    A network that spans a large geograpic area likea  city, state or country.

### Network Tools

- ### Hub 
    A network device that broadcasts information to every device on the network

- ### Switch
    A device that makes connections between specific devices on a network by sending and receiving data between them
    (switch is more intelligent than hub, as it sends/recieves data to/from specific devices only)

- ### Router
    A network device that connects multiple networks together

- ### Modems
    A device that connects router to the internet and brings internet access to the LAN

## Virtualization Tools
    Pieces of software that perform network operations

### Firewalls
    A firewall is a network security device that monitors traffic to or from your network. Firewalls often reside between the secured and controlled internal network and the untrusted network resources outside the organization, such as the internet. 

### Servers
    Servers provide information and services for devices like computers, smart home devices, and smartphones on the network.


## Network Diagrams 
    Network diagrams are maps that show the devices on the network and how they connect. Network diagrams allow network administrators and security personnel to imagine the architecture and design of their organization’s private network.

## Cloud Computing
    THe practice of using remote servers, application, and network services that are hosted on the internet instead of on local physical devices

### Cloud Network
    A collection of servers or computers that stores resources and data in remote data centeres that can be accessed via the internet.

### Cloud Service providers offer:
    - On-demand storage
    - Processing power
    - Analytics

### Cloud Service Providers three categories of service:
- #### Software as a Service (SaaS)
    software suites operated by the cloud service provider that a company can use remotely without hosting the software.

- #### Infrastructure as a Service (IaaS)
    use of virtual computer components offerered by the CSP. These include virtual containers and storage that are configuredd remotely through the CSP's API or web console. Existing applications can be modified to take advantage of the availability, performance, and security fetures that are unique to cloud provider services.

- ####  Platform as a Service (PaaS)
    refers to tools that application developers can use to design custom application for their compant. Custom applications are designed and accessed in the cloud and used for a company's specific business goals.

    ![alt text](csp_services.png)

#### Hybrid Cloud Environments
> When organizations use a CSP’s services in addition to their on-premise computers, networks, and storage, it is referred to as a hybrid cloud environment.
When organizations use more than one CSP, it is called a **multi-cloud environment**. 

### Benefits of cloud computing and software-defined networks 

- Reliability
- Cost
- Scalability


## Data packet
> A basic unit of information that travels from one device to another within a network

## Bandwitdth
> The amount of data a device received every second

## Speed
>  The rate at which data packets are received or downloaded

## Packet Sniffing
> The practice of capturing and inspecting data packets across a network


# TCP/IP Model (Transmission Control Protocol / Internet Protocol)
- TCP
    Transmission Control Protocol is an internet communication protocol that allows two devices to form a connection and stream data
- IP
    Internt Protocol is a set of standards used for routing and addressing data packetss ass they travel between devices on a network

### Port
    A software-based location that orgainzes the sending and receiving of data between devices on a network
    Common port numbers:
    - Port 25: Emails
    - Port 443: Secure internet communication
    - Port 20: Large file transfers

## Four Layers of TCP/IP Model
#### **TCP/IP Model**
> A framework used to visualize how data is organized and transmitted across the network

### Four Layers:

> ### 1. Network Access Layer (Data Link Layer)
> Deals with creation of data packets and their transmission across the network.
> Ex: Ethernet, Wireless Lan

> ### 2. Internet Layer
>  Here the IP addresses are attached to data packets to indicate location of sender/receiver and also how networks connect to each other.
> Ex: IPv4/IPv6

> ### 3. Transport Layer
> Includes protocol to control flow of traffic across a network. Here the device allows/denies connection with other devices and also has status of the connection
> Ex: TCP, UDP

> ### 4. Application Layer
> Protocols determining how the data packets will interact with receiving devices.
> Ex: HTTP, TLS, DNS

## OSI Model
> The OSI model is a standardized concept that describes the seven layers computers use to communicate and send data over the network. 

#### Layers:
> ### 7. Application layer
> The application layer includes processes that directly involve the everyday user. This layer includes all of the networking protocols that software applications use to connect a user to the internet.

> ### 6. Presentation Layer:
> Functions at the presentation layer involve data translation and encryption for the network. This layer adds to and replaces data with formats that can be understood by applications (layer 7) on both sending and receiving systems.

> ### 5. Session Layer
> A session describes when a connection is established between two devices. An open session allows the devices to communicate with each other. Session layer protocols keep the session open while data is being transferred and terminate the session once the transmission is complete. 

> ### 4. Transport Layer
> The transport layer is responsible for delivering data between devices. This layer also handles the speed of data transfer, flow of the transfer, and breaking data down into smaller segments to make them easier to transport.

> ### 3. Network Layer
> The network layer oversees receiving the frames from the data link layer (layer 2) and delivers them to the intended destination.

> ### 2. Data Link Layer
> The data link layer organizes sending and receiving data packets within a single network. The data link layer is home to switches on the local network and network interface cards on local devices.

> ### 1. Physical Layer
> As the name suggests, the physical layer corresponds to the physical hardware involved in network transmission. Hubs, modems, and the cables and wiring that connect them are all considered part of the physical layer. To travel across an ethernet or coaxial cable, a data packet needs to be translated into a stream of 0s and 1s. The stream of 0s and 1s are sent across the physical wiring and cables, received, and then passed on to higher levels of the OSI model.




### Internet Protocol (IP) address
    A unique string of characters that identifies the location of a device on the internet
    Two types:
   - IP version 4 (IPv4)
        four 1,2 or 3 digit nunmber seperated by decimal points
        ex: 192.168.63.1
   - IP version 6 (IPv6)
        upto 32 characters
       ex: 6D66:0000:1353:43469:12398:8341:asd81:8

    It can be public or private.
    Public IP address is assigned by ISP.
    Private IPs can only be seen by locally connected devices.

    > All data packets, also known as IP packets, include an IP address.
    
    > Each packet has two parts
    - Header
        The header contains information more than just the destination address. It includes source IP address, size of the packet and which protocol will be used for the data portion of the packet.

    - Data
        the information sent by the other device.

![alt text](image-3.png)

> - An IPv4 header format is determined by the IPv4 protocol and includes the IP routing information that devices use to direct the packet. The size of the IPv4 header ranges from 20 to 60 bytes. The first 20 bytes are a fixed set of information containing data such as the source and destination IP address, header length, and total length of the packet. The last set of bytes can range from 0 to 40 and consists of the options field.

> - The length of the data section of an IPv4 packet can vary greatly in size. However, the maximum possible size of an IPv4 packet is 65,535 bytes. It contains the message being transferred over the internet, like website information or email text. 

![alt text](image-4.png)

> There are 13 fields within the header of an IPv4 packet:

> - Version (VER): This 4 bit component tells receiving devices what protocol the packet is using. The packet used in the illustration above is an IPv4 packet.
> - IP Header Length (HLEN or IHL): HLEN is the packet’s header length. This value indicates where the packet header ends and the data segment begins. 
> - Type of Service (ToS): Routers prioritize packets for delivery to maintain quality of service on the network. The ToS field provides the router with this information.
> - Total Length: This field communicates the total length of the entire IP packet, including the header and data. The maximum size of an IPv4 packet is 65,535 bytes.
> - Identification: IPv4 packets can be up to 65, 535 bytes, but most networks have a smaller limit. In these cases, the packets are divided, or fragmented, into smaller IP packets. The identification field provides a unique identifier for all the fragments of the original IP packet so that they can be reassembled once they reach their destination.
> - Flags: This field provides the routing device with more information about whether the original packet has been fragmented and if there are more fragments in transit.
> - Fragmentation Offset: The fragment offset field tells routing devices where in the original packet the fragment belongs.
> - Time to Live (TTL): TTL prevents data packets from being forwarded by routers indefinitely. It contains a counter that is set by the source. The counter is decremented by one as it passes through each router along its path. When the TTL counter reaches zero, the router currently holding the packet will discard the packet and return an ICMP Time Exceeded error message to the sender. 
> - Protocol: The protocol field tells the receiving device which protocol will be used for the data portion of the packet.
> - Header Checksum: The header checksum field contains a checksum that can be used to detect corruption of the IP header in transit. Corrupted packets are discarded.
> - Source IP Address: The source IP address is the IPv4 address of the sending device.
> - Destination IP Address: The destination IP address is the IPv4 address of the destination device.
> - Options: The options field allows for security options to be applied to the packet if the HLEN value is greater than five. The field communicates these options to the routing devices.


### MAC address
    A unique alphanumeric identifier that is assigned to each physical device on a network


# Module 2

## Network Protocols
> A set of rules used by two or more devices on a network to describe the order of delivery and structure of the data

## Transmission Control Protocol (TCP)
> An internet communications protocol that allows two devices to form a  connection and stream data

## Address Resolution Protocol (ARP)
> A network protocol used to determine the MAC address of the next router or device on the path

## Hyper Text Trannfer Protocol Secure (HTTPS)
> A network protocol that provides a secure method of communication between clients and website servers

## Domain Name System (DNS)
> A network protocol that translates internet domain names into IP addressses


## Three Categories of Network Protocols

>### 1. Communication Protocols
>   Communication protocols govern the exchange of information in the network transmission. They dictate how the data is transmitted between deviec and the time of the communication. THey also include methods to recover data lost in transit. <br>
>    Few communication protocols are:  <br>
>>   - **Transmission Control Protocol (TCP):**  <br>
            TCP uses a three-way handshake process. First, the device sends a synchronize (SYN) request to a server. Then the server responds with a SYN/ACK packet to acknowledge receipt of the device's request. Once the server receives the final ACK packet from the device, a TCP connection is established. In the TCP/IP model, TCP occurs at the transport layer.
>>   - **User Datagram Protocol (UDP):**  <br>
            is a connectionless protocol that does not establish a connection between devices before a transmission. This makes it less reliable than TCP. But it also means that it works well for transmissions that need to get to their destination quickly. In the TCP/IP model, UDP occurs at the transport layer.
>>  - **Hypertext Transfer Protocol (HTTP):**  <br>
            is an application layer protocol that provides a method of communication between clients and website servers. HTTP uses port 80. HTTP is considered insecure, so it is being replaced on most websites by a secure version, called HTTPS that uses encryption from SSL/TLS for communication. However, there are still many websites that use the insecure HTTP protocol. In the TCP/IP model, HTTP occurs at the application layer.
>>  - **Domain Naming System (DNS):**  <br>
            is a protocol that translates internet domain names into IP addresses. When a client computer wishes to access a website domain using their internet browser, a query is sent to a dedicated DNS server. The DNS server then looks up the IP address that corresponds to the website domain. DNS normally uses UDP on port 53. However, if the DNS reply to a request is large, it will switch to using the TCP protocol. In the TCP/IP model, DNS occurs at the application layer. 

> ### 2. Management Protocols:
> Second category of network protocols is management protocols.These are used for monitoring and managaing activity on a network. They uncluse protocols for error reporting and optimizing performance on the network.
>> - **Simple Network Management Protocol (SNMP):**
>> is a network protocol used for monitoring and managing devices on a network. SNMP can reset a password on a network device or change its baseline configuration. It can also send requests to network devices for a report on how much of the network’s bandwidth is being used up. In the TCP/IP model, SNMP occurs at the application layer.
>> - **Internet Control Message Protocol (ICMP):** 
>> is an internet protocol used by devices to tell each other about data transmission errors across the network. ICMP is used by a receiving device to send a report to the sending device about the data transmission. ICMP is commonly used as a quick way to troubleshoot network connectivity and latency by issuing the “ping” command on a Linux operating system. In the TCP/IP model, ICMP occurs at the internet layer.

> ### 3. Security Protocols
> Security protocols are network protocols that ensure that data is sent and received securely across a network. Security protocols use encryption algorithms to protect data in transit. Below are some common security protocols.
>> - **Hypertext Transfer Protocol Secure (HTTPS):**
>> is a network protocol that provides a secure method of communication between clients and website servers. HTTPS is a secure version of HTTP that uses secure sockets layer/transport layer security (SSL/TLS) encryption on all transmissions so that malicious actors cannot read the information contained. HTTPS uses port 443. In the TCP/IP model, HTTPS occurs at the application layer.
>> - **Secure File Transfer Protocol (SFTP):**
>> is a secure protocol used to transfer files from one device to another over a network. SFTP uses secure shell (SSH), typically through TCP port 22. SSH uses Advanced Encryption Standard (AES) and other types of encryption to ensure that unintended recipients cannot intercept the transmissions. In the TCP/IP model, SFTP occurs at the application layer. SFTP is used often with cloud storage. Every time a user uploads or downloads a file from cloud storage, the file is transferred using the SFTP protocol.



> ## IEEE 802.11 (wifi)
> A set of standards that define communication for wireless LANs  <br>
> ### WiFi Protected Access (WPA)
> A wireless security protocol for devices to connect to the internet
> (improvement of WEP) <br>
> #### Wired Equivalent Privacy (WEP)
> Wired equivalent privacy (WEP) is a wireless security protocol designed to provide users with the same level of privacy on wireless network connections as they have on wired network connections. <br>
> ### WPA2
> The second version of Wi-Fi Protected Access—known as WPA2—was released in 2004. WPA2 improves upon WPA by using the Advanced Encryption Standard (AES). WPA2 also improves upon WPA’s use of Temporal Key Integrity Protocol (TKIP). WPA2 uses the Counter Mode Cipher Block Chain Message Authentication Code Protocol (CCMP), which provides encapsulation and ensures message authentication and integrity.


> ## Firewall
> A network security device that monitors traffic to and from your network <br>
> #### Port Filtering
>  A firewall function that blocks ot allows certain port numbers to limit unwanted communication <br>
> ### Cloud-based firewalls
> Software firewalls that are hosted by a cloud service provider <br>

> ### Stateful
> A class of firewall that keeps track of information passing through it and proactively filters out threats

> ### Stateless
> A class of firewall that operates based on predefined rules and does not keep track of information from data packs.

> #### Benefits of Next Generation firewalls (NGFWs)
> - Deep packet inspection
> - Intrusion protection
> - Threat Intelligence

> ## Virtual Private Network (VPN)
> A network security service that changes your public IP address and hides your virtual location so that you can keep your data private when you are using a public network like the internet. It also encrypts data and performs encapsulation
> **Encapsulation** is a process performed by a VPN service that protects your data by wrapping sensitive data in other data packets

> ## Security Zone
> A segment of a network that protects the internal network from the internet
> ### Network Segmentation
> A security technique that divides the network into segments
## 2 types of security zones
> ### 1. Uncontrolled Zone
>  Any network outside of the organization's control
> ### 2. Controlled Zone
> A subnet that protects the internal network from the uncontrolled zone

> #### Areas in the controlled zone
> - Demilitarized zone (DMZ)
> - Internal Network
> - Restricted Zone
<br>


> ## Subnetting 
> is the subdivision of a network into logical groups called subnets. It works like a network inside a network. Subnetting divides up a network address range into smaller subnets within the network. 

> ## Classless Inter-Domain Routing (CIDR)
> is a method of assigning subnet masks to IP addresses to create a subnet. 

> ## Proxy servers
>> A server that fulfill the requests of a client by forwarding them on to other servers
>> ### Forward proxy server
>>> Regulates and restricts a person's access to the internet
>> ### Reverse proxy server
>>> Regulates and restricts the internet's access to an internal server


# Module 3 **Secure Against Network Intrusions**

### Attacks

> #### Network Interception Attacks
> Network interception attacks work by intercepting network traffic and stealing valuable information or interfering with the transmission in some way.

> #### Backdoor Attacks
> This kind of attacks are done by people who are part of the organisation. They take advantage of their access privileges 

>> #### Possible impact on organisation
> - Financial
> - Reputation
> - Public safety


> ## Denial Of Service Attacks (DoS)
> A DoS attack is an attack that targets a network or server and floods it with network traffic.

> ### Distributed Denial Of Service attack (DDoS)
> A type of denial of service attack that uses multiple devices or servers in different locations to flood the target network with unwanted 

> ## Network Level DoS attacks
> ### SYN (synchronize) Flood Attack
>> A type of DoS atack that simulates a TCP connection and floods a server with SYN 

>>> #### Internet Conotrol Message Protocol (ICMP)
>>>> An internet protocol used by devices to tell each other about data transmission errors across the network  

> ### ICMP Flood Attack 
>> A type of DoS attack performed by an attacker repeatedly sending ICMP packets to a network server

> ### Ping of Death
>> A type of DoS attack caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64KB

> ##  Network Protocol Analyzer
> sometimes called a packet sniffer or a packet analyzer, is a tool designed to capture and analyze data traffic within a network. They are commonly used as investigative tools to monitor networks and identify suspicious activity. There are a wide variety of network protocol analyzers available, but some of the most common analyzers  include:
> - SolarWinds NetFlow Traffic Analyzer
> - ManageEngine OpManager
> - Azure Network Watcher
> - Wireshark
> - tcpdump

> ### tcpdump
> tcpdump is a command-line network protocol analyzer. It is popular, lightweight–meaning it uses little memory and has a low CPU usage–and uses the open-source libpcap library. tcpdump is text based, meaning all commands in tcpdump are executed in the terminal. It can also be installed on other Unix-based operating systems, such as macOS®. It is preinstalled on many Linux distributions. <br> <br>
> tcpdump provides a brief packet analysis and converts key information about network traffic into formats easily read by humans. It prints information about each packet directly into your terminal. tcpdump also displays the source IP address, destination IP addresses, and the port numbers being used in the communications. 

> #### botnet
>> A botnet is a collection of computers infected by malware that are under the control of a single threat actor, known as the “bot-herder." 


> ## Packet Sniffing
>> The act of capturing and inspecting packets in a network.
>> Packet sniffing can be of two types:
> ### Passive packet sniffing
>> A type ofa ttack where data packets are read in transit
> ### Active packet sniffing
>> A type of attack where data packets are manipulated in transit

### Ways of preventing packet sniffing:
> - Using VPN
> - Make sure websites use HTTPS
> - Avoid using unprotected wifi

> ## IP Spoofing
>> A network attack performed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network

> ### Common IP spoofing attacks:
> - **On-path attack** (meddler-in-the middle attack)
>> An attack where a malicious actor places themselves in the middle of an authorized connection and intercepts or alters the data in transit
> - **Replay attack**
>> A network attack performed when a malicious actor intercepts a data packet in transit and delays it or repeats in at another time
> - **Smurf aattack**
>> a network attack performed when an attacker sniffs an authorized user's IP address and floods it with packets. (Combination of DoS and IP Spoofing)

> #### How to protect form IP spoofing:
>> - Encryption
>> - Configuring Firewalls