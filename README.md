# Jeremy Lee

**Biomedical Engineering + Electrical Engineering @ Case Western Reserve University** · Expected Fall 2028

I build things where hardware, signals and software meet: embedded systems, computer vision, developer tooling, and AI projects.

---

## Projects

### [agentview](https://github.com/jlee056/agentview) · `Python` `Textual`
Every Claude Code session in one terminal window, read-only. Merged feed, grid and per-session views, live status dots, and a pixel-art **kitchen** where each session is a chef wandering around: tool stations, sous-chefs for sub-agents, a day/night window and a cat. Runs on Mac, Linux and Windows.

### [Agent Mission Control](https://github.com/jlee056/agent-mission-control) · `TypeScript` `Fastify` `SQLite` `WebSocket`
Real-time dashboard that turns Claude Code hook events into pixel-art agents working in a virtual office. Session replay, a communication graph, a file-activity inspector, anomaly detection for stuck loops, and a scrum board.

### [Foundry Studio](https://github.com/jlee056/foundry-studio) · `Next.js 16` `React 19` `Tailwind v4` `Framer Motion`
Marketing site for a web design and AI automation studio aimed at small trade businesses. Fraunces display type, full-bleed color bands, JSON-LD schemas and an `llms.txt` for AI-search visibility. [Live site](https://foundry-studio-flax.vercel.app).

### [Ultrasonic Tactile Alert](https://github.com/jlee056/Ultrasonic-Tactile-Alert) · `Arduino` `C++`
Early exploration of tactile feedback for blind and low-vision navigation: an HC-SR04 ultrasonic sensor, an LCD readout and a servo that responds as objects get close.

### Published hardware work: *Science* (2024)
Built the **Arduino-controlled pressure rig** used in a Johns Hopkins study published in *Science* (vol. 385, eadi1650): programmable cycling of 1 kPa at 0.025 Hz (20 s on / 20 s off) applied to cell cultures for 30 minutes. Also trained the image-segmentation model used to quantify the results. [doi:10.1126/science.adi1650](https://doi.org/10.1126/science.adi1650)

### More builds
*Local or private repos, so no links yet.*

- **JARVIS**: an always-on local voice assistant. A "Hey Jarvis" wake word, local speech-in and speech-out, Claude as the brain, and my whole notes vault as memory. A code-enforced safety gate sits in front of risky actions. *In progress.*
- **Table Vision**: a webcam watches a table and names the objects on it, live. YOLO11 nano and OpenCV, fully local, about 28 FPS on CPU. Capture, inference and drawing run on separate threads so the video never stutters.
- **APOBEC3A Protocol Optimizer**: a browser port of NEB's unfinished EM-seq protocol optimizer. Found and fixed 9 upstream defects, then solved the kinetic ODE in closed form so a sweep of 41,160 protocols runs in about 60 ms instead of minutes.
- **Threat-intel pipeline**: ingests CISA KEV, abuse.ch and RSS feeds daily, has Claude enrich and triage each item into a linked knowledge graph, and drafts a weekly report that only publishes after I approve it.
- **ORB trading bot**: a Python bot for the Opening Range Breakout strategy on MNQ futures through the Interactive Brokers API. It runs layered filters and logs the trades each filter would have skipped, so I can measure which ones add edge before risking money. Paper trading only.

---

## Tech

**Languages** `Python` `TypeScript` `C / C++` `MATLAB` `Java`
**Web** `Next.js` `React` `Tailwind CSS` `Framer Motion` `shadcn/ui` `Vercel`
**Embedded and hardware** `Arduino` `ESP32` `Raspberry Pi` `I²C / SPI / UART` `KiCad` `LTspice` `Multisim` `SolidWorks`
**AI and tooling** `Claude Code` `MCP` `YOLO` `OpenCV` `Playwright` `Git`

---

## Education

**Case Western Reserve University**, Cleveland, OH: BS Biomedical Engineering + BS Electrical Engineering (double major)
**Gilman School**, Baltimore, MD

## Contact

- LinkedIn: [linkedin.com/in/jlee056](https://www.linkedin.com/in/jlee056)
- Email: leejeremy056@hotmail.com
