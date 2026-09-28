## How it's computed

Stretch a string by exactly 3/2, fold the result back into one octave by halving as needed, and repeat. Twelve repetitions — worked out in [[why_12_notes]] — give all twelve pitch classes.

## The tuning

Laid out along one octave:

![[notes/resources/images/why12_points.svg]]

Every interval here comes only from the 3:2 step and the 2:1 fold; thirds are never built directly, just whatever four stacked fifths happen to land on.

Below, C3 to C4, naturals only, tuned to Pythagorean — press **Play ascending** for the scale.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean.html
280
```

## Do the good

Any two notes one step apart in the chain — C–F, F–B♭, B♭–E♭, ... D–G — are a perfectly pure fifth; eleven of the twelve sit this way, and the octaves are pure too.

Below, C3 and G3 start held. Play together, then switch to Equal and play again: Pythagorean's fifth is exactly pure, Equal's is two cents flat — small, but it's why singers and string players drift toward pure fifths by ear.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean_good.html
280
```

## Do the bad

The twelfth fifth, G back to C, was never a built step — it's the leftover, sharp by the full [[pythagorean_comma|comma]], the infamous "wolf" (traditionally between G♯ and E♭). Thirds fare worse: one built from four fifths (C to E) comes out noticeably wide, the flaw [[meantone]] was built to fix.

Below, G♯3 and D♯4 start held — the wolf fifth. Play together, then switch to Equal: the same two keys go from sour to ordinary. For the subtler version, try C4, E4 and G4 instead.

```html-embed
tuning/resources/html/piano_keyboard_pythagorean_bad.html
280
```

## History

Legend credits Pythagoras (6th century BCE) with noticing that a string stopped at 2/3 of its length sounds settled against the open string. Euclid's *Sectio Canonis* (c. 300 BCE) already works the same arithmetic. The system dominated Europe through the medieval period, until its flaws — the wolf, the wide thirds — pushed theorists toward [[meantone]] from the 15th–16th century on.
