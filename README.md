# DevOps

This is a 90-day DevOps learning mail where everything about DevOps will be found sequentially, useful for freshers, experienced, and even non-IT guys planning to switch to IT via DevOps.

> DevOps is a set of practices, tools, and a cultural philosophy that combines software development (Dev) and IT operations (Ops) to shorten the software development lifecycle and provide continuous delivery with high software quality. It focuses on collaboration, automation, and monitoring to ensure faster and more reliable software releases.

https://github.com/NeerCodes/DevOps/


### Key Principles of DevOps:
**i. Collaboration**: Bridging the gap between development and operations teams to work together efficiently. 

**ii. Automation:** Automating repetitive tasks like code integration, testing, and deployment.

**iii. Continuous Integration and Continuous Deployment (CI/CD):** Frequent code integration and automated deployment to production environments.

**iv. Monitoring and Feedback:** Real-time tracking of applications and infrastructure to provide insights and improvements.

**v. Security (DevSecOps):** Embedding security into the DevOps lifecycle to ensure secure applications.

### DevOps Lifecycle Phases:
**Plan:**
- Tools: Jira, Trello
- Agile methodologies to plan and track work progress.

**Develop:**
- Tools: Git, GitHub, GitLab
- Writing and managing code collaboratively.


**Build:**
- Tools: Maven, Gradle
- Compiling source code into deployable artifacts.

**Test:**
- Tools: Selenium, JUnit, TestNG
- Automated testing to ensure software quality.

**Release:**
- Tools: Jenkins, GitHub Actions, GitLab CI/CD
- CI/CD pipelines for smooth delivery.


**Deploy:**
- Tools: Kubernetes, Docker, Ansible
- Automating deployment in cloud or on-premise environments.

**Operate:**
- Tools: Prometheus, Grafana, ELK Stack
- Monitoring application performance and infrastructure health.

**Monitor:**
- Tools: Nagios, Splunk
- Continuous feedback and logging for improvements.



## NETWORKING (for DevOps)
### All about Networking required for DevOps

- The internet is a vast global network of optical fiber cables, many of which are laid under the ocean, enabling the transfer of data across the world.

These undersea cables are primarily owned and operated by Tier-1 companies, which form the backbone of the internet.

