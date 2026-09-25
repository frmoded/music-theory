Stack twelve pure fifths and you land close to, but not on, seven pure octaves. That leftover is the **Pythagorean comma**: roughly a quarter of a semitone, about 23.5 cents. [[why_12_notes]] shows how the twelve strings get there; this note is about what is left over.

**Table 1 — Twelve fifths against seven octaves.** *Both paths should end on the same note; they miss by about a quarter of a semitone.*
| Path | Frequency ratio | Cents |
|---|---:|---:|
| Twelve pure fifths, (3/2)^12 | 129.7463 | 8423.5 |
| Seven pure octaves, 2^7 | 128.0000 | 8400.0 |
| The difference: the comma | 1.0136 | 23.5 |

The mismatch is arithmetic, not a rounding error. Those two numbers would be equal if twelve steps genuinely closed the loop back onto seven octaves, and they never can be: one is a power of 3 over a power of 2, the other is purely a power of 2, and no power of 3 is ever exactly a power of 2. Twelve is simply the smallest number of steps where the near-miss becomes small enough to look, by ear, almost like a match — which is exactly what makes it the dangerous one, the point where a tuner is most tempted to declare the gap closed and move on.

Take the log of each normalized length and the twelve points spread out by pitch position instead of by raw ratio, making the drift from a perfectly even scale visible:

![[notes/resources/images/why12_log.svg]]

Wrap that same pitch position around a circle instead of along a line, and the twelve steps almost close a perfect loop back onto themselves — almost. The small gap next to the first point, on both diagrams, is the comma:

![[notes/resources/images/why12_circle.svg]]

This is the same relationship as [[nice]]'s 2:3 ratio, just run the other way: lengthening by 3/2 drops the pitch a step instead of raising it, but the same twelve-step mismatch shows up either direction.

Every tuning system invented since — [[meantone]], [[well_temperament]], today's [[equal_temperament]] — is a different way of spreading or hiding that same twelve-step leftover; none of them make it genuinely vanish, because the arithmetic above doesn't allow it to. The [[Tuning]] chapter collects them all, from [[pythagorean_tuning]] to equal temperament.

## History

Ancient Greek theory was not caught off guard by this. Euclid's *Sectio Canonis* (c. 300 BCE) works the same ratio arithmetic through and shows explicitly that a stack of fifths never lands exactly on a stack of octaves — the comma was a proven consequence of Pythagorean number-ratio theory, not a later, embarrassing discovery made once instruments got precise enough to expose it.
