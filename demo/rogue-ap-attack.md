# 📡 Rogue Access Point (Evil Twin) – Wi-Fi Attack Demo

This simulation sets up a rogue Wi-Fi AP to impersonate a legitimate network and capture user credentials via a fake captive portal.

---

## 🧰 Tools Required

- `hostapd`
- `dnsmasq`
- `iptables`
- `nginx` or custom captive portal
- Kali Linux or any Linux distro

---

## ⚙️ Setup Steps

1. **Configure `hostapd.conf`:**

```bash
interface=wlan0
driver=nl80211
ssid=FreeWiFi
hw_mode=g
channel=6
```
