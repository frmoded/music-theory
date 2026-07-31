---
inputs: [chord_tonic, quality, bass]
recipe_version: 1
---

# Description


# Recipe

Return {{ [music21.pitch.Pitch(bass).transpose(-12).nameWithOctave] + [p.nameWithOctave for p in [music21.pitch.Pitch(chord_tonic).transpose(music21.interval.Interval(iv)) for iv in {"major": ["P1","M3","P5"], "minor": ["P1","m3","P5"], "diminished": ["P1","m3","d5"], "augmented": ["P1","M3","A5"]}[quality]]] }}.
