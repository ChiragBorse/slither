# Slither

A calm, good-looking snake game that runs in your browser. It comes as a single HTML file with no build step and no dependencies.

**Live demo:** https://YOUR-USERNAME.github.io/slither

## Features

- **Two modes**
  - **Classic:** solid walls, and the speed builds gently as you grow.
  - **Zen:** walls wrap around, and only your own tail ends a round.
- **Light and dark mode** with a toggle in the navigation bar. It follows your device setting on the first visit and remembers your choice afterwards.
- **Smooth animation:** the snake glides between grid cells, and eating an orb triggers a particle burst and ring.
- **Score history:** your best score and last 14 rounds are saved on your device and drawn as a line chart.
- **Works on desktop and mobile:** keyboard, swipe and on-screen direction buttons.
- **Accessible:** keyboard focus styles, and reduced-motion preferences are respected.

## Controls

| Action | Keyboard | Touch |
| --- | --- | --- |
| Steer | Arrow keys or `W` `A` `S` `D` | Swipe on the board, or use the on-screen buttons |
| Pause or resume | `Space` or `P` | Tap Resume on the overlay |
| Start or restart | `Space` or any direction key | Tap Start or Play again |

## Run it locally

1. Download or clone this repository.
2. Open `index.html` in any modern browser.

That's all. There is nothing to install.

## Deploy with GitHub Pages

1. Push `index.html` to a public repository.
2. Go to **Settings > Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. Save, wait a minute or two, and your site will be live at `https://YOUR-USERNAME.github.io/REPO-NAME`.

## Tech

- Plain HTML, CSS and JavaScript in one file
- HTML5 Canvas for the game board
- Inline SVG for the score chart
- Fonts from Google Fonts: Fraunces, Plus Jakarta Sans and JetBrains Mono (system fonts are used as a fallback if they can't load)
- `localStorage` for the best score, round history and theme choice

## Customize

- **Board size:** change `var N = 18;` in the script.
- **Speed:** edit `baseTick()` and the minimum values in the `step()` function.
- **Colors:** edit the CSS variables at the top of the `<style>` block (`--accent`, `--mint`, `--bg` and others).
- **Name:** search for "Slither" and replace it.

## Notes

- Scores and settings are stored in your browser, so they don't carry over to another device or browser.
- Clearing your browser data resets your scores.

## License

Free to use, modify and share. Add a license of your choice, such as MIT, if you want to make the terms explicit.
