---
type: action
inputs:
  - guess
recipe_version: 1
sync_state: synced
---

# Description

Complete the C major scale you heard in [[exercises/complete_this_scale_challenge]]. Using the major interval pattern (W‑W‑H‑W‑W‑W‑H), work out the four notes that finish the octave after C‑D‑E‑F and set them as your `guess` — e.g. `["G4", "A4", "B4", "C5"]`. Press **Run** for note-by-note feedback. Concept refresher: [[music_theory/scale]].

# Recipe

Let true_tonic = "C".
Let true_mode = "major".
Let scale = Call [[diatonic_scale]] with tonic=true_tonic, mode=true_mode.
Return {{ ("Correct! You completed the C major scale: " + str(scale)) if guess == scale[4:] else ("Not yet. Note by note, here's how your guess lines up: " + str([str(g) + (" OK" if (i < len(scale[4:]) and g == scale[4:][i]) else " X") for i, g in enumerate(guess)]) + ". Hint: after F, the major pattern continues whole-whole-whole-half — work out G, A, B, then a half-step up to the octave C. Adjust your guess and Run again.") }}.
