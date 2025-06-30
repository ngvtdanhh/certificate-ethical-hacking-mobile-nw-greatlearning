# 🛡️ Threat Modeling – STRIDE for Mobile & Network Systems

This document applies the STRIDE framework to assess potential security threats across mobile platforms and network architecture components.

---

## 🔍 What is STRIDE?

| Threat     | Description                              |
|------------|------------------------------------------|
| S – Spoofing        | Pretending to be another user/device |
| T – Tampering       | Unauthorized modification of data   |
| R – Repudiation     | Denying performed actions           |
| I – Information Disclosure | Exposing sensitive data          |
| D – Denial of Service | Disrupting availability             |
| E – Elevation of Privilege | Gaining unauthorized access       |

---

## 📱 Mobile App Threat Model (STRIDE)

| STRIDE Category | Example                                  | Impact                              |
|-----------------|------------------------------------------|-------------------------------------|
| Spoofing         | SIM Swap, Fake app login                | Unauthorized access to account      |
| Tampering        | App memory patching (Frida, Xposed)     | Business logic bypass               |
| Repudiation      | No secure logs in mobile app            | Deny fraud, legal gaps              |
| Info Disclosure  | Local storage in plaintext              | Leak of tokens, PII                 |
| DoS              | Crash via malformed inputs              | App downtime, poor UX               |
| Privilege Escalation | Root access via vulnerable componen
