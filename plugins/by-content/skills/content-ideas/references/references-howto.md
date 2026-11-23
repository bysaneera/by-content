# References — where to take them, slots by format, how to choose, technical steps

Part of the content-ideas skill. Read together with its SKILL.md.

## 6. References

### Where to take them — strictly in this order
1. **The project's Pinterest board.** If the project files contain a board link — use it. Otherwise, if the user's Pinterest profile is known (from memory, project files or the library settings `pinterestProfile`), open it in the browser (the user is logged in), open the board list and find the board named after the project — case-insensitive and in all spellings (Latin and local script). If several match — take the closest. If the board has sections ("Photo", "Graphics", "Covers") — search the needed one first. No profile known — ask once for the profile or board link; if there's no answer, go to step 3.
2. **Similar to the board.** If the board lacks something suitable — take from "More ideas" under the board and "More like this" under its pins.
3. **General search** (Pinterest, Vimeo, aesthetic videos) — only if the first two steps gave nothing suitable. Then one line at the start of the reply: "No board for [client]" or "Nothing on the board for [what] — part comes from general search".
For each reference state the source: "board", "similar" or "general search".

### A reference strictly matches the format
The picture in a slot must match the slot's format and the post's content: a "photo" slot — a photo, "graphics" — graphics, "motion" — animation or gif. If the post is about family — a family photo on the cover; if it's product graphics — product layout.

**Slots by basic format:**
- **Photo.** The main photo reference and next to it [1] Angle, [2] Light, [3] Props, matching the reference. If the post is about a look or style — 3–4 photos with different posing (in motion, close-up, from behind, seated) with a caption on which pose we take and why.
- **Video.** Storyboard [1] Start, [2] Middle, [3] End — the visual of the frames (light, colour, location, posing). For trend and entertaining types — plus 1–2 links to real videos as a format example (from the library card's `examples`, Spyglass, Apify, vidIQ) with the @author and one phrase on what we take (hook, transition, sound). For other types — optional. Write "what we take" only from what you saw: from the card's `hook` or by watching the video with a video-watching skill. Don't download others' videos — link only.
- **Graphics.** Layout, fonts, plates, how text sits on the background.
- **Motion.** Animation style, transitions, how text moves (often gif and video pins).

**Combinations split slots between formats.** For example:
- "Photo + Graphics": [1] photo, [2] style of the graphics on top, [3] an example of the combination (if found).
- "Video + Motion": [1]–[2] video frames, [3] style of the effects on top.
Under each slot a label: "photo", "graphics", "video" or "effect". If the format is "Photo + Graphics" but the references are only photos — the post isn't ready, find the graphics.

**Carousel.** Two references: [1] cover, [2] what the graphics inside look like. Below — the approximate number of slides and one line on each.
**Stories.** [1] Hook, [2] Interactive, [3] Ending.
**Variants.** If there are two real directions — "Variant A / B", differing in approach, not three similar pictures.

### How to choose
- Start from everything at once: topic mood, brand book, the client's past references, the trend (if any), people and shoot location. Not a literal illustration of the topic, but the frame that fits the mood best.
- Choose for the scenario and location: shooting outdoors — city photos, in the mountains — mountains. The client's product may not be in the reference.
- Under each picture, briefly: what we take and where the product accent is. E.g.: "We take the low angle and motion blur. Product accent: it's closest to the camera."
- General search queries — in English, 4–7 words of visual features: "street style film photography city candid", "product drop poster", "day in my life color block time carousel". If results go off — rephrase.
- Select by eye from a screenshot, not the first pins. Pictures the user sent in this chat or that were already on the client's past boards are not passed off as new finds: they set the direction, but slots get new pins (from the project board — allowed). Don't repeat one pin in different posts. Others' photos with children and celebrities can be used as a reference (as a pin link), not as the final visual.

### Technically
1. In the browser open the board (or `https://www.pinterest.com/search/pins/?q=<query>`), wait ~3 s, take a screenshot (scale 0.6). Via a JavaScript tool collect from `div[data-grid-item]` the pin id (from href `/pin/<id>`), the image src and the card centre coordinates to match with the screenshot.
2. Download images to the working folder at `https://i.pinimg.com/736x/<path>.jpg` (replace originals and 474x with 736x). For gif and video pins take the .jpg as a preview frame, caption the slot "animation — see link" and put the pin link. If i.pinimg.com can't be downloaded from the working environment — don't substitute another image: leave the pin link in the slot and say so in one line.
3. Build a contact sheet (PIL) and check by eye that images match the slots, format and captions.
4. External images don't load in published artifacts — publish them as files together with the board (publish_files).
5. Close your browser tab.
