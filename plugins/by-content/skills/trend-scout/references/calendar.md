# Seasonal themes, market calendars and events

Part of the trend-scout skill. Read together with its SKILL.md.

## Seasonal themes (`type` "Season")
Cultural themes that return every year. They don't expire; each year check for a reason to boost the theme (anniversary, new season, remake) and add to `signal`. Status "Used" is not set for them — the theme is adapted anew each time. Build the starter list on first run for the user's market (holidays, school year, local celebrations) plus global ones. Global pop-culture seasons, for example:
- **September–October:** "Twilight", "Gilmore Girls", "Practical Magic", autumn aesthetics, back to school, pumpkin spice, Halloween;
- **November:** Black Friday, Cyber Monday and 11.11, holiday prep, advent calendars;
- **December:** "Harry Potter", "Home Alone", "Love Actually", "Elf", local holiday classics, year in review, Pantone colour of the year;
- **January–February:** "new year, new me", Valentine's Day;
- **spring–summer:** graduation, vacation, summer in the city, "hot girl summer"-type seasonal memes.
Market calendars (pick the user's market; check floating dates every year):
- **US:** Super Bowl, Valentine's, St. Patrick's, Easter, Mother's Day, Memorial Day, Pride Month, Father's Day, Fourth of July, back to school (August), Labor Day, Halloween, Thanksgiving, Black Friday / Cyber Monday, Hanukkah, Christmas;
- **UK:** Valentine's Day, Pancake Day, Mother's Day (March), Easter, bank holidays, Father's Day (June), Halloween, Bonfire Night, Black Friday, Christmas markets, Boxing Day;
- **Continental Europe:** Carnival / Fasching, Easter, Mother's Day (May in most countries), Midsummer (Nordics), summer and winter sales seasons, St Nicholas (6 December), Christmas markets, Three Kings (6 January, Spain);
- **Kazakhstan / CIS:** New Year, 14 February, 8 March, Nowruz, 1 September, Independence Day, Mother's Day (date differs by country);
- **Japan:** Shōgatsu (New Year, the biggest holiday — nengajō cards, osechi, fukubukuro lucky bags), Coming of Age Day, Valentine's Day (women give chocolate), White Day (14 March, return gifts), sakura / hanami season (late March–April, forecast by region), new school & work year (April), Golden Week (late April–early May), rainy season, Tanabata (7 July), summer festivals and fireworks, Obon (mid-August), autumn leaves (kōyō), Halloween, Black Friday, Christmas (a couples' holiday + Christmas cake and fried chicken), year-end parties (bōnenkai);
- **South Korea:** Seollal (Lunar New Year), Valentine's Day, White Day (14 March), Black Day (14 April), Children's Day (5 May), Parents' Day (8 May), Teachers' Day, cherry blossoms, summer vacation, Chuseok (autumn harvest holiday), Hangul Day (9 October), Suneung exam day (November), Pepero Day (11.11), Christmas (couples), year-end;
- **China / Greater China:** Spring Festival (Lunar New Year, red envelopes), Lantern Festival, 520 (20 May, "I love you"), 618 shopping festival, Dragon Boat Festival, Qixi (Chinese Valentine's), Mid-Autumn Festival (mooncakes), National Day Golden Week, Double 11 (Singles' Day);
- **Southeast Asia:** Lunar New Year, Ramadan and Hari Raya / Lebaran, Songkran (Thailand, April), 9.9 / 10.10 / 11.11 / 12.12 mega sales;
- **cross-market:** Lunar New Year, Ramadan and Eid, Diwali.

**Platforms by market.** Adjust the search route to where trends live: **Japan** — X (Twitter) is central for trends and memes, plus TikTok, Instagram, YouTube Shorts and LINE; check Yahoo! Japan real-time search and X trending. **South Korea** — Instagram, YouTube Shorts, TikTok, Naver (blogs, Naver DataLab instead of Google Trends), KakaoTalk; K-pop comebacks and challenge dances are a major trend source. **China** — Douyin, Xiaohongshu (RED), Weibo hot search, Bilibili (often need the user's own access; skip if unavailable and say so).

## Events and cultural moments (`type` "Event")
Big events produce two kinds of trends: the event itself (line-up, show, award) and viral moments inside it that viewers re-shoot and retell. Catch both.

**Track constantly:** world tours and concerts of big artists, including concerts in the user's local market; fashion shows and weeks, awards, festivals, sports finals, big premieres and releases; moments from them that viewers repeat.

**News of the day — in every search.** Besides social media, web-search the top news of the last 24 hours that everyone is talking about: space and tech (launches, product presentations), big game, film and album releases, sport and wins of local athletes, records, loud brand launches. Take it if 2+ outlets write about it and TikTok already has videos. `type` "News hook", `stage` "peak", `lifespan` 3–5 days, `expiresHint` required; `howToUse` — how to joke about it in 3+ niches; `examples` — eyewitness footage. No politics, wars, disasters, crime or deaths.

**Annual calendar (check dates by search every year):**
- January–February: Golden Globes, Grammys, Super Bowl (ads and halftime show), fashion weeks;
- March: Oscars;
- April: Coachella;
- May: Met Gala, Eurovision, Cannes Film Festival;
- June–July: Wimbledon, big summer festivals;
- September: fashion weeks, Apple event, Emmys;
- October: Victoria's Secret show;
- autumn: Coachella line-up announcement;
- US-specific: NFL Draft (April), NBA Finals (June), NFL season start (September), World Series (October), Thanksgiving Day Parade (November);
- December: year-in-review (Spotify Wrapped and similar).
Add local events for the user's market on first run. 1–2 days before an event and the day after — a separate search: what's discussed, which moments were re-shot, which looks are analysed.

**How to record:** `type` "Event"; `signal` — event date and who covers it; `howToUse` — ideas for at least 3 niches; `stage` and `lifespan` — accounting for the second wave. If the user spotted a moment and there are no confirming videos yet — save with status "New" and a note in `signal`, then find 3+ examples in the browser.
