# Volleyball Scorekeeper

A lightweight, mobile-friendly volleyball scorekeeping web app. No installation required — open `index.html` in any browser and start scoring.

## Features

- **Tap to score** — tap (or click) each team's panel to add a point
- **Set tracking** — finish a set to record the winner; dot indicators show sets won
- **Undo / Redo** — step back or forward through every scoring action
- **Custom teams** — set team names and colors via the Settings menu
- **Keyboard shortcuts** — score and navigate without touching the screen
- **No dependencies** — single HTML file, works offline

## Usage

Open `index.html` directly in a browser. No server or build step needed.

### Scoring

| Action | How |
|---|---|
| Add point — Home | Tap the left (blue) panel |
| Add point — Away | Tap the right (red) panel |
| Undo last action | `←` toolbar button or `Ctrl+Z` |
| Redo | `→` toolbar button or `Ctrl+Y` |

### Keyboard shortcuts

| Key | Action |
|---|---|
| `←` or `A` | Score for Home |
| `→` or `D` | Score for Away |
| `Ctrl+Z` / `Cmd+Z` | Undo |
| `Ctrl+Y` / `Cmd+Y` | Redo |

### Bottom toolbar

| Button | Action |
|---|---|
| Undo / Redo arrows | Step through scoring history |
| Checkmark (blue) | Open "Finish Set" — records the set winner and resets current scores to 0 |
| Refresh (red) | Reset everything — clears all scores and set counts |
| Gear | Open Settings — change team names and panel colors |

### Finishing a set

Tap the blue checkmark to open the Finish Set dialog. It shows the current scores and names the leading team as set winner. Confirming awards the set and resets both scores to 0. Tied sets are recorded with no winner awarded.

## Customization

Open Settings (gear icon) to change:
- Home and Away team names (up to 16 characters)
- Home and Away panel colors (color picker)

Settings are applied immediately and are included in the undo history.

## Running locally

```bash
# Clone the repo
git clone https://github.com/johnfettig/volleyball-scorekeeper.git
cd volleyball-scorekeeper

# Open in your default browser
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

## License

See [LICENSE](LICENSE).
