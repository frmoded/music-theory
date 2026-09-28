## How it's computed

Every pitch comes from repeatedly lengthening (or, run the other way, shortening) a string by exactly 3/2, then folding each result back into a single octave by dividing by 2 as many times as it takes. Twelve repetitions, worked out in full in [[why_12_notes]], produce all twelve pitch classes — no other ratio is used anywhere in the system.

## The tuning

The result, laid out along one octave:

![[notes/resources/images/why12_points.svg]]

Every interval in Pythagorean tuning reduces to nothing but the 3:2 step itself and the 2:1 fold. Thirds are never built directly — they fall out as whatever four stacked fifths happen to produce, pure or not.

Every key below is held and set to Pythagorean by default — press **Play ascending** to hear all twelve pure fifths (and the one wolf) laid out in pitch order, C3 up to C5.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean.html
280
```

## The good

Any two notes exactly one step apart in the chain — C and F, F and B♭, B♭ and E♭, and so on all the way to D and G — form a perfectly pure, beatless fifth, because that ratio *is* the definition of the step. Eleven such pure fifths sit among these twelve notes. Octaves are pure too, by construction of the fold itself.

## Do It Good

**Challenge 1:** hold C3 and G3 together (a fifth, well inside the safe part of the chain) and press **Play together** in Pythagorean, then switch to Equal and play the same two keys. Pythagorean's fifth here is exact 3:2 — 701.96 cents; Equal's is 700, two cents flat. It's a small gap, not the wolf's obvious sourness, but it's real: it's why singers and string players who tune by ear keep drifting toward pure fifths instead of equal-tempered ones.

**Challenge 2:** hold C3, G3 and D4 together (two of those fifths stacked) and do the same comparison. In Pythagorean, both fifths are exactly pure; in Equal, both are ever so slightly flat, and the gaps add up the more you stack. This is the flip side of the wolf below — the eleven fifths Pythagorean gets right, it gets exactly right, not approximately.

## The bad

The twelfth relationship — from G back up to C, closing the circle — was never one of the built steps; it's the leftover, and it's badly out of tune, sharp by the full [[pythagorean_comma|Pythagorean comma]] (traditionally placed between G♯ and E♭ on a 12-note keyboard as the infamous "wolf fifth"). Thirds fare worse still: a third built from four stacked fifths (e.g. C up to E) comes out noticeably wider than a pure 5:4 third — the harsh "Pythagorean third" that later theorists singled out as the system's real weak point, and the specific problem [[meantone]] was invented to fix. See [[thirds_and_fifths]] for the intervals themselves.

## Do It Bad

**Challenge 1:** hold G♯3 and D♯4 together (a fifth apart) and press **Play together** in Pythagorean, then switch to Equal and play the same two keys. In Pythagorean that's the wolf fifth — it lands at about 678 cents instead of the normal ~702, so it sounds noticeably sour and out of tune. In Equal every fifth is identical (700 cents), so the same two keys sound like a completely ordinary fifth. That contrast is the clearest demonstration there is.

**Challenge 2:** play a full C major triad (C4, E4, G4) together in both tunings, back to back. Pythagorean's major third is wider (407.82 cents vs. Equal's 400), so the chord sounds a touch brighter and beats a little faster — subtler than the wolf fifth, but it's the more musically typical difference you'd actually notice in real playing.

## History

Credited by legend to Pythagoras (6th century BCE), who is said to have noticed that a string stopped at 2/3 of its length sounds remarkably settled against the open string — the observation credited with starting the idea that music is made of numbers — and to the string-and-ratio tradition built in his name. The system was already being analyzed rigorously by the time of Euclid's *Sectio Canonis* (c. 300 BCE), which works out the same comma arithmetic explicitly. Pythagorean tuning remained Europe's dominant tuning theory through the medieval period and into the early Renaissance, before its flaws — the wolf fifth, the wide thirds — drove the move to [[meantone]] from around the 15th–16th century onward.
