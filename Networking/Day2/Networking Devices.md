22/4/25
###### A **Computer Network ** is a digital telecommunications network which allows ==nodes== to share ==resources==


###### **Client:** A Client is a device that accesses a service made available by a server.

###### **Server:**  A Server is a device that provides functions or services for clients.

A **switch** is a smart networking device used within a **Local Area Network (LAN)** to connect multiple devices (like PCs, printers, servers). It uses **MAC addresses** to forward data directly to the intended device, making communication faster and more efficient.

### 🧩 **Key Characteristics of a Switch:**

- ✅ **Layer 2 Device:**  
    Primarily operates at the **Data Link Layer (Layer 2)** of the OSI model.
- ✅ **MAC Address Learning:**  
    Maintains a **MAC address table** to track which device is connected to which port.
- ✅ **Unicast Forwarding:**  
    Sends data only to the intended recipient’s port, unlike hubs that broadcast.
- ✅ **Full-Duplex Communication:**  
    Allows devices to **send and receive data simultaneously**, improving speed.
- ✅ **Collision Domain Isolation:**  
    Each port has its own **collision domain**, reducing traffic issues.
- ✅ **VLAN Support (Managed Switches):**  
    Enables network segmentation for better security and management.
- ✅ **Layer 3 Switching (Optional):**  
    Some switches have routing capabilities and operate at **Layer 3** as well.
- ✅ **Port Density:**  
    Switches typically have **8, 12, 24, 48, or more Ethernet ports** depending on their size and purpose.  
    (Used in small offices to large enterprise networks.)
- ✅ **Speed Variants:**  
    Support for **10/100 Mbps (Fast Ethernet), 1 Gbps, 10 Gbps** and higher port speeds.
    
eg: Cisco Catalyst 9200, Catalyst 3250

A **router** is a **Layer 3** (Network Layer) device in the OSI model that connects **multiple networks together** and manages traffic between them. It determines the **best path** for data to travel across interconnected networks using **IP addresses**.

For example, when you connect your home devices to the internet, your **Wi-Fi router** directs traffic between your devices and the internet.

---

### 🧩 **Key Characteristics of a Router:**

Routers have fewer network interface than switches 

- ✅ **Network Layer Device (Layer 3):**  
    Works at the **Network Layer** of the OSI model and uses **IP addresses** for routing.
- ✅ **Connects Multiple Networks:**  
    Bridges different networks such as **LAN to WAN**, or **LAN to LAN**.
- ✅ **Routing Tables:**  
    Maintains a **routing table** to decide the most efficient path for data packets.
- ✅ **Supports Dynamic Routing Protocols:**  
    Uses protocols like **OSPF, EIGRP, BGP** to update and manage routing paths dynamically.
- ✅ **Packet Forwarding:**  
    Examines IP headers to **forward packets** to the correct destination network.
- ✅ **Traffic Management:**  
    Can perform **NAT (Network Address Translation)** and **QoS (Quality of Service)** to manage bandwidth and improve performance.
- ✅ **Security Features:**  
    Often includes **firewall capabilities**, **ACLs (Access Control Lists)**, and **VPN support** for secure communication.
- ✅ **Fewer Ports Than Switches:**  
    Typically has **2 to 8 interfaces**—commonly **WAN and multiple LAN ports**.
- ✅ **Inter-VLAN Routing:**  
    Can route traffic between different VLANs in a network.
eg: ISR 1000, ISR 900

Firewall : Firewalls are network security devices that control network traffic entering and existing our network.


eg: ASA-5500x (Adaptive security appliance), Next gen firewall.

###### Characteristics of a Firewall:
- Monitor and control network traffic based on configured rules.
- Firewalls can be placed outside or inside the network.
- Firewalls are known as Next generation firewalls when they include more modern and advanced filtering capabilities.

Host Based Firewalls: are software applications that filter traffic entering and exiting a host machine, like a PC

