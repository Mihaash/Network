The **OSI Model (Open Systems Interconnection Model)** is a **conceptual framework** used to understand and describe how data moves through a network — from one computer (or device) to another.


**Physical Layer**
It is responsible for the **actual transmission of raw data bits (0s and 1s)** over a physical medium — like cables, fiber optics, or radio waves

**Data Link Layer**
It is responsible for the **reliable transfer of data** across a physical link — from one device (like a computer or switch) to another — by organizing raw bits from the Physical Layer into **frames** and ensuring **error-free** delivery.

**Network Layer**
The **Network Layer** is the **3rd layer** of the **OSI Model**, and it plays a key role in **moving data between different networks** — not just within a single local network.
The **Network Layer** delivers data **from one network to another**, possibly across the world.

**Transport Layer**
**segments** data from the upper layers, ensures **error-free delivery**, and provides **flow control**.  
It uses protocols like **TCP** (reliable, connection-oriented) and **UDP** (fast, connectionless).  
In short, it ensures that data is **delivered completely, correctly, and in order**

**Session Layer**
It is responsible for **establishing, managing, and terminating sessions** between two devices or applications.

**Presentation Layer**
This layer is responsible for **data formatting, encryption, and compression** to ensure that data is readable by both sender and receiver.

**Application Layer**
It provides **network services directly to end users and applications**, like web browsers and email clients.
Common examples include **HTTP/HTTPS**, **FTP**, **SMTP**, **DNS**, and **Telnet**.
# **What is NDP (Neighbor Discovery Protocol)?**

**NDP** is a protocol used by IPv6 devices to:

- Discover **neighbors** on the same link
- Find **MAC addresses** of IPv6 devices (like ARP in IPv4)
- Discover **routers**
- Automatically configure IPv6 addresses (SLAAC)
- Check if a neighbor is reachable

**what is Maximum Transmission Unit (MTU)
The **Maximum Transmission Unit (MTU)** is the **largest size (in bytes)** of a data packet that can be **sent over a network link** **without being fragmented**.
If MTU = **1500 bytes** and your IP header (20 bytes) + ICMP header (8 bytes) = 28 bytes,  
then your data payload can be **1472 bytes** →

### **Common MTU Values**

| **Network Type**     | **Typical MTU Size** |
| -------------------- | -------------------- |
| Ethernet             | **1500 bytes**       |
| Wi-Fi (802.11)       | ~2304 bytes          |
| PPPoE                | **1492 bytes**       |
| VPN (IPsec, GRE)     | 1400–1460 bytes      |
| Loopback (localhost) | 65535 bytes          |

**what is fragement

**Fragmentation** is the process of **breaking a large IP packet** into smaller packets (fragments) so they can pass through a network with a smaller MTU.


### 🧭 **Types of Network Topologies**

| **Topology**                        | **Structure / Description**                                            | **Advantages**                                                                  | **Disadvantages**                                                            |
| ----------------------------------- | ---------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **1. Bus Topology**                 | All devices share a **single central cable** (the bus).                | Easy to install, low cost for small networks.                                   | If the main cable fails, the whole network stops; difficult to troubleshoot. |
| **2. Star Topology**                | All devices connect to a **central hub or switch**.                    | Easy to add/remove devices; failure of one device doesn’t affect others.        | If the central hub fails, the entire network goes down.                      |
| **3. Ring Topology**                | Each device connects to **two others**, forming a **circular path**.   | Data travels in one direction, reducing collisions.                             | Failure in one cable or device breaks the loop (unless dual-ring is used).   |
| **4. Mesh Topology**                | Every device connects **directly to every other device**.              | Very reliable and fault-tolerant; if one link fails, data can use another path. | Very expensive and complex for large networks.                               |
| **5. Tree (Hierarchical) Topology** | A combination of **star topologies** connected to a main bus backbone. | Scalable and easy to manage.                                                    | Failure of the main backbone affects the whole network.                      |
| **6. Hybrid Topology**              | A mix of two or more topologies (e.g., star-bus, star-ring).           | Flexible and efficient; used in large networks.                                 | Complex design and maintenance.                                              |
|                                     |                                                                        |                                                                                 |                                                                              |
### **Examples**
- **Office network:** Often a **Tree or Hybrid topology**.
- **Data centers:** Commonly use **Mesh or Partial Mesh** for high reliability.


