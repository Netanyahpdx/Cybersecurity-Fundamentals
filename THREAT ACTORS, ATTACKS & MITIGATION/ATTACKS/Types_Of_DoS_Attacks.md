## TYPES OF DoS ATTACKS
**WHAT IS A DOS ATTACK?**
<br>A Denial of Service (DoS) attack disrupts the availability of a service by overwhelming a system, network, or application with malicious traffic or requests.

### VOLUMETRIC ATTACKS:
**WHAT IT IS:** Overwhelms a network’s bandwidth with excessive traffic, rendering it unusable.
<br>**HOW IT WORKS:** Attackers flood a server or network with junk traffic (e.g., ICMP packets) to exhaust bandwidth.
<br>**EXAMPLE:** A Ping Flood sends millions of ICMP Echo requests to a server, consuming all available bandwidth.

### PROTOCOL ATTACKS:
**WHAT IT IS:** Exploits weaknesses in protocols to exhaust server resources like memory or CPU.
<br>**HOW IT WORKS:** Attackers send a flood of connection requests without completing them, causing resource exhaustion.
<br>**EXAMPLE:** SYN Flood: Sends SYN packets to initiate TCP handshakes but never completes them, leaving resources tied up.

### APPLICATION LAYER ATTACKS:
**WHAT IT IS:** Overloads specific applications or services with excessive requests.
<br>**HOW IT WORKS:** Attackers target specific URLs or APIs with fake requests that mimic legitimate traffic.
<br>**EXAMPLE:** HTTP GET Flood: Sends continuous GET requests to a web page until the server crashes.

### ICMP FLOOD / PING FLOOD:
**WHAT IT IS:** Overwhelms a target with ICMP Echo Request (ping) packets.
<br>**HOW IT WORKS:** The attacker sends a flood of ping requests to the target, which exhausts its ability to respond.
<br>**EXAMPLE:** Sending continuous pings using a script: 
<br>**INPUT:** *ping -f victim_ip_address* 
<br>**RESULT:** Network congestion and potential server unavailability.

### SLOWLORIS ATTACK:
**WHAT IT IS:** Keeps many server connections open for a long time by sending partial requests.
<br>**HOW IT WORKS:** Attackers send incomplete HTTP headers, forcing the server to wait indefinitely for the rest of the data. This exhausts connection slots.
<br>**EXAMPLE:** An attacker sends this request repeatedly:
<br>**INPUT:**
<br>*GET / HTTP/1.1*  
*Host: victim.com*
<br>**RESULT:** The web server runs out of available connections for legitimate users.

### PING OF DEATH:
**WHAT IT IS:** Sends oversized or malformed ICMP packets to crash a target system.
<br>**HOW IT WORKS:** The attacker sends an ICMP packet larger than the maximum size allowed (65,535 bytes), which can cause buffer overflows on the target.
<br>**EXAMPLE:** Using tools to craft oversized ping packets to a victim’s IP.
<br>**RESULT:** The system crashes or restarts

### TEARDROP ATTACK:
**WHAT IT IS:** Exploits vulnerabilities in how systems handle fragmented packets.
<br>**HOW IT WORKS:** Sends overlapping packet fragments that cannot be properly reassembled, leading to crashes.
<br>**EXAMPLE:** Attackers send maliciously fragmented packets like:
<br>**INPUT:**
<br>*Fragment 1: [Data 1 to 20]*  
*Fragment 2: [Data 15 to 35]*
<br>**RESULT:** The system becomes unstable and crashes.

### HTTP FLOOD:
**WHAT IT IS:** Floods a server with HTTP requests, often appearing legitimate.
<br>**HOW IT WORKS:** Attackers send a high volume of GET or POST requests to overwhelm the server. Unlike other DoS attacks, it doesn’t require a large bandwidth advantage.
<br>**EXAMPLE:** Tools like HOIC (High Orbit Ion Cannon) send fake web requests:
<br>**INPUT:**
<br>*GET /index.html HTTP/1.1*
<br>*Host: victim.com*
<br>**RESULT:** The system becomes unresponsive.

### SYN-ACK REFLECTION ATTACK
**WHAT IT IS:** A variation of SYN Flood, exploiting the TCP three-way handshake.
<br>**HOW IT WORKS:** Attackers send spoofed SYN packets with fake source IPs. When the server replies with SYN-ACK packets, it directs the response to the victim’s IP instead of the attacker.
<br>**EXAMPLE:** Victim’s server receives thousands of unsolicited SYN-ACK responses, causing exhaustion of resources.

### RESOURCE EXHAUSTION ATTACKS / RAM/CPU EXHAUSTION
**WHAT IT IS:** Overwhelms system resources by sending requests requiring intensive processing.
<br>**HOW IT WORKS:** Attackers target applications that require heavy computations (e.g., encryption processing).
<br>**EXAMPLE:** Sending multiple HTTPS requests that overload the SSL/TLS handshake process.
<br>**RESULT:** Server CPU and RAM usage spike, causing system slowdown or crash.

### UDP FLOOD ATTACK
**WHAT IT IS:** Sends a large number of UDP packets to random ports, consuming network bandwidth and server resources.
<br>**HOW IT WORKS:** The server tries to process these packets or respond with ICMP Destination Unreachable messages, leading to resource exhaustion.
<br>**EXAMPLE:** Tools like LOIC (Low Orbit Ion Cannon) can generate UDP floods.
<br>**RESULT:** Network slowdown and server unavailability.
