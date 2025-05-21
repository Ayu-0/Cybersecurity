# OSI AND TCP/IP MODELS -

Basically it's a internet protocol suite, it's a framework that organizes the protocols used for communication on the internet. You can say it's a main protocol.

OSI : Open source interconneted models ( conceptual framework )
TCP/IP : Foundation of Internet communications and is more practical compared to the OSI model

OSI model Layers : 
1. Application - Provides an interface for the end-user
2. Presentation - Transaltes data from computer code into network-formatted code
3. Session - Establishes request/response interaction between two network hosts
4. Transport - Manager traffic flow through the network layer
5. Network  - Determines what path data packets will be taking to get from one network to another
6. Data Link- Breaks data into frames that will be transmitted over a physical layer
7. Physical - Converts digital data into optical, electrical or radio signals


TCP/IP Model Layers :
1. Application
2. Transport
3. Network
4. Data-Link
5. Physical

We'll study TCP/IP here -






3. Network Layer :


- It defines the protocols which are responsible for the logical transmission of data over the entire network. 
- It exchange information through intermediate system called routers.
- And the unit of information in network layer called packets.
- The main protocols residing at this layer are as follows:

IP:IP stands for Internet Protocol and it is responsible for delivering packets from the source host to the destination host by looking at the IP addresses in the packet headers. IP has 2 versions: IPv4 and IPv6. IPv4 is the one that most websites are using currently. But IPv6 is growing as the number of IPv4 addresses is limited in number when compared to the number of users.

ICMP:ICMP stands for Internet Control Message Protocol. It is encapsulated within IP datagrams and is responsible for providing hosts with information about network problems.

ARP:ARP stands for Address Resolution Protocol. Its job is to find the hardware address of a host from a known IP address. ARP has several types: Reverse ARP, Proxy ARP, Gratuitous ARP, and Inverse ARP.


4. Data-Link Layer :


## Flow Control -




5. Physical Layer :

