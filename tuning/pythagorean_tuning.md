## How it's computed

Every pitch comes from repeatedly lengthening (or, run the other way, shortening) a string by exactly 3/2, then folding each result back into a single octave by dividing by 2 as many times as it takes. Twelve repetitions, worked out in full in [[why_12_notes]], produce all twelve pitch classes — no other ratio is used anywhere in the system.

## The tuning

The result, laid out along one octave:

![[notes/resources/images/why12_points.svg]]

Every interval in Pythagorean tuning reduces to nothing but the 3:2 step itself and the 2:1 fold. Thirds are never built directly — they fall out as whatever four stacked fifths happen to produce, pure or not.

Every natural key below is held by default, no sharps, tuned to Pythagorean — press **Play ascending** to hear the plain C D E F G A B scale, C3 up to C5.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean.html
280
```

## The good

Any two notes exactly one step apart in the chain — C and F, F and B♭, B♭ and E♭, and so on all the way to D and G — form a perfectly pure, beatless fifth, because that ratio *is* the definition of the step. Eleven such pure fifths sit among these twelve notes, octaves are pure too, and none of the natural-key scale above ever touches the twelfth, leftover one.

**Try it:** the keyboard below starts on C3 and G3, tuned to Pythagorean — press **Play together**, then flip the dropdown to Equal and play the same two keys again. Pythagorean's fifth here is an exact 3:2 (701.96 cents); Equal's is 700, two cents flat. Small, but real — it's why singers and string players who tune by ear keep drifting toward pure fifths instead of tempered ones.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean_good.html
280
```

## The bad

The twelfth relationship — from G back up to C, closing the circle — was never one of the built steps; it's the leftover, and it's badly out of tune, sharp by the full [[pythagorean_comma|Pythagorean comma]] (traditionally placed between G♯ and E♭ on a 12-note keyboard as the infamous "wolf fifth"). Thirds fare worse too: one built from four stacked fifths (C up to E) comes out noticeably wider than a pure 5:4 — the harsh "Pythagorean third" that later theorists singled out as the system's real weak point, and the specific problem [[meantone]] was invented to fix. See [[thirds_and_fifths]] for the intervals themselves.

**Try it:** the keyboard below starts on G♯3 and D♯4, tuned to Pythagorean — press **Play together**, then switch the dropdown to modern Equal temperament and play the same two keys again. In Pythagorean that's the wolf fifth, landing around 678 cents instead of the normal ~702, so it sounds noticeably sour; in Equal every fifth is identical (700 cents), so the same two keys suddenly sound perfectly ordinary. For a subtler version of the same comparison, hold C4, E4 and G4 instead: Pythagorean's major third beats a little faster than Equal's.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean_bad.html
280
```

## History

Credited by legend to Pythagoras (6th century BCE), who is said to have noticed that a string stopped at 2/3 of its length sounds remarkably settled against the open string — the observation credited with starting the idea that music is made of numbers — and to the string-and-ratio tradition built in his name. The system was already being analyzed rigorously by the time of Euclid's *Sectio Canonis* (c. 300 BCE), which works out the same comma arithmetic explicitly. Pythagorean tuning remained Europe's dominant tuning theory through the medieval period and into the early Renaissance, before its flaws — the wolf fifth, the wide thirds — drove the move to [[meantone]] from around the 15th–16th century onward.
