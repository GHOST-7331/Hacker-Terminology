# Must-Know Network Terminology for Penetration Testers

## Basic Networking Terms
- **IP Address (Internet Protocol Address)**: A unique identifier for a device on a network. It can be IPv4 (e.g., `192.168.1.1`) or IPv6 (e.g., `2001:0db8:85a3:0000:0000:8a2e:0370:7334`).
- **MAC Address (Media Access Control Address)**: A hardware address assigned to a network interface card (NIC) for unique identification within a local network.
- **Subnet**: A logical division of an IP network into smaller subnetworks. It helps with efficient IP address management and routing.
- **Gateway**: A device (typically a router) that connects different networks and routes traffic between them.
- **DNS (Domain Name System)**: The system that translates human-readable domain names (e.g., `www.example.com`) into IP addresses (e.g., `192.0.2.1`).
- **DHCP (Dynamic Host Configuration Protocol)**: A protocol that automatically assigns IP addresses to devices on a network.
- **HTTP (Hypertext Transfer Protocol)**: The protocol used for transferring web pages over the internet (port 80).
- **HTTPS (Hypertext Transfer Protocol Secure)**: A secure version of HTTP that uses encryption via SSL/TLS (port 443).
- **Ping**: A network utility used to test the reachability of a host on an IP network by sending ICMP echo requests and measuring the response time.
- **Traceroute**: A tool used to trace the path packets take from one network to another, showing the routers they pass through.

## OSI Model Overview (Layered Approach)
- **Layer 1 – Physical Layer**: The hardware layer that deals with the physical transmission of data over a medium (e.g., cables, wireless signals). Includes devices like switches and network cables.
- **Layer 2 – Data Link Layer**: Responsible for node-to-node data transfer and error correction. Common protocols include Ethernet and Wi-Fi. MAC addresses operate at this layer.
- **Layer 3 – Network Layer**: Responsible for routing packets across networks. The Internet Protocol (IP) and routing protocols like OSPF and BGP operate at this layer.
- **Layer 4 – Transport Layer**: Ensures reliable data transfer between two devices. Protocols like TCP (Transmission Control Protocol) and UDP (User Datagram Protocol) operate here.
- **Layer 5 – Session Layer**: Manages sessions or connections between applications. Handles authentication, authorization, and session maintenance.
- **Layer 6 – Presentation Layer**: Responsible for data translation, encryption, and compression. It ensures the data is in a usable format for the application.
- **Layer 7 – Application Layer**: The top layer where end-user software operates. Protocols like HTTP, FTP, DNS, and SMTP operate here, enabling communication between applications.

## Intermediate Networking Terms
- **TCP (Transmission Control Protocol)**: A connection-oriented protocol that guarantees reliable data transmission by establishing a connection between sender and receiver (e.g., web browsing, file transfers).
- **UDP (User Datagram Protocol)**: A connectionless protocol that sends data without establishing a connection, offering faster transmission at the cost of reliability (e.g., streaming, VoIP).
- **Port Scanning**: The process of scanning a device’s open ports to determine which services are running and potentially vulnerable to attacks. Tools like Nmap are commonly used.
- **ARP (Address Resolution Protocol)**: A protocol used to map an IP address to a MAC address on a local network.
- **NAT (Network Address Translation)**: A technique used by routers to modify IP address information in packet headers for routing purposes, commonly used to allow multiple devices in a private network to share a single public IP address.
- **VPN (Virtual Private Network)**: A technology that creates a secure, encrypted connection between a user’s device and a remote network, often used for secure browsing or remote access.
- **Firewall**: A network security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules.
- **Load Balancer**: A device or software that distributes incoming network traffic across multiple servers to ensure even distribution of workloads and avoid server overloads.

