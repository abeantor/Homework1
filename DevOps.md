# **DevOps**

## **Overview**

# **DevOps Study Guide**

## **Commands Covered**

### **File System Navigation**

- `cd` - Change directory.
- `cd ..` - Move to the parent directory.
- `cd ~` (macOS/Linux) - Move to the home directory.
- `cd \` (Windows) - Move to the root directory.
- `pwd` - Print working directory.
  - `pwd` (macOS/Linux).
  - `echo %cd%` (Windows).
- `ls` (macOS/Linux) / `dir` (Windows) - List directory contents.

### **File and Directory Operations**

- `mkdir` - Create a new directory.
- `rmdir` (Windows/macOS/Linux) - Remove an empty directory.
- `rmdir /s` (Windows) - Remove a directory and its contents.
- `rm` (macOS/Linux) - Remove files or directories.
- `cp` (macOS/Linux) / `copy` (Windows) - Copy files or directories.
- `mv` (macOS/Linux) / `move` (Windows) - Move or rename files and directories.
- `ren` (Windows) - Rename files or directories.

### **File Viewing**

- `cat` (macOS/Linux) / `type` (Windows) - Display the content of a file.
- `less` (macOS/Linux) - View a file one screen at a time.
- `head` (macOS/Linux) - Display the first few lines of a file.
- `tail` (macOS/Linux) - Display the last few lines of a file.

### **File Permissions**

- `chmod` (macOS/Linux) - Change file permissions.
- `chown` (macOS/Linux) - Change file ownership.

### **Process Management**

- `tasklist` (Windows) / `ps` (macOS/Linux) - List running processes.
- `taskkill` (Windows) - Terminate a process.
- `kill` (macOS/Linux) - Terminate a process.
- `top` (macOS/Linux) - Display system performance and running processes.

---

## **DevOps Networking Guide**

### **OSI Model (Open Systems Interconnection Model)**

The **OSI model** is a conceptual framework that standardizes the functions of a networking system into **seven layers**. This model helps in designing and troubleshooting network issues by defining clear roles for each layer.

#### **Layers of the OSI Model:**

1. **Physical Layer (Layer 1):**
   - Handles the transmission of raw data bits over physical media (e.g., cables, wireless).
   - **Examples**: Ethernet, fiber optics, Wi-Fi.

2. **Data Link Layer (Layer 2):**
   - Ensures error-free data transfer between nodes on the same network.
   - Adds MAC (Media Access Control) addresses to frames for node-to-node delivery.
   - **Examples**: Ethernet, ARP.

3. **Network Layer (Layer 3):**
   - Responsible for routing and forwarding data packets between networks.
   - Uses logical addressing (IP addresses).
   - **Examples**: IPv4, IPv6, ICMP.

4. **Transport Layer (Layer 4):**
   - Ensures reliable delivery of data using protocols like **TCP** (Transmission Control Protocol) and **UDP** (User Datagram Protocol).
   - Handles flow control, segmentation, and error recovery.
   - **Examples**: TCP, UDP.

5. **Session Layer (Layer 5):**
   - Manages and maintains sessions between applications.
   - Handles session creation, management, and termination.
   - **Examples**: NetBIOS, RPC.

6. **Presentation Layer (Layer 6):**
   - Translates data between application formats and network formats (e.g., encryption, compression).
   - **Examples**: SSL/TLS, JPEG.

7. **Application Layer (Layer 7):**
   - Interfaces directly with user applications, enabling network communication.
   - **Examples**: HTTP, FTP, DNS.

---

## **IP Addressing**

An **IP address** is a unique identifier assigned to devices on a network. It helps in locating and identifying devices for communication over the internet or local networks.

### **Types of IP Addresses:**

1. **IPv4:**
   - 32-bit address (e.g., 192.168.1.1).
   - Supports up to ~4.3 billion addresses.
   - Format: Dotted-decimal notation.

2. **IPv6:**
   - 128-bit address (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
   - Supports a vast number of addresses.
   - Format: Hexadecimal.

### **Private vs Public IP:**
- **Private IP:** Used within local networks (e.g., `192.168.x.x`, `10.x.x.x`).
- **Public IP:** Globally unique and assigned by ISPs for internet-facing devices.

### **Dynamic vs Static IP:**
- **Dynamic IP:** Assigned by DHCP and changes over time.
- **Static IP:** Manually assigned and remains constant.

---

## **Ports**

A **port** is a logical endpoint that helps distinguish between different types of network traffic on the same device. Ports work in conjunction with IP addresses to route data to the correct application or process.

### **Port Categories:**

1. **Well-Known Ports (0–1023):**
   - Assigned for widely used services.
   - **Examples**:
     - HTTP: `80`
     - HTTPS: `443`
     - FTP: `21`
     - SSH: `22`

2. **Registered Ports (1024–49151):**
   - Used by software applications (e.g., database services, email).

3. **Dynamic/Private Ports (49152–65535):**
   - Assigned dynamically for temporary connections.

### **Common Port Scenarios:**
- **Firewalls and Port Forwarding:** Ensure the required ports are open to enable communication.
- **Load Balancing:** Distribute traffic to different application instances based on port numbers.

---

These topics form the foundation of networking knowledge for **DevOps engineers**. Let me know if you'd like any topic expanded further!
