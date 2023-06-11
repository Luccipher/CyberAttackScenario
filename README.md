# CyberAttackScenario
Based on the information provided, the attack appears to be a Distributed Denial of Service (DDoS) attack. A DDoS attack occurs when an attacker overwhelms a target system, such as a web server, with a flood of incoming requests, rendering it unable to respond to legitimate traffic.

Section 2: Explain how the attack is causing the website to malfunction.

In this case, the attacker is sending a large number of TCP SYN (synchronization) requests to the web server. When a client wants to establish a TCP connection with a server, it initiates a three-way handshake by sending a SYN packet. The server responds with a SYN-ACK packet, and the client acknowledges with an ACK packet, establishing the connection.

In a SYN flood attack, the attacker sends a high volume of SYN requests but does not respond to the SYN-ACK packets from the server, causing the server to keep waiting for acknowledgments that never arrive. This results in the depletion of server resources, such as memory and processing power, as it has to maintain half-open connections for each unacknowledged SYN request.

As the server becomes overwhelmed with incoming SYN requests, it reaches a point where it cannot handle any more connections, leading to a denial of service. Legitimate users trying to access the website are unable to establish connections, resulting in a connection timeout error message in their browsers.

In summary, the DDoS attack through SYN flooding is causing the website to malfunction by flooding the server with a high volume of SYN requests, overwhelming its resources and preventing it from responding to legitimate traffic.
