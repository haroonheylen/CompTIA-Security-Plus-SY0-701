# 🛠️ Security+ PBQ Cheat Sheet (SY0-701)

This guide covers **Performance-Based Question (PBQ) scenarios** commonly seen on the Security+ exam.

PBQs test your ability to:

- Configure security tools
- Analyze logs
- Identify attacks
- Secure networks
- Troubleshoot systems

---

# 🔥 Firewall Rule Order (Common PBQ)

Firewall rules are evaluated **top-down**.

```
First match = rule applied
```

Example:

| Rule | Action |
|-----|-------|
| Allow HTTPS | Allow |
| Block All | Deny |

Traffic hitting rule 1 **never reaches rule 2**.

### Exam Trap

A **deny rule above an allow rule** will block everything.

---

# 🧱 Network Segmentation PBQs

Purpose:

- Reduce attack surface
- Prevent lateral movement

Common segmentation methods:

| Method | Description |
|------|-------------|
| VLAN | Logical network separation |
| Subnetting | Network division |
| DMZ | Public-facing servers |
| Air gap | Completely isolated system |

### Typical PBQ Task

Place servers into the correct zones:

| Zone | Typical Systems |
|----|----------------|
| Internal | Workstations |
| DMZ | Web servers |
| Secure zone | Databases |

---

# 🌐 Network Diagram Identification

You may be asked to **identify insecure components**.

Example diagram issues:

| Problem | Fix |
|------|------|
| Telnet used | Replace with SSH |
| HTTP login | Use HTTPS |
| Flat network | Segment with VLANs |
| No firewall | Add perimeter firewall |

---

# 📜 Log Analysis PBQs

Logs often reveal attacks.

### Brute Force Example

```
Failed login attempt
Failed login attempt
Failed login attempt
Account locked
```

Attack: **Password brute force**

---

### Port Scan Example

```
Connection attempt: 22
Connection attempt: 23
Connection attempt: 80
Connection attempt: 443
```

Attack: **Port scanning**

---

### Data Exfiltration Example

```
Large outbound traffic
Unknown destination IP
Outside business hours
```

Attack: **Data exfiltration**

---

# 🔍 Packet Analysis

Look for suspicious traffic.

Example packet indicators:

| Indicator | Meaning |
|---------|---------|
| Unknown protocol | Suspicious traffic |
| Repeated SYN packets | SYN flood attack |
| Large outbound transfer | Data leak |

---

# ⚠️ Attack Recognition PBQs

### Man-in-the-Middle

Indicators:

- Unexpected certificates
- Redirected traffic
- Duplicate packets

Fix:

```
Enable certificate validation
Use HTTPS
```

---

### DNS Poisoning

Symptoms:

- Users redirected to fake websites

Fix:

```
Use DNSSEC
Secure DNS servers
```

---

### ARP Spoofing

Symptoms:

- Duplicate MAC addresses
- Traffic interception

Fix:

```
Enable Dynamic ARP Inspection
```

---

# 🧪 Malware Identification

| Behavior | Malware |
|-------|--------|
| Encrypts files | Ransomware |
| Self-spreads | Worm |
| Disguised software | Trojan |
| Hidden persistence | Rootkit |

---

# 🔑 Identity & Access PBQs

You may need to **assign the correct authentication method**.

| Scenario | Solution |
|-------|--------|
| Remote employees | VPN |
| Sensitive systems | MFA |
| Internal authentication | Kerberos |
| Network devices | TACACS+ |

---

# 🧱 Access Control Placement

Typical PBQ example:

Assign correct access control.

| Role | Access |
|----|------|
| Employee | Standard user |
| Admin | Full system access |
| Contractor | Limited access |

Correct solution:

```
RBAC (Role-Based Access Control)
```

---

# 📶 Wireless Security PBQs

Typical tasks:

- Identify insecure wireless settings
- Configure secure protocols

### Correct configuration

| Setting | Secure Option |
|------|-------------|
| Encryption | WPA3 |
| Authentication | WPA2 Enterprise |
| Disable | WEP |

---

# 🔐 Encryption Selection PBQs

Match algorithm to purpose.

| Task | Best Choice |
|----|------------|
| File encryption | AES |
| Key exchange | Diffie-Hellman |
| Digital signatures | RSA |
| Password hashing | bcrypt |

---

# 🧾 Certificate Errors

Common certificate problems:

| Error | Cause |
|----|------|
| Certificate expired | Expiration date passed |
| Untrusted CA | Unknown certificate authority |
| Name mismatch | Wrong domain |

---

# ☁️ Cloud Security PBQs

You may need to assign **shared responsibility**.

| Model | Provider Responsibility |
|----|----------------|
| IaaS | Infrastructure |
| PaaS | Platform |
| SaaS | Application |

---

# 🧪 Vulnerability Scanner Output

Example report:

```
Port 23 open
Service: Telnet
```

Solution:

```
Disable Telnet
Use SSH
```

---

# 🧠 Command-Line Tools (PBQ Favorite)

| Command | Purpose |
|------|--------|
| ping | Connectivity test |
| ipconfig | Show IP configuration |
| netstat | Active connections |
| tracert | Network path |
| nslookup | DNS lookup |

---

# 📊 Security Tool Identification

| Tool | Function |
|----|--------|
| SIEM | Log aggregation |
| IDS | Detect attacks |
| IPS | Block attacks |
| DLP | Prevent data leaks |
| NAC | Network access control |

---

# 🔧 Incident Response PBQs

Correct response order:

```
Preparation
Identification
Containment
Eradication
Recovery
Lessons Learned
```

---

# 🧠 PBQ Strategy Tips

### 1️⃣ Read the Scenario First

Identify:

- What system is affected
- What attack is occurring
- What the goal is

---

### 2️⃣ Eliminate Insecure Options

Common insecure options:

- Telnet
- FTP
- WEP
- HTTP login

---

### 3️⃣ Apply Security Principles

Choose answers that follow:

- Least privilege
- Defense in depth
- Zero trust

---

# 🏁 Final PBQ Advice

PBQs often test:

- Firewall rules
- Log interpretation
- Network diagrams
- Security configuration

You don’t need **perfect commands**, just understand **how security systems work**.

---

# ⭐ Final Tip

If you're stuck on a PBQ:

1. Skip it
2. Finish multiple-choice questions
3. Return later

PBQs are **time-consuming but high value**.