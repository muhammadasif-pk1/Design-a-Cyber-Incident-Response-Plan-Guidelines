# Ransomware Attack Simulation

## 1. Introduction

This document presents a simulated ransomware attack against Internee.pk. The purpose of the simulation is to demonstrate how a ransomware incident can be detected, contained, investigated, eradicated, and recovered from.

The simulation is designed for cybersecurity awareness and incident-response training. It does not involve deploying or executing real ransomware.

---

# 2. Simulation Objectives

The objectives of this exercise are to:

* Demonstrate a realistic ransomware incident.
* Practice threat detection.
* Test incident escalation procedures.
* Practice containment and isolation.
* Protect organizational backups.
* Practice evidence preservation.
* Test recovery procedures.
* Train staff to respond during an emergency.
* Identify weaknesses in existing security controls.
* Develop lessons learned.

---

# 3. Attack Scenario

An employee receives a convincing phishing email that appears to come from a legitimate business contact. The message contains a malicious attachment.

The employee opens the attachment, resulting in suspicious activity on the workstation.

The security team receives endpoint alerts indicating unusual process and file activity.

Further investigation shows that the compromised workstation is attempting suspicious communication with other systems.

Later, multiple files on affected systems become inaccessible and receive unusual file extensions. A ransom note appears on the affected computers.

The incident-response team declares a critical cybersecurity incident.

---

# 4. Simulated Attack Timeline

| Stage | Simulated Activity                   | Expected Response                       |
| ----- | ------------------------------------ | --------------------------------------- |
| 1     | Employee receives phishing email     | Employee reports suspicious email       |
| 2     | Attachment is opened                 | Security monitoring generates an alert  |
| 3     | Suspicious process activity detected | Security team investigates              |
| 4     | Workstation appears compromised      | Endpoint is isolated                    |
| 5     | Suspicious account activity detected | Account is investigated and contained   |
| 6     | Multiple files are modified          | Ransomware activity suspected           |
| 7     | Ransom note appears                  | Critical incident declared              |
| 8     | Other systems are checked            | Potentially affected systems identified |
| 9     | Backups are protected and checked    | Clean recovery sources identified       |
| 10    | Compromised systems are rebuilt      | Recovery begins                         |
| 11    | Restored systems are monitored       | Security validation performed           |
| 12    | Incident is closed                   | Lessons-learned review conducted        |

---

# 5. Phase 1 — Detection

The security team receives several indicators:

* Endpoint security alerts.
* Unusual file modifications.
* Suspicious process activity.
* Unexpected network connections.
* Multiple files becoming inaccessible.
* Reports from employees about unusual computer behavior.

The security team validates the alerts and determines that the activity is consistent with a potential ransomware incident.

---

# 6. Phase 2 — Incident Declaration

Because multiple systems may be affected, the incident is classified as **Critical**.

The incident-response lead is notified.

The following actions are initiated:

* Incident-response team is activated.
* Management is notified.
* Incident documentation begins.
* A timeline is created.
* Communication procedures are activated.
* Technical containment begins.

---

# 7. Phase 3 — Containment

The immediate objective is to prevent the ransomware from spreading.

The response team:

1. Isolates affected endpoints.
2. Identifies potentially compromised systems.
3. Disables compromised accounts where necessary.
4. Restricts suspicious network communication.
5. Protects backup systems.
6. Blocks known malicious indicators.
7. Monitors unaffected systems.
8. Preserves relevant evidence.

The team avoids unnecessary actions that could destroy evidence.

---

# 8. Phase 4 — Investigation

The security team investigates the incident to determine:

* Initial entry point.
* Affected workstation.
* Compromised accounts.
* Other potentially affected systems.
* Approximate time of compromise.
* Suspicious processes.
* Network activity.
* Files affected.
* Whether sensitive information may have been accessed or stolen.

The team reviews available:

* Endpoint logs
* Authentication logs
* Email logs
* Firewall logs
* Network logs
* Security alerts
* File-system activity

---

# 9. Phase 5 — Evidence Preservation