Ethernet: Ethernet is a collection of network protocols/standards 
Defined in IEEE 802.3 standard in 1983
- The copper cables used in the Ethernet cables is UTP Cables( Unshielded Twisted Pair ) - 8 pins.
- Ethernet uses full - duplex transmission (Thats why no collisions ) 
- 10-Base-T, 100-Base-T are latest RG Ethernet standard cables ( 4 pins 2 for Tx, 2 for Rx) 1,2,3 and 6.
- If pin1 connects to pin1 of other device and pin2 connects to pin2........ then that is known as Straight -through cable
crossover cable uses to connect b/w similar kind of devices (refer Jeremy IT's Lab day2 video )
![[Screenshot 2025-04-22 at 14.55.56.png]]

Auto-MDI-x are latest cables they can adjust transfer and receive data accordingly

advanced cables are Fiber optic cables 

An **SFP port** (Small Form-factor Pluggable) is a **network interface slot** found on **network switches, routers, and other networking devices** that allows you to **insert SFP transceivers** for **fiber optic** or **copper connections**.

### 🔸 **Single-Mode Fiber (SMF)**

- 🌈 **Core Size**: Very small core (≈ 8 to 10 microns)
- 💡 **Light Source**: Uses a **laser** as a light source
- 🛣️ **Distance**: Supports **long-distance** transmission (up to 100+ km)
- 🚀 **Speed & Bandwidth**: High bandwidth, best for **long-haul networks**
- 💰 **Cost**: More expensive (cable and equipment)
- 📍 **Application**: Used in **telecom, ISP backbone**, and **large data centers**
    

---

### 🔹 **Multi-Mode Fiber (MMF)**

- 🌈 **Core Size**: Larger core (≈ 50 to 62.5 microns)
- 💡 **Light Source**: Uses **LEDs** as a light source
- 🛣️ **Distance**: Best for **short distances** (up to 2 km typically; ~300–600m for 10Gbps)
- 🚀 **Speed & Bandwidth**: Lower bandwidth compared to single-mode
- 💰 **Cost**: More affordable (cable and connectors are cheaper)
- 📍 **Application**: Ideal for **LAN, campus networks**, and **short-range connections**

### **Straight-Through Cable**

🟢 **Used for connecting different types of devices**

- Examples:
    
    - PC/Laptop → Switch
    - Switch → Router
    - Access Point → Switch  
        📌 **Reason:**
        
- Devices of different types **transmit (Tx)** and **receive (Rx)** on **opposite pins**, so no swapping is required.
    
- Straight-through cable maintains the pin alignment (Tx to Rx, Rx to Tx).
    

---

### 🔹 **Crossover Cable**

🔁 **Used for connecting similar types of devices directly**

- Examples:
    
    - PC ↔ PC
    - Switch ↔ Switch
    - Router ↔ Router  
        📌 **Reason:**
        
- Similar devices **transmit and receive on the same pins**, so crossover cables **swap Tx and Rx lines** to allow proper communication.
    
- Tx on one end goes to Rx on the other, and vice versa.
    

---

### 🟡 **Single-Mode Fiber Cable**

🌍 **Used for long-distance, high-speed connections**

- Examples:
    
    - Data center interconnects across cities
    - Telecom networks  
        📌 **Reason:**
        
- Uses **laser light** with a very narrow core (≈9 µm) allowing light to travel in a single path (mode), minimizing signal loss and dispersion over long distances.
    
- Ideal for **distances > 2 km**
    

---

### 🟠 **Multi-Mode Fiber Cable**

🏢 **Used for short-distance, high-bandwidth connections**

- Examples:
    
    - In-building data connections
    - Short-distance switch-to-switch connections  
        📌 **Reason:**
        
- Uses **LED light** with a wider core (≈50–62.5 µm) allowing multiple light paths (modes), which causes more dispersion and limits distance.
- Cost-effective for **shorter distances (< 2 km)**

What is Networking model ?
Networking models categorize and provide a structure for networking and standards.
###### OSI Model: (Open Systems Interconnection) model
created by ISO(International organization for standardization)

There are 7 Layers.

###### 7. Application Layer:
- This Layer is closest to the end user.
- Interacts with software apps, for example web browser (Chrome, Brave, Safari etc..)
http://www.cisco.com

http and https are Layer 7 protocols

###### 6. Presentation Layer: 
- Data in the application layer is in application format
- It needs to be translated to a different format to be sent over the network.
- The presentation layer job is to translate b/w application and network formats
- For example Encryption and decryption while sending and receiving
- Also translates b/w different application layer formats.
###### 5. Session Layer
- Controls sessions b/w communicating hosts.
- Eg: Browser sessions 
Till here all are managed by app developers.

###### 4. Transport Layer:
- Segments and reassembles data for communication b/w end hosts.
- Breaks large pieces of data into smaller segments which can be more easily sent over the network and are less likely to cause transmission problems if error occurs.
- Data + Level4 header is called as a segment.
- It provides end to end communication.

###### 3. Network Layer: 
- Provides connectivity b/w end hosts on different networks (i.e Outside of the LAN)
- provides logical addressing (IP addressing)
- provides path selection b/w source and destination.
- Data + Layer 4 header and Layer 3 header is known as packet.
- Routers operate at Layer 3.

###### 2. Data Link Layer:
- provides node to node connectivity (PC to Switch, Switch to PC, Router to Switch, Switch to Router, Router to Router)
- Layer 2 uses Mac addressing 
- Switches operates at Layer 2
- L2 Trailer+ Data+L4 header + L3 header + L2 header is called as frame 
###### 1. Physical Layer:
- Defines physical characteristics of a medium
- Digital bits are converted into electrical (for wired) or radio for (wireless)
------------------------------------------------------------------------
---

### **7️⃣ Application Layer (Layer 7)**

- Closest to the end user.
- Interfaces with software like browsers, email clients, etc.
- **Function**: Provides network services to applications.
- **Examples**: HTTP, FTP, DNS, SMTP
- **PDU**: **Data**

---

### **6️⃣ Presentation Layer (Layer 6)**

- Translates, encrypts, or compresses data for the application layer.
- Ensures data is in readable format.
- **Examples**: SSL/TLS, JPEG, MPEG
- **PDU**: **Data**
    

---

### **5️⃣ Session Layer (Layer 5)**

- Manages and maintains sessions between devices.
- Starts, manages, and terminates communication sessions.
- **Examples**: NetBIOS, PPTP
- **PDU**: **Data**
---

### **4️⃣ Transport Layer (Layer 4)**

- Ensures reliable delivery (TCP) or faster delivery (UDP).
- Handles segmentation, flow control, and error handling.
- **Protocols**: TCP, UDP
- **PDU**: **Segment**
    

---

### **3️⃣ Network Layer (Layer 3)**

- Responsible for addressing and routing between networks.
- Determines the best path for data.
- **Devices**: Routers
- **Protocols**: IP, ICMP
- **PDU**: **Packet**
    

---

### **2️⃣ Data Link Layer (Layer 2)**

- Delivers frames within the same local network.
- Uses MAC addresses for local addressing.
- **Devices**: Switches, Bridges
- **Protocols**: Ethernet, PPP
- **PDU**: **Frame**
    

---

### **1️⃣ Physical Layer (Layer 1)**

- Transmits raw binary data (0s and 1s).
- Includes physical elements: cables, connectors, signals.
- **Devices**: Hubs, NICs, Cables
- **PDU**: **Bit**
------------------------------------------------------------------------
