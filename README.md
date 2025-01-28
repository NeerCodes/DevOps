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

### Internet Service Provider (ISP) Hierarchy
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


### OSI Model & TCP/IP Model
- According to the International Organization for Standardization (ISO), the OSI (Open Systems Interconnection) model defines a 7-layer communication framework that helps understand how network systems interact.

#### OSI Model (Theoretical Model):
**1. Physical Layer –** Transmission of raw data (bits) over physical media.

**2. Data Link Layer –** Error detection, correction, and framing (MAC, Ethernet).

**3. Network Layer –** Routing and addressing (IP addresses).

**4. Transport Layer –** Reliable data delivery, flow control (TCP/UDP).

**5. Session Layer –** Establishing, managing, and terminating sessions.

**6. Presentation Layer –** Data translation, encryption, compression.

**7. Application Layer –** User interface and application services (HTTP, FTP, etc.).

**Key Point:** The OSI model provides a conceptual understanding of how the internet theoretically works.

#### TCP/IP Model (Practical Model):
- In real-world applications, the TCP/IP (Transmission Control Protocol/Internet Protocol) model, which powers the modern internet, simplifies the OSI model into 4 layers, combining similar functionalities:

**1. Network Interface Layer (Combines OSI Physical + Data Link) –** Handles hardware addressing, physical transmission, and framing (Ethernet, Wi-Fi).

**2. Internet Layer (OSI Network Layer) -** Responsible for addressing and routing data (IP, ICMP).

**3. Transport Layer (Same as OSI Transport Layer) –** Ensures end-to-end communication (TCP/UDP).

**4. Application Layer (Combines OSI Application + Presentation + Session) –** Provides services to end users (HTTP, FTP, DNS).

**Key Point:** The TCP/IP model is the real-world implementation used for internet communication.


### Internet Protocols
#### 1. Application layer Protocols
> These protocols provide end-user services and enable communication between applications. Common protocols include:
- **HTTP/HTTPS (HyperText Transfer Protocol/Secure)**
  - Used for web browsing and data transfer over the web.
  - **Ports:** 80 (HTTP), 443 (HTTPS)
- 
- **SMTP (Simple Mail Transfer Protocol)**
  - Used for sending emails.
  - **Ports:** 25, 587 (SMTP with encryption)
- **FTP (File Transfer Protocol)**
  - Used for file transfers between systems
  - **Ports: 21** (control), 20 (data transfer)
- **Actionable Tip:** Ensure familiarity with port numbers for security configurations and firewall rules.

in Transport,
-TCP(YouTube)
-UDP(Live Stream, Gaming, Vdo call)

in Internet,
-IP

in N/W,
-

