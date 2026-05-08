# Methodology  
### Independent Threat Intelligence Research – ShinyHunters / UNC6040 / UNC6240  

This document outlines the methodology used to conduct my threat‑intelligence investigation into **ShinyHunters**, **UNC6040**, **UNC6240**, and related infrastructure.

---

## 1. Research Objectives
- Identify and analyze ShinyHunters’ extortion infrastructure  
- Attribute hosting and network resources to supporting entities
- Map attacker TTPs to MITRE ATT&CK
- Understand cloud‑identity attack vectors, especially OAuth abuse
- Produce a professional‑grade intelligence brief suitable for industry review

## 2. Data Collection Techniques

### 2.1 OSINT Sources
The following open‑source intelligence tools and datasets were used:

- **Shodan** – IP fingerprinting, service enumeration
- **ExifTool** – Metadata viewing, and editing
- **BGPView / RIPEstat** – ASN ownership, routing history
- **Passive DNS** – Domain resolution history
- **WHOIS** – Registration metadata
- **Darknet leak sites** – Actor‑controlled infrastructure
- **Public reporting** from security vendors (Mandiant, CrowdStrike, Recorded Future)

---

## 3. Actor Analysis

### 3.1 Threat Actor Clustering
Actor behaviors were compared against known profiles for:

- **[ShinyHunters](ca://s?q=Tell_me_more_about_ShinyHunters)**  
- **[UNC6040](ca://s?q=Explain_UNC6040)**  
- **[UNC6240](ca://s?q=Explain_UNC6240)**  
- **[Scattered Spider](ca://s?q=Tell_me_more_about_Scattered_Spider)**  

Clustering was based on:
- TTP similarity
- Verified reports
- Infrastructure overlap
- Extortion patterns
- Communication channels
- Victimology

---

## 4. Infrastructure Attribution

### 4.1 IP & ASN Analysis
- Queried IP ranges associated with ShinyHunters’ leak site  
- Identified leak page hosting provider as Prospero OOO (AS200593)
- Analyzed BGP announcements, routing paths, and geolocation  
- Cross‑referenced with known bulletproof hosting indicators  

### 4.2 Service Fingerprinting
- Enumerated open ports
- Identified hosting stack (Linux, Cyberoam UTM firewall)
- Checked for reused TLS certificates or SSH keys

---

## 5. MITRE ATT&CK Mapping
Mapped observed behaviors to ATT&CK techniques including:

- **[T1598](ca://s?q=Explain_ATT%26CK_T1598)** – Vishing  
- **[T1671](ca://s?q=Explain_ATT%26CK_T1671)** – OAuth abuse  
- **[T1213.004](ca://s?q=Explain_ATT%26CK_T1213.004)** – Cloud data access  
- **[T1550](ca://s?q=Explain_ATT%26CK_T1550)** – MFA bypass  
- **[T1567](ca://s?q=Explain_ATT%26CK_T1567)** – Exfiltration via cloud APIs  

---

## 6. Cloud Identity Analysis

### 6.1 OAuth Attack Vector
Reviewed how attackers:
- Created malicious OAuth applications  
- Elevated permissions  
- Leveraged service principals for persistence  
- Bypassed MFA using token‑based authentication  

### 6.2 Case Study Review
Analyzed a multi‑stage compromise involving:
- Initial OAuth abuse  
- Patch remediation  
- Secondary exploitation via unknown vulnerability  

---

## 7. Limitations 
- Certain vulnerabilities remain undisclosed publicly  
- Actor identity overlaps are based on behavioral analysis, not confirmed law‑enforcement attribution  

---

## 8. Conclusion
This methodology demonstrates a full‑spectrum threat‑intel workflow, including OSINT collection, actor profiling, infrastructure attribution, and cloud‑identity attack analysis.  
It reflects real‑world processes used by threat‑intel teams and SOC analysts.

