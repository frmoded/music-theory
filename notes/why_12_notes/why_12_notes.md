Put the question the way the Pythagorean tradition is supposed to have posed it: if lengthening a string by 3/2 gives one good, consonant interval — the pitch dropping by that same simple ratio — what happens if you keep doing it, continuously? Lengthen the new string by 3/2 again. And the next one. And the next.

**Table 1 — Raw string lengths, in build order.** *Twelve successive 3/2 lengthenings, before folding into an octave.*

| Note # | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| Length | 1.0000 | 1.5000 | 2.2500 | 3.3750 | 5.0625 | 7.5938 | 11.3906 | 17.0859 | 25.6289 | 38.4434 | 57.6650 | 86.4976 |

There's a second piece of understanding this needs: halve a string's length and you get "the same" note — same pitch class, unmistakably higher to the ear. That's what makes the question answerable at all: every one of these ever-longer strings can be folded back — divided by 2, and by 2 again as many times as it takes — until it lands between the open string and its octave, where it can be compared directly against everything else.

Sort that folded data by its normalized length instead of by build order, and name each string by its pitch class, and the twelve notes lay themselves out as the chromatic scale — nothing was arranged to make that happen, it falls out of the ratios on its own:

**Table 2 — Folded lengths, sorted, with pitch names.** *The same twelve strings, normalized into one octave and sorted — the chromatic scale falls out on its own.*

| Note # | Normalized length | Note name |
|---|---|---|
| 1 | 1.0000 | C |
| 8 | 1.0679 | B |
| 3 | 1.1250 | B♭ |
| 10 | 1.2014 | A |
| 5 | 1.2656 | A♭ |
| 12 | 1.3515 | G |
| 7 | 1.4238 | G♭ |
| 2 | 1.5000 | F |
| 9 | 1.6018 | E |
| 4 | 1.6875 | E♭ |
| 11 | 1.8020 | D |
| 6 | 1.8984 | D♭ |

Laid out as points along the octave itself:

![[notes/resources/images/why12_points.svg]]

A guitar makes this same idea mechanical, string by string: each fret is a fixed division point, and pressing a string down at a fret shortens the vibrating length to whatever ratio that fret marks — exactly what a monochord's movable bridge does. See [[guitar]] for the physical layout, with one real difference from the tables above: modern frets aren't cut at these Pythagorean ratios at all. They're cut for equal temperament (see [[equal_temperament]]), so a guitar's twelve frets per octave are twelve *identical* steps, not twelve unevenly-spaced whole-number ratios.

This note is already getting long — it'll get split up later — but two more views of the same twelve numbers are worth seeing before that happens. Take the log of each normalized length and the twelve points spread out by pitch position instead of by raw ratio, making the drift from a perfectly even scale visible:

![[notes/resources/images/why12_log.svg]]

Wrap that same pitch position around a circle instead of along a line, and the twelve steps almost close a perfect loop back onto themselves — almost:

![[notes/resources/images/why12_circle.svg]]

This is the same relationship as [[nice]]'s 2:3 ratio, just run the other way: lengthening by 3/2 drops the pitch a step instead of raising it, but the same twelve-step mismatch shows up either direction.

The mismatch is arithmetic, not a rounding error. Stack twelve of these steps and you've multiplied the starting frequency by (3/2)^12 ≈ 129.75. Stack seven pure octaves instead and you've multiplied it by 2^7 = 128. Those two numbers should be equal if twelve steps genuinely closed the loop back onto seven octaves — they aren't, and they never can be: one is a power of 3 over a power of 2, the other is purely a power of 2, and no power of 3 is ever exactly a power of 2. Twelve is simply the smallest number of steps where the near-miss becomes small enough to look, by ear, almost like a match — which is exactly what makes it the dangerous one, the point where a tuner is most tempted to declare the gap closed and move on.

The leftover gap — roughly a quarter of a semitone, marked on the diagrams above as the small gap next to the first point — is the **Pythagorean comma**. Every tuning system invented since — [[meantone]], [[well_temperament]], today's [[equal_temperament]] — is a different way of spreading or hiding that same twelve-step leftover; none of them make it genuinely vanish, because the arithmetic above doesn't allow it to.

Ancient Greek theory was not caught off guard by this. Euclid's *Sectio Canonis* (c. 300 BCE) works the same ratio arithmetic through and shows explicitly that a stack of fifths never lands exactly on a stack of octaves — the comma was a proven consequence of Pythagorean number-ratio theory, not a later, embarrassing discovery made once instruments got precise enough to expose it.
