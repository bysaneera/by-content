# Trend card fields

Part of the trend-scout skill. Read together with its SKILL.md.

## Trend card fields
- `tier` — Trend | Find | Page (a brand account with beautiful presentation, see Curaeted);
- `title` — short name;
- `summary` — what it is, 1–2 sentences;
- `signal` — why it's a trend: figures or observations from the source. Every figure has a source and date ("TikTok sound page, 20 Nov"); service estimates are marked "vidIQ estimate". Views of one video don't prove a trend;
- `evidence` — one line with the main proof and date: "sound: 12,400 videos (TikTok page, 20 Nov)" or "6 creators in 7 days". Prepend new values, keep old ones — shows the dynamics;
- `author` — @handle of the original video's author (first in `examples`). Required for anything with a video or post: no author — don't save. For "Page" — the brand's @handle. Seasons, news hooks and events without videos have no author;
- `soundUrl` — for sounds and videos on a sound: link to the sound page (tiktok.com/music/…). Used for duplicate checks;
- `howToUse` — ideas for at least 3 niches as "Beauty: … Auto: … Fintech: …"; rotate niches;
- `howTo` — link to a "how to make it" breakdown or template (tutorial, CapCut template), if any;
- `platform` — Instagram | TikTok | YouTube | X | Threads | Douyin | Xiaohongshu | Naver | Other | All;
- `type` — Format | Visual | Sound | Topic | News hook | Discussion / meme | Season | Event:
  - "News hook" — unplanned news (outage, release, record, CEO exit), lives 3–5 days;
  - "Event" — scheduled (award, tour, show, premiere) and moments inside it;
  - "Discussion / meme" — discussed without a news trigger;
  - "Topic" — a long consumer theme lasting months (e.g. JOMO);
- `origin` — International | Regional | Local (Local = `localMarket`, Regional = `region` from settings);
- `stage` — rising | peak | declining. Required only for `tier` "Trend" (except "Season"); not set for "Find" and "Page";
- `lifespan` — rough life: sound ~1–2 weeks, format ~a month, discussion — a few days;
- `months` — only for "Season": active months (numbers 1–12);
- `moodFit` — true if the technique suits moody/aesthetic posts;
- `niche` — comma-separated niches from "Who the library is for" (or "all niches"); `client` — the client it was found for, if any;
- `examples` — 3–6 `{url, label}` objects (a "Find" can have 1), only links to specific videos or posts on Instagram, TikTok, YouTube, Threads or the market's main video platform (X, Douyin, Xiaohongshu, Bilibili, Naver Clip / Naver TV); no Telegram channels, Pinterest, articles or compilations (a breakdown goes only to `howTo`); the original video first. Exception: for "Page" the first link is the brand profile. A news hook without videos may have empty `examples`;
- `hook` — what happens in the first second and what text is on screen;
- `thumb` — a frame from the original video (no celebrities or children), uploaded with `upload_asset`; store the **asset id** that `upload_asset` returns (its `opaque_id`, not a URL) — the library page renders it from that id;
- `source` — joined with ", " from: vidIQ | Apify | Spyglass | News | Instagram | TikTok | YouTube | Threads | Know Your Meme | Creative Center | Curaeted | Pinterest | Google Trends | Telegram | Web round-up | User (saved) | User (repost) | User (Pinterest) | User | Manual (added on the library page);
- `status` — New | In progress | Used | Outdated. Shared across all clients;
- `usedFor` — which clients it was already used for;
- `foundAt` — date and time added (ISO 8601);
- `checkedAt` — when the stage was last rechecked (ISO 8601);
- `verified` — false if links weren't checked in the browser (by default not set);
- `expiresHint` — for news hooks and seasonal formats, the date after which the trend loses meaning, always ISO `YYYY-MM-DD` (the library page compares it as a string). Human-readable dates in `signal`/`evidence` may use the user's locale.
