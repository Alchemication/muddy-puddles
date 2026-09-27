# Peppa's Muddy Puddles 🐷

A tiny, toddler-friendly browser game that teaches the arrow keys. It's one HTML file with no dependencies, and everything in it was generated with AI.

Walk Peppa to the muddy puddle with the arrow keys. Each splash earns a ⭐.

## Play

Open `index.html` in a browser and click **Play**.

- **Level 1:** a single row, so only ◀ ▶ are needed.
- **Level 2:** after 5 puddles the field grows to 3 rows, and ▲ ▼ join in.
- On-screen arrows light up when pressed, and a voice says the direction.
- If your child gets stuck, the arrow they need glows. After several wrong keys, a gentle voice hint follows.
- There's no way to lose. Wrong keys and bumping into edges are harmless.
- The built-in music is an original tune that reacts to the game. It gets calmer while waiting, bouncier while walking and twinkly near the puddle. The key changes after each splash, and a soft beat joins in at level 2.
- The 🎵 button (mouse only) turns music on and off. Press Esc to leave full screen.

To use your own background music, put a `music.mp3` next to `index.html`. It's git-ignored, so it's never committed.

## Using it to test AI models

[PROMPT.md](PROMPT.md) has the short prompt that produced this game and a 15-point scorecard. Use them to compare how well different models handle intelligence and UX on the same task.
