# 🛡️ CompTIA Security+ (SY0-701) Ultimate Exam Cheat Sheet

A **comprehensive quick-reference** for the most important Security+ concepts, including **common exam traps**.

Use this for:
- Rapid revision
- Practice exam review
- Final exam-day cram

---

# 🌐 Common Network Ports

| Protocol | Port | Notes |
|--------|------|------|
| FTP | 20/21 | File transfer |
| SSH | 22 | Secure remote login |
| Telnet | 23 | Insecure remote login |
| SMTP | 25 | Email sending |
| DNS | 53 | Domain name resolution |
| DHCP | 67/68 | IP assignment |
| TFTP | 69 | Lightweight file transfer |
| HTTP | 80 | Web traffic |
| POP3 | 110 | Email retrieval |
| NTP | 123 | Time sync |
| IMAP | 143 | Email retrieval |
| SNMP | 161 | Network management |
| SNMP Trap | 162 | SNMP alerts |
| LDAP | 389 | Directory services |
| HTTPS | 443 | Secure web traffic |
| SMB | 445 | Windows file sharing |
| Syslog | 514 | Logging |
| LDAPS | 636 | Secure LDAP |
| FTPS | 989/990 | Secure FTP |
| RDP | 3389 | Remote desktop |

### ⚠️ Exam Trap

Know the **secure versions**:

| Insecure | Secure |
|--------|--------|
| HTTP | HTTPS |
| Telnet | SSH |
| FTP | FTPS / SFTP |
| LDAP | LDAPS |

---

# 🔐 Encryption & Cryptography

## Symmetric Encryption

Fast encryption using **one shared key**.

| Algorithm | Notes |
|---------|------|
| AES | Current standard |
| DES | Deprecated |
| 3DES | Legacy |
| Blowfish | Fast cipher |
| Twofish | AES alternative |

### Exam Tip

AES key sizes:

```
AES-128
AES-192
AES-256
```

---

## Asymmetric Encryption

Uses **public/private keys**.

| Algorithm | Purpose |
|---------|---------|
| RSA | Key exchange |
| ECC | Modern lightweight crypto |
| Diffie-Hellman | Secure key exchange |
| ElGamal | Public key encryption |

### ECC Exam Trap

ECC provides **same security with smaller keys**.

---

## Hashing Algorithms

| Algorithm | Status |
|---------|------|
| MD5 | Broken |
| SHA-1 | Weak |
| SHA-256 | Secure |
| SHA-512 | Strong |
| bcrypt | Password hashing |

---

# 🔑 Authentication Methods

## Authentication Factors

| Factor | Example |
|------|---------|
| Something you know | Password |
| Something you have | Smart card |
| Something you are | Biometrics |
| Somewhere you are | GPS |
| Something you do | Typing pattern |

### Exam Trap

**MFA requires different factor categories**, not just multiple passwords.

---

## Authentication Protocols

| Protocol | Use |
|--------|------|
| Kerberos | Ticket-based authentication |
| RADIUS | Remote authentication |
| TACACS+ | Network device authentication |
| LDAP | Directory services |
| SAML | Web SSO |
| OAuth | Authorization |
| OpenID Connect | Authentication layer |

---

# 📶 Wireless Security

| Protocol | Security Level |
|--------|---------------|
| WEP | Broken |
| WPA | Weak |
| WPA2 | Strong |
| WPA3 | Strongest |

### Exam Trap

```
WPA3 uses SAE instead of PSK
```

SAE = Simultaneous Authentication of Equals

---

# 🧠 Access Control Models

| Model | Description |
|------|-------------|
| DAC | Owner controls permissions |
| MAC | System enforces permissions |
| RBAC | Role-based access |
| ABAC | Attribute-based access |

### Exam Tip

```
RBAC = job roles
ABAC = dynamic attributes
```

---

# 🧱 Security Architecture

## Firewalls

| Type | Purpose |
|----|------|
| Packet filtering | Basic filtering |
| Stateful | Tracks connections |
| Proxy firewall | Application layer |
| NGFW | Advanced inspection |

---

## Network Security Tools

| Tool | Function |
|----|-----------|
| IDS | Detect attacks |
| IPS | Block attacks |
| SIEM | Log analysis |
| SOAR | Automated response |
| XDR | Cross-platform detection |

---

# 🧪 Malware Types

| Malware | Description |
|------|-------------|
| Virus | Infects files |
| Worm | Self-spreading |
| Trojan | Disguised malware |
| Ransomware | Encrypts data |
| Spyware | Steals information |
| Rootkit | Hides system access |

