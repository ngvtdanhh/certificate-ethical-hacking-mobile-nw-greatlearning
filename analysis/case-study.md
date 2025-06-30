# 🧪 Case Study – Mobile & Network Exploits in the Wild

Real-world cases where mobile and network-level vulnerabilities were exploited.

---

## 🐎 Pegasus Spyware (NSO Group)

- Attack vector: Malicious link (Zero-click via iMessage/WhatsApp)
- Exploit type: Kernel privilege escalation, sandbox escape
- Target: iOS & Android
- Impact: Full device access (camera, mic, files, location)
- Lesson: Even hardened OSs can be bypassed via 0-day chain

---

## 📶 IMSI Catchers in Protests

- Location: Belarus, Hong Kong, USA
- Threat: Devices forced onto rogue BTS (2G) to leak IMSI
- Technique: Stingrays emulate base stations
- Purpose: Crowd monitoring, dissident tracking
- Defense: TMSI, Disable 2G fallback, Airplane Mode

---

## 🎯 Fake Wi-Fi at Airports

- Scenario: Rogue AP mimicking airport network name
- Users auto-connect (SSID remembered)
- Captive portal serves phishing login for email credentials
- Attacker collects session tokens or installs malware
- Defense: Avoid saved SSIDs, use VPN, verify HTTPS certs

