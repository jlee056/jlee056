# Concert Ticket Alert — Project CLAUDE.md

## Address
Always address Jeremy as **Sir Jeremy** at the start of every response.

## Project
This repo is a concert ticket alert app. It monitors Korean ticketing platforms (Melon Ticket, Interpark, YES24, etc.) for on-sale events and sends Sir Jeremy a phone notification the moment tickets become available — fast enough to beat the queue manually.

## Google Drive reference
Sir Jeremy's master CLAUDE.md lives in Google Drive at:
- **Path:** Google Drive → `claude` folder → `.claude` folder → `CLAUDE.md`
- **File ID:** `1aiRy9y89Ghp-CRxeXe1FWg5Zgzvg1V5J`

Check that file for working-style rules and the full wiki workflow before starting any session.

## Working style
**Most important rule: Never start a task without a complete brief.**
- Before writing any code, building anything, or making decisions — ask every question needed first
- If anything is unclear, ambiguous, or missing, stop and ask before proceeding
- Do not make assumptions and fill in the gaps silently — surface them
- One focused question at a time if there are several, not a wall of questions at once

## Obsidian wiki (second brain)
Sir Jeremy's Obsidian vault is at `C:\wiki`. Claude owns the `C:\wiki\wiki\` directory entirely. Jeremy owns `C:\wiki\raw\` (source files — never modify).

### Directory structure
```
C:\wiki\wiki\
├── index.md          ← catalog of all wiki pages (Claude maintains)
├── log.md            ← append-only activity log (Claude maintains)
├── overview.md       ← high-level business synthesis (Claude maintains)
├── daily/            ← one page per day (Claude maintains)
├── clients/          ← one page per prospect or client
├── concepts/         ← design patterns, techniques, research notes
└── resources/        ← tools, references, competitors, inspiration
```

### Page format
Every wiki page uses this frontmatter:
```yaml
---
title: Page Title
type: client | concept | resource | overview
tags: [tag1, tag2]
updated: YYYY-MM-DD
sources: N
---
```
Use `[[page-name]]` syntax for internal links (Obsidian-compatible).

### When to update the wiki
**On conversation update** — when Sir Jeremy shares progress, decisions, or anything that happened:
1. Check if today's daily note exists at `wiki/daily/YYYY-MM-DD.md` — create it if not, then add what happened
2. Prefer creating a new page over editing an old one
3. Only add to an existing page if the update is clearly about the same ongoing concept
4. Append an entry to `wiki/log.md`
5. Update `wiki/index.md` for any new pages created

**Do this proactively** — don't wait for Sir Jeremy to say "update the wiki."

**On ingest** — when Sir Jeremy says a file is in `raw/`:
1. Read the source
2. Discuss key takeaways briefly
3. Write or update relevant wiki pages
4. Update `wiki/index.md` and append to `wiki/log.md`

**On query** — when Sir Jeremy asks a question:
1. Read `wiki/index.md` to find relevant pages
2. Read relevant pages and answer with citations
3. File anything worth keeping as a new page or section

### Log format
```
## [YYYY-MM-DD] type | description
Brief note on what changed and why.
```
Types: `ingest`, `update`, `query`, `lint`, `new-page`

### Principles
- Prefer new pages over rewriting old ones — the history is the value
- Every piece of info Sir Jeremy shares is potentially wiki-worthy. Err on the side of filing.
- Keep pages concise. Dense 200-word page with good links beats a 1000-word dump.
- Index, log, and today's daily note are always up to date. Never skip updating them.

## Repo navigation
```
/
├── CLAUDE.md          ← this file
├── src/
│   ├── monitor.py     ← main polling loop (checks ticket availability)
│   ├── notify.py      ← phone notification sender (Pushover / ntfy.sh)
│   └── config.py      ← targets: URLs, selectors, check interval
├── tests/
└── requirements.txt
```

## Tech stack
- **Language:** Python 3.11+
- **HTTP:** `httpx` (async)
- **Browser automation (if needed):** Playwright (headless Chromium)
- **Notifications:** ntfy.sh (free, no app install) or Pushover
- **Scheduling:** simple `asyncio` loop with configurable interval
