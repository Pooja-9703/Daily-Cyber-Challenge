# **Assignment \#5 – Understanding TCP/IP & OSI Model**

## THEORY

**1. What is Ethernet?**
    Ethernet is a widely used networking technology for connecting devices over a wired Local Area Network (LAN). It defines how data is transmitted between devices using cables and Ethernet frames.

**2. What is an Ethernet frame?**
    An Ethernet frame is a unit of data used at the Data Link Layer to transmit information across a local network. It contains information such as source and destination MAC addresses, data, and error-checking information.

**3. What is a MAC address?**
    A MAC address is a unique hardware address assigned to a network interface. It is used to identify a device or network interface during communication on a local network.

**4. What does MAC stand for?**
    MAC stands for **Media Access Control**. It refers to the addressing system used at the Data Link Layer for communication within a local network.

**5. Difference between a MAC address and an IP address?**
    A MAC address is used for communication within a local network, while an IP address is used for logical addressing and communication between different networks. MAC addresses operate at Layer 2, while IP addresses operate at Layer 3.

**6. What is a MAC Address Table?**
    A MAC Address Table is a table maintained by a network switch that maps MAC addresses to specific switch ports. It helps the switch determine where to forward Ethernet frames.

**7. How does a switch learn MAC addresses?**
    A switch learns MAC addresses by examining the **source MAC address** of incoming Ethernet frames. It records the source MAC address along with the port on which the frame was received.

**8. What is a source MAC address?**
    The source MAC address identifies the network interface that originally sent the Ethernet frame. A switch uses it to learn where that device is located on the network.

**9. What is a destination MAC address?**
    The destination MAC address identifies the network interface that should receive the Ethernet frame. A switch uses this address to determine where the frame should be forwarded.

**10. What is an unknown unicast frame?**
    An unknown unicast frame is an Ethernet frame whose destination MAC address is not present in the switch's MAC Address Table. The switch does not know which port leads to the destination.

**11. What is flooding?**
    Flooding is the process of forwarding an Ethernet frame out of multiple switch ports when the destination MAC address is unknown. The frame is normally sent to all relevant ports except the port where it was received.

**12. What is known unicast forwarding?**
    Known unicast forwarding occurs when a switch knows the destination MAC address and its associated port. The switch forwards the frame only through that specific port.

**13. At which OSI layer does Ethernet switching primarily operate?**
    Ethernet switching primarily operates at the **Data Link Layer (Layer 2)** of the OSI model, where switches use MAC addresses to forward Ethernet frames.

**14. Why does a switch maintain a MAC Address Table?**
    A switch maintains a MAC Address Table to efficiently forward frames to the correct port instead of sending them to every connected device. This reduces unnecessary network traffic.

**15. Why is Ethernet knowledge important in cybersecurity?**
    Understanding Ethernet helps cybersecurity professionals analyze local network traffic, understand MAC addresses and frames, detect suspicious network activity, investigate attacks such as MAC spoofing, and understand how switches forward traffic.

---

## Command

The `getmac` command is a Windows command used to display the **MAC (Media Access Control) addresses** of network adapters available on the system.

### Example Output

    Physical Address    Transport Name
    =================   =================================
    XX-XX-XX-XX-XX-XX   \Device\Tcpip_{...}

### Information Provided

- **Physical Address:** The MAC address of the network adapter.
- **Transport Name:** The system identifier associated with the network interface.

### Why It Is Useful

`getmac` can be used to:

- Identify network interfaces and their MAC addresses.
- Verify the MAC address of a network adapter.
- Troubleshoot network configuration.
- Support network inventory and security investigations.
