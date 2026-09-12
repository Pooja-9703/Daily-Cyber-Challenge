# **Assignment \#7 – IPv4 Addressing Pt.2 & IP Configuration**

## **THEORY**

**1\. What is a network address?**  
    A network address identifies a specific network or subnet rather than an individual device. It is the first address in a subnet and is reserved for identifying the network.

**2\. What is a broadcast address?**  
    A broadcast address is used to send data to all devices within a particular subnet. It is normally the last address in the subnet.

**3\. What is a usable host address?**  
    A usable host address is an IP address within a subnet that can be assigned to a device such as a computer, server, or router interface.

**4\. What is the first usable IP address?**  
    The first usable IP address is the address immediately after the network address. For example, in 192.168.1.0/24, the first usable address is 192.168.1.1.

**5\. What is the last usable IP address?**  
    The last usable IP address is the address immediately before the broadcast address. For example, in 192.168.1.0/24, the last usable address is 192.168.1.254.

**6\. What does /24 mean?**  
    /24 is CIDR notation indicating that the first 24 bits of an IPv4 address represent the network portion, leaving 8 bits for the host portion.

**7\. What subnet mask corresponds to /24?**  
    The subnet mask corresponding to  /24 is 255.255.255.0.

**8\. What is a default gateway?**  
    A default gateway is usually a router interface that forwards traffic from a local network to other networks when the destination is outside the local subnet.

**9\. Why does a router interface need an IP address?**  
    A router interface needs an IP address to provide logical addressing and communicate with devices on its connected network. It also allows the router to route traffic between different networks.

**10\. What is a static IP configuration?**  
    A static IP configuration is a network configuration where the IP address, subnet mask, gateway, and other settings are manually assigned and remain fixed unless changed by an administrator.

**11\. What does "show ip interface brief" display?**  
    “show ip interface brief” is a Cisco IOS command that provides a summary of router interfaces, including their interface names, assigned IP addresses, and status.

**12\. What does "no shutdown" do conceptually on a Cisco interface?**  
    The “no shutdown” command administratively enables a Cisco interface, allowing it to become operational if the physical connection and other required conditions are working.

**13\. What does interface status "up/up" generally indicate?**  
    An up/up interface generally indicates that the interface is administratively enabled and its physical/data-link connection is operational.

**14\. Why should network configuration always be verified?**  
    Network configuration should be verified to ensure that IP addresses, interfaces, gateways, and other settings are correct and to identify configuration errors that could cause connectivity or security problems.

**15\. Why is IPv4 configuration important in cybersecurity?**  
    Understanding IPv4 configuration helps cybersecurity professionals identify hosts and networks, analyze traffic, understand routing, configure security controls, perform network reconnaissance, and investigate suspicious network activity.
