## TYPES OF DDoS ATTACKS

---

**WHAT IS A DDOS ATTACK?**
<br>A DDoS (Distributed Denial of Service) attack is a cyberattack where multiple compromised devices (often part of a botnet) flood a target—such as a server, network, or website—with overwhelming traffic. The goal is to exhaust the target's resources, making it unavailable to legitimate users.

<br>**WHAT IS THE DIFFERENCE BETWEEN A DoS ATTACK AND A DDoS ATTACK?**
<br> A DoS (Denial of Service) attack comes from a single source, where one system sends excessive requests or data to the target to disrupt its functionality. DDoS is distributed, using many devices to attack, making it harder to block or mitigate.
DoS is localized, easier to trace, and typically less damaging because it lacks the scale of a DDoS attack.

---

### AMPLIFICATION ATTACK:
**WHAT IT IS:** Leverages vulnerable protocols to amplify traffic sent to the target.
<br>**HOW IT WORKS:** Attackers send small requests to servers (e.g., DNS), which respond with larger replies sent to the target.
<br>**EXAMPLE:** DNS Amplification: A small query generates a large DNS response, flooding the victim.

---

### BOTNET BASED ATTACK:
**WHAT IT IS:** Uses a network of infected devices to flood a target with malicious traffic.
<br>**HOW IT WORKS:** Devices in a botnet execute commands from the attacker to send coordinated traffic.
<br>**EXAMPLE:** Mirai Botnet: Compromised IoT devices flooded Dyn’s DNS servers, disrupting major websites.

---

### NTP AMPLIFICATION ATTACK:
**WHAT IT IS:** Exploits vulnerabilities in Network Time Protocol (NTP) servers to amplify traffic directed at a victim.
<br>**HOW IT WORKS:** Attackers send small requests to NTP servers using a spoofed source IP (the victim’s IP). The servers respond with large amounts of data, overwhelming the victim.
<br>**EXAMPLE:** Using the *monlist* command, an attacker can request a server’s traffic statistics, producing a response up to 200 times larger than the request.

---

### IoT BASED DDoS:
**WHAT IT IS:** Exploits insecure IoT devices to perform large-scale DDoS attacks.
<br>**HOW IT WORKS:** Attackers infect IoT devices with malware to form a botnet. These devices then bombard the target with traffic.
<br>**EXAMPLE:** Attackers use smart thermostats and cameras to launch DDoS attacks on cloud services.

---

### HTTP / 2 FLOOD:
**WHAT IT IS:** Exploits features of the HTTP/2 protocol, such as multiplexing, to overload servers.
<br>**HOW IT WORKS:** Attackers send many small, seemingly legitimate requests simultaneously, which the server struggles to handle.
<br>**EXAMPLE:** A single client opens numerous streams within one connection, each making small data requests, overwhelming the server.

---

### SMURF ATTACK:
**WHAT IT IS:** Amplifies traffic by using broadcast addresses to flood the victim with ICMP replies.
<br>**HOW IT WORKS:** Attackers send ICMP Echo requests to a broadcast address with a spoofed source IP (the victim’s IP). All devices on the network reply to the victim, creating a flood of traffic.
<br>**EXAMPLE:** A request sent to *192.168.0.255* (broadcast address) causes all devices in the subnet to send replies to the victim.

---

### APPLICATION LAYER DDoS (SLOW POST / SLOWLORIS):
**WHAT IT IS:** Targets specific applications rather than the entire network.
<br>**HOW IT WORKS:** Attackers send slow, partial HTTP POST requests to tie up server threads. Legitimate traffic is blocked as the server struggles to process the incomplete requests.
<br>**EXAMPLE:** Sending POST headers one byte at a time:
<br>**INPUT:** 
<br>*POST /login HTTP/1.1*
<br>*Host: victim.com*
<br>*Content-Length: 10000*
<br>**RESULT:** This keeps the server waiting indefinitely for the full data.

---

### DNS FLOODING:
**WHAT IT IS:** Overwhelms a DNS server with requests, making it unable to resolve domain names for legitimate users.
<br>**HOW IT WORKS:** Attackers send massive numbers of DNS queries for random subdomains (NXDOMAIN flood) or repeatedly request legitimate domains to overload the server.
<br>**EXAMPLE:** Querying *random123.example.com* repeatedly, which doesn’t exist, forcing the DNS server to search for a response each time.

---

### RUDY (R-U-DEAD-YET?) ATTACK:
**WHAT IT IS:** Targets web forms by sending very slow form field submissions. 
<br>**HOW IT WORKS:** Attackers open a connection and send form data one byte at a time. The server stays engaged with the slow connection, consuming resources.
<br>**EXAMPLE:** Sending slow requests to a login form, blocking other users from submitting legitimate credentials.

---

### REFLECTION BASED DDoS ATTACK:
**WHAT IT IS:** Uses legitimate servers to reflect and amplify attack traffic to a victim.
<br>**HOW IT WORKS:** Spoofed requests are sent to servers (e.g., DNS, NTP, or SNMP), which respond to the victim’s IP with amplified data.
<br>**EXAMPLE:** Using open SNMP servers to amplify a single request into hundreds of packets directed at the victim.

---

### IoT-BASED DDoS (ZOMBIE DEVICES):
**WHAT IT IS:** Harnesses insecure IoT devices to form a botnet, launching attacks on targets.
<br>**HOW IT WORKS:** Malware infects IoT devices (e.g., smart cameras, thermostats), and they send coordinated requests to overwhelm the target.
<br>**EXAMPLE:** The Mirai Botnet infected millions of IoT devices, launching attacks that took down major platforms like DynDNS in 2016.

---

### (SSDP) SIMPLE SERVICE DISCOVERY PROTOCOL AMPLIFICATON:
**WHAT IT IS:** Exploits the SSDP protocol used in UPnP devices for amplification attacks.
<br>**HOW IT WORKS:** Attackers send SSDP queries with a spoofed source IP. The devices respond with large payloads to the victim.
<br>**EXAMPLE:** A single query to a UPnP device generates 30-40 times the response size, overwhelming the victim’s network.
