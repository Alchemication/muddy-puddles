# Test prompt for AI models

The prompt is deliberately short. If it spelled everything out, it would only test whether a model follows instructions. A short prompt shows whether the model thinks of the toddler-friendly details on its own.

## The prompt

```
Build a simple Peppa Pig game as a single HTML file to teach my 2-year-old
basic keyboard navigation with the arrow keys. Make it large, super simple
and clear, with gentle sounds and cheerful background music. Explain how it works.
```

## Scorecard (1 point each)

**Understanding the child**
1. Starts with left/right only and adds up/down later
2. No way to lose or fail, and bumping an edge is harmless
3. Pressing the wrong key is handled gently: a hint first, and a voice only occasionally
4. Holding a key down or mashing keys doesn't break the game or skip ahead

**Teaching the keys**

5. On-screen arrows are laid out like the real keyboard and light up when pressed
6. The arrow the child needs glows as a hint when they're stuck
7. A voice says the direction ("left", "up") and celebrates success

**Toddler-friendly handling**

8. Blocks keys that would scroll or change the page, while keeping a way out for the adult
9. A start button that turns on sound (browsers require a click first) and full screen
10. Big layout that fits any screen without scrolling

**Sound**

11. Sounds are genuinely soft: they fade in and out, with no square or sawtooth buzz
12. Music changes with what's happening, or at least doesn't repeat every few seconds
13. The music gets quieter when the voice speaks

**Judgement**

14. Handles the copyright question sensibly (an original tune and drawing, not copying the theme or artwork) without refusing
15. Works first time with no errors, and explains it clearly for a parent

## Tips for comparing models

- **Hand it off as-is:** give the prompt once with no follow-ups, then score it. Separately, count how many follow-up requests it takes to reach something you'd give your child. That's a good measure of UX sense.
- **The real test is the child:** check whether they can play for 2 minutes without help. No model's own description of its game can tell you that.
- **Harder version:** add *"I'm SSH-ed into another Mac. Help me open it on my laptop"* to test whether the model thinks about where the game will actually be played.
