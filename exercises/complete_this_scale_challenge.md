---
type: action
inputs: []
recipe_version: 1
sync_state: synced
---

# Description

Press **Run** to hear the first four notes of a C major scale. Your task: work out the four notes that complete the octave — then check yourself in [[exercises/complete_this_scale_submit]]. New to scales? Start with [[music_theory/scale]].

# Recipe

Let true_tonic = "C".
Let true_mode = "major".
Let scale = Call [[diatonic_scale]] with tonic=true_tonic, mode=true_mode.
Return {{ music21.stream.Part([music21.note.Note(n, quarterLength=1.0) for n in scale[:4]]) }}.