**Types of computer networks**

| **Network Type**  | **Full Form**             | **Coverage Area**            | **Example**                 | **Speed**                      | **Used For**                       |
| ----------------- | ------------------------- | ---------------------------- | --------------------------- | ------------------------------ | ---------------------------------- |
| **PAN**           | Personal Area Network     | A few meters (1–10m)         | Bluetooth, Hotspot          | Low                            | Connecting personal devices        |
| **LAN**           | Local Area Network        | Within a building            | Home/Office Wi-Fi, Ethernet | Very High (100 Mbps – 10 Gbps) | Internal office or home networks   |
| **MAN**           | Metropolitan Area Network | Within a city or campus      | Cable TV, City Wi-Fi        | High                           | Connecting LANs across a city      |
| **WAN**           | Wide Area Network         | Across countries/continents  | Internet                    | Medium to High                 | Global communication between LANs  |
| **CAN**           | Campus Area Network       | Large campus or organization | University network          | High                           | Interconnecting departmental LANs  |
| **GAN**           | Global Area Network       | Worldwide                    | Satellite networks          | Medium                         | Global business or airline systems |
| **VPN**           | Virtual Private Network   | Virtual (over Internet)      | Remote office access        | Depends on Internet            | Secure remote connection           |
| **P2P**           | Peer-to-Peer              | Depends on peers’ connection | BitTorrent, Blockchain      | Varies                         | File sharing and decentralized use |
| **Client-Server** | —                         | Depends on server setup      | Web servers, Email servers  | High                           | Centralized control and management |
|                   |                           |                              |                             |                                |                                    |


**Internet Service Provider
SmartJack
- A **SmartJack** is a device installed by the ISP at the customer’s site.
- It acts as the **connection point between the ISP network and the customer’s network**.
- It helps in **signal conversion, testing, and troubleshooting** of WAN lines.
**Demarcation Point**
- The **Demarcation Point (Demarc)** is the **physical boundary** between ISP and customer equipment.
- It defines **who is responsible** for maintenance — ISP or customer.
- The SmartJack is usually located **at or near the demarcation point**.
- Together, they ensure **clear separation and smooth communication** between ISP and user networks.

**Digital Subscriber Line**
1. existing **copper telephone wires** to transmit digital data.
2. It provides **high-speed Internet** without interrupting phone calls.
3. Works by separating **voice and data signals** using filters or splitters.
4. Common types include **ADSL (Asymmetric DSL)** and **VDSL (Very-high-bit-rate DSL)**.
5. **ADSL** gives higher download speed than upload speed (for home users).
6. **VDSL** offers much faster speeds for short distances.
7. DSL speeds usually range from **1 Mbps to 100 Mbps**, depending on line quality.
|**Feature**|**ADSL (Asymmetric DSL)**|**VDSL (Very-high-bit-rate DSL)**|
|---|---|---|
|**Full Form**|Asymmetric Digital Subscriber Line|Very-high-bit-rate Digital Subscriber Line|
|**Speed**|Download: 1–24 MbpsUpload: 128 Kbps–3 Mbps|Download: 50–300 MbpsUpload: 10–100 Mbps|
|**Speed Type**|**Asymmetric** — download is faster than upload|**Symmetric or nearly symmetric** — both are fast|
|**Distance from ISP**|Works up to **5 km** from the telephone exchange|Works best within **1–1.5 km** (speed drops with distance)|
|**Technology Generation**|Older DSL technology|Newer, improved version of DSL|
|**Use Case**|Home users — web browsing, email, streaming|Businesses or heavy users — HD streaming, gaming, VoIP|
|**Line Type**|Uses existing copper telephone line|Uses copper or fiber-to-the-cabinet (FTTC)|
|**Performance**|Lower speed, stable long-distance|Higher speed, short-distance optimized|

