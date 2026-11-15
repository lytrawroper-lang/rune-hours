# Rune Hours

A single-page rune app: the rune of the current hour, a rune wheel, readings,
a dictionary, games, and tools for writing in runes.

Live at: https://lytrawroper-lang.github.io/rune-hours/

## What's on the page

- **The Hours** — the rune of this hour, runes of the night and day, rune of
  a birth hour, the moon tonight, the Wheel of the Year, and runes of the
  day, week and month.
- **Cast** — the three-ring Rune Wheel, rune readings (3, 5 and 9 runes),
  a yes/no stone, and a journal for saved readings and casts.
- **Learn** — the 24-rune Elder Futhark dictionary (plus Younger Futhark and
  Anglo-Saxon tabs), lore and rune history, a quiz, and games (memory match
  and draw-a-rune).
- **Yours** — write in runes, bind runes, and settings (name, paint colour,
  sound and alarm, sunrise/sunset hours).

## The hour tables

The starting times and runes are copied from a chalk board. The night table
runs 4:30 PM–7:00 AM (12 runes) and the day table 7:00 AM–4:30 PM (12 runes);
with sunrise/sunset mode on, the split follows the sun for a chosen place.

Note: the tables place Perthro just before Eihwaz, which differs from the
usual rune order used in the dictionary. See the note on the Hours page.

## Running it

No build step and no dependencies. Open `index.html` in a browser, or serve
the folder (`python3 -m http.server`) and visit http://localhost:8000/.

The only external requests are Google Fonts.

## Files

- `index.html` — the whole site: markup, styles and script in one file.

## Where the rune data lives

All in `index.html`:

- `dict` — the 24 runes: name, letter sound, literal meaning, linked ideas.
- `P` — the carved glyph for each rune, as SVG path data.
- `DEF` — the night and day hour tables.
- `MAP` — the letter-to-rune map used by Write in Runes, with TH, NG and X
  handled as special cases.

## Contributing

Suggestions and fixes are welcome as issues or pull requests.