🌐 Explore the global network topology: Submarine Cable Map (https://www.submarinecablemap.com/)

### <ins> Internet Service Provider (ISP) Hierarchy </ins>
#### Tier-1 ISPs (Global Backbone Providers):
- These companies own and maintain the core infrastructure, including submarine cables and major routing networks.
- They provide connectivity to Tier-2 ISPs via direct peering agreements.
- Examples: Tata Communications, AT&T, NTT Communications.

#### Tier-2 ISPs (Regional Providers):
- They lease bandwidth from Tier-1 providers to extend connectivity to different regions or countries.
- They may provide services to businesses and individual users or sell bandwidth to Tier-3 ISPs.
- Examples: BSNL, Jio, Airtel.

#### Tier-3 ISPs (Local Providers):
- They lease bandwidth from Tier-2 providers and offer internet access to end-users (homes and businesses).
- They often focus on specific cities or localities and provide last-mile connectivity.
- Examples: YOU Broadband, Craze Wifi, ion N/W, Jio Fiber.


### <ins> OSI Model & TCP/IP Model </ins>
- According to the International Organization for Standardization (ISO), the OSI (Open Systems Interconnection) model defines a 7-layer communication framework that helps understand how network systems interact.

#### _OSI Model (Theoretical Model):_
**1. Physical Layer –** Transmission of raw data (bits) over physical media.

**2. Data Link Layer –** Error detection, correction, and framing (MAC, Ethernet).

**3. Network Layer –** Routing and addressing (IP addresses).

**4. Transport Layer –** Reliable data delivery, flow control (TCP/UDP).

**5. Session Layer –** Establishing, managing, and terminating sessions.

**6. Presentation Layer –** Data translation, encryption, compression.

**7. Application Layer –** User interface and application services (HTTP, FTP, etc.).

**Key Point:** The OSI model provides a conceptual understanding of how the internet theoretically works.

#### _TCP/IP Model (Practical Model):_
- In real-world applications, the TCP/IP (Transmission Control Protocol/Internet Protocol) model, which powers the modern internet, simplifies the OSI model into 4 layers, combining similar functionalities:

**1. Network Interface Layer (Combines OSI Physical + Data Link) –** Handles hardware addressing, physical transmission, and framing (Ethernet, Wi-Fi).

**2. Internet Layer (OSI Network Layer) -** Responsible for addressing and routing data (IP, ICMP).

**3. Transport Layer (Same as OSI Transport Layer) –** Ensures end-to-end communication (TCP/UDP).

**4. Application Layer (Combines OSI Application + Presentation + Session) –** Provides services to end users (HTTP, FTP, DNS).

**Key Point:** The TCP/IP model is the real-world implementation used for internet communication.


### <ins> Internet Protocols </ins>
#### 1. Application layer Protocols
> These protocols provide end-user services and enable communication between applications. Common protocols include:
- **HTTP/HTTPS (HyperText Transfer Protocol/Secure)**
  - Used for web browsing and data transfer over the web.
  - **Ports:** 80 (HTTP), 443 (HTTPS)
 
- **SMTP (Simple Mail Transfer Protocol)**
  - Used for sending emails.
  - **Ports:** 25, 587 (SMTP with encryption)
  - 
- **FTP (File Transfer Protocol)**
  - Used for file transfers between systems
  - **Ports: 21** (control), 20 (data transfer)
   
- **Actionable Tip:** Ensure familiarity with port numbers for security configurations and firewall rules.

#### 2. Transport Layer Protocols
> This layer is responsible for end-to-end communication, error handling, and data flow control.
- **TCP (Transmission Control Protocol)**
  - Reliable, connection-oriented protocol.
  - Used in applications like YouTube, web browsing, email.
  - **Characteristics:** Error checking, retransmissions, packet ordering.
 
- **UDP (User Datagram Protocol)**
  - Fast, connectionless protocol with minimal overhead.
  - Used for real-time applications like live streaming, gaming, video calls.
  - **Characteristics:** No retransmission, lower latency, potential data loss.
    
- **Key Ports:**
  - TCP: 80 (HTTP), 443 (HTTPS), 22 (SSH), 21 (FTP), 25 (SMTP)
  - UDP: 53 (DNS), 123 (NTP), 161 (SNMP)

#### 3. Internet Layer Protocols
> Provides logical addressing and routing functions to connect devices across networks.
- **IP (Internet Protocol)**
  - Responsible for addressing and routing packets across networks.
  - Versions: IPv4 (32-bit addressing) and IPv6 (128-bit addressing).
  - Core Functions: Addressing, packet fragmentation, and reassembly.
 
#### 4. Network Access Layer Protocols
> The lowest layer of the networking model, dealing with physical transmission and data framing.
- **Ethernet (IEEE 802.3) –** Wired networking standard.
- **Wi-Fi (IEEE 802.11) –** Wireless communication protocol.
- **ARP (Address Resolution Protocol) –** Resolves IP addresses to MAC addresses.
- **PPP (Point-to-Point Protocol) –** Used for direct communication between two nodes.


### <ins> IPv4 vs IPv6 </ins>
**1. Address Length**

 - **IPv4:** 32 bits (e.g., 192.168.0.1)
 
 - **IPv6:** 128 bits (e.g., 2001:0db8:85a3:0000:0000:8a2e:0370:7334)

 
**2. Address Space**

 - **IPv4:** ~4.3 billion addresses (2³²); address exhaustion issue.
 
 - **IPv6:** Virtually unlimited (~3.4×10³⁸ or 2¹²⁸); sufficient for IoT and future needs.


**3. Configuration**

 - **IPv4:** Manual configuration or via DHCP.
 
 - **IPv6:** Auto-configuration using SLAAC (Stateless Address Autoconfiguration).


**4. Security**

 - **IPv4:** Optional IPSec support.
 
 - **IPv6:** Built-in IPSec for encryption and authentication.

**5. Header Size**

 - **IPv4:** 20 bytes.
 
 - **IPv6:** 40 bytes (simplified header for better performance).

**6. Communication Types**

 - **IPv4:** Unicast, Multicast, and Broadcast.
 
 - **IPv6:** Unicast, Multicast, and Anycast (no Broadcast).

**7. Fragmentation**

 - **IPv4:** Done by both routers and the sender.
 
 - **IPv6:** Only the sender handles fragmentation.

**8. Routing Efficiency**

 - **IPv4:** Larger routing tables, less efficient.
 
 - **IPv6:** Hierarchical addressing improves routing efficiency.

**9. Checksum**

 - **IPv4:** Checksum field in header (slows down processing).
 
 - **IPv6:** No checksum (handled at other layers).

**10. Deployment**

 - **IPv4:** Widely deployed; used in most networks.
 
 - **IPv6:** Gradual adoption; coexists with IPv4 in dual-stack systems.

**11. Quality of Service (QoS)**

 - **IPv4:** Limited QoS with Type of Service (ToS) field.
 
 - **IPv6:** Enhanced QoS with Flow Label field for traffic prioritization.

**Quick Summary:**
IPv6 solves IPv4's address exhaustion, offers better security, auto-configuration, and improved performance, but adoption is slower due to compatibility challenges.


### <ins> Subnet </ins>
**1. What is a Subnet?**
 - A subnet (short for "subnetwork") is a logically segmented portion of a larger network.
 - It divides a network into smaller, manageable sections to enhance performance, security, and organization.

**2. What is Subnetting?**
 - Subnetting is the process of splitting a larger IP network into smaller subnets.
 - This allows efficient utilization of IP addresses and reduces network congestion
 - Helps in isolating traffic for security and better control.

**3. Why is Subnetting Important?**
 - **Efficient IP Address Management:** Conserves IP addresses by avoiding wastage.
 - **Improved Network Performance:** Limits broadcast traffic within a subnet.
 - **Enhanced Security:** Isolates different network segments.
 - **Simplifies Administration:** Makes troubleshooting easier by segmenting networks.

**4. Key Components of Subnetting**

 - **IP Address:** Identifies a device on a network (e.g., 192.168.1.1).
  
 - **Subnet Mask:** Determines which part of the IP address is the network and which part is the **host**
   - Example: 255.255.255.0 (Class C network)..
  
 - **CIDR Notation:** Specifies the subnet mask using a /n format, where n is the number of bits in the network part.
   - Example: 192.168.1.1/24 means the first 24 bits are the network portion.

**5. Classes of IP Addresses (Default Subnet Masks)**

 - **Class - A**
   - **Range:** 0.0.0.0 – 127.255.255.255
 
   - **Default Subnet Mask:** 255.0.0.0
   - **CIDR:** /8

 - **Class - B**
   - **Range:** 128.0.0.0 – 191.255.255.255
 
   - **Default Subnet Mask:** 255.255.0.0
   - **CIDR:** /16

- **Class - C**
   - **Range:** 192.0.0.0 – 223.255.255.255
 
   - **Default Subnet Mask:** 255.255.255.0
   - **CIDR:** /24

**6. How to Subnet?**
  - **Determine Subnet Requirements:**
      - Number of subnets needed.
      - Number of hosts per subnet.
   
  - **Calculate Subnet Mask:**
      - Use bits from the host portion to create more subnets.
      - Example: For 4 subnets, borrow 2 bits (since 2 <sup>2</sup> = 4).

  - **Divide IP Range:**
      - Split the IP range according to the new subnet mask.

  **7. Example of Subnetting**
  
  - Given an IP Address: 192.168.1.0/24
  
    - **Original Subnet Mask:** 255.255.255.0 (256 IPs, 2<sup>8</sup> ).
     
    - **Subnet into 4 networks:** Borrow 2 bits → /26 (Subnet Mask = 255.255.255.192).
    - **New Subnet Ranges:**
        - 192.168.1.0 – 192.168.1.63
        - 192.168.1.64 – 192.168.1.127
        - 192.168.1.128 – 192.168.1.191
        - 192.168.1.192 – 192.168.1.255


  **8. Important Terms**
  - **Network Address:** First address in a subnet (e.g., 192.168.1.0).
  - **Broadcast Address:** Last address in a subnet (e.g., 192.168.1.255).
  - **Usable Hosts:** Total addresses minus the network and broadcast addresses.
      - Example: For /26, 2<sup>6</sup> −2 = 62 usable addresses.


  **9. VLSM (Variable Length Subnet Mask)**
  - Allows subnetting with different subnet masks in the same network.
  - More efficient IP allocation by customizing subnet sizes.

  **Summary:**
  - Subnetting helps divide a large network into smaller, manageable pieces.
  - It improves IP management, performance, and security.
  - Calculating subnets involves understanding binary operations and subnet masks.

        
    
### <ins> IP and MAC Address </ins>
- **IP Address (Internet Protocol Address):**
  - Logical address used for identifying devices across networks.
  - Assigned by ISPs or network admins (Dynamic via DHCP / Static).
  - Can change based on network (dynamic/static).
  - Can be IPv4 (32-bit) or IPv6 (128-bit).
  - Works at the Internet layer (Layer 3).
    
- **MAC Address (Media Access Control Address):**
  - Unique hardware identifier for a device.
  - Physical address, assigned to NIC (Network Interface Card) by the manufacturer.
  - 48-bit hexadecimal format (e.g., 00:1A:2B:3C:4D:5E)
  - Unique to each device and does not change with networks.
  - Works at the Data Link layer (Layer 2).

**How They Work Together?**
- When a device sends data, the IP address determines the destination **across networks**.
- The MAC address ensures that data reaches the correct device **within the local network**.
- **ARP (Address Resolution Protocol)** maps an IP address to a MAC address for communication.


### <ins> Router & Switch </ins>
- **Router:**
  - Connects different networks (e.g., home network to the internet).
  - Operates at the Network Layer (Layer 3).
  - ISP provides internet via a router.
  - Assigns IP addresses via DHCP.
  - Uses routing protocols (RIP, OSPF, BGP) to find the best path for data transmission.
  - Routes data between LAN, WAN, and the internet.


- **Switch:**
  - Connects devices within the same network (e.g., PC to PC in LAN).
  - Operates at the Data Link Layer (Layer 2).
  - Uses MAC addresses for device-to-device communication.
  - Improves network performance by reducing data collisions.  
  - Used in LAN to improve communication between devices.


- **Server = Machine = Host = Laptop = Instance(AWS) = VM(Azure) = Compute Engine(GCP)**


### <ins> Keypair </ins>
- **Keypairs** are used for secure authentication in SSH (Secure Shell) and cloud platforms (AWS, Azure).
- Consist of **private key** (kept secret) and **public key** (shared).

#### File Formats: 
- .pem (**Privacy-Enhanced Mail**) → Used in **Linux/macOS** for SSH authentication.
- .ppk (**PuTTY Private Key**) → Used in **Windows** with PuTTY SSH client.

###### Conversions:
- Convert .pem to .ppk using PuTTYgen:
   - puttygen key.pem -o key.ppk

- Convert .ppk to .pem using PuTTYgen:
   - Load .ppk in PuTTYgen → Export OpenSSH Key


### <ins> Client-Server Architecture </ins>
- A network model where a client requests services, and a server provides them.
- Used in web applications, databases, cloud computing, and network communications.

#### Components:
**1. Client:**
- Sends requests to the server.
- Can be a browser, mobile app, or any networked device.
- Example: Web browser accessing a website.

**2. Server:**
- Processes client requests and sends responses.
- Can be a web server, database server, or application server.
- Example: Nginx, Apache, MySQL.

#### Workflow:
1. Client initiates a request (e.g., HTTP request to fetch a webpage).
2. Server processes the request and retrieves data.
3. Server sends a response back to the client.

#### Types:
- **Two-Tier Architecture:** Direct communication between client and server.
- **Three-Tier Architecture:** Uses an intermediate application layer (e.g., frontend → backend → database).
- **Multi-Tier Architecture:** Scalable, with load balancers, caching, and microservices.


#### ------------------------------------------------------------ #####
1️⃣ **Network Fundamentals**

- OSI & TCP/IP Model (Layers & Differences)

- IP Addressing (IPv4 vs IPv6)

- Subnetting & CIDR Notation
  
- MAC Address vs IP Address

- Private vs Public IPs

- NAT (Network Address Translation)

- DNS (Domain Name System) & Resolution Process

- DHCP (Dynamic Host Configuration Protocol)

  
2️⃣ **Network Devices & Communication**

- Router vs Switch vs Hub vs Modem

- Load Balancers (Types: L4 vs L7, HAProxy, Nginx, ALB/ELB in AWS)

- Firewall (WAF - Web Application Firewall)

- VPN (Virtual Private Network)

- Proxy vs Reverse Proxy


3️⃣ **Protocols & Ports**

- Common Protocols & Ports:

- HTTP (80), HTTPS (443)

- FTP (21), SFTP (22), FTPS (990)

- SMTP (25), IMAP (143), POP3 (110)

- SSH (22), Telnet (23), RDP (3389)

- Difference: TCP vs UDP (Use Cases: YouTube vs Gaming)

- ICMP (Ping, Traceroute, Packet Loss)

-WebSockets (Real-time Communication)


4️⃣ **Security & Performance**

- SSL/TLS & HTTPS

-Rate Limiting & Throttling

- DDoS Attacks & Mitigation

- IP Whitelisting & Blacklisting

- Port Forwarding & Reverse SSH Tunneling

- CDN (Content Delivery Network) - How it Works?

- Latency, Bandwidth, Throughput


5️⃣ **Cloud & DevOps Networking**

- VPC (Virtual Private Cloud) & Subnets

- VPN vs Direct Connect

- Ingress & Egress Traffic in Cloud

- Containers & Networking (Docker, Kubernetes, Service Mesh)

- Microservices Communication (API Gateway, Service Discovery)


6️⃣ **Advanced Networking Concepts**

- BGP (Border Gateway Protocol) - Internet Routing

- SDN (Software-Defined Networking)

- VXLAN (Virtual Extensible LAN)

- Packet Sniffing (Wireshark, TCPDump)

- Anycast, Unicast, Multicast, Broadcast

#### ><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><><

🔹 **NAT (Network Address Translation)**
 - Converts **private IPs** to **public IPs** for internet access, enabling multiple devices to share a single public IP.

🔹 **DNS (Domain Name System) & Resolution Process**
 - Translates **domain names** (e.g., google.com) into **IP addresses** for browsers to access websites. Resolution involves recursive and authoritative DNS servers.

🔹 **DHCP (Dynamic Host Configuration Protocol)**
 - Automatically assigns **IP addresses** and other network configurations (Gateway, DNS) to devices in a network.

🔹 **Router vs Switch vs Hub vs Modem**
 - Router → Connects **different networks** (ISP to home network).
 - Switch → Connects devices in **same network** (LAN).
 - Hub → Broadcasts data to all connected devices (obsolete).
 - Modem → Converts **analog signals** (ISP) to **digital** for communication.
   
🔹 **Load Balancers (L4 vs L7, HAProxy, Nginx, ALB/ELB in AWS)**
Distributes traffic across multiple servers.

 - **L4** → Operates at the **Transport Layer** (IP/Port-based).
 - **L7** → Operates at the **Application Layer** (URL-based routing).

🔹 **Firewall (WAF - Web Application Firewall)**
 - Monitors and filters incoming/outgoing traffic based on security rules. **WAF** protects web apps from attacks like **SQL injection, XSS**.

🔹 **VPN (Virtual Private Network)**
 - Encrypts data to create a **secure private connection** over a **public network (Internet)**.

🔹 **Proxy vs Reverse Proxy**
 - **Proxy** → Acts as an intermediary for clients accessing the internet (hides client identity).
 - **Reverse Proxy** → Sits in front of servers to handle traffic and improve security/performance.
   
🔹 **ICMP (Ping, Traceroute, Packet Loss)**
Used for **network diagnostics**:

 - **Ping** → Checks if a host is reachable.
 - **Traceroute** → Tracks the route packets take.
 - **Packet Loss** → Measures dropped packets in transmission.

   
🔹 **WebSockets (Real-time Communication)**
 - Provides **full-duplex** (bi-directional) communication over a **single TCP connection** (e.g., chat apps, live updates).

🔹 **Rate Limiting & Throttling**
 - **Rate Limiting** → Restricts the number of requests **per unit time** (security & performance).
   
 - **Throttling** → Dynamically **slows dow**n request processing instead of blocking them.

🔹 **DDoS Attacks & Mitigation**
 - **Distributed Denial of Service (DDoS)** floods a network/server with excessive requests, making it unavailable.
 - **Mitigation**: Firewalls, Rate Limiting, Cloud-based DDoS protection (Cloudflare, AWS Shield).

🔹 **IP Whitelisting & Blacklisting**
 - **Whitelisting** → Only allows specified IPs to access resources.
 - **Blacklisting** → Blocks known malicious IPs.

🔹 **Port Forwarding & Reverse SSH Tunneling**
 - **Port Forwarding** → Redirects network traffic from one port/IP to another (used in hosting services).
 - **Reverse SSH Tunneling** → Allows a remote machine to access local services securely.

🔹 **CDN (Content Delivery Network) - How it Works?**
 - Distributes website content across **multiple geographically distributed server**s to reduce latency and improve speed.

🔹 **Latency, Bandwidth, Throughput**
 - **Latency** → Delay in data transmission (measured in ms).
 - **Bandwidth** → Maximum data transfer capacity (measured in Mbps/Gbps).
 - **Throughput** → Actual data transferred in a given time.

🔹 **VPC (Virtual Private Cloud) & Subnets**
 - **VPC** is a logically isolated **cloud network**. **Subnets** segment the network into smaller parts for better security and traffic control.

🔹**VPN vs Direct Connect**
 - **VPN** → Encrypted connection over the internet.
 - **Direct Connect** → Dedicated private connection to a cloud provider (faster, more secure).

🔹 **Ingress & Egress Traffic in Cloud**
 - **Ingress** → Incoming traffic to cloud services.
 - **Egress** → Outgoing traffic from cloud services (often charged by cloud providers).

🔹 **Containers & Networking (Docker, Kubernetes, Service Mesh)**
 - **Docker Networking** → Bridge, Host, Overlay networks.
 - **Kubernetes Networking** → Service discovery, Load balancing, Ingress controllers.
 - **Service Mesh** → Handles microservices communication (Istio, Linkerd).

🔹 **Microservices Communication (API Gateway, Service Discovery)**
 - **API Gateway** → Manages microservices API requests (Authentication, Rate limiting).
 - **Service Discovery** → Automatically detects services in a dynamic environment.

🔹 **BGP (Border Gateway Protocol) - Internet Routing**
 - Protocol that controls **how data is routed** between ISPs and across the internet.

🔹 **SDN (Software-Defined Networking)**
 - Decouples network **control plane** from **data plane**, enabling centralized network management.

🔹 **VXLAN (Virtual Extensible LAN)**
 - Encapsulates Layer 2 traffic over Layer 3 networks, extending **traditional VLANs** across data centers.

🔹 **Packet Sniffing (Wireshark, TCPDump)**
 - **Wireshark** → GUI-based tool to analyze network packets.
 - **TCPDump** → CLI tool for capturing network traffic in Linux.

🔹 **Anycast, Unicast, Multicast, Broadcast**
 - **Unicast** → One-to-one communication.
 - **Broadcast** → One-to-all communication.
 - **Multicast** → One-to-many (specific group).
 - **Anycast** → One-to-nearest (used in **CDNs, BGP routing**).


🔹 **SSH vs Firewall**
- **SSH** stands for secure shell. It is a secure protocol used to remotely access and manage servers or devices over an encrypted connection. By encrypting data and providing authentication, SSH ensures secure communication between two systems. Common uses include logging into remote servers, transferring files, and more.
- A **firewall** is like a security guard for your network. It watches over the data coming in and going out and decides what to allow or block based on set rules. It protects your private network from threats by preventing unauthorized access while allowing safe connections.
- In Leyman langauge,
  - SSH is a secure way to connect to the server 
  - A firewall is like a security guard where you can make sure what goes in and out on your network
- Both serve different purposes











## LINUX (for DevOps)
### All about Linux required for DevOps
> Linux is a critical skill for DevOps engineers, as most DevOps tools and practices rely on Linux-based systems.
### Why Linux for DevOps?
- **Widely Used:** Most servers, cloud platforms, and DevOps tools run on Linux.

- **Open Source:** Highly customizable and adaptable for DevOps workflows.

- **Command-Line Power:** Linux CLI is essential for automation, scripting, and managing infrastructure.

- **Tooling:** DevOps tools like Docker, Kubernetes, Jenkins, and Ansible are designed to work seamlessly on Linux.


### Essential Linux Concepts for DevOps
- **File System Hierarchy**
  - **/:** Root directory.

  - **/bin:** Essential command binaries.

  - **/etc:** Configuration files.

  - **/var:** Variable data (logs, databases).

  - **/home:** User home directories.

  - **/tmp:** Temporary files.

  - **/usr:** User-installed software and libraries.


- **Users and Permissions**
  - **Users:** Each user has a unique ID (UID) and home directory.

  - **Groups:** Users can belong to groups for shared permissions.

  - **Permissions:** Files and directories have read (r), write (w), and execute (x) permissions for owner, group, and others.

    - Example: **rwxr-xr--** means:

      - **Owner:** read, write, execute.

      - **Group:** read, execute.

      - **Others:** read.


- **Processes**
  - **Process:** A running instance of a program.

  - **PID:** Process ID (unique identifier).

  - **Foreground vs Background:** Processes can run in the foreground (interactive) or background (non-interactive).


- **Networking**
  - **IP Addresses:** Identify devices on a network.

  - **Ports:** Endpoints for communication (e.g., port 80 for HTTP).

  - **Firewall:** Controls incoming and outgoing traffic (e.g., **iptables**, **ufw**).


### Essential Linux Commands for DevOps
-  **File and Directory Management**
  - **ls:** List files and directories.
    ```
    ls -l  # Long listing
    ls -a  # Include hidden files

    fgfdg
   

