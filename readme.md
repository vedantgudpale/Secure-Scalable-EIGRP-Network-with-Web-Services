# Secure & Scalable EIGRP Network with Web Services

## Project Overview

This Cisco Packet Tracer project demonstrates the design and implementation of a secure and scalable enterprise-class network using Enhanced Interior Gateway Routing Protocol (EIGRP) with route summarization and MD5 authentication. The network simulates a small business or organization network, featuring:

*   **Multiple Departments:** Simulated by separate PC networks, representing different departments or office locations.
*   **Centralized Server Farm:** Providing essential network services including DNS, DHCP, and Web services.
*   **Robust Backbone:** A redundant ring topology backbone infrastructure using EIGRP for efficient and resilient routing.
*   **Simulated Web Presence:** Custom-designed websites, including a personalized portfolio site ("Bedge.in"), to showcase web service integration.

## Network Topology

**Devices Used:**

*   **Routers (6):** Cisco ISR 4331 Integrated Services Routers (R1, R2, R3, R4, R5, R6)
*   **Switches (6):** Cisco Catalyst 2960 Series Switches (SW-PC1, SW-PC2, SW-PC3, SW-PC4, SW-PC5, SW-Server)
*   **PCs (30):** Generic PCs, 6 connected to each PC Switch
*   **Servers (4):** Generic Servers (DNS-Server, Web-Server (www.cisco.com), Web-Server-2 (www.bedge.in), DHCP-Server, Email-Server - Email-Server is present but not fully configured in this version for simplicity)

**Interface Connections (Key Backbone Links):**

*   R1: Gig0/0/0 <--> R2: Gig0/0/0
*   R2: Gig0/0/1 <--> R3: Gig0/0/0
*   R3: Gig0/0/1 <--> R4: Gig0/0/0
*   R4: Gig0/0/1 <--> R5: Gig0/0/0
*   R5: Gig0/0/1 <--> R6: Gig0/0/0
*   R6: Gig0/0/1 <--> R1: Gig0/0/1

## Concepts Demonstrated

This project demonstrates the following key networking concepts and technologies:

*   EIGRP Dynamic Routing: Implemented EIGRP for automatic route discovery and maintenance within the network.
*   Route Summarization: Configured manual route summarization to aggregate PC network routes and simplify routing tables, enhancing scalability.
*   EIGRP MD5 Authentication: Secured EIGRP routing updates using MD5 authentication to prevent route manipulation and enhance network security.
*   DHCP (Dynamic Host Configuration Protocol): Centralized DHCP server and relay configuration for efficient IP address management and automatic client configuration.
*   DNS (Domain Name System): Implemented a DNS server to resolve domain names (www.cisco.com, www.bedge.in) to IP addresses, enabling user-friendly access to web services.
*   Simulated Web Services: Simulated functional web services using Packet Tracer's built-in web server capabilities, including custom-designed webpages and a dark mode toggle feature.
*   Redundant Network Topology: Utilized a ring topology for the router backbone to provide path redundancy and improve network resilience.
*   Enterprise-Class Network Design Principles: Applied principles of hierarchical network design, scalability, and security in a simulated enterprise environment.

## Website Simulation

The project includes two simulated websites hosted on Packet Tracer web servers:

*   **www.cisco.com (Web-Server-1):** A professionally designed webpage simulating a corporate website, featuring a light and dark mode toggle and basic content structure.
*   **www.bedge.in (Web-Server-2):** A personalized portfolio/landing page showcasing author profile information (Vedant Gudpale), links to LinkedIn and GitHub profiles, and a simulated search box. The "Bedge.in" website is designed with a visually appealing dark mode theme and a functional dark mode toggle button.

## Accessing the Simulated Websites

To access the simulated websites from within the Packet Tracer network:

1.  **Power on all devices** in the Packet Tracer simulation.
2.  **Wait for network convergence:** Allow time for EIGRP routing to converge and DHCP to assign IP addresses (indicated by green port lights and successful pings).
3.  **Open a web browser on any PC** (e.g., PC1, PC7, PC15, etc.).
4.  **In the web browser's URL address bar, type the domain name of the desired website:**
    *   For Cisco Simulated Website: `www.cisco.com`
    *   For Bedge.in Personalized Website: `www.bedge.in`
5.  **Click "Go" or press Enter.** The corresponding simulated website should load in the web browser window.
6.  **For Bedge.in, test the "Search" button and the "Dark Mode" toggle button to verify their functionality.


## Further Enhancements (Optional)

This project can be further enhanced and expanded upon. Some potential enhancements include:

*   Implementing VLANs and Inter-VLAN Routing to further segment the network.
*   Adding more diverse server services, such as a fully functional Email Server, FTP Server, or a Database Server to create a more comprehensive simulated business environment.
*   Implementing Access Control Lists (ACLs) on routers and switches to filter traffic based on various criteria and enhance network security.
*   Configuring Quality of Service (QoS) policies to prioritize certain types of traffic, such as voice or video, to simulate real-world network traffic management.
*   Exploring integration with a real web server hosted outside of Packet Tracer using port forwarding or other techniques (for advanced users) to test web services in a more realistic scenario.
*   Adding network monitoring and management tools within Packet Tracer, such as Syslog server or SNMP, to simulate network management practices.
*   Implementing IPv6 addressing and routing alongside IPv4 to explore dual-stack network configurations and prepare for IPv6 adoption.
*   Extending the network topology to simulate a larger enterprise network with multiple branches or geographical locations, further testing EIGRP scalability and summarization capabilities.

## Author:

**Vedant Gudpale**

**Enthusiastic about Network Security and Cybersecurity.**

*   LinkedIn: https://www.linkedin.com/in/vedantgudpale
*   GitHub: https://github.com/vedantgudpale


**Disclaimer**
*   This project serves as a foundational example of a client-server web network built and simulated within Packet Tracer, suitable for educational purposes and demonstrating basic networking principles.


