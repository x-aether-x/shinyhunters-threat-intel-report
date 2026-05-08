# Indicators of Compromise (IOCs)  
### ShinyHunters / UNC6040 / UNC6240

This file contains infrastructure‑level indicators identified during the investigation.

## 1. IP Addresses
91.215.85.103   # ShinyHunters pay_or_leak server
91.202.233.0/24 # Prospero OOO range
91.215.85.0/24  # Prospero OOO range
193.24.123.0/24 # Prospero OOO range

## 2. Domains
shinyhunte.rs
pro-spero.ru

## 3. Darknet Services
shnyhntww34phqoa6dcgnvps2yu7dlwzmy5lkvejwjdo6z7bmgshzayd.onion

## 4. Email Addresses
shinygroup@onionmail.com

## 5. Actor Infrastructure Notes
- Hosting provider: Prospero OOO (AS200593)
- Geolocation: St. Petersburg, Russia
- Hosting type: BPH ("Bulletproof" Hosting)
- Firewall: Cyberoam UTM

## 6. MITRE ATT&CK Techniques
- **[T1598](ca://s?q=Explain_ATT%26CK_T1598)** – Vishing
- **[T1671](ca://s?q=Explain_ATT%26CK_T1671)** – OAuth abuse
- **[T1213.004](ca://s?q=Explain_ATT%26CK_T1213.004)** – Cloud data access
- **[T1550](ca://s?q=Explain_ATT%26CK_T1550)** – MFA bypass
- **[T1567](ca://s?q=Explain_ATT%26CK_T1567)** – Exfiltration

## 7. Notes
These IOCs should be treated as medium‑confidence indicators.  
They are suitable for:
- Threat hunting  
- SOC enrichment  
- Blocklists  
- Cloud identity monitoring  

