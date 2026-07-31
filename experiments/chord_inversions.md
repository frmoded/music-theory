---
inputs: [tonic, quality, inversion]
recipe_version: 1
---

# Description


# Recipe

Return {{ (lambda ps: [p.nameWithOctave for p in (ps[inversion:] + [p.transpose('P8') for p in ps[:inversion]])])([music21.pitch.Pitch(tonic).transpose(music21.interval.Interval(iv)) for iv in {"major": ["P1","M3","P5"], "minor": ["P1","m3","P5"], "diminished": ["P1","m3","d5"], "augmented": ["P1","M3","A5"]}[quality]]) }}.
