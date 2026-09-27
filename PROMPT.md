# The prompt

Every game in this repo is generated from this prompt in a single shot: one message, no follow-ups. The people who play the games do the comparing.

```
Build a Peppa Pig game as a single self-contained HTML file (no external
files, libraries or audio files) that teaches my 2-year-old the arrow keys.
Keep it large, simple and clear. Draw Peppa yourself and compose original
music; don't copy the show's artwork or theme tune.

Gameplay
- The arrow keys walk Peppa one step at a time across a grassy field to a
  muddy puddle. When she lands in it: a splash, a voice cheers, a star is
  added, and a new puddle appears somewhere else.
- Level 1 is one row, so only left and right are needed. After 5 puddles the
  field grows to 3 rows and up and down join in.
- No way to lose. Walking into an edge makes Peppa wiggle, holding a key
  moves her only one step, and Space makes her jump and oink.

Teaching
- Big on-screen arrows laid out like a keyboard. They light up when pressed
  and can be clicked or tapped.
- A friendly voice says each direction as she moves.
- After a few idle seconds, the needed arrow glows and Peppa turns and waves
  toward the puddle.
- Wrong keys: the needed arrow glows at once. Only after several misses in a
  row does the voice nudge ("Try the right arrow!"), at most once every few
  seconds.

Toddler-proofing
- A big Play button starts sound and full screen.
- Block keys that scroll or change the page; Esc and normal shortcuts still
  work for adults.
- Fits any screen without scrolling.

Phones and tablets
- Swiping anywhere moves Peppa (a tap is not a swipe).
- Held upright, the arrows go under the field, sized to the screen width.
- The page never scrolls, zooms or pull-to-refreshes.

Peppa
- Subtly alive: she breathes, blinks and wags her tail, and hops with
  swinging legs when she walks.
- After a splash she cheers with her arms up and gets mud spots that fade by
  the next puddle.
- In the rain she looks up at the sky now and then.

Weather
- It moves one step per puddle, never mid-move: sunny, cloudy, light rain,
  rainbow, then sunny again.
- Each change fades slowly: sky and grass colour, clouds over the sun, light
  rain over the field (not over the arrows), and a soft rainbow.

Splash
- Always subtle and timed to her landing: the puddle squishes, ripples spread
  out, and mud drops arc up and fall back.
- It suits the weather. Cloudy: a darker puddle and a few more drops. Rain:
  a fuller puddle with raindrop rings on it, and a bigger, wetter splash.
  Rainbow: a faint rainbow sheen, and some drops twinkle in rainbow colours.

Sound and music
- Every sound is soft and gentle, never harsh or buzzy.
- Cheerful background music that reacts to the game: calmer while waiting,
  bouncier while Peppa walks, twinkly when she is one step from the puddle.
  It changes key after each puddle, plays a small fanfare after each round,
  and adds a soft beat in level 2.
- The music suits the weather: slower and softer when cloudy, dreamy with
  raindrop plinks in the rain, bright with a harp run for the rainbow.
- Sound effects are in the music's key, and the music gets quieter whenever
  the voice speaks.
- A small music on/off button that responds only to the mouse or touch.

Finish with a short explanation of how the game works, for a parent.
```