The response team preserves relevant evidence before performing destructive recovery actions whenever practical.

Evidence may include:

* Security alerts
* System logs
* Authentication records
* Email messages
* Network records
* File metadata
* Screenshots
* System timelines

Evidence should be stored securely and access should be restricted to authorized personnel.

---

# 10. Phase 6 — Eradication

After the affected systems have been contained, the organization removes the malicious activity.

Actions include:

* Removing malware.
* Removing unauthorized access.
* Resetting compromised credentials.
* Patching affected systems.
* Rebuilding compromised machines when appropriate.
* Checking other systems for signs of compromise.
* Reviewing privileged accounts.
* Strengthening security controls.

The security team verifies that the attacker no longer has access before beginning full recovery.

---

# 11. Phase 7 — Backup Verification

Before restoring systems, the organization verifies that available backups are clean and usable.

The team checks:

* Backup availability.
* Backup integrity.
* Backup dates.
* Whether backups were affected by the incident.
* Whether restoration has been tested.
* Which backup represents the safest recovery point.

Only trusted backups should be used for recovery.

---

# 12. Phase 8 — Recovery

Recovery begins after containment and eradication.

The organization:

1. Rebuilds compromised systems.
2. Applies security patches.
3. Restores data from verified backups.
4. Resets affected credentials.
5. Re-enables required services.
6. Monitors restored systems.
7. Validates applications.
8. Confirms data availability.
9. Gradually returns systems to normal operation.

---

# 13. Phase 9 — Recovery Monitoring

After restoration, systems are continuously monitored for signs of additional compromise.

The security team checks:

* Endpoint alerts.
* Authentication activity.
* Network connections.
* File modifications.
* Privileged-account activity.
* Malware detections.
* Unusual system behavior.

If suspicious activity is detected again, the affected system is isolated and investigated.

---

# 14. Phase 10 — Incident Closure

The incident can be closed after:

* Affected systems have been recovered.
* Security controls are functioning.
* No continuing malicious activity is detected.
* Required data has been restored.
* Credentials have been secured.
* Management confirms that normal operations have resumed.

The incident-response lead completes the final incident report.

---

# 15. Staff Actions During the Simulation

Employees should follow these procedures:

### If a suspicious email is received:

* Do not click unknown links.
* Do not open suspicious attachments.
* Do not enter credentials into suspicious websites.
* Report the email to IT/security.

### If the computer behaves unusually:

* Stop interacting with suspicious files.
* Follow the organization's device-isolation instructions.
* Contact IT/security immediately.
* Do not attempt unauthorized malware removal.

### If a ransom note appears:

* Stop using the affected computer.
* Do not attempt to negotiate independently.
* Do not make unauthorized payments.
* Notify IT/security immediately.
* Follow the incident-response team's instructions.

---

# 16. Communication During the Simulation

Communication should follow the organization's escalation structure.

**Employee → IT/Security Team → Incident Response Lead → Management**

Only authorized personnel should communicate externally about the incident.

The response team should maintain a record of important decisions and communications.

---

# 17. Simulation Success Criteria

The exercise is considered successful if the organization can:

* Detect the simulated ransomware activity.
* Report the incident quickly.
* Identify affected systems.
* Isolate affected systems.
* Protect backups.
* Preserve evidence.
* Contain the simulated attack.
* Restore systems from trusted backups.
* Communicate effectively.
* Document the incident.
* Identify security improvements.

---

# 18. Lessons Learned

After the simulation, the team should review:

* How quickly the attack was detected.
* How quickly employees reported it.
* How effective endpoint monitoring was.
* Whether backups were protected.
* Whether recovery procedures worked.
* Whether communication was effective.
* Whether staff understood their responsibilities.
* Which security controls require improvement.

---

# 19. Conclusion

The ransomware simulation demonstrates the importance of preparation, rapid detection, effective containment, evidence preservation, secure backups, system recovery, and staff awareness.

Regular ransomware exercises can help Internee.pk identify weaknesses before a real incident occurs and improve the organization's ability to respond to cybersecurity emergencies.
