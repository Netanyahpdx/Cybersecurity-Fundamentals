# SECURITY CONTROLS

Security controls are safeguards designed to reduce specific security risks. They include a wide range of tools that protect assets before, during, and after an event.

Security controls can be organized into three types:
- **TECHNICAL**: Include the many technologies used to protect assets. This includes encryption, authentication systems, and others.
- **OPERATIONAL**: Relate to maintaining the day-to-day security environment. Generally, people perform these controls like awareness training and incident response.
- **MANAGERIAL**: Are centered around how the other two reduce risk.  
  - Examples of management controls:
    - Policies
    - Standards
    - Procedures

## Administrative/Managerial Controls

Administrative/Managerial controls address the human component of cybersecurity. These controls include policies and procedures that define how an organization manages data and clearly defines employee responsibilities, including their role in protecting the organization. While administrative controls are typically policy-based, the enforcement of those policies may require the use of technical or physical controls.

## Technical Controls

Technical controls consist of solutions such as firewalls, intrusion detection systems (IDS), intrusion prevention systems (IPS), antivirus (AV) products, encryption, etc. Technical controls can be used in a number of ways to meet organizational goals and objectives.

## Physical Controls

Physical controls include door locks, cabinet locks, surveillance cameras, badge readers, etc. They are used to limit physical access to physical assets by unauthorized personnel.

## Control Types

Control types include, but are not limited to:
1. **Preventative**: Designed to prevent an incident from occurring in the first place.
2. **Corrective**: Used to restore an asset after an incident.
3. **Detective**: Implemented to determine whether an incident has occurred or is in progress.
4. **Deterrent**: Designed to discourage attacks.

These controls work together to provide defense in depth and protect assets.

### Clarifying Control Categories
Security controls can be categorized in two ways:
- **By Type**: (Technical, Operational, Managerial)
  - This focuses on who or what enforces the controls (technology, people, or policies).
- **By Purpose**: (Preventative, Detective, Corrective, Deterrent)
  - This focuses on what the control is meant to achieve (prevent, detect, correct, or deter).

Controls can overlap across these categories:
- A control might be both **technical** and **preventative**, like a **firewall**, which is a technical tool used to prevent malicious traffic from entering a network.
- A **CCTV camera** might be both **physical** and **preventative/detective**, as it can deter attacks and also provide evidence in the event of an incident.

### Administrative Controls

| Control Name                  | Control Type | Control Purpose                                                                 |
|-------------------------------|--------------|---------------------------------------------------------------------------------|
| Least Privilege               | Preventative | Reduce risk and overall impact of malicious insider or compromised accounts     |
| Disaster Recovery Plans       | Corrective   | Provide business continuity                                                     |
| Password Policies             | Preventative | Reduce likelihood of account compromise through brute force or dictionary attack techniques |
| Access Control Policies       | Preventative | Bolster confidentiality and integrity by defining which groups can access or modify data |
| Account Management Policies   | Preventative | Managing account lifecycle, reducing attack surface, and limiting overall impact from disgruntled former employees and default account usage |
| Separation of Duties          | Preventative | Reduce risk and overall impact of malicious insider or compromised accounts     |

### Technical Controls

| Control Name                  | Control Type | Control Purpose                                                                 |
|-------------------------------|--------------|---------------------------------------------------------------------------------|
| Firewall                      | Preventative | To filter unwanted or malicious traffic from entering the network                 |
| IDS/IPS                        | Detective    | To detect and prevent anomalous traffic that matches a signature or rule        |
| Encryption                    | Deterrent    | Provide confidentiality to sensitive information                                |
| Backups                       | Corrective   | Restore/recover from an event                                                  |
| Password Management           | Preventative | Reduce password fatigue                                                        |
| Antivirus (AV) Software       | Corrective   | Detect and quarantine known threats                                             |
| Manual Monitoring, Maintenance, and Intervention | Preventative | Necessary to identify and manage threats, risks, or vulnerabilities to out-of-date systems |

### Physical Controls

| Control Name                  | Control Type    | Control Purpose                                                                 |
|-------------------------------|-----------------|---------------------------------------------------------------------------------|
| Time-controlled Safe          | Deterrent       | Reduce attack surface and overall impact from physical threats                  |
| Adequate Lighting             | Deterrent       | Deter threats by limiting “hiding” places                                       |
| Closed-circuit Television (CCTV) | Preventative/Detective | CCTV can be both a preventative and detective control. It reduces risk and can inform after an event |
| Locking Cabinets (for Network Gear) | Preventative | Bolster integrity by preventing unauthorized personnel from accessing network infrastructure |
| Signage Indicating Alarm Service Provider | Deterrent | Deter threats by making the likelihood of a successful attack seem low          |
| Locks                         | Deterrent/Preventative | Bolster integrity by deterring and preventing unauthorized access to assets    |
| Fire Detection and Prevention (Fire Alarm, Sprinkler System, etc.) | Detective/Preventative | Detect fire and prevent damage to physical assets such as inventory, servers, etc. |
