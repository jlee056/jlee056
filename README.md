# Jeremy Lee

**Biomedical Engineering + Electrical Engineering @ Case Western Reserve University**

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
Automates the Opening Range Breakout strategy on Micro Nasdaq-100 futures via the Interactive Brokers API. Locks the 30-min opening range at 10:00 AM ET, enters long on a 5-min close above the range, and manages the trade with an ATR-based stop that moves to breakeven at 75% of the way to target — force-closing at 3:50 PM ET (1:30 PM on FOMC days). Layered, data-backed filters: VIX band, 20-day EMA trend confirmation, overnight gap, range-width, an economic-calendar / earnings day filter (FOMC, CPI, PPI, PCE, GDP, Mag-7), and daily/monthly loss limits — every parameter validated against a 6,142-day ES/NQ dataset and cross-checked on 2025 live data. 1.5% risk per trade with automatic size reduction after 3 consecutive losses. Currently in a paper-log-only validation phase: every filter records the trade it *would* have skipped so I can measure which filters actually add edge before going live. Benchmarks: 73.44% win rate (Edgeful live, Jan–Jul 2025) · 74.6% win rate / 433% annual return (Cory Mitchell, 114 trades).

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