| Feature           | **Fiber Ethernet**                                                                     | **Metro Ethernet**                                                                                             |
| ----------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Definition**    | Uses optical fiber cables to connect a single site or building to the Internet or LAN. | A city-wide (metropolitan area) Ethernet network connecting multiple sites/offices within the same metro area. |
| **Coverage Area** | Local (within a building or campus).                                                   | Wide (across a city or metro region).                                                                          |
| **Purpose**       | Provides high-speed connectivity to a single location or network segment.              | Connects multiple business branches or data centers in a city using Ethernet technology.                       |
| **Speed**         | Typically 1 Gbps to 100 Gbps.                                                          | Typically 10 Mbps to 10 Gbps, depending on service plan.                                                       |
| **Topology**      | Point-to-point (LAN or WAN link).                                                      | Multipoint or mesh (Metro Area Network).                                                                       |
| **Ownership**     | Usually owned and managed by the organization.                                         | Provided and managed by a telecom/ISP.                                                                         |
| **Use Case**      | Internet access or internal LAN backbone.                                              | Interconnecting multiple company branches within a city.                                                       |
| **Example**       | Fiber line connecting your office to the Internet.                                     | Metro Ethernet linking head office and branch offices in the same city.                                        |

**IPv4 Address Types**
|**Class**|**Range**|**Default Subnet Mask**|**Use Case**|
|---|---|---|---|
|**Class A**|1.0.0.0 – 126.255.255.255|255.0.0.0|Used for **very large networks** (e.g., ISPs, big organizations).|
|**Class B**|128.0.0.0 – 191.255.255.255|255.255.0.0|Used for **medium-sized networks** (universities, companies).|
|**Class C**|192.0.0.0 – 223.255.255.255|255.255.255.0|Used for **small networks** (home or office LANs).|
|**Class D**|224.0.0.0 – 239.255.255.255|—|Used for **multicasting** (sending data to multiple systems).|
|**Class E**|240.0.0.0 – 255.255.255.255|—|**Experimental / Research** use only.|

| **Class**   | **Private Range**             | **Range Size (Number of IPs)** | **Use Case**        |
| ----------- | ----------------------------- | ------------------------------ | ------------------- |
| **Class A** | 10.0.0.0 – 10.255.255.255     | **≈ 16,777,216 addresses**     | Very large networks |
| **Class B** | 172.16.0.0 – 172.31.255.255   | **≈ 1,048,576 addresses**      | Medium networks     |
| **Class C** | 192.168.0.0 – 192.168.255.255 | **≈ 65,536 addresses**         | Small/home networks |

**Router**
### **Functions of a Router:**

1. **Routing:** Finds the most efficient path for data to reach its destination.
2. **Network Connection:** Connects your local network (LAN) to the Internet (WAN).
3. **IP Address Assignment:** Often provides IP addresses to devices via **DHCP**.
4. **Network Address Translation (NAT):** Converts private IP addresses into a single public IP for Internet access.
5. **Firewall & Security:** Protects your network by blocking unwanted traffic.
**NAT Overload**
**NAT Overload** is the **most common form of NAT** used in home and office routers.  
It allows **many devices on a private network** to **share one public IP address** when connecting to the Internet.
### **How It Works:**

1. Each device inside your LAN has a **private IP** (e.g., `192.168.1.10`, `192.168.1.11`).
2. When these devices access the Internet, the router replaces their **private IPs** with a **single public IP** (assigned by the ISP).
3. The router uses **different port numbers** to keep track of which request belongs to which device.
    - Example:
        - Laptop → Google.com → uses port `1025`
        - Phone → YouTube.com → uses port `1026`
|**Device**|**Private IP**|**Public IP (Router)**|**Port**|
|---|---|---|---|
|Laptop|192.168.1.10|103.24.45.5|1025|
|Phone|192.168.1.11|103.24.45.5|1026|
|PC|192.168.1.12|103.24.45.5|1027|

