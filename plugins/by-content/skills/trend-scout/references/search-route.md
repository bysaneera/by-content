# Where to search — the mandatory route

Part of the trend-scout skill. Read together with its SKILL.md.

## Where to search
**Mandatory route — on any "find trends", "any new trends?", "what's trending now" and in the morning run.** Don't cut it down to one platform (TikTok only is a mistake). Go through all steps in this order:
1. The `inbox` queue and links the user sent.
2. News of the last 24 hours by web search (space, tech, releases, sport, records, brand launches; world and local market) and this week's events calendar → type "News hook"/"Event" with `expiresHint`.
3. The user's Instagram Saved and reposts — only if `instagramHandle` is set (item 1 below).
4. The user's Pinterest ideas board — only if `pinterestIdeasBoard` is set (item 1a).
5. Curaeted — TRENDS and NEW (item 1b).
6. Accounts from `sources` (item 2).
7. Search on both Instagram and TikTok (item 3), including niche queries and local-language songs.
8. Google Trends for the local market and worldwide (item 4).
9. TikTok Creative Center and sound pages (item 5).
10. X/Threads, regional messengers (Telegram via TGStat for CIS; LINE/KakaoTalk open channels where relevant), Know Your Meme (items 6–8).
11. Paid services (vidIQ, Apify, Spyglass) and web trend round-ups — last, as a supplement (items 9–11).
Every answer has one line "Checked: … / unavailable: …" — so no source is silently skipped. Which tool to use and when a source counts as unavailable — see "Tool order" above.

1. **The user's Instagram** (browser, logged in): Saved (`https://www.instagram.com/<handle>/saved/`) and the reposts tab. If `instagramTrendsCollection` is set — read it first. Go from new to old and take only things about brands, visuals, formats, editing and sounds; skip anything personal and don't record it anywhere. Repeated by 3+ creators — `tier` "Trend"; otherwise, if well made or moody — "Find" with a note in `signal`. Mark aesthetic items `moodFit`. `source` — "User (saved)" or "User (repost)", the post link first in `examples`. Don't reprocess what's already in the library.
1a. **The user's Pinterest ideas board** (browser; pin.it short links may not open — use the full URL). Go from new pins to old, don't reprocess. **Everything from this board is `tier` "Find"**, even if several pins are similar. "Trend" — only if the user called it a trend or you found 3+ creators with it outside the board. If a pin leads to an Instagram or TikTok video — open the original and put it first in `examples`. `source` — "User (Pinterest)".
1b. **Curaeted** — https://www.curaeted.co (browser; may require login). TRENDS (?category=trends) — visual trends with descriptions and brand examples. `tier` "Trend" only if 3+ brands are confirmed by their own posts in the last 30 days (open them); otherwise "Find". NEW and categories — beautiful brand pages: `tier` "Page", `moodFit` true, 0–2 per run: what hooks (grid, light, colour, typography, product presentation) and how to adapt to niches. `title` — "Brand — what hooks"; `examples` — the brand's Instagram (not Curaeted), `source` — "Curaeted". Pages the user sends — the same way (`source` "User"). These are references for own shoots: links, not copies of others' photos.
2. **Sources** — new posts of accounts in `sources` (editing breakdowns, trend round-ups, aesthetics).
3. **Instagram and TikTok search** in the browser — the main method. Look at results and select what repeats. Most reliable signals — captions "finally did the trend", "hopping on this trend" and the same on-screen line from different creators.
   - English: "trending transitions", "trending hooks", "trending reels", "trending audio", "viral edit", "trends this week";
   - round-ups: "current trends", "trends of [month]", "[month] social media trends", "winter trends", "christmas content ideas" — open carousels and write each trend out separately, then verify each by searching its phrase or sound. The source is the carousel and its author. Such round-ups often give moody and auteur techniques — mark `moodFit`;
   - in the user's `languages`: the local equivalents of "trending transitions", "trend of the week", "trends of [month]", "challenge", "prank on mom", "parents' reaction", local humour.
   - **Working cycle:**
     1. World: fresh weekly trend posts from marketing accounts and "trending audio for business this week" videos from strategists on TikTok. Take the hook or sound from each.
     2. Region and local market: search TikTok in local languages for "we did the trend too", "did the trend with colleagues", "recreated the trend". The same caption from different offices is a signal.
     3. For each candidate open the sound page (the /music/ link on the video page): record the video count with a date and look for local and regional businesses (restaurants, airlines, offices). 3+ local/regional businesses — `origin` Local/Regional.
     4. Verify the text hook with 3+ creators by searching the phrase itself.
     5. The run result is a mix: world trends + at least 2 local/regional, each sound with a dated video count.
4. **Google Trends** (local market and worldwide) — rising queries.
5. **TikTok Creative Center** (https://ads.tiktok.com/creative/creativeCenter/trends/hashtag, browser) — trending hashtags, videos and sounds for 7 days. Switch countries: US, UK and 1–2 more; the user's market first if it's listed. Foreign items there are an early signal: verify by searching local and regional creators; 3+ — `origin` Local/Regional, otherwise "International" with "may arrive" in `signal`.
   **Sounds, additionally:** trending sounds in Reels (the ↗ arrow next to the sound), Spotify Viral 50 and Shazam charts for the local market — what starts playing before it reaches videos.
6. **News, X, Threads** — what's discussed right now.
7. **Regional channels and meme pages** — for CIS markets Telegram via TGStat; elsewhere the market's equivalent (skip if there's none).
8. **Know Your Meme** — memes and their origins.
9. **vidIQ** — trending videos and outliers on Instagram, TikTok, YouTube; **Apify** — latest posts and reels of tracked accounts with numbers.
10. **Spyglass** — campaigns, formats and hooks of category brands.
11. **Web search** — news hooks and platform trend round-ups.

**"How to make it" breakdowns.** If an editing-breakdown creator shows a technique — find the original video it came from: it goes first in `examples`, the breakdown — in `howTo`.

**Local.** In every search and morning run aim for `localShare` (default one third) of trends from the local market and region. Pay attention to: family humour, parents trying new things, pranks on kids and parents, recognisable local situations, local sounds and phrases, local creators picking up a foreign sound. A local trend is checked by the same rule (at least 3 creators in the local-language segment). If nothing local is good enough — say so, don't add weak items to hit the quota.
