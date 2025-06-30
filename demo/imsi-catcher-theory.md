# 📶 IMSI Catcher (Fake BTS) – Theoretical Simulation

This note explains how rogue BTS (e.g., via SDR) can be used to track mobile users and intercept metadata.

---

## 📡 What is an IMSI Catcher?

- Device that mimics legitimate cell towers (2G/3G).
- Forces nearby phones to connect and reveal IMSI.

---

## 🧰 Tools (theoretical lab)

- `OpenBTS` / `YateBTS`
- USRP SDR (Universal Software Radio Peripheral)
- `kalibrate-rtl` for scanning GSM frequencies

---

## 🛑 Legal Warning

Operating fake BTS is **illegal** in most countries. This content is for educational awareness only.

---

## 🔐 Defensive Notes

- New SIMs use temporary TMSI instead of IMSI.
- Modern networks (4G+) use mutual authentication.
- Monitor for rogue towers with apps like SnoopSnitch.

---

## 🧠 Red Team Tip

IMSI catchers are used in real-world espionage and law enforcement. Understanding the concepts helps in threat modeling and detection.
