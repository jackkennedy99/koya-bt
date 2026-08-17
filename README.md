# Daily Brain Training

A seven-day set of short memory exercises. One game per day of the week; `index.html`
reads the visitor's device clock and shows the right one, with the option to play any
of the others.

## Files

| File | Day | What it trains |
|---|---|---|
| `index.html` | — | Landing page, day routing, calendar |
| `monday-names-and-faces.html` | Monday | Putting a name to a face |
| `tuesday-shopping-list.html` | Tuesday | Holding a list in your head |
| `wednesday-where-did-i-put-it.html` | Wednesday | Remembering places, not things |
| `thursday-tip-of-my-tongue.html` | Thursday | Finding a word you already know |
| `friday-hold-the-number.html` | Friday | Keeping something in the air |
| `saturday-what-happened-next.html` | Saturday | What stays with you from reading |
| `sunday-weekly-round.html` | Sunday | One short go at all six |

## How it works

Every file is self-contained — plain HTML, CSS and JavaScript in a single document.
No build step, no framework, no package install. The only external request is a
Google Fonts stylesheet, and the pages fall back to system serif and sans-serif
if it doesn't load.

Nothing is stored. No cookies, no local storage, no accounts, no analytics. Scores
exist in memory for the length of a session and are gone when the tab closes.

## Hosting

Drop all eight HTML files in the root of a repo and turn on GitHub Pages
(Settings → Pages → Deploy from a branch → `main` / `root`). No configuration needed.

Any static host works the same way — Netlify, Cloudflare Pages, or a folder on your
own domain. Keep the filenames as they are; `index.html` links to the others by
relative path.

## Content pools

Monday, Wednesday and Friday generate their material procedurally, so they don't
repeat in any noticeable way. Three days draw on written pools that will eventually
cycle:

- **Tuesday** — 14 shopping aisles, effectively non-repeating at 6–8 items a session
- **Thursday** — 76 words
- **Saturday** — 6 stories

Over a 90-day run that's roughly 13 visits to each day. Thursday and Saturday will
start repeating before the end; ~150 words and 12–15 stories would cover it
comfortably. Both pools are plain arrays near the top of their `<script>` block and
can be extended without touching anything else.

## A note on framing

These are exercises for practice and enjoyment. Nothing here is a test, a screening
tool, or an assessment of anyone's health, and the copy throughout is written to
avoid implying otherwise. If you edit the text, keep it that way.
