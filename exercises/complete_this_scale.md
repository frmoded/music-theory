---
type: action
inputs: []
recipe_version: 1
sync_state: synced
---

# Description

Below are the first 4 notes of a mystery scale: **C4, D4, E4, F4**. What are the remaining 4 notes that complete it (through the octave)? Set `guess` to a list like ["G4", "A4", "B4", "C5"]. Then click Forge for feedback.

# Recipe

Let true_tonic = "C".
Let true_mode = "major".
Let scale = Call [[diatonic_scale]] with tonic=true_tonic, mode=true_mode.
Let answer = Call [[pick_indices]] with lst=scale, indices=[4, 5, 6, 7].
Return {{ ("Correct! The full scale is " + str(scale)) if guess == answer else ("Not quite — the remaining 4 notes were " + str(answer) + ". Full scale: " + str(scale)) }}.
