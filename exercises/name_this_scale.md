---
type: action
inputs: []
recipe_version: 1
sync_state: synced
---

# Description

Below you'll see + hear a mystery scale. What mode is it? Set the `guess` input to one of: "major", "minor", "pentatonic". Then click Forge.

# Recipe

Let true_tonic = "C".
Let true_mode = "major".
Let scale = Call [[diatonic_scale]] with tonic=true_tonic, mode=true_mode.
Return {{ ("Correct! It was " + true_mode + " starting at " + true_tonic + ": " + str(scale)) if guess == true_mode else ("Not quite — actual mode was " + true_mode + ". Scale: " + str(scale)) }}.
