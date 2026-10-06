A **step sequencer** turns a bar of music into a grid: time runs left to right in fixed slots, and each slot is either on or off for a given sound. The grid below quantizes each beat into four 16th notes — the standard resolution for a drum pattern, fine enough for most grooves without needing to place a note "between the lines." Sixteen steps make one 4/4 bar; the thicker dividers mark where each beat starts, the same "landmark, not every line" idea as [[note_value|beat subdivisions]] in standard notation.

Program a pattern by clicking steps for kick, snare and hi-hat, then press Play. Mute (M) and Solo (S) isolate a channel; Swing delays every off-beat 16th for a looser feel; four pattern banks (A–D) let you switch between variations without stopping playback — useful for building up a beat section by section, the same way a real drum machine's pattern-chaining works.

```html-embed
music_instruments/resources/html/rhythm_box.html
360
```

**Edit a pattern that lives in a note.** The rhythm data notes in `rhythm_data/` are just JSON, and you can drive them from the grid instead of hand-typing booleans like an animal. Open one and hit **Open as Beat Box** in the note's header (or run *Edit rhythm in Rhythm Box* from the command palette): the same tab turns into this widget, loaded with the note's pattern. Click cells, change the tempo, swing or time signature, and it saves itself a moment after you stop — the little status next to the note's name says *Saving…* then *Saved*, and there's no Save button to forget. Play, mute, solo, volume and the banks never touch the note. **Open as JSON** in the header flips the tab back to the plain text. Change the time signature and you'll be asked first, because it wipes the pattern.
