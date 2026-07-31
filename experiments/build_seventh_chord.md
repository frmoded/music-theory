---
inputs: [tonic, quality]
recipe_version: 1
---

# Description


# Recipe

Return {{ [p.nameWithOctave for p in [music21.pitch.Pitch(tonic).transpose(music21.interval.Interval(iv)) for iv in {"maj7": ["P1","M3","P5","M7"], "dom7": ["P1","M3","P5","m7"], "min7": ["P1","m3","P5","m7"], "half_dim7": ["P1","m3","d5","m7"], "dim7": ["P1","m3","d5","d7"], "dom9": ["P1","M3","P5","m7","M9"], "dom11": ["P1","M3","P5","m7","M9","P11"], "dom13": ["P1","M3","P5","m7","M9","P11","M13"]}[quality]]] }}.
