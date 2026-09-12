# **Assignment \#6 – Understanding IPv4 Addressing**

**THEORY**

**1\. What is IPv4?**  
      IPv4 (Internet Protocol version 4\) is a protocol used to identify devices on a network and route data between them using IP addresses.

**2\. How many bits are in an IPv4 address?**  
      An IPv4 address contains 32 bits, divided into four 8-bit sections called octets.

**3\. What is an octet?**  
      An octet is a group of 8 bits in an IPv4 address. Each octet can have a value from 0 to 255\.

**4\. How many octets are in an IPv4 address?**  
      An IPv4 address contains four octets, written in decimal form and separated by periods, such as 192.168.1.10.

**5\. What is a subnet mask?**  
      A subnet mask is used to determine which part of an IP address represents the network and which part represents the host. For example, 255.255.255.0 is a common subnet mask.

**6\. Difference between network portion and host portion?**  
     The network portion identifies the network, while the host portion identifies a specific device within that network. The subnet mask determines which bits belong to each portion.

**7\. What is a private IPv4 address?**  
      A private IPv4 address is an IP address reserved for use within private networks such as home, office, and internal networks. Private addresses are not directly routable on the public Internet.

**8\. Write all three private IPv4 ranges.**  
      The three private IPv4 ranges are 10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16.

**9\. What is a public IPv4 address?**  
      A public IPv4 address is an address that can be routed across the Internet and is typically assigned to an Internet-connected device or network by an Internet service provider.

**10\. What is the IPv4 loopback address?**  
       The IPv4 loopback range is 127.0.0.0/8, with 127.0.0.1 being the most commonly used loopback address. It allows a device to communicate with itself.

**11\. What is APIPA?**  
       APIPA (Automatic Private IP Addressing) is a feature that automatically assigns a device an IPv4 address when it cannot obtain an address from a DHCP server.

**12\. What does 169.254.x.x commonly indicate?**  
       An address in the 169.254.0.0/16 range commonly indicates that the device could not obtain an IPv4 address from a DHCP server and assigned itself an APIPA address.

**13\. What is a default gateway?**  
       A default gateway is the device, usually a router, that forwards traffic from a local network to other networks. It is commonly used when the destination is outside the local network.

**14\. Static vs dynamic IP addressing?**  
       A static IP address is manually configured and normally remains fixed, while a dynamic IP address is automatically assigned, usually by a DHCP server, and may change over time.

**15\. What is DHCP?**  
       DHCP (Dynamic Host Configuration Protocol) automatically provides network configuration information to devices, such as an IP address, subnet mask, default gateway, and DNS server.

**16\. What is a network address?**  
       A network address identifies a network or subnet rather than an individual host. It is the first address in a subnet and cannot normally be assigned to a host.

**17\. What is a broadcast address?**  
       A broadcast address is used to send data to all hosts on a particular IPv4 subnet. It is normally the last address in the subnet and cannot normally be assigned to a host.

**18\. Why is IPv4 knowledge important in cybersecurity?**  
       Understanding IPv4 helps cybersecurity professionals analyze network traffic, identify hosts and networks, investigate suspicious IP addresses, understand routing, configure firewalls, perform network reconnaissance, and investigate security incidents.
