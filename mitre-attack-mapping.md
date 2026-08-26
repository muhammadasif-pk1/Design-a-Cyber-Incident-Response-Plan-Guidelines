# MITRE ATT&CK Mapping

## 1. Introduction

The MITRE ATT&CK framework provides a knowledge base of adversary tactics and techniques based on real-world observations. It can be used to understand attacker behavior and improve cybersecurity detection and response.

This document maps the activities in the simulated ransomware incident to relevant MITRE ATT&CK tactics and techniques.

---

# 2. Attack Scenario Mapping

| Attack Activity                 | MITRE ATT&CK Tactic | Technique                              | Technique ID |
| ------------------------------- | ------------------- | -------------------------------------- | ------------ |
| Phishing email                  | Initial Access      | Phishing                               | T1566        |
| Malicious attachment            | Initial Access      | Phishing: Spearphishing Attachment     | T1566.001    |
| User opens malicious attachment | Execution           | User Execution                         | T1204        |
| Malicious software executes     | Execution           | Command and Scripting Interpreter      | T1059        |
| System information gathering    | Discovery           | System Information Discovery           | T1082        |
| Network information gathering   | Discovery           | System Network Configuration Discovery | T1016        |
| Credential-related activity     | Credential Access   | OS Credential Dumping                  | T1003        |
| Access to another system        | Lateral Movement    | Remote Services                        | T1021        |
| Files encrypted                 | Impact              | Data Encrypted for Impact              | T1486        |
| Recovery mechanisms targeted    | Impact              | Inhibit System Recovery                | T1490        |

---

# 3. Initial Access

## Technique: Phishing

**MITRE ATT&CK ID:** T1566

The simulated attack begins with a phishing email sent to an employee.

The attacker attempts to convince the employee to interact with a malicious message.

### Detection Opportunities

Security teams can detect phishing through:

* Email security systems.
* Suspicious sender analysis.
* Malicious attachment detection.
* URL reputation checks.
* User reports.
* Email gateway logs.

### Defensive Measures

* Employee phishing awareness training.
* Email filtering.
* Attachment scanning.
* Link protection.
* Multi-factor authentication.
* User reporting mechanisms.

---

# 4. Spearphishing Attachment

## Technique: T1566.001

The simulated attacker uses a malicious attachment to gain initial access.

The employee opens the attachment, allowing suspicious activity to begin.

### Detection Opportunities

* Email security alerts.
* Attachment scanning.
* Endpoint detection alerts.
* Suspicious process creation.
* Unusual application behavior.

### Defensive Measures

* Block dangerous attachment types where appropriate.
* Use email sandboxing.
* Train employees.
* Restrict unnecessary execution of downloaded files.
* Deploy endpoint protection.

---

# 5. User Execution

## Technique: T1204

The attacker relies on the employee to interact with the malicious content.

This demonstrates the importance of employee cybersecurity awareness.

### Detection Opportunities

* Endpoint process monitoring.
* Application execution logs.
* EDR alerts.
* Suspicious child processes.

### Defensive Measures

* Security awareness training.
* Application control.
* Endpoint protection.
* Least-privilege access.

---

# 6. Command and Scripting Interpreter

## Technique: T1059

In the simulated scenario, suspicious command or scripting activity may occur after the initial compromise.

Security monitoring should identify unexpected command-line activity, especially when it originates from unusual applications or user contexts.

### Detection Opportunities

* Command-line logging.
* Endpoint detection.
* Process monitoring.
* Script execution monitoring.

### Defensive Measures

* Restrict unnecessary scripting capabilities.
* Monitor administrative activity.
* Apply least privilege.
* Use endpoint detection and response.

---

# 7. System Information Discovery

## Technique: T1082

An attacker may attempt to identify information about the compromised computer.

Examples include:

* Operating system information.
* Computer name.
* System configuration.
* Installed software.

### Detection Opportunities

Security teams should monitor unusual discovery activity, particularly when combined with other suspicious behavior.

---

# 8. System Network Configuration Discovery

## Technique: T1016

An attacker may attempt to identify network configuration and connected network information.

This information can help an attacker understand the environment.

### Defensive Measures

* Network monitoring.
* Segmentation.
* Endpoint monitoring.
* Least-privilege access.

---

# 9. OS Credential Dumping

## Technique: T1003

The simulated attacker may attempt to obtain credentials from a compromised system.

Credential theft can allow an attacker to access additional resources.

### Detection Opportunities

* EDR alerts.
* Authentication monitoring.
* Privileged-account monitoring.
* Suspicious access to credential stores.

### Defensive Measures

* Multi-factor authentication.
* Credential protection.
* Least privilege.
* Privileged access management.
* Strong authentication controls.

---

# 10. Remote Services

## Technique: T1021

An attacker may attempt to move from one compromised system to another using available remote services.

### Detection Opportunities

* Unusual authentication patterns.
* Unexpected remote connections.
* Lateral movement alerts.
* Network monitoring.

### Defensive Measures

* Network segmentation.
* Restrict remote services.
* MFA.
* Strong access controls.
* Monitor administrative connections.

---

# 11. Data Encrypted for Impact

## Technique: T1486

This is the primary impact technique in the ransomware simulation.

The attacker encrypts files to prevent legitimate users from accessing them.

### Detection Opportunities

Indicators can include:

* Large numbers of file modifications.
* Rapid file renaming.
* Unusual file extensions.
* High-volume file activity.
* Endpoint security alerts.
* Ransom notes.

### Defensive Measures

* Secure backups.
* Endpoint protection.
* File activity monitoring.
* Network segmentation.
* Least privilege.
* Rapid endpoint isolation.

---

# 12. Inhibit System Recovery

## Technique: T1490

Attackers may attempt to prevent an organization from recovering systems after ransomware activity.

### Detection Opportunities

Security teams should monitor unexpected changes to:

* Backup systems.
* Recovery mechanisms.
* System recovery configurations.

### Defensive Measures

* Offline or isolated backups.
* Restricted backup administration.
* Backup monitoring.
* Regular restoration testing.
* Separate backup credentials.

---

# 13. MITRE ATT&CK Attack Chain

The simulated attack can be summarized as:

```text
Phishing
   ↓
Spearphishing Attachment
   ↓
User Execution
   ↓
Suspicious Command/Script Activity
   ↓
System Discovery
   ↓
Credential Access
   ↓
Lateral Movement
   ↓
Data Encryption
   ↓
Impact
```

---

# 14. Defensive Detection Strategy

The MITRE ATT&CK mapping can be used to improve defensive monitoring.

| ATT&CK Area         | Defensive Monitoring                  |
| ------------------- | ------------------------------------- |
| Phishing            | Email security and user reporting     |
| User Execution      | Endpoint monitoring                   |
| Command Execution   | Process and command-line logging      |
| Discovery           | Endpoint and network monitoring       |
| Credential Access   | Authentication and EDR monitoring     |
| Lateral Movement    | Network and authentication monitoring |
| Data Encryption     | File activity monitoring              |
| Recovery Inhibition | Backup monitoring                     |

---

# 15. Conclusion

Mapping the ransomware simulation to MITRE ATT&CK helps Internee.pk understand how an attacker may progress through different stages of an intrusion.

The mapping also provides opportunities to identify defensive controls and monitoring requirements at each stage of the attack.

By combining MITRE ATT&CK with incident-response procedures, Internee.pk can improve threat detection, containment, investigation, and recovery capabilities.
