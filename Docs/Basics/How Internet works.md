
We'll look at just overview of it, just how things works, Ok
So at first we start with physical system then go to internal mechanism :

? What is internet.
The Internet is a global network of interconnected computers and servers that communicate with each other using standardized protocols. It allows billions of devices (such as computers, smartphones, and servers) to share and exchange information across the world

? How Internet is Provided -
Undersea Cables: Physical cables that connect continents and allow data to cross oceans.
Satellites: For connecting remote or hard-to-reach areas.
Servers: Computers that host websites, applications, and services.
Routers: Devices that direct data packets to their correct destinations.


In wired way Internet is provided via these methods :
1. LAN
So, LAN is your local area network. A network that connects computers and devices within a limited area like a home, office, or school. Usually owned, controlled and managed by a single organization

2. MAN
Man means Metropolitan area network, Often used by municipalities, universities, or large organizations. Interconnects multiple LANs within a city. These are operated by large Internet Service Providers (ISPs).

3. WAN
Wide area networks: It's where internet begins with, it connects countries, continents with a long very long wire called optical fibre.



But, How Data Actually Flows :

When you request to a website let say google:

Your computer sends a request through your LAN (your home network)
Your router forwards this to your ISP network.
Your ISP routes it through increasingly larger networks.
The request travels through multiple network switches, each figuring out where to send it next
Eventually, it reaches google's server in their data centers
Google's servers process your request and send data back
The data travels back through the same networks in reverse
Your computer receives and displays the webpage

The entire process involves numerous protocols working together, including TCP/IP (how data is packaged and addressed), DNS (translating google.com to an IP address), and HTTP/HTTPS (how web data is formatted).


# How data is transmitted over the internet ?

Internet works using TCP/IP (also OSI but not practical) as main protocol -

It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP). The Internet protocol suite is the conceptual model and set of communications protocols used on the Internet and similar computer networks. It is commonly known as TCP/IP because the foundational protocols in the suite are the Transmission Control Protocol (TCP) and the Internet Protocol (IP).

TCP/IP, is a suite of communication protocols used to interconnect network devices on the internet. TCP/IP can also be used as a communications protocol in a private network (an intranet or an extranet).

There are two IP protocols, TCP and UDP. There are 65335 ports that can be assigned to each. Per IANA, the first 1024 (0–1023, so count 0 as a port, too) ports are reserved for specific standardized services. So there are 2048 ports reserved for standardized protocols- 1024 for TCP, 1024 for UDP.


In simple terms :
When we talk about data transfer across the internet, we're actually dealing with two essential requirements for successful communication 

1. Physical data transmission - Can the bits and bytes physically move from point A to point B?
2. Semantic understanding - Can the receiving end interpret the meaning of those bits and bytes?