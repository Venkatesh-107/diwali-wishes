# Diwali Wishes

A Diwali greeting with a modern retro-90s interface, 3D diya scene, illustrated character expressions, two festival games, and a shareable scorecard.

## Play online

Visit [Diwali Wishes](https://venkatesh-107.github.io/diwali-wishes/).

## Player flow

1. Enter a name and choose male or female.
2. See a personalized “Happy Diwali, [name]!” greeting.
3. Warm up with the trick question: “Tell me a joke.” The answer is the word `joke`; players get three guesses and an optional hint after the second incorrect guess.
4. Play **Diya Dash**: move the diya to catch 8 falling lights before the 35-second timer expires. Use arrow keys or A/D, the on-screen controls, or drag on the playfield.
5. Play **Rangoli Memory**: watch the petals light up and repeat the growing sequence. It has six petals and up to five rounds.
6. View the scorecard, then copy the site link or share the wish using your device’s share menu.

Each caught light is worth 125 points and each cleared memory round is worth 200 points. The whole experience has ambient animated firework bursts, rising cracker trails, and festive string lights around the wishing cards and page. The scorecard adds a glowing night-sky celebration inside and around its panel. Its **Copy link** action copies the current site URL; **Share wish** opens the native sharing menu where available, and copies the link on browsers without native sharing.

## Run locally

Serve this folder with a static file server:

```sh
python3 -m http.server 8000
```

Open `http://localhost:8000`. The app and its styling are in [index.html](./index.html). Three.js and Google Fonts load from CDNs for the 3D scene and typefaces. If Three.js or WebGL is unavailable, the game still works with a decorative diya fallback.

## Character expressions

The guide’s supplied character poses are in `assets/character/`. Its double-size circular, bordered portrait sits to the left of a large, high-contrast cloud speech bubble above the card, with a clear gap between them. The bubble and pose change for greetings, hints, thinking, and celebrations. If all three riddle guesses are missed, the guide playfully reveals the answer based on the selected gender. Decorative icons are inline SVGs rather than emoji.

The footer credits Venkatesh and links to the GitHub profile [@Venkatesh-107](https://github.com/Venkatesh-107). It stays anchored to the bottom, wraps on narrow screens, and accounts for mobile safe-area insets. Dialog cards are sized to avoid internal scrolling.

## Publish with GitHub Pages

GitHub Pages is enabled for the `main` branch root. New commits to `main` publish automatically.