## **Unicast**
Unicast is **one-to-one communication** — data is sent from **one sender to one specific receiver**.

You open a website — your computer sends a request **directly to one web server**.
**🎯 Used For:**
- Web browsing (HTTP/HTTPS)
- File transfers (FTP)
- Email (SMTP, POP3)

---

## **2. Broadcast**

Broadcast is **one-to-all communication** — data is sent from **one sender to all devices** on the same network.
When a computer first connects to a network and sends an **ARP request** —  
“Who has IP 192.168.1.1?” — every device receives it.
**🎯 Used For:**
- ARP (Address Resolution Protocol)
- DHCP (to find IP addresses)
- Network discovery
Broadcast works only in **Local Area Networks (LANs)** — routers **do not forward broadcast packets** beyond a network.

---

## ** Multicast**

**📘 Definition:**  
Multicast is **one-to-many communication**, but only to **specific group members**, not everyone.

Video streaming or live IPTV — the server sends one stream, and multiple subscribers receive it if they’ve joined that group.
**🎯 Used For:**
- Video conferencing (Zoom, IPTV)
- Online gaming
- Streaming live events

**💡 IP Range:**  
`224.0.0.0 – 239.255.255.255` (IPv4 multicast range)

---
## 📍 ** Anycast**

**📘 Definition:**  
Anycast is **one-to-one-of-many communication** — data is sent to **the nearest or best destination** in a group of possible receivers.
When you use **Google DNS (8.8.8.8)**, your query goes to the **nearest Google DNS server**, not all of them.
**🎯 Used For:**
- **CDNs (Content Delivery Networks)** like Cloudflare, Google, or Akamai
- **DNS servers** and **load balancing** for performance and reliability

### Subnet

A **subnet** (short for **subnetwork**) is a **smaller, logical section of a larger IP network**.  
It’s used to **divide a big network into smaller, manageable parts** for better performance, security, and organization
A **subnet** is a **group of IP addresses** that share the same **network prefix**.  
Subnetting means **splitting one large network** (like `192.168.0.0/16`) into **smaller subnetworks** (like `192.168.1.0/24`, `192.168.2.0/24`, etc.).
###  **Why Subnets Are Used**

1. ✅ **Improves network performance** — reduces unnecessary broadcast traffic.
2. 🔒 **Enhances security** — isolates parts of the network (e.g., servers separate from users).
3. 🧩 **Simplifies management** — easier to locate and troubleshoot devices.
A **subnet mask** tells which portion of the IP address represents the **network** and which part represents the **host**.
|**CIDR Notation**|**Subnet Mask**|**Usable Hosts**|
|---|---|---|
|`/24`|255.255.255.0|254|
|`/25`|255.255.255.128|126|
|`/26`|255.255.255.192|62|
|`/30`|255.255.255.252|2|

| **Class** | **Network Range**           | **Default Subnet Mask** | **CIDR Notation** | **No. of Networks** | **Hosts per Network (Usable)** | **First Octet Range** | **Purpose**                                     |
| --------- | --------------------------- | ----------------------- | ----------------- | ------------------- | ------------------------------ | --------------------- | ----------------------------------------------- |
| **A**     | 0.0.0.0 – 127.255.255.255   | 255.0.0.0               | /8                | 128                 | 16,777,214                     | 1 – 126               | Very large networks (ISPs, enterprises)         |
| **B**     | 128.0.0.0 – 191.255.255.255 | 255.255.0.0             | /16               | 16,384              | 65,534                         | 128 – 191             | Medium-sized networks (universities, companies) |
| **C**     | 192.0.0.0 – 223.255.255.255 | 255.255.255.0           | /24               | 2,097,152           | 254                            | 192 – 223             | Small networks (homes, small offices)           |
| **D**     | 224.0.0.0 – 239.255.255.255 | Not used                | —                 | —                   | —                              | 224 – 239             | Multicasting                                    |
| **E**     | 240.0.0.0 – 255.255.255.255 | Not used                | —                 | —                   | —                              | 240 – 255             | Experimental / Research                         |


