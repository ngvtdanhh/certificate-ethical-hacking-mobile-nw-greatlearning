# 📡 Wi-Fi Attack Vectors

Key wireless attack techniques relevant to mobile users and infrastructure.

---

## 🎯 Common Wi-Fi Attacks

- Rogue Access Point (Evil Twin)
- Deauthentication attacks
- Captive portal phishing
- ARP spoofing / MITM

---

## 🧪 Tools & Techniques

| Tool        | Use Case                  |
|-------------|---------------------------|
| `aircrack-ng` | Packet sniffing, deauth  |
| `hostapd`     | Rogue AP creation        |
| `dnsmasq`     | DHCP + DNS spoofing      |
| `mitmproxy`   | HTTP/HTTPS interception  |

---

## 🛡️ Mitigation

- Use WPA3 if supported
- Enable MAC randomization
- Avoid open Wi-Fi networks
- Use VPN on public Wi-Fi
