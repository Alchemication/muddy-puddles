# Peppa's Muddy Puddles 🐷

A tiny, toddler-friendly browser game that teaches the arrow keys. Each version is one HTML file with no dependencies, generated entirely by an AI model. This repo collects versions from different models so they can be compared side by side.

Walk Peppa to the muddy puddle with the arrow keys. Each splash earns a ⭐.

## Play

Open the root `index.html` in a browser and pick a model with the arrow keys and Enter, or with a click. Then click **Play**. The selection page has its own friendly background tune, which starts on the first click or key press. Each game has its own music.

| Model | Folder |
|---|---|
| Claude Opus 5.5 | [models/claude-opus-5-5](models/claude-opus-5-5/index.html) |

## The Claude Opus 5.5 version

- **Level 1:** a single row, so only ◀ ▶ are needed.
- **Level 2:** after 5 puddles the field grows to 3 rows, and ▲ ▼ join in.
- On-screen arrows light up when pressed, and a voice says the direction.
- If your child gets stuck, the arrow they need glows. After several wrong keys, a gentle voice hint follows.
- When Peppa lands in the puddle, it squishes, ripples spread out and mud drops arc up and fall back.
- There's no way to lose. Wrong keys and bumping into edges are harmless.
- The built-in music is an original tune that reacts to the game. It gets calmer while waiting, bouncier while walking and twinkly near the puddle. The key changes after each splash, and a soft beat joins in at level 2.
- The 🎵 button (mouse only) turns music on and off. Press Esc to leave full screen.

To use your own background music, put a `music.mp3` next to that model's `index.html`. It's git-ignored, so it's never committed.

## Adding a new model

1. Give the new model the prompt from [PROMPT.md](PROMPT.md).
2. Save its game as `models/<model-name>/index.html`, using a lowercase folder name with dashes, like `gpt-6` or `gemini-4-pro`.
3. Add one line to the `MODELS` list near the bottom of the root [index.html](index.html), plus a row to the table above.

## Using it to test AI models

[PROMPT.md](PROMPT.md) has the short prompt that produced this game and a 16-point scorecard. Use them to compare how well different models handle intelligence and UX on the same task.
