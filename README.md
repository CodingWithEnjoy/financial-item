# 📈 Financial Data Dashboard (Hourly)

A fully automated system that **collects, stores, and visualizes hourly financial market data** using **GitHub Actions** and a **modern Chart.js dashboard** — no backend, no database, no servers.

---

## ✨ Features

- ⏱ **Hourly data collection** via GitHub Actions  
- 📁 **One JSON file per day** (append-only, versioned)  
- 📊 **Modern dashboard UI** with large charts  
- 🌙 **Dark, clean fintech-style design**  
- 🌍 **Hosted free on GitHub Pages**  
- ⚙️ **Zero backend / zero Node.js**

---

## 📊 Tracked Assets

| Asset                | Source Key  | Currency |
|---------------------|------------|---------|
| 💵 USD              | `usd`      | Toman   |
| 💶 EUR              | `eur`      | Toman   |
| 🪙 Sekkeh (Emami)   | `sekkeh`   | Toman   |
| 🥇 Gold 18k (Tala)  | `18ayar`   | Toman   |
| ₿ Bitcoin           | `usd_btc`  | USD     |

---

## 🔄 How Data Collection Works

1. **GitHub Actions** runs every hour  
2. Fetches financial data from:  
   `https://api.dastyar.io/express/financial-item`  
3. Appends a new hourly snapshot into:  
   `data/YYYY-MM-DD.json`  
4. Commits the update automatically

✔ Secure  
✔ No tokens required  
✔ Fully auditable history  

---

## 📈 Visualization

- Each asset has its **own large chart**  
- Hourly X-axis (00 → 23)  
- Real values (no normalization)  
- Responsive layout (desktop & mobile)  

The dashboard reads data **directly from the repo**, making it fast and simple.

---

## 🚀 Live Demo

Once GitHub Pages is enabled:

https://codingwithenjoy.github.io/financial-item/


---

## ▶️ Manual Run

You can trigger data collection manually:

1. Go to **Actions**  
2. Select **Hourly Financial Data Save**  
3. Click **Run workflow**

---

## ⏱ Limits & Reliability

- GitHub Actions usage: ✅ well within free limits  
- Data growth: ~130 MB/year (safe for years)  
- Runs hourly (not real-time — by design)

> This project treats GitHub as a **time-series archive**, not a database.

---

## 🛠 Tech Stack

- **GitHub Actions** (automation)  
- **Bash + curl + jq** (data processing)  
- **Chart.js** (visualization)  
- **GitHub Pages** (hosting)  

No frameworks. No servers. No build steps.

---

## 🔮 Possible Enhancements

- 📉 Percentage change charts  
- 🧭 Zoom & pan  
- 📊 Multi-day comparison  
- 🌓 Light / Dark toggle  
- 📦 Yearly data archiving  
- 📱 Mobile-first dashboard

---

## 📜 License

MIT — use it, fork it, build on it.

---

## ⭐ Why this project?

Because **simple, transparent, and automated systems** often beat complex stacks.  

If you like it, ⭐ the repo 🙂

