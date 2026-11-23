# Agent team (search and morning run)

Part of the trend-scout skill. Read together with its SKILL.md.

## Agent team (search and morning run)
In "Find trends" and "Morning digest" work as a team: scouts → critic → writer. You are the lead: hand out tasks, check against the library, save. If there is no Agent tool — go through the same stages yourself, in order.

**1. Scouts (in parallel, 3 agents).** Each gets its part of the "Where to search" route, dates (last 1–3 days), the library index (`title`, first link, `soundUrl`, `hook`) so as not to bring what's already saved, the settings, and the sections "What counts as a trend", "What not to add", "Default taste". They return only a candidate list: name, gist, links to originals, author, figures with source and date (video count on the sound, views), how many creators found, `origin`. They don't write to the library.
- **Browser scout** — the only one working in the browser (there is one browser; two agents in it get in each other's way): the user's Saved and reposts (if set), the Pinterest ideas board (if set), Curaeted, Instagram and TikTok search by the working cycle, sound pages, Creative Center.
- **News scout** — no browser: news of 24 hours, events calendar, Google Trends, X/Threads, TGStat (CIS markets), Know Your Meme, web trend round-ups.
- **Services scout** — vidIQ, Apify (accounts from `sources`), Spyglass; within a budget of 12 calls.
The browser scout checks all candidate links (its own and others') and returns for each a mark "opened, technique present, date". While it works, the lead doesn't use the browser. If the browser is unavailable — the browser scout isn't launched; this goes into the "unavailable" line.

**2. Lead** merges candidates and removes duplicates between scouts and against the library by the duplicate rule.

**3. Critic (1 agent that hasn't seen the search).** Gets the candidates and the sections "What counts as a trend", "What not to add", "Default taste", "Who the library is for", "Daily quota". For each — a verdict: "Trend" / "Find" / "Reject" and a one-line reason (e.g. "one video, no repeats", "cheesy", "doesn't transfer to 3 niches", "no original"). Rejects candidates without the browser scout's link-check mark (in a run without a browser — passes them with `verified: false`) and figures without source and date; invents nothing. Watches the quota: local share and per-type norms; doesn't pass weak items for quantity.

**4. Writer (1 agent).** For approved items writes `hook`, `howToUse` (at least 3 niches, rotating) and `summary` in a "fun, not cheesy" tone.

**5. Lead** saves per "Saving" and writes the reply or the morning message. At the end — a line "Team: found N, critic passed M, rejected K (main reasons)".

No more than 5 agents per run: each one spends the user's limits.
