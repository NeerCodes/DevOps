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

**1. What is a Subnet?**
 - Subnetting is the process of splitting a larger IP network into smaller subnets.
 - This allows efficient utilization of IP addresses and reduces network congestion
 - Helps in isolating traffic for security and better control.

**2. What is Subnetting?**
 - Subnetting is the process of splitting a larger IP network into smaller subnets.
 - This allows efficient utilization of IP addresses and reduces network congestion
 - Helps in isolating traffic for security and better control.

**3. Why is Subnetting Important?**
 - **Efficient IP Address Management:** Conserves IP addresses by avoiding wastage.
 - **Improved Network Performance:** Limits broadcast traffic within a subnet.
 - **Enhanced Security:** Isolates different network segments.
 - **Simplifies Administration:** Makes troubleshooting easier by segmenting networks.
