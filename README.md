# Sideline Scoreboard

A one-page volleyball scoreboard for keeping score from the bench on a phone. Tap a team's half of the screen to give them the point. No install, no accounts, no network — one HTML file.

**Live:** https://pfonbuena.github.io/Volleyball-scorecard/

## What it does

- **Tap to score.** Each team owns half the screen. Tapping also moves the serve indicator to that team.
- **Set tracking.** Best of 3 by default: sets 1 and 2 to 25 (cap 30), deciding set 3 to 15 (cap 20). A Best of 5 toggle moves the deciding set to 5.
- **Timeouts.** A T/O button in each team's corner with two pips, matching the two-per-team-per-set allowance. Resets when the set ends.
- **Undo.** Every scoring action, timeout, serve change and swap is undoable. `Z` on a keyboard.
- **Team colors.** A color picker per side. Score text switches between white and near-black automatically, whichever has the higher contrast ratio against the chosen color.
- **Rules sheet.** UIL Texas junior-high (7th & 8th grade) match format plus a referee signal reference with drawn diagrams.
- **Picks up where you left off.** Match state is kept in `localStorage`, so closing the tab mid-match is fine.

## Keyboard

| Key | Action |
| --- | --- |
| `←` | Point, left team |
| `→` | Point, right team |
| `Z` | Undo |
| `Esc` | Close the rules sheet |

## Rules note

The scoring follows the UIL volleyball rally scoring regulations for junior high: best of 3 to 25 capped at 30, with the third set to 15 capped at 20 (some districts play the third to 25). District and tournament directors set their own variations, so confirm the format with the host before first serve.

Source: [UIL Volleyball Rally Scoring Regulations](https://www.uiltexas.org/volleyball/page/volleyball-rally-scoring-regulations)

The referee signal diagrams are simple original drawings meant as a memory aid, not a substitute for the official NFHS signal chart.

## Running it

Open `index.html` in any browser. That's the whole app — no build step, no dependencies beyond two Google Fonts.

## License

MIT
