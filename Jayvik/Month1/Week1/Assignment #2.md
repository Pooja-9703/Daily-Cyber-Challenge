# **Assignment \#2 \- Understanding My Network**

## **THEORY**

### **1\. What is a computer network?**  
 	   A computer network is a group of interconnected devices that communicate with each other to share data, resources, and services.

### **2\. What is the difference between a client and a server?**  
     A client is a device or application that requests a service or resource. A server is a device or application that provides the requested service or resource.

### **3\. What is a LAN?**  
     A Local Area Network (LAN) connects devices within a small geographical area, such as a home, office, school, or building.

### **4\. What is a WAN?**  
    A Wide Area Network (WAN) connects networks across a large geographical area. The Internet is the largest example of a WAN.

### **5\. What is the purpose of a switch?**  
    A switch connects multiple devices within a LAN and forwards data to the correct device using MAC addresses.

### **6\. What is the purpose of a router?**  
    A router connects different networks and forwards data packets between them using IP addresses.

### **7\. What is a firewall?**  
     A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predefined security rules.

### **8\. What is an IP address?**  
    An IP address is a logical address assigned to a device on a network. It allows devices to be identified and communicate with each other.

### **9\. What is a MAC address?**  
    A MAC address is a unique hardware-level address associated with a network interface. It is mainly used for communication within a local network.

### **10\. What is a default gateway?**  
      A default gateway is usually a router that a device uses to communicate with devices outside its local network.

### **11\. What is DNS?**  
      DNS (Domain Name System) translates human-readable domain names, such as google.com, into IP addresses that computers can use to communicate.

### **12\. Why is networking knowledge important for cybersecurity?**  
      Networking knowledge helps cybersecurity professionals understand network traffic, identify suspicious connections, detect attacks, secure systems, and investigate security incidents.

---

## **YOUR NETWORK INFORMATION**

This section explains how to find the required network information on both Windows and Linux.

### 13. Private IPv4 Address

A **private IPv4 address** identifies a device within a local or private network.

#### Windows

Use the following command:

    ipconfig

For detailed network information:

    ipconfig /all

#### Linux

Use:

    ip addr

### 14. Default Gateway

A **default gateway** is normally the router that a computer uses to communicate with devices outside its local network.

#### Windows

Use:

    ipconfig

#### Linux

Use:

    ip route

### 15. DNS Server

A **DNS (Domain Name System) server** translates domain names such as `google.com` into IP addresses.

#### Windows

Use:

    ipconfig /all

#### Linux

Use:

    resolvectl status

---

## COMMANDS

### 1. IP Configuration

#### Windows

    ipconfig

For detailed information:

    ipconfig /all

#### Linux

    ip addr

##### What it does

These commands display network configuration information such as:

- IPv4 addresses
- IPv6 addresses
- Network interfaces
- Default gateway
- DNS information
- MAC addresses

---

### 2. Ping

`ping` is available on both Windows and Linux.

#### Windows

    ping 8.8.8.8

#### Linux

    ping 8.8.8.8

##### What it does

`ping` tests whether a destination is reachable over a network.

It sends ICMP Echo Request packets and waits for responses.

Example:

    Reply from 8.8.8.8: bytes=32 time=20ms TTL=117

A successful response indicates that the destination responded to the request.

`ping` can be useful for:

- Testing network connectivity
- Troubleshooting network problems
- Checking whether a host is reachable
- Basic network reconnaissance

---

### 3. Tracert

#### Windows

    tracert 8.8.8.8

#### Linux 

    traceroute 8.8.8.8

If `traceroute` is unavailable, another option is:

    tracepath 8.8.8.8

##### What it does

`tracert` and `traceroute` show the network path between a computer and a destination.

Example:

    1    192.168.1.1
    2    ...
    3    ...
    4    8.8.8.8

Each hop generally represents a router or other Layer 3 device along the path.

Traceroute can help with:

- Understanding network paths
- Troubleshooting connectivity
- Identifying routing problems
- Understanding network infrastructure

---
