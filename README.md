# Endless Chain

An unlimited word-chain puzzle that runs in the browser. Each puzzle is a chain of 7 words where the first and last are given. Fill in the 5 middle words so every neighboring pair forms a phrase or compound word (for example SUN → FLOWER → POT).

Unlike daily puzzles, you can play as many chains as you like. Hit **Next puzzle** or **New** any time.

## Features

- Unlimited play, with puzzles shuffled so you don't see repeats until you've seen them all
- Tap any open row to solve in any order
- Wrong guesses keep the correctly placed letters and flash yellow/gray feedback
- Reveal Letter hints, score, timer, and a best-score record saved in your browser
- On-screen and physical keyboard support, light and dark mode, mobile friendly
- No build step, no dependencies: one `index.html` file

## Play locally

Open `index.html` in any browser.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `endless-chain`).
2. Upload `index.html`, `README.md` and `LICENSE` to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then Save.
5. After a minute, your game is live at `https://YOUR-USERNAME.github.io/endless-chain/`.

## Add your own puzzles

Open `index.html` and find the `CHAINS` array near the top of the script. Add a new line with 7 words where each neighboring pair makes a common phrase:

```js
["SUN","FLOWER","POT","HOLE","PUNCH","LINE","DANCE"],
```

## License

MIT, see `LICENSE`.
