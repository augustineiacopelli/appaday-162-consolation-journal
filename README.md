# Consolation Journal | AppADay 162

**Category:** S (Spirituality)  
**Live:** https://augustineiacopelli.github.io/appaday-162-consolation-journal/  
**Portfolio:** https://augustineiacopelli.github.io/appaday/

Log the interior movements of a retreat as consolation or desolation using St. Ignatius's Rules for the Discernment of Spirits. Each entry records what came just before and three discernment questions, with a standing caution against deciding in desolation and a color ribbon of your day.

## How it works

Tap Consolation or Desolation to name the movement. Each choice carries a short gloss of Rule 3 or Rule 4 so the distinction is in front of you. Set the time (the Now button fills the current moment), write up to 280 characters about what happened just before, and optionally answer three questions: is this leading toward God or away, does it leave peace or agitation, and is this a time to decide or to hold steady. Save stays disabled until a kind is chosen.

The Rule 5 card is always visible. When you mark desolation it turns slate and says so, and if you mark Desolation and Decide together it warns you inline to postpone the decision. Below it, a counsel line paraphrases Rules 6 to 8 during desolation and Rules 10 and 11 during consolation; tap it for the next counsel.

The day view shows a ribbon running from at least 6 AM to 10 PM (wider if you log earlier or later). Each entry colors the ribbon gold (C) or slate (D) until the next entry; on today the last segment runs to the current time. Prev, Today, and Next move between days, and the time ordered list below shows each entry with its answers as chips and a delete button.

## The Rules it draws on

The Rules for the Discernment of Spirits appear in the Spiritual Exercises of St. Ignatius of Loyola. The app uses the First Week rules: Rule 3 (consolation), Rule 4 (desolation), Rule 5 (make no change in desolation), Rules 6 to 8 (how to stand in desolation), and Rules 10 and 11 (how to receive consolation). All wording in the app is a short paraphrase. The journal is a notebook, not a director; bring what you notice to a spiritual director.

## Privacy

Everything is stored in your browser's localStorage under the key `appaday-162-journal`. Nothing is sent anywhere, there are no accounts, and the app makes no network requests beyond loading its own page, icon, and the shared Save to Phone script. If storage is unavailable (for example in some private browsing modes), entries are kept for the session only and the app tells you so.

## Export and import

Open the gear menu. Export downloads `consolation-journal-YYYY-MM-DD.json`. Import validates the file, drops anything malformed, and then offers Merge (keep your entries and add new ones by id) or Replace. Clear all entries asks first through an in-app confirmation sheet.

Data shape:

```json
{ "v": 1, "entries": [ { "id": "...", "ts": 1760000000000, "kind": "consolation", "before": "...", "toward": "toward", "tone": "peace", "season": "steady" } ] }
```

`kind` is consolation or desolation; `toward` is toward or away; `tone` is peace or agitation; `season` is decide or steady; the last three may be null.

## Build notes

Single index.html with inline CSS and JS, system serif font stack, no frameworks, no canvas, no fetch calls, ASCII clean source, 44px tap targets, tested at 375px.