## **EUI(Extended Unique Identifier)?**

**EUI** is a **standard format** developed by the **IEEE** to create **unique identifiers** for network devices (like network cards).
||**Type**|**Bits**|**Used In**|**Example**|
|---|---|---|---|
|**EUI-48**|48 bits|Standard **MAC addresses** (used in IPv4 & Ethernet)|`00-1A-2B-3C-4D-5E`|
|**EUI-64**|64 bits|**IPv6 Interface IDs** (used in IPv6 addresses)|`021A:2BFF:FE3C:4D5E`|

## **EUI-48 (MAC Address)**

- Each device’s **Network Interface Card (NIC)** has a **48-bit unique address**.
- Example: `00:1A:2B:3C:4D:5E`
- It’s globally unique and assigned by the manufacturer.

---
## **EUI-64 (Used in IPv6)**

- When IPv6 was developed, we needed a **64-bit interface ID**.
- So, EUI-64 was created by **expanding** the 48-bit MAC address.\
MAC:   00:1A:2B:3C:4D:5E
EUI-64: 021A:2BFF:FE3C:4D5E

| Step | Operation    | Result                        |
| ---- | ------------ | ----------------------------- |
| 1    | Start MAC    | 00:1A:2B:3C:4D:5E             |
| 2    | Insert FFFE  | 00:1A:2B:FF:FE:3C:4D:5E       |
| 3    | Flip 7th bit | 02:1A:2B:FF:FE:3C:4D:5E       |
| 4    | Add prefix   | 2001:db8::021A:2BFF:FE3C:4D5E |
**What is a NATed IPv4 Address**
- belongs to a **private IP range**
- is **not directly reachable from the Internet**
- is **translated** by the router into a **public IP** when accessing the Internet

# **What is Miredo?**

**Miredo** is a software client and server that implements the **Teredo tunneling protocol** on Linux systems
# **What is Dual Stack Routing?**
➡️ Devices have **two IP addresses**: one IPv4 and one IPv6  
➡️ Routers forward **both IPv4 and IPv6 traffic**  
➡️ Networks can communicate with **both IPv4-only** and **IPv6-only** systems
**Dual Stack = running IPv4 + IPv6 simultaneously.**

# **What is NDP (Neighbor Discovery Protocol)?**
- Discover **neighbors** on the same link
- Find **MAC addresses** of IPv6 devices (like ARP in IPv4)
- Discover **routers**
- Automatically configure IPv6 addresses (SLAAC)
- Check if a neighbor is reachable
#  **What is SLAAC?**

**SLAAC** allows an IPv6 host (computer, phone, router, etc.) to **automatically generate its own IPv6 address** using information provided by the **network’s router**.
# **What is DAD (Duplicate Address Detection)?**

**DAD** is a process in IPv6 used to check if an IPv6 address is **already being used** by another device on the same network.
Before a device starts using an IPv6 address, it must first ensure **no duplicate exists**.

# 0 to 1023 port 

Port numbers **0 through 1023** are known as **Well-Known Ports** or **System Ports**.  
They are assigned by **IANA** (Internet Assigned Numbers Authority) and used by **important, standard network services and protocols**.
|Range|Name|Purpose|
|---|---|---|
|**0–1023**|Well-Known Ports|Standard services (HTTP, DNS, SSH)|
|**1024–49151**|Registered Ports|User applications (e.g., Skype, games)|
|**49152–65535**|Dynamic/Ephemeral Ports|Temporary ports used by client machines|

# **Registered Ports (1024 – 49151)**

These ports are also called **User Ports** or **Registered Service Ports**.
- **User applications**
- **Network services**
- **Third-party software**
- **Games**
- **Custom servers**

They are **not reserved** like ports 0–1023, but they are **registered with IANA** to avoid conflicts.

