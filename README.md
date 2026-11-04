# Dotted

A dot-matrix logic puzzle inspired by Nothing's design language. Fill the board with red and black keys without breaking three rules.

> Fan project, not affiliated with Nothing.

## Rules

1. No three keys of the same color in a row or column.
2. Every row and column has an equal number of each color.
3. No two rows or columns can be identical.

Tap a key to cycle: empty, red, black.

## Modes

- **Time Attack:** solve as many boards as you can; each solved board adds time.
- **Daily:** the same puzzle for everyone, every day.
- **Free:** no timer, pick your own board size.

## Design notes

- Light and dark themes share one component set; only surface and shadow values change.
- No image assets for the keys and panels: raised, pressed and error states are layered shadows and borders.
- Icons are pattern strings rendered as dots, so a new icon takes one line.

## Tech

Plain HTML, CSS and vanilla JavaScript in a single `index.html`. No build step, no backend. Progress and settings are stored in `localStorage`.
Fonts (Bitcount Single, Space Mono, Inter Tight) are loaded from Google Fonts, so an internet connection is needed on first load.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Contributing

Ideas, issues and pull requests are welcome: new modes, sounds, haptics, accessibility improvements, better difficulty curves.

## License

MIT, see [LICENSE](LICENSE).
