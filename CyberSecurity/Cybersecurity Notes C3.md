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

