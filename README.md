# Jeremy Lee

**Biomedical Engineering + Electrical Engineering @ Case Western Reserve University 

---

## What I'm Building

### [Foundry Studio](https://github.com/jlee056/foundry-studio) — Web Design + AI Automation Agency `public`
Full-stack marketing site and service business targeting small trade companies (HVAC, plumbing, electrical). Services: website design, AI automation (chatbot, phone receptionist, review automation), and Google Business Profile optimization / local SEO. Built a 200+ lead prospect list with Firecrawl-verified website audits; completed GBP audits on individual businesses.

**Stack:** Next.js 16 · React 19 · TypeScript · Tailwind CSS v4 · shadcn/ui · Motion · Vercel · Firecrawl

---

### [Weverse Ticket Bot](https://github.com/jlee056/weverse-ticket-bot) — Precision Event Registration Bot `private`
Clicks a Weverse fan event submit button at the mathematically correct millisecond. Implements four layers of timing compensation: NTP clock sync, Weverse server clock offset (via `Date:` header), min-RTT one-way latency, and in-browser `dispatchEvent` to bypass Playwright IPC overhead.

**Stack:** Python · asyncio · Playwright · ntplib · HTTP latency measurement

---

### [ORB Trading Bot](https://github.com/jlee056/orb-bot) — Automated MNQ Futures Trading `public`
Automates the Opening Range Breakout strategy on Micro Nasdaq-100 futures via the Interactive Brokers API. Locks the 30-min opening range at 10:00 AM ET, enters long on 5-min close confirmation above the range, exits at target or stop, force-closes at 3:50 PM. Built-in VIX filter, 20-day EMA trend filter, overnight gap filter, and daily/monthly loss limits — every parameter data-backed against a 6,142-day ES/NQ dataset and cross-validated against 2025 live market data. 1.5% risk per trade with automatic size reduction after 3 consecutive losses. Benchmarks: 73.44% win rate (Edgeful live, Jan–Jul 2025) · 74.6% win rate / 433% annual return (Cory Mitchell, 114 trades). Currently in paper trading phase.

**Stack:** Python · ib_insync · yfinance · Interactive Brokers API · pandas

---

## Tech Stack

**Frontend**
`Next.js` `React` `TypeScript` `Tailwind CSS` `Framer Motion` `shadcn/ui`

**Backend & Automation**
`Python` `asyncio` `Playwright` `REST APIs` `ntplib`

**Hardware & Embedded**
`Arduino` `ESP32` `I²C / SPI / UART` `signal processing` `PCB prototyping`

**Tools**
`Git` `Vercel` `VS Code` `TWS (Interactive Brokers)`

**Languages**
`TypeScript` `Python` `C++` `Java` `MATLAB`

**Simulation & EDA**
`KiCad` `LTspice` `NI Multisim` `ModelSim` `SolidWorks`

---

## Education

**Case Western Reserve University** — Cleveland, OH
BS Biomedical Engineering + BS Electrical Engineering *(double major)*

**Gilman School** — Baltimore, MD

---

## Contact

- Email: leejeremy056@hotmail.com
- LinkedIn: [linkedin.com/in/jlee056](https://www.linkedin.com/in/jlee056)
- GitHub: [github.com/jlee056](https://github.com/jlee056)
