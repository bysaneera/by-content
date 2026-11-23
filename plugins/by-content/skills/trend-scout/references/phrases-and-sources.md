# Slang dictionary and the sources collection

Part of the trend-scout skill. Read together with its SKILL.md.

## Slang dictionary (collection `phrases`)
Words and phrases that everyone starts saying — for captions, on-screen text and scripts. Track them along the way in every run:
- read captions, on-screen text and comments in TikTok and Instagram results: a word or phrase repeated by different creators is a candidate;
- TikTok search suggestions ("what does … mean") and Google Trends for the local market (rising "what does [word] mean") — confirmation;
- X and the market's messengers (Telegram for CIS) — where people discuss "suddenly everyone started saying…".
Speech in videos can be transcribed with a video-watching skill; words that are only spoken count too.
A word enters the dictionary if 3+ different creators used it in the last 2 weeks and mentions are growing. Worn-out words — skip. Target 1–3 words a week, not daily.
Fields: `phrase`, `meaning` (what it means and how it's used), `signal` (how many creators, where seen), `howToUse` (how a brand can use it, 2–3 niches), `examples` (2–4 `{url, label}` links), `origin`, `stage`, `source`, `status` (New | In progress | Outdated), `foundAt`. Save to `phrases` by the "Saving" rules (slug without date, check that `doc_id` is free). In the morning message new words go in a separate "Slang" line.

## Collection `sources`
Fields: `handle`, `platform`, `url`, `kind` (editing breakdowns | trend round-ups | aesthetics | memes | media), `region` (International | Regional | Local), `note`, `addedAt`.
Starts empty, except suggest @curaeted.co (Instagram, aesthetics) on first run. If you notice an account that regularly posts breakdowns or round-ups (e.g. monthly "trends of the month" for the region) — suggest adding it to `sources`; don't add it yourself.
