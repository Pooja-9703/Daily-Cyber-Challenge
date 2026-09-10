# **Assignment \#4 – Understanding TCP/IP & OSI Model**

## **THEORY**

**1\. What is a network protocol?**  
    A network protocol is a set of rules that defines how devices communicate and exchange data over a network. Examples include TCP, UDP, IP, HTTP, and DNS.

**2\. What is the OSI Model?**  
    The OSI (Open Systems Interconnection) Model is a seven-layer framework used to understand how data is transmitted between devices over a network. Each layer performs a specific networking function.

**3\. Name all seven OSI layers in correct order.**  
    The seven OSI layers from Layer 7 to Layer 1 are: Application, Presentation, Session, Transport, Network, Data Link, and Physical.

**4\. What is the purpose of the Application Layer?**  
    The Application Layer is the top layer of the OSI model and provides network services directly to applications. Protocols such as HTTP, HTTPS, DNS, FTP, and SMTP operate at this layer.

**5\. What is the purpose of the Transport Layer?**  
    The Transport Layer provides end-to-end communication between devices and manages data delivery. It handles segmentation, flow control, error handling, and uses protocols such as TCP and UDP.

**6\. What is the purpose of the Network Layer?**  
    The Network Layer is responsible for logical addressing and routing data between different networks. It uses IP addresses to determine the source, destination, and path of packets.

**7\. What is the purpose of the Data Link Layer?**  
    The Data Link Layer provides communication between devices on the same local network. It uses MAC addresses and is responsible for creating frames and detecting transmission errors.

**8\. What is the purpose of the Physical Layer?**  
    The Physical Layer is responsible for transmitting raw bits over a physical medium such as Ethernet cables, fiber-optic cables, or wireless signals.

**9\. What is the TCP/IP Model?**  
    The TCP/IP Model is a networking framework used for communication over the Internet. It consists of four main layers: Application, Transport, Internet, and Network Access.

**10\. Explain the difference between OSI and TCP/IP models.**  
      The OSI Model has seven layers and is mainly used as a conceptual framework for understanding networking. The TCP/IP Model commonly has four layers and is the practical model used for Internet communication.

**11\. What is encapsulation?**  
      Encapsulation is the process of adding headers and other protocol information to data as it moves down through the network layers before being transmitted over the network.

**12\. What is decapsulation?**  
      Decapsulation is the reverse process of encapsulation, where protocol information is processed and removed as data moves up through the network layers at the receiving device.

**13\. Which layer uses IP addresses?**  
      IP addresses are used at the Network Layer (Layer 3\) to provide logical addressing and allow packets to be routed between different networks.

**14\. Which layer uses MAC addresses?**  
      MAC addresses are used at the Data Link Layer (Layer 2\) to identify devices and deliver data within a local network.

**15\. Which layer uses TCP and UDP?**  
      TCP and UDP are used at the Transport Layer (Layer 4\) to provide communication between applications running on different devices.

**16\. Which layer includes HTTP and HTTPS?**  
      HTTP and HTTPS operate at the Application Layer (Layer 7\) and are used for communication between web browsers and web servers.

**17\. Why should cybersecurity professionals understand networking layers?**  
      Understanding networking layers helps cybersecurity professionals analyze network traffic, identify suspicious connections, investigate attacks, configure security controls, and troubleshoot network-related security issues.

**18\. Explain how network data travels from a browser to a server.**  
      When a user enters a website address, the browser first uses DNS to find the server's IP address. The data then moves through the network layers, where TCP/UDP, IP addresses, and MAC addresses are added before transmission. The server receives the data, processes it through the layers, and sends a response back to the browser.

      
