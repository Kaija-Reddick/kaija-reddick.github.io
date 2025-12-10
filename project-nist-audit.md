## 📊 Incident Summary (DoS Attack)

The organization experienced a Distributed Denial of Service (DDoS) attack where all network services suddenly stopped responding. Security analysts discovered the attack was caused by a flood of ICMP packets. Internal users were unable to reach network resources for approximately two hours until the attack was mitigated.

The security team blocked the attack traffic and temporarily shut down non-critical services so that critical systems could be restored first.

---

## 🧠 CSF Function Breakdown — Using My Analysis Notes

### 🔎 Identify (ID)
- The attack targeted the network through an **unconfigured firewall** that allowed excessive ICMP traffic.
- Entire network and mission-critical systems were impacted and needed rapid recovery.

**Gap:** Lack of asset awareness and firewall configuration standards  
**Risk:** High — complete operational disruption

---

### 🔐 Protect (PR)
- New firewall configuration applied to **rate-limit ICMP packets**
- IDS/IPS deployed to filter ICMP packets with **suspicious behavior** patterns

**Improvement:** Better perimeter protections and traffic controls  
**Strength:** Faster blocking capability for future attacks

---

### 🚨 Detect (DE)
- Firewall updated with **source IP verification** to prevent spoofing
- Network monitoring software installed to alert on **abnormal traffic spikes**

**FYI:** Logging and alerting are essential for early warning  
**Improvement:** Added visibility into threat patterns

---

### 🧯 Respond (RS)
- Future responses will include **network segmentation** to isolate attack zones
- Critical system restoration prioritized
- Post-event **log analysis** identifies patterns for future prevention
- Incident reports escalated to leadership and, if needed, legal authorities

**Strength:** Defined escalation and communication flow  
**Improvement:** Faster containment and triage processes

---

### 🔁 Recover (RC)
- Critical network functions restored first
- Non-critical systems kept offline until attack traffic subsided
- Firewall rule tuning to block external ICMP floods during recovery

**Goal:** Reduce downtime + return system stability faster

---

## 🛠 Recommendations (My Final Assessment)
- Enforce firewall hardening **before** incidents occur  
- Automate **DDoS detection and blocking** at perimeter  
- Improve **asset inventory** & network segmentation  
- Run **tabletop exercises** for similar incident types

---

## 🧾 Evidence & Screenshots

📌 Screenshots of the **analysis notes** and **CSF mapping** will be added here:

> ![DoS Incident Analysis Notes](./assets/incident-note-1.png)
> *Notes describing the event, weaknesses, and NIST-aligned improvements.*