---

# 🎭 Social Engineering Attacks

| Attack | Description |
|------|-------------|
| Phishing | Fake emails |
| Spear phishing | Targeted phishing |
| Whaling | Executive targeting |
| Vishing | Voice phishing |
| Smishing | SMS phishing |

---

# 🌐 Network Attacks

| Attack | Description |
|------|-------------|
| MITM | Intercept communication |
| DNS poisoning | Redirect domain |
| ARP spoofing | Fake MAC mapping |
| Replay attack | Reuse captured data |
| Session hijacking | Take over sessions |
| DoS | Service disruption |
| DDoS | Distributed attack |

---

# ☁️ Cloud Security Models

| Model | Responsibility |
|----|------|
| IaaS | Infrastructure |
| PaaS | Platform |
| SaaS | Software |

### Exam Trap

**Responsibility shared between provider and customer**

---

# 🏛️ Security Frameworks

| Framework | Purpose |
|---------|---------|
| NIST CSF | Cybersecurity framework |
| ISO 27001 | Security management |
| COBIT | IT governance |
| CIS Controls | Security best practices |
| PCI DSS | Payment security |

---

# 🔐 PKI Components

| Component | Role |
|----------|------|
| CA | Certificate authority |
| RA | Registration authority |
| CRL | Revoked certificate list |
| OCSP | Real-time revocation |

### Exam Trap

```
OCSP is faster than CRL
```

---

# 🧾 Digital Certificates

Contain:

- Public key
- Certificate authority
- Expiration date
- Digital signature

---

# 🧱 Zero Trust Model

Principle:

```
Never trust
Always verify
```

Core ideas:

- Continuous authentication
- Least privilege
- Microsegmentation

---

# 🛠️ Incident Response

## 6 Phases

| Step | Description |
|----|-------------|
| Preparation | Tools and policies |
| Identification | Detect incident |
| Containment | Stop spread |
| Eradication | Remove threat |
| Recovery | Restore systems |
| Lessons Learned | Improve defenses |

### Memory Trick

```
PICERL
```

---

# 🧪 Vulnerability Management

| Tool | Purpose |
|----|--------|
| Nmap | Network scanning |
| Nessus | Vulnerability scanning |
| OpenVAS | Security scanning |
| Metasploit | Exploit framework |

---

# 🧾 Logging & Monitoring

| Tool | Function |
|----|-----------|
| SIEM | Log aggregation |
| NetFlow | Network traffic analysis |
| Packet capture | Deep analysis |

---

# 🛡️ Security Principles

### CIA Triad

| Principle | Meaning |
|---------|--------|
| Confidentiality | Prevent disclosure |
| Integrity | Prevent modification |
| Availability | Ensure access |

---

### Security Concepts

| Principle | Meaning |
|---------|--------|
| Least privilege | Minimal access |
| Separation of duties | Split responsibilities |
| Defense in depth | Layered security |

---

# 🚨 Risk Management

| Term | Meaning |
|----|--------|
| Risk | Potential loss |
| Threat | Possible attack |
| Vulnerability | Weakness |
| Exploit | Attack method |

### Risk Formula

```
Risk = Threat × Vulnerability × Impact
```

---

# 📊 Disaster Recovery

| Metric | Meaning |
|------|--------|
| RTO | Recovery time objective |
| RPO | Recovery point objective |
| MTTR | Mean time to repair |
| MTBF | Mean time between failures |

---

# 🧠 Common Exam Traps

### Trap 1

```
Authentication ≠ Authorization
```

Authentication = identity  
Authorization = permissions

---

### Trap 2

```
Hashing ≠ Encryption
```

Hashing = one-way  
Encryption = reversible

---

### Trap 3

```
IDS detects
IPS blocks
```

---

### Trap 4

```
RBAC = role
ABAC = attributes
```

---

# 🏁 Final Exam Strategy

### Focus on:

✔ Ports  
✔ Encryption types  
✔ Attack scenarios  
✔ Authentication methods  
✔ Incident response order  

Most questions are **scenario based**, not memorization.

---

# ⭐ Quick 60-Second Review

```
CIA Triad
PICERL Incident Response
Common Ports
Encryption vs Hashing
RBAC vs ABAC
IDS vs IPS
WPA2 vs WPA3
```

---

# 🎯 Final Advice

Security+ is **less about memorization and more about understanding security concepts**.

If you understand:

- how networks work
- how attacks happen
- how defenses operate

…most exam questions become **logical instead of difficult**.