# 🇹🇭 Pi-hole Whitelist (Thailand Edition)
**Maintained by [7MannSo](https://github.com/ihacked07)**  
> Latest version: `pi-hole-whitelist-latest.txt`

---

## 🧩 Overview
This whitelist is designed for **Thai Pi-hole users** who want popular apps and services to work without being blocked.  
It includes trusted domains for:
- 🟦 Social Media (Facebook, LINE, IG, X, TikTok)
- 🛍️ Shopping (Shopee, Lazada, JD Central)
- 💳 Thai Banking & Finance (SCB, KBank, Krungsri, AEON, Umay+)
- 🎓 Education (Thai universities)
- 🎬 Streaming (YouTube, Netflix, Spotify)
- ☁️ Cloud/CDN/Push services (AWS, FCM, APNs)
- 🏛️ Government & Utilities (EGAT, PEA, MEA, go.th)

---

## ⚙️ Installation (Pi-hole)
### Option 1 — Import via command
1. Download the latest whitelist:
   ```bash
   wget https://raw.githubusercontent.com/<your-username>/pi-hole-whitelist/main/pi-hole-whitelist-latest.txt
Add all domains to whitelist:

bash
Copy code
sudo pihole -w $(cat pi-hole-whitelist-latest.txt | grep -v '^#')
Restart Pi-hole DNS service:

bash
Copy code
pihole restartdns
Option 2 — Manual import via web admin
Open: http://<your-pihole-ip>/admin

Go to Group Management → Adlists / Whitelist

Paste or upload the file pi-hole-whitelist-latest.txt

🔄 Auto-Update (optional)
You can set Pi-hole to auto-update this whitelist weekly:

bash
Copy code
sudo crontab -e
Add this line:

bash
Copy code
0 3 * * 1 wget -q -O /etc/pihole/whitelist.txt https://raw.githubusercontent.com/<your-username>/pi-hole-whitelist/main/pi-hole-whitelist-latest.txt && \
sudo pihole -w $(cat /etc/pihole/whitelist.txt | grep -v '^#') && \
pihole restartdns
🧠 Notes
✅ Recommended for home / café / small business Pi-hole setups in Thailand

⚠️ Always review domains before use — only whitelist trusted sources

🕒 Update every 2–3 months for best compatibility

🏷️ Credits
Maintained by ihacked07
Contributors welcome — open a PR or issue if you want to suggest new domains.
