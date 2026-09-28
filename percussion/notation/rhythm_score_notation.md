A **time signature** is two numbers stacked on top of each other doing all the talking: top for how many, bottom for of what. That's the whole contract, and somehow entire semesters get built defending it.

Here's one **measure**, four **quarter notes**, the plain **beat** made visible — this is what a 4/4 **time signature** actually buys you:

![[percussion/notation/resources/images/rhythm_beat_quarters.svg]]

The full doubling ladder, one note at a time. A **whole note**:

![[percussion/notation/resources/images/rhythm_note_whole.svg]]

A **half note**:

![[percussion/notation/resources/images/rhythm_note_half.svg]]

An **eighth note** — and halve the quarter-note measure above, and the same bar holds twice as many, beamed in groups of four so the eye can still find the beat:

![[percussion/notation/resources/images/rhythm_beat_eighths.svg]]

A **sixteenth note**:

![[percussion/notation/resources/images/rhythm_note_sixteenth.svg]]

A **32nd note**:

![[percussion/notation/resources/images/rhythm_note_32nd.svg]]

A **64th note** — the ladder runs out of easy names before it runs out of flags:

![[percussion/notation/resources/images/rhythm_note_64th.svg]]

**Rests** are that same ladder, just quiet about it — one gap in this vault's scores: the renderer behind these images takes pitches, not silence, so a rest can't get an honest picture here the way every sounded value above just did.

**Dots and ties** run their own hustle. A **tie** links two notes of the *same* pitch into one longer note — five quarters' worth of "C," which doesn't fit in one measure, so it has to tie across the bar line to get there:

![[percussion/notation/resources/images/rhythm_note_tie.svg]]

A **slur** does connected phrasing across *different* pitches instead — a similar curve, a completely different job, and half of music notation's confusion lives in that distinction. (No picture for this one either: a slur needs two different pitches and an explicit articulation the renderer doesn't expose.)

A **dot** adds half the note's own value back onto itself — a quarter note plus an eighth, written as one dotted quarter:

![[percussion/notation/resources/images/rhythm_note_dot.svg]]

**Double-dotted notes** stack a second dot worth a quarter of the original — diminishing returns, like everything else that compounds:

![[percussion/notation/resources/images/rhythm_note_doubledot.svg]]

Underneath all of it sits the **beat**, the pulse you'd tap a foot to, a.k.a. the **pulse**, and how fast it goes is the **tempo** — Allegro, Andante, or just a number if you're not feeling poetic; neither has its own picture, since both are about *speed*, not *shape*, and a still image can't move. **Meter** is how many beats live in a **measure** (the **bar**, pictured above) and how those beats split. **Duple**, **triple**, **quadruple** meter: two, three, or four beats a bar. **Simple meter** splits each beat into two; **compound meter** splits it into three, which is what a time signature with 6, 9, or 12 on top is quietly telling you. None of these six get a picture either — the renderer always assumes 4/4 and never draws a different time signature, so a genuine 2/4, 3/4, or 6/8 measure isn't something it can actually show, only fake.

And when a beat gets greedy, a **tuplet** crams notes where they don't belong: a **triplet** fits three notes where two normally live, a **quintuplet** fits five, a **sextuplet** six, a **septuplet** seven. Compound meter runs the trick backward — a **duplet** squeezes two notes into a dotted note's space, a **quadruplet** squeezes four. Tried to picture every one of these too, and pulled them back out: the renderer gets the *durations* exactly right but never draws the bracket-and-number that's the entire visual point of a tuplet, so the result looked like plain, oddly-spaced notes instead — wrong enough to mislead, not just incomplete.

## Sources

MT21C §4.1–4.5 Basics of Rhythm.
