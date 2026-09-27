# Peppa's Muddy Puddles 🐷

A toddler-friendly browser game that teaches the arrow keys. Each version is one HTML file with no dependencies, generated entirely by an AI model. This repo collects versions from different models so they can be compared side by side.

Walk Peppa to the muddy puddle with the arrow keys. Each splash earns a ⭐.

## Play

**Online:** https://alchemication.github.io/pepa-slop/. It's redeployed automatically on every push to `main` that changes the games.

**Locally:** open the root `index.html` in a browser and pick a model with the arrow keys and Enter, or with a click. Then click **Play**.

The selection page has its own friendly background tune, which starts on the first click or key press. Each game has its own music.

| Model | Folder |
|---|---|
| Claude Opus 5.5 | [models/claude-opus-5-5](models/claude-opus-5-5/index.html) |

## The Claude Opus 5.5 version

### Gameplay
- **Level 1:** a single row, so only ◀ ▶ are needed.
- **Level 2:** after 5 puddles the field grows to 3 rows, and ▲ ▼ join in.
- There's no way to lose. Bumping into an edge makes Peppa wiggle, and holding a key down moves her only one step.
- **Space** makes Peppa jump and oink.

### Teaching the keys
- Big on-screen arrows are laid out like a real keyboard. They light up when pressed, and clicking them moves Peppa too.
- A voice says each direction ("left", "up") and cheers "Muddy puddle! Hooray!".
- After 4 seconds without a key press, the arrow your child needs glows.
- **Wrong keys:** the right arrow glows straight away. After 3 wrong keys in a row, the voice gives a gentle nudge like *"Try the right arrow!"*, at most once every 8 seconds. In level 1, ▲ ▼ count as wrong keys.

### Toddler-proofing
- The **Play** screen turns on sound and full screen.
- Keys that would scroll or change the page are blocked. Esc and normal shortcuts still work for adults.
- The layout fits any screen without scrolling.

### Phones and tablets
- **Swipe** anywhere to move Peppa. Small taps are ignored, so only real swipes count. The on-screen arrows can be tapped too.
- Held upright, the arrows sit under the field and everything is sized to the screen width. Sideways, it uses the same layout as on a computer.
- The page never scrolls, zooms or pull-to-refreshes while playing.
- Tip: on iPhone, the silent switch mutes the music and sounds. Adding the page to the Home Screen gives it the whole screen.

### Splash
When Peppa lands in the puddle, it squishes, two ripples spread out and mud drops arc up and fall back. It's timed to her landing, together with a soft "bloop" and a rising chime.

### Weather
The weather moves one step after each puddle: ☀️ sunny → ⛅ cloudy → 🌧️ light rain → 🌈 rainbow → ☀️ sunny. Each change fades over about 3 seconds:
- The sky and grass change colour.
- Clouds drift in and cover the sun.
- Light rain falls over the field only, never over the arrow keys.
- A soft rainbow appears after the rain.

### Sound and music
- Every sound is soft. Notes fade in and out, and everything goes through a limiter and a gentle high-frequency cut.
- The **built-in music** is an original four-part tune that reacts to the game:
  - It's calmer while your child is thinking, bouncier while Peppa walks, and twinkly when she's one step from the puddle.
  - It changes key after each puddle and plays a fanfare at the end of each round.
  - In level 2, a soft beat joins in and the tempo picks up slightly.
- **The music follows the weather.** Cloudy makes it a little slower and softer, with a held chord. Rain makes it dreamy, with little "raindrop" plinks. The rainbow brings a harp run and extra sparkle.
- Sound effects play in the music's current key, so everything fits together.
- The music gets quieter whenever the voice speaks.
- The 🎵 button turns music on and off. It only responds to the mouse, so key-mashing can't switch it off.

## Adding a new model

1. Give the new model the prompt from [PROMPT.md](PROMPT.md).
2. Save its game as `models/<model-name>/index.html`, using a lowercase folder name with dashes, like `gpt-6` or `gemini-4-pro`.
3. Add one line to the `MODELS` list near the bottom of the root [index.html](index.html), plus a row to the table above.

## Using it to test AI models

[PROMPT.md](PROMPT.md) has:
- A **full prompt** describing every feature above, for testing how well a model delivers a detailed spec in one go.
- A **blind** short variant, for testing whether a model thinks of good toddler UX on its own.
- A **23-point scorecard** that works for both.