| Port     | Protocol | Service                        |
| -------- | -------- | ------------------------------ |
| **1433** | TCP      | Microsoft SQL Server           |
| **1812** | UDP      | RADIUS Authentication          |
| **2049** | TCP/UDP  | NFS (Network File System)      |
| **3306** | TCP      | MySQL                          |
| **3389** | TCP      | Remote Desktop Protocol (RDP)  |
| **3690** | TCP      | Subversion (SVN)               |
| **5000** | TCP/UDP  | UPnP / Custom apps             |
| **5060** | UDP      | SIP (VoIP)                     |
| **5432** | TCP      | PostgreSQL                     |
| **8080** | TCP      | HTTP-Alternate (proxy servers) |

# Port Ranges
| Port Range      | Name                    | Purpose                             |
| --------------- | ----------------------- | ----------------------------------- |
| **0–1023**      | Well-known ports        | Standard protocols (HTTP, DNS, SSH) |
| **1024–49151**  | Registered ports        | Applications, databases, servers    |
| **49152–65535** | Dynamic/Ephemeral ports | Temporary client communication      |
**Port 25 — Server-to-Server SMTP  VS  Port 587 — Mail Submission (Recommended)
|Feature|Port 25|Port 587|
|---|---|---|
|Purpose|Server-to-server SMTP|Client-to-server SMTP submission|
|Authentication|❌ No|✔ Yes|
|Encryption|❌ None (unless manually configured)|✔ STARTTLS supported|
|ISP Blocking|✔ Often blocked|❌ Rarely blocked|
|Secure?|❌ Less secure|✔ Secure & recommended|
|Use Case|Mail relay between servers|Sending email from clients/apps|

# **POP (Post Office Protocol)**
**Purpose:** Download emails from the server to your device.
### ✔ How it works
- POP **downloads emails** to your device.
- Emails are usually **removed from the server** after download.
- You read emails **offline** after downloading.
### ✔ POP Ports
- **Port 110** → POP (unsecured)
- **Port 995** → POP3S (secure, SSL/TLS)
# **IMAP (Internet Message Access Protocol)**
**Purpose:** Sync email between server and multiple devices.
### ✔ How it work
- IMAP **keeps emails on the server**.
- Your device only **views and syncs** messages.
- Any action (delete, read, move) updates everywhere.
### ✔ IMAP Ports
- **Port 143** → IMAP (unsecured)
- **Port 993** → IMAPS (secure, SSL/TLS)
### ✔ Good for:
- Using email on **multiple devices**
- Keeping messages synced
- Accessing emails everywhere
## **SSL (Secure Sockets Layer)**
**SSL** is the **older** protocol used to secure data between a client and a server.
- Created by Netscape in the 1990s
- Versions: **SSL 1.0, 2.0, 3.0**
- **All SSL versions are now deprecated & insecure**
- Vulnerable to attacks like POODLE, BEAST, DROWN
## **TLS (Transport Layer Security)**
**TLS** is the **newer, more secure, improved version** of SSL.
- Created to replace SSL
- Versions: **TLS 1.0, 1.1, 1.2, 1.3**
- **TLS 1.2 & TLS 1.3 are secure and widely used today**
- TLS provides better:
    - Encryption
    - Authentication
    - Performance
    - Security
**What is Syslog**
**Syslog** is a **standard protocol** used to collect, store, and send **system logs** (messages) from devices such as routers, switches, firewalls, servers, and applications to a **central log server**.
**Syslog (System Logging Protocol)** is used for:
- Logging system events
- Sending logs to a remote server
- Centralized monitoring
- Troubleshooting network devices
- Security auditing
It is supported by almost all network devices:
- Cisco routers
- Firewalls
- Linux servers
- Load balancers
- Switches
- Applications
|Level|Name|Meaning|
|---|---|---|
|0|**Emergency**|System unusable|
|1|**Alert**|Immediate action needed|
|2|**Critical**|Critical condition|
|3|**Error**|Error condition|
|4|**Warning**|Warning|
|5|**Notice**|Normal but important|
|6|**Informational**|General info|
|7|**Debug**|Debugging messages|


