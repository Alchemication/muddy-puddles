# Test prompt for AI models

The full prompt below describes every feature of the reference game (the Claude Opus 5.5 version in [models/claude-opus-5-5](models/claude-opus-5-5/index.html)). Give it to a model in one message, with no follow-ups, and score the result with the scorecard.

## The prompt

```
Build a Peppa Pig game as a single HTML file (no external files or libraries)
to teach my 2-year-old basic keyboard navigation with the arrow keys.
Make it large, super simple and clear. Explain how it works.

Gameplay
- Peppa stands in a big grassy field. The arrow keys walk her one step at a
  time to a muddy puddle. When she reaches it she jumps in, a voice cheers,
  a star is added, and a new puddle appears somewhere else.
- Level 1 is a single row, so only left and right are needed. After 5 puddles
  the field grows to 3 rows and up and down join in.
- There is no way to lose. Walking into an edge just makes Peppa wiggle.
  Holding a key down moves her only one step. Space makes her jump and oink.

Teaching
- Show big on-screen arrow keys laid out like a real keyboard. They light up
  when pressed, and clicking them also moves Peppa.
- A friendly voice says each direction ("left", "up") as she moves.
- If my child does nothing for a few seconds, the arrow they need gently glows.
- Other keys never do anything bad. A wrong key makes the right arrow glow
  straight away. Only after several wrong keys in a row does the voice give
  a gentle nudge like "Try the right arrow!", and never more than once every
  few seconds.

Toddler-proofing
- Start with a big Play button that turns on sound and full screen.
- Block keys that would scroll or change the page, but let an adult leave
  with Esc or normal shortcuts.
- Fit any screen without scrolling.

Phones and tablets
- It must also work on a phone or tablet: swiping anywhere moves Peppa in
  that direction (a tap is not a swipe), and the on-screen arrows can be
  tapped.
- Held upright, put the arrows under the field, with everything sized to the
  screen width. The page must never scroll, zoom or pull-to-refresh.

Splash
- When Peppa lands in the puddle, show a subtle splash timed to her landing:
  the puddle squishes, ripples spread out and a few mud drops arc up and fall.

Weather
- The weather changes gently with progress, one step per puddle and never
  while my child is thinking: sunny, cloudy, light rain, rainbow, sunny again.
- Each change fades slowly and affects the environment: sky and grass colour,
  clouds covering the sun, light rain over the field (not over the arrow
  keys), and a soft rainbow.

Sound and music
- All sounds must be soft and gentle, never harsh or buzzy.
- Play cheerful original background music (not the real Peppa Pig theme)
  that reacts to the game. It gets calmer while waiting, bouncier while
  Peppa walks and twinkly when she is one step from the puddle. It changes
  key after each puddle, plays a small fanfare at the end of a round, and
  adds a soft beat in level 2.
- The music suits the weather: softer and slower when cloudy, dreamy with
  raindrop sounds in the rain, and bright with a harp run when the
  rainbow appears.
- Sound effects fit in the music's current key.
- The music gets quieter whenever the voice speaks.
- Add a small music on/off button that only responds to the mouse.
```

## Scorecard (1 point each, 23 total)

**Gameplay**

1. Arrow keys walk Peppa one step at a time to the puddle. Reaching it gives a jump, a cheer, a star and a new puddle
2. Level 1 is left/right only, and up/down are added after 5 puddles
3. No way to lose: edges are harmless, holding a key moves one step, and Space jumps

**Teaching**

4. On-screen arrows are laid out like the keyboard, light up when pressed, and can be clicked
5. A voice says each direction
6. The needed arrow glows after a few idle seconds
7. Wrong keys: the arrow glows at once, and the voice nudges only after several misses, with a gap between nudges

**Toddler-proofing**

8. A Play button turns on sound and full screen
9. Page-changing keys are blocked, and Esc still works for the adult
10. Fits the screen with no scrolling, with big, clear visuals

**Phones and tablets**

11. Swiping moves Peppa (taps don't), and the on-screen arrows can be tapped. It works upright and sideways, with no scrolling, zooming or pull-to-refresh

**Splash**

12. A subtle splash (squish, ripples, arcing drops) happens exactly when Peppa lands

**Weather**

13. Weather changes one step per puddle, in the right order, never mid-move
14. Changes fade slowly and affect sky, grass, clouds and sun
15. Rain stays over the field, and the rainbow is soft

**Sound and music**

16. All sounds are genuinely soft: they fade in and out, with no square or sawtooth buzz
17. The music is original, and not a copy of the Peppa Pig theme
18. The music reacts to what's happening: waiting, walking, near the puddle, key change, fanfare, level 2 beat
19. The music's mood follows the weather
20. Sound effects are in the music's key
21. The music gets quieter when the voice speaks
22. The mouse-only music button turns the music on and off

**Overall**

23. Works first time with no errors, and the explanation is clear for a parent

## Blind variant

The full prompt tests how well a model delivers a detailed spec. To test whether a model thinks of good toddler UX on its own, use this short version instead. Score it on the same card, and expect fewer points.

```
Build a simple Peppa Pig game as a single HTML file to teach my 2-year-old
basic keyboard navigation with the arrow keys. Make it large, super simple
and clear, with gentle sounds and cheerful background music. When Peppa jumps
into a muddy puddle, show a subtle splash animation. Explain how it works.
```

## Tips for comparing models

- **One shot:** give the prompt once with no follow-ups, then score it. Separately, count how many follow-up requests it takes to reach something you'd give your child.
- **The real test is the child:** check whether they can play for 2 minutes without help. No model's own description of its game can tell you that.
- **Harder version:** add *"I'm SSH-ed into another Mac. Help me open it on my laptop"* to test whether the model thinks about where the game will actually be played.
