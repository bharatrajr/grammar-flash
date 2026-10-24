# Grammar Flash — SSC CGL

Anki-style spaced-repetition flashcards for:

- **100 Grammar Rules** (Aman Sir's 100 concepts, simplified, with errors fixed)
- **Direct & Indirect Speech** — every rule and edge case
- **Active & Passive Voice** — every rule and edge case

No build step, no server, works offline once opened.

## Put it on GitHub Pages

1. Create a new repository (e.g. `grammar-flash`) on GitHub.
2. Upload every file in this folder (keep the `icons` folder).
3. Repo → **Settings → Pages** → Source: *Deploy from a branch* → Branch `main`, folder `/ (root)` → Save.
4. Open `https://<your-username>.github.io/grammar-flash/` after a minute.
5. On Android Chrome: menu → **Install app**. On iPhone Safari: Share → **Add to Home Screen**.

## Features

- SM-2 scheduling like Anki: Again / Hard / Good / Easy with next-interval preview, learning & relearning steps, day rolls over at 4 am
- Daily new-card and review limits; decks and individual topics can be switched on/off
- Three card types: recall the rule, spot & fix the error, convert (narration/voice)
- Optional **type-the-answer** mode with a word-by-word diff for convert cards
- Cram / practice mode (all, starred, weak spots, a topic) that doesn't touch your schedule
- Browse with search and filters; star, suspend or reset any card; leech detection
- Stats: retention, streak, 20-week heatmap, 14-day forecast, mastery per topic
- Undo, keyboard shortcuts, swipe to grade, read-aloud, dark mode, text size
- Export / import backup (progress lives in the browser's localStorage)

## Editing cards

All cards are in `cards.js` as `[deck, topic-or-concept-number, type, front, back]`.
Wrap words in `**double stars**` to highlight them. A card's progress is keyed to its deck + front text, so editing the *back* keeps progress; editing the *front* makes it a new card.

After changing anything, bump `VERSION` in `sw.js` (e.g. `gf-1.0.1`) so installed copies update.

## Keyboard

Space = flip / Good · 1–4 = grade · Z = undo · S = star · T = read aloud · Esc = exit