**Syslog Uses Port 514**
|Transport|Port|Usage|
|---|---|---|
|UDP|**514**|Most common, fast|
|TCP|**514**|Reliable delivery|
|TCP+TLS|**6514**|Encrypted Syslog|

 **Network Time Protocol(NTP)**
 
 (Network Time Protocol**NTP)** is a protocol used to **synchronize the clock (time and date)** of computers, servers, routers, switches, and other devices over a network.
 |Protocol|Port|Purpose|
|---|---|---|
|**UDP**|**123**|Time synchronization|

**SIP
**SIP (Session Initiation Protocol)** is a **signaling protocol** used to **set up, manage, and end real-time communication sessions** over IP networks.

These sessions can include:
- Voice calls (VoIP)
- Video calls
- Messaging
- Conferencing
|Protocol|Port|
|---|---|---|
|**UDP 5060**|Most common||
|**TCP 5060**|Some systems||
|**TCP/TLS 5061**|Secure SIP (SIPS)||

# **How SIP Works (Simple Example)**

### 1️⃣ Caller sends **INVITE**

### 2️⃣ Callee replies **180 Ringing**

### 3️⃣ When answered → **200 OK**

### 4️⃣ Caller sends **ACK**

### 5️⃣ Call media sent using **RTP**

### 6️⃣ End call with **BYE**

# **VPNs Are Used**

- **Privacy:** Hide your IP and online activity
- **Security:** Encrypt all traffic (public WiFi protection)
- **Remote Access:** Employees connect to office network
- **Site-to-Site Networking:** Connect multiple branches
- **Bypass restrictions:** Access blocked content
**What is IPsec**
**IPsec** is a framework of protocols that provides:
### ✔ Encryption (confidentiality)
### ✔ Authentication (identity verification)
### ✔ Integrity (no tampering)
### ✔ Anti-replay protection
It is used mainly for **VPNs** (Virtual Private Networks), especially **site-to-site and remote-access VPNs**.
# **ESP (Encapsulating Security Payload)

**ESP (Encapsulating Security Payload)** is one of the **main protocols inside IPsec**, used to **encrypt and protect data** traveling across a network.

# **DHCP (Dynamic Host Configuration Protocol)**
**DHCP (Dynamic Host Configuration Protocol)** is a network protocol that automatically assigns **IP addresses and network settings** to devices on a network.

✔ IP Address  
✔ Subnet Mask  
✔ Default Gateway  
✔ DNS Server  
✔ Lease Time
# **DHCP 4-Step Process (DORA)**

### 1️⃣ Discovery
Client broadcasts:  
“I need an IP!”
### 2️⃣ Offer
Server replies with available IP offer.
### 3️⃣ Request
Client requests the offered IP.
### 4️⃣ Acknowledgment
Server confirms and assigns the IP.
This is called **DORA**.

---
#  **DHCP Ports**

| Direction       | Protocol | Port   |
| --------------- | -------- | ------ |
| Client → Server | UDP      | **67** |
| Server → Client | UDP      | **68** |

# **recursive DNS query**
**recursive DNS query** is when a DNS client asks a DNS server to _fully resolve_ a domain name **on its behalf**, and the DNS server takes responsibility for finding the final answer.

👉 The DNS server will keep querying other DNS servers  
👉 Until it finds the correct IP  
👉 Then returns the final result to the client
**“What is the IP of google.com?”**
Your resolver (like 8.8.8.8) will:
1. Ask Root DNS servers
2. Ask TLD servers (.com)
3. Ask Authoritative server (google)
4. Get the final IP
5. Send it back to you
# **DNS Record**
A **DNS Record** is a database entry inside a DNS zone file that maps a domain name to specific information (like IP address, mail server, etc.)
**Most Common DNS Record Types (Explained Simply)**
### 1️⃣ **A Record**

Maps a domain → IPv4 address  
Example:  
`google.com → 142.250.182.78`

---

### 2️⃣ **AAAA Record**

