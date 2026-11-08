# Endless Chain

An unlimited word-chain puzzle that runs in the browser. Each puzzle is a chain of 7 words where the first and last are given. Fill in the 5 middle words so every neighboring pair forms a phrase or compound word (for example SUN → FLOWER → POT).

Unlike daily puzzles, you can play as many chains as you like. Finish one and hit **Next puzzle**, or tap the ↻ button to skip.

## Features

- Unlimited play with 36 chains, shuffled so none repeat until you have seen them all
- Three difficulty levels: Easy (first letters filled in), Normal, and Hard (no color feedback)
- Tap any open row to solve in any order, or use the up and down arrow keys
- Wrong guesses keep correctly placed letters and flash yellow/gray feedback
- Reveal Letter hints, live score, and a timer that pauses when the tab is hidden or a window is open
- Progress is saved automatically, so a refresh will not lose your game
- Stats screen (solved, best score, average, perfect chains) saved in your browser
- Share button that copies an emoji summary of your result
- On-screen and physical keyboard support, light and dark mode, mobile friendly, screen reader labels
- No build step, no dependencies: one `index.html` file

## Scoring

Your score starts at the difficulty's base (Easy 80, Normal 100, Hard 120). It drops by 5 per revealed letter, 2 per wrong guess, and 1 for every 30 seconds (up to 25 points).

## Play locally

Open `index.html` in any browser.

## Publish on GitHub Pages

1. Create a new repository on GitHub (for example `endless-chain`).
2. Upload `index.html`, `README.md` and `LICENSE` to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, pick `main` and `/ (root)`, then Save.
5. After a minute, your game is live at `https://YOUR-USERNAME.github.io/endless-chain/`.

## Add your own puzzles

Open `index.html` and find the `CHAINS` array near the top of the script. Add a new line with 7 words in capital letters (2 to 9 letters each) where each neighboring pair makes a common phrase:

```js
["SUN","FLOWER","POT","HOLE","PUNCH","LINE","DANCE"],
```

Any line that is not exactly 7 capitalized words is skipped automatically, and a warning is printed in the browser console.

## License

MIT, see `LICENSE`.