## Advanced Networking Terms for Penetration Testers
- **Man-in-the-Middle Attack (MitM)**: An attack where an adversary intercepts and potentially alters the communication between two parties, often through techniques like ARP spoofing or session hijacking.
- **DNS Spoofing (Cache Poisoning)**: An attack that manipulates a DNS server’s cache to redirect traffic to malicious websites.
- **IP Spoofing**: The act of sending IP packets with a fake source address to deceive the receiver into thinking the packets are from a trusted source.
- **VLAN (Virtual Local Area Network)**: A logical segmentation of a network into smaller, isolated subnets, even if the devices are physically connected to the same switch.
- **Packet Sniffing**: The act of capturing and analyzing network traffic to gather information or exploit weaknesses. Tools like Wireshark are commonly used.
- **Flood Attack**: A type of DoS (Denial of Service) attack where a large volume of traffic is sent to a target to overwhelm its resources, such as a DDoS (Distributed Denial of Service) attack.
- **Session Hijacking**: A technique where an attacker takes control of an active session between a client and a server by stealing session tokens or cookies.
- **SQL Injection (SQLi)**: A code injection attack that allows attackers to execute malicious SQL queries to manipulate a database, often resulting in unauthorized access or data manipulation.
- **IPSec (Internet Protocol Security)**: A suite of protocols that encrypts and authenticates IP packets to secure communications over IP networks, often used in VPNs.
- **BGP Hijacking**: A method of manipulating the Border Gateway Protocol to redirect traffic to an attacker-controlled network.
- **SMB (Server Message Block)**: A network file-sharing protocol used for sharing files, printers, and other network resources. SMBv1 is notoriously insecure and a target for exploitation (e.g., EternalBlue).
- **Rogue DHCP Server**: A malicious device that provides incorrect DHCP configuration information to network clients, potentially leading to man-in-the-middle attacks or network disruptions.
- **Eavesdropping**: The act of silently intercepting network traffic, often for the purpose of gathering sensitive data (e.g., passwords, unencrypted communication).
- **WEP/WPA/WPA2 (Wired Equivalent Privacy/Wi-Fi Protected Access)**: Security protocols used to secure wireless networks. WEP is outdated and vulnerable, while WPA2 provides stronger encryption.
- **802.1X**: An IEEE standard for port-based network access control that provides an authentication mechanism to devices trying to connect to a network.

## Network Penetration Testing Tools & Techniques
- **Nmap**: A powerful open-source tool for network discovery and vulnerability scanning. It can be used for port scanning, service enumeration, and OS fingerprinting.
- **Wireshark**: A network protocol analyzer that captures and inspects packets to help identify vulnerabilities or suspicious activities on a network.
- **Netcat**: A versatile networking tool used for port scanning, banner grabbing, creating backdoors, and network troubleshooting.
- **Aircrack-ng**: A suite of tools for assessing Wi-Fi network security, including cracking WEP/WPA/WPA2 passwords.
- **Metasploit**: A penetration testing framework that provides a range of exploits and payloads for attacking network services, including those vulnerable to remote code execution.
- **Hping3**: A network tool that can craft custom TCP/IP packets to perform security auditing and penetration testing, useful for DoS testing and network discovery.

## Advanced Network Security Concepts
- **Zero Trust Network**: A security model where no device, user, or system is trusted by default, and verification is required for every access request regardless of the user's location within or outside the network.
- **IDS/IPS (Intrusion Detection/Prevention System)**: Security systems that monitor network traffic for malicious activity and can alert administrators or take action to block attacks.
- **Network Segmentation**: The practice of dividing a network into smaller, isolated segments to improve security and reduce the impact of potential breaches.
- **Port Knocking**: A technique used to establish a secure connection to a server by sending a sequence of "knocks" (specific port accesses) to a closed server, which then opens the firewall.
- **DNSSEC (DNS Security Extensions)**: A set of extensions to DNS that add security by enabling DNS responses to be digitally signed, preventing DNS spoofing attacks.
- **Network Forensics**: The process of capturing, storing, and analyzing network traffic to investigate security incidents or breaches.