Maps a domain → IPv6 address  
Example:  
`google.com → 2404:6800:4009:80c::200e`

---

### 3️⃣ **CNAME Record**

Alias → points one name to another name  
Example:  
`www.example.com → example.com`

(cannot point to an IP, only to another hostname)

---

### 4️⃣ **MX Record**

Mail Exchange record  
Specifies the email server for the domain  
Example:  
`example.com → mail handled by gmail`

---

### 5️⃣ **TXT Record**

Stores text information  
Used for:
- SPF
- DKIM
- Domain verification
- Google verification
Example:  
`v=spf1 include:_spf.google.com ~all`

---

### 6️⃣ **NS Record**

Nameserver record  
Specifies which DNS servers host the domain.

Example:  
`ns1.cloudflare.com`  
`ns2.cloudflare.com`

---

### 7️⃣ **PTR Record**

Pointer → used for Reverse DNS  
Maps `IP → Domain`
Opposite of A record.
Example:  
`142.250.182.78 → google.com`
Used for:
- Email validation
- Network diagnostics
---

### 8️⃣ **SRV Record**
Service record  
Specifies port + protocol for a service.
Example:  
`_sip._tcp.example.com`
Used for:
- SIP
- VoIP
- Skype
- Teams
---

### 9️⃣ **SOA Record**

Start of Authority  
Contains info for:
- Primary DNS server
- Refresh timers
- Admin email
- Serial number

**STP vs RSTP** 

|Feature|**STP (Spanning Tree Protocol)**|**RSTP (Rapid Spanning Tree Protocol)**|
|---|---|---|
|Standard|IEEE **802.1D**|IEEE **802.1w**|
|Speed|**Slow convergence** (30–50 sec)|**Very fast convergence** (1–3 sec)|
|Purpose|Prevent loops|Prevent loops, faster recovery|
|Port Roles|Root, Designated, Blocking|Root, Designated, Alternate, Backup|
|Port States|Blocking, Listening, Learning, Forwarding, Disabled|Discarding, Learning, Forwarding|
|BPDU Handling|Sent by Root only|Sent by ALL switches|
|Topology change reaction|Slow|Immediate|
**What is GCMP**
**GCMP (Galois/Counter Mode Protocol)** is an **encryption algorithm** used in Wi-Fi.
It is stronger and faster than the older CCMP/AES mode.
provides:

✔ Confidentiality  
✔ Integrity  
✔ Authentication  
✔ High performance

## **2G Encryption**

Very weak / broken today

Algorithms:
- **A5/1**    
- **A5/2**
- **A5/3** (_better, rarely used_)
## **3G Encryption**
Much stronger than 2G
Algorithms:
- **KASUMI (UEA1 / UIA1)**
- **SNOW 3G (UEA2 / UIA2)**
## **4G (LTE) Encryption**
Very strong modern encryption
Algorithms:
- **AES**
- **SNOW 3G**
- **ZUC**
## **5G Encryption**
Strongest and most advanced
Algorithms:
- **AES-128**
- **ZUC-256**
- **SNOW 3G (fall-back)**
**Audit Logs**
**Audit Logs** (also called **Audit Trails**) are records that track and document **important actions and events** that happen inside a system, network, application, or device.
# **What do Audit Logs record?**

Examples:

- User login / logout
    
- Failed login attempts
    
- Password changes
    
- System configuration changes
    
- File access
    
- Admin actions
    
- Program installation
    
- Authorization changes
    
- Security events
    
- Network access attempts
**Syslog**
**Syslog** (System Logging Protocol) is a **standard protocol** used to send system logs, alerts, and event messages from devices to a **central log server**.
Syslog is a protocol that allows devices to send log messages to a **central logging system** using standard message formatting and ports.
# Syslog is used by:

✔ Firewalls  
✔ Routers  
✔ Switches  
✔ Servers  
✔ Linux systems  
✔ Windows (via agents)  
✔ IDS / IPS  
✔ Applications  
✔ Access points
