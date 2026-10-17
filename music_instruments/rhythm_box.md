A **step sequencer** turns a bar of music into a grid: time runs left to right in fixed slots, and each slot is either on or off for a given sound. The grid below quantizes each beat into four 16th notes — the standard resolution for a drum pattern, fine enough for most grooves without needing to place a note "between the lines." Sixteen steps make one 4/4 bar; the thicker dividers mark where each beat starts, the same "landmark, not every line" idea as [[note_value|beat subdivisions]] in standard notation.

Program a pattern by clicking steps for kick, snare and hi-hat, then press Play. Mute (M) and Solo (S) isolate a channel; Swing delays every off-beat 16th for a looser feel; four pattern banks (A–D) let you switch between variations without stopping playback — useful for building up a beat section by section, the same way a real drum machine's pattern-chaining works.

```html-embed
music_instruments/resources/html/rhythm_box.html
360
```

**Edit a pattern that lives in a note.** The rhythm data notes in `rhythm_data/` are just JSON, and you can drive them from the grid instead of hand-typing booleans like an animal. Open one — from the explorer, a link, anywhere — and it opens *as* this widget, loaded with the note's pattern. Click cells, change the tempo, swing or time signature, and it saves itself a moment after you stop: the little status next to the note's name says *Saving…* then *Saved*, and there's no Save button to forget. Play, mute, solo and volume never touch the note. **Open as JSON** in the tab's header flips it to the plain text and keeps it there until you navigate away; **Open as Beat Box** flips it back (so does *Edit rhythm in Rhythm Box* in the command palette). A note holds exactly one pattern, so there are no banks in here: want a variation, make another note — that's what the graph is for. Time signature, **Random** and **Clear** ask first — a small bar appears right in the widget — because each one rewrites the whole pattern in the note. Made a mess? *Restore to last commit* in the same header puts the note back.

**Three views of one note.** The tab of a rhythm note has three modes, and the header buttons flip between them: **Beat Box** (the grid, the default), **JSON** (the plain text, for the hand-editors) and **Score** — the same bar engraved as notation, one staff per instrument, accents as `>`, with a play button. The Score is a *view*: nothing is converted, no note is created, and it re-draws itself when the note changes. It needs the music edition of the plugin; on the lean one you get Beat Box and JSON. To change a hit, go back to the Beat Box — the score is for reading, not for fiddling.

**Beyond the kit.** The grid isn't limited to kick, snare and hi-hat anymore: **Add instrument** brings in a bell, claves, a high conga and a low conga, and a rhythm note shows exactly one row for each instrument it contains — so a bell pattern is a single row, honest and uncluttered. The meter menu has grown to match: 4/4, 3/4, **12/8**, **6/8** and **5/4**, with the steps grouped the way the meter feels (threes in 12/8 and 6/8, fours in 5/4). Open `rhythm_pattern_bell_12_8` for the West African bell, `rhythm_pattern_clave_son_3_2` for the clave that half of Latin music hangs on, `rhythm_pattern_tresillo` for the 3+3+2 cell, `rhythm_pattern_hemiola` for two-against-three, and `rhythm_pattern_tha_dhi_gi_na_thom` for a Carnatic five-beat phrase played on hand drums — a stylised kit rendering, the drums standing in for the syllables. Same grid, very different worlds.

**Grid or circle.** The **Grid | Circle** switch above the pattern redraws the same bar as a circle: step 1 at the top, time running clockwise, one ring per instrument (the first one outermost). Click a dot to toggle a hit, exactly as in the grid; **Show shape** joins one ring's hits into a polygon, which is the quickest way to *see* why a rhythm feels the way it does — and **Rotate left / Rotate right** slide every instrument one step round the circle, and **Left a beat / Right a beat** slide them a whole beat at a time (one group of steps: four in 4/4, three in 12/8), so the son clave's 3-2 turns into a 2-3 after two beats under your hands. Nothing about the note changes except the hits themselves; the view is only how you look at them. Up to four instruments fit legibly — with more, the circle says so and the grid stays. The meter menu also offers **4/4 (eighth notes)**: one bar in eight steps instead of sixteen, for patterns that never need the in-between 16ths.

**Put a rhythm in your own note.** Don't copy the pattern and don't paste a second widget — point at the data note and let it play right where you're writing. Drop a `forge-rhythm` block into any note, with a link to a rhythm data note on its first line:

````
```forge-rhythm
[[rhythm_pattern_tresillo]]
```
````

That's the whole thing: the rhythm shows up as a Beat Box in place, headed with the note's name, with **Open note** beside it. Three optional lines can follow the link — `height: 480` (pixels), `title: Three-three-two` (the heading) and `view: circle` (start in the circle view; `view: grid` is the default) — and nothing else; a typo gets you a plain message, not a silent shrug.

It's a playground, on purpose. Click cells, shove the tempo, change the meter, hit Random — nothing is saved, ever, and the label says so. **Reset** puts the rhythm back exactly as it is in the note; **Open note** opens the real thing in its own tab, where changes *are* saved. If the note changes while you're mid-experiment, your experiment wins until you press Reset. Start a second embed and the first one shuts up — one groove at a time. In the music edition there's also a **Score** button that engraves what's on screen *right now*, your edits included, and the same button flips back to the grid. Here's the tresillo, ready to wreck:

```forge-rhythm
[[rhythm_pattern_tresillo]]
```
