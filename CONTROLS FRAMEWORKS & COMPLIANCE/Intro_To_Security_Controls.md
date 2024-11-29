# SECURITY CONTROLS

Security controls are safeguards designed to reduce specific security risks. They include a wide range of tools that protect assets before, during, and after an event.

Security controls can be organized into four primary types:
- **TECHNICAL**: These involve technologies that protect assets, such as encryption, authentication systems, firewalls, and more.
- **OPERATIONAL**: These relate to maintaining the day-to-day security environment, typically involving people to perform tasks like awareness training, incident response, and system maintenance.
- **ADMINISTRATIVE/MANAGERIAL**: These controls focus on policies, procedures, and management practices designed to guide the security program and ensure that other controls are properly implemented.
- **PHYSICAL**: These include measures to protect the physical environment and restrict unauthorized access to assets, such as locks, surveillance, and environmental controls.

## Control Types

Security controls can also be categorized by their purpose. These control types work together to provide defense in depth and protect assets:

1. **Preventative**: Designed to prevent an incident from occurring in the first place.
2. **Corrective**: Used to restore an asset after an incident.
3. **Detective**: Implemented to determine whether an incident has occurred or is in progress.
4. **Deterrent**: Designed to discourage attacks.

It’s important to note that some controls can belong to multiple categories. For example, a control might be both **technical** and **preventative**, such as a **firewall**, which is a technical tool used to prevent malicious traffic from entering a network.

Similarly, a **CCTV camera** might be both **physical** and a combination of **preventative** and **detective**, as it can deter attacks and also provide evidence in the event of an incident.

### Administrative/Managerial Controls

Administrative/Managerial controls address the human component of cybersecurity. These controls include policies and procedures that define how an organization manages data and clearly define employee responsibilities, including their role in protecting the organization. While administrative controls are typically policy-based, the enforcement of those policies may require the use of technical or physical controls.

| Control Name                  | Control Type | Control Purpose                                                                 |
|-------------------------------|--------------|---------------------------------------------------------------------------------|
| Least Privilege               | Preventative | Reduce risk and overall impact of malicious insider or compromised accounts     |
| Disaster Recovery Plans       | Corrective   | Provide business continuity                                                     |
| Password Policies             | Preventative | Reduce likelihood of account compromise through brute force or dictionary attack techniques |
| Access Control Policies       | Preventative | Bolster confidentiality and integrity by defining which groups can access or modify data |
| Account Management Policies   | Preventative | Managing account lifecycle, reducing attack surface, and limiting overall impact from disgruntled former employees and default account usage |
| Separation of Duties          | Preventative | Reduce risk and overall impact of malicious insider or compromised accounts     |

### Technical Controls

Technical controls consist of solutions such as firewalls, intrusion detection systems (IDS), intrusion prevention systems (IPS), antivirus (AV) products, encryption, etc. Technical controls can be used in a number of ways to meet organizational goals and objectives.

| Control Name                  | Control Type | Control Purpose                                                                 |
|-------------------------------|--------------|---------------------------------------------------------------------------------|
| Firewall                      | Preventative | To filter unwanted or malicious traffic from entering the network                |
| IDS/IPS                        | Detective    | To detect and prevent anomalous traffic that matches a signature or rule        |
| Encryption                    | Deterrent    | Provide confidentiality to sensitive information                                |
| Backups                       | Corrective   | Restore/recover from an event                                                  |
| Password Management           | Preventative | Reduce password fatigue                                                        |
| Antivirus (AV) Software       | Corrective   | Detect and quarantine known threats                                             |
| Manual Monitoring, Maintenance, and Intervention | Preventative | Necessary to identify and manage threats, risks, or vulnerabilities to out-of-date systems |

### Physical Controls

Physical controls include door locks, cabinet locks, surveillance cameras, badge readers, etc. They are used to limit physical access to physical assets by unauthorized personnel.

| Control Name                  | Control Type    | Control Purpose                                                                 |
|-------------------------------|-----------------|---------------------------------------------------------------------------------|
| Time-controlled Safe          | Deterrent       | Reduce attack surface and overall impact from physical threats                  |
| Adequate Lighting             | Deterrent       | Deter threats by limiting “hiding” places                                       |
| Closed-circuit Television (CCTV) | Preventative/Detective | CCTV can be both a preventative and detective control. It reduces risk and can inform after an event |
| Locking Cabinets (for Network Gear) | Preventative | Bolster integrity by preventing unauthorized personnel from accessing network infrastructure |
| Signage Indicating Alarm Service Provider | Deterrent | Deter threats by making the likelihood of a successful attack seem low          |
| Locks                         | Deterrent/Preventative | Bolster integrity by deterring and preventing unauthorized access to assets    |
| Fire Detection and Prevention (Fire Alarm, Sprinkler System, etc.) | Detective/Preventative | Detect fire and prevent damage to physical assets such as inventory, servers, etc. |

