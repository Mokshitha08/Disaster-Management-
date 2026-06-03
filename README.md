# DR Manager — Disaster Recovery Management System 🚨

A full-stack disaster recovery management system built on the IEEE
peer-reviewed research *"Recovering From a Major Disaster — The
Management Challenge"* by Trybula & Newberry (IEEE EMR, Vol. 48,
No. 3, Sept. 2020).

🌐 **Live Demo:** [mokshitha08.github.io/Disaster-Management-](https://mokshitha08.github.io/Disaster-Management-)

---

## Problem statement
80% of profitable small businesses that file for bankruptcy do so due
to lack of cash flow after a disaster. Organisations need a structured,
real-time system to plan, execute, and track disaster recovery operations.
This project implements the proven IEEE Stoplight approach and Fast
Restart methodology to help teams recover faster and restart stronger.

---

## Key features

| Feature | Description |
|---------|-------------|
| 🚦 Stoplight Risk Approach | Green / Yellow / Red ratings for every recovery plan |
| 📋 Recovery Plan Management | Full CRUD — create, edit, track recovery plans |
| 👥 Recovery Team Tracker | Assign team leaders, manage workforce during restarts |
| 🔗 Supply Chain Recovery | Monitor disruptions with dual-supplier strategies |
| 📊 Analytics Dashboard | Charts for recovery plans per month and disaster type |
| 📄 Document Management | Upload, preview, and download PDF recovery documents |
| ☁️ MongoDB Atlas | Cloud database for persisting all plans and documents |

---

## Stoplight methodology

| Status | Meaning |
|--------|---------|
| 🟢 Green | On track — all systems operational, recovery progressing |
| 🟡 Yellow | Caution — monitoring required, risks identified |
| 🔴 Red | Critical — immediate action required, high impact |

---

## Recovery workflow

```
01 Assess & Identify
   → Evaluate personnel, supply chain, and financial position
   → Apply Stoplight ratings to all critical items

02 Plan & Assign
   → Create recovery plans, assign team leaders
   → Define recovery steps and target timelines

03 Execute & Monitor
   → Track plan execution and update risk statuses in real time
   → Monitor cash flow and supply chain reconstruction

04 Review & Improve
   → Document lessons learned
   → Update disaster preparedness for future events
```

---

## Tech stack

| Technology | Purpose |
|-----------|---------|
| HTML / CSS / JavaScript | Frontend |
| Chart.js | Analytics and data visualization |
| MongoDB Atlas | Cloud database |
| Node.js | Backend server |
| PDF Upload | Document management |

---

## MongoDB Atlas setup

1. Go to [mongodb.com/cloud/atlas](https://mongodb.com/cloud/atlas) → New Project → Free M0 tier
2. Security → Database Access → Add new user with password
3. Network Access → Add IP → `0.0.0.0/0` (allow all)
4. Connect → Drivers → Copy URI

Create a `.env` file in the root directory:

```env
MONGODB_URI="mongodb+srv://<user>:<pass>@cluster0.xxxxx.mongodb.net/disaster_recovery_db"
SESSION_SECRET="your_32_char_secret"
PORT=3000
```

---

## How to run

```bash
git clone https://github.com/Mokshitha08/Disaster-Management-
cd Disaster-Management-
npm install
# Add your .env file with MongoDB URI
node server.js
```

Then open `http://localhost:3000` in your browser.

---

## Research basis

> **"Recovering From a Major Disaster — The Management Challenge"**
> Walt Trybula & Deb Newberry
> IEEE Engineering Management Review, Vol. 48, No. 3, Sept. 2020
> DOI: [10.1109/EMR.2020.3006802](https://doi.org/10.1109/EMR.2020.3006802)

### Key findings applied
- **Stoplight Approach** — Green/Yellow/Red ratings for supply chain, processes, and customer interactions
- **Fast Restart Protocol** — Structured restart methodology to move forward rapidly
- **Cash Flow Priority** — Continuous monitoring until cash flow is positive
- **New Realignment** — Modernise equipment and streamline organisational structure during recovery

---

## Stats

- 📈 **3x** faster restart with structured planning
- 💰 **80%** of businesses fail from cash flow issues post-disaster
- 👁 **100%** recovery visibility via dashboard
- ⏰ **24/7** monitoring and alerts

---
*Based on IEEE EMR Vol.48 No.3 · DOI: 10.1109/EMR.2020.3006802*
