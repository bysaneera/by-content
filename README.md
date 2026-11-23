# by-content — SMM content skills for Claude

Created by **Sanira Baitassova**.

| Skill | What it does |
|---|---|
| `trend-scout` | Finds content trends — sounds, formats, visuals, news hooks, events, slang — across Instagram, TikTok, YouTube, X and the platforms of your market, and keeps them in your own **Trend Library** (a private page with a database in your Claude account). Modes: find trends, add from a link or screenshot, pick from the library, update statuses, daily morning digest. |
| `content-ideas` | Turns a brief for a month, season or campaign into post ideas with visual reference boards: content types, formats, shoot plan, hooks, references from your Pinterest boards. Outputs a responsive web board in a team and a client version. |
| `content-setup` | A guided first-run chat: creates your Trend Library and connects your market, niches, Instagram, Pinterest, seasons and an optional morning digest. |

Built for any market — holiday calendars and number/date/unit formats adapt to the market you set (US, UK/Europe, Japan, South Korea, China, Southeast Asia, Kazakhstan/CIS and others), including Japanese, Korean and Chinese typesetting. Ad-disclosure rules are built in for the US, UK, Japan and South Korea; for other markets Claude asks for the local requirement. Skills are written in English; Claude answers in the language you write in.

Looking for layout, presets and motion? See **[by-design](https://github.com/bysaneera/by-design)**.

---

## Install

### Option 1 — by link (recommended)
**Claude app (desktop / web):**
1. Open **Customize** → **Plugins** → **Manage marketplaces** → **Add marketplace** and paste the link below.
2. Click **Done**, find **by-content** in the plugins list and click **Install**.
3. To get updates later: **Manage marketplaces** → **…** next to by-content → sync.

```
https://github.com/bysaneera/by-content
```

The marketplace is only the source — the plugin itself still needs **Install**. Plugins work where Claude runs tasks with tools (the desktop app's task mode and Claude Code), not in a plain chat.

**Claude Code:**
```
/plugin marketplace add bysaneera/by-content
/plugin install by-content@by-content
```

**Organisations:** organisation-wide sync from GitHub works only with private or internal repositories connected through the Claude GitHub App — an admin can fork this repo privately and sync that, or upload the file below.

### Option 2 — upload the file
Download [`dist/by-content.zip`](dist/by-content.zip) (or the identical [`dist/by-content.plugin`](dist/by-content.plugin)) and upload it in Claude: Customize → Plugins → upload a plugin file.

---

## First run — setup chat

After installing, start a task and write something like:

> Let's set up the skills — trends and content ideas

Claude walks you through it step by step (every step is optional and can be changed later):
1. Creates your private **Trend Library**.
2. Market, region, languages, time zone — e.g. US / North America / English, Japan / East Asia / Japanese, or Kazakhstan / CIS / Russian + Kazakh.
3. Niches and current clients.
4. **Instagram** — your handle; Claude checks it can open your Saved in your browser (read only) and uses what you save as trend sources.
5. **Pinterest** — your profile (project reference boards are found by name) and an ideas board.
6. Accounts to track, Curaeted, connectors (vidIQ, Apify, Spyglass) if you have them.
7. Seasonal themes and holidays for your market.
8. Your taste: what to always / never pick.
9. Optional daily **morning trend digest** as a scheduled task.

Claude only **reads** your accounts — it never posts, pins, likes, follows or enters passwords (you log in yourself in your browser).

---

## How to use

- "Find trends", "What's trending in beauty right now?"
- "Add to trends" + a link or screenshot (or paste links into the library page from your phone)
- "Pick trends for <client> for December"
- "Ideas for <client> for January: 12 posts, 2 shoot days, …" → a web board with team and client versions
- "Clean up the library"

---

## Requirements
- **Artifacts** (Claude's published pages with storage) for the Trend Library and reference boards. Without them the skills still work and return results in chat.
- A browser Claude can use (Claude in Chrome or the desktop app's built-in browser) for Instagram, TikTok, Pinterest and Curaeted.
- Optional connectors: vidIQ, Apify, Spyglass (trend data).

## Privacy
No personal data, accounts or libraries ship with these skills. Every user's settings, libraries and brand memory live in their own Claude account.

## Author and licence
All skills in this repository were created by **Sanira Baitassova**. Licensed under [CC BY 4.0](LICENSE): you can use, share and adapt them, including commercially, as long as you credit the author.
