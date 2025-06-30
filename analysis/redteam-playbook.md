# 🎯 Red Team Playbook – Mobile & Network Targets

This checklist covers offensive actions and tools to test the resilience of mobile infrastructure, apps, and Wi-Fi.

---

## 🔓 Mobile App Testing

- [ ] Static Analysis (APKTool, MobSF)
- [ ] Dynamic Analysis (Frida, Xposed)
- [ ] Certificate pinning bypass
- [ ] Check insecure storage (shared_prefs, SQLite)
- [ ] Test for insecure Intents/Broadcast Receivers

---

## 📡 Wi-Fi Attacks

- [ ] Set up Evil Twin with `hostapd` + `dnsmasq`
- [ ] Inject captive portal to collect credentials
- [ ] Deauth connected users (aircrack-ng suite)
- [ ] Sniff ARP/DNS/HTTP traffic (Wireshark / mitmproxy)

---

## 📶 Cellular / Telecom

- [ ] Passive sniffing via SDR (Kalibrate, GQRX)
- [ ] Analyze GSM channel leaks
- [ ] Theoretical BTS emulation (OpenBTS/YateBTS)  
⚠️ Legal restrictions apply

---

## 🧪 Post-Exploitation (Rooted/Test Device)

- [ ] Dump app memory, analyze with Ghidra/r2
- [ ] Extract JWT tokens, session cookies
- [ ] Test escalation vectors (sudo misconfig, SUID)

