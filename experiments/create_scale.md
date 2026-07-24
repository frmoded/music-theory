---
type: action
inputs: []
recipe_version: 1
---

# Description

Return the diatonic scale for a given tonic and mode as ascending pitch names, tonic to tonic inclusive. Given a tonic note name (e.g. "C", "F#", "Bb") and a mode ("major" or "minor"), return the eight pitch names of one ascending octave of that scale — from the tonic up to the tonic an octave above. Pitch names use music21 spelling with octave designations (flats written with `-`, e.g. "B-4").

## Inputs

- tonic — tonic note name string (e.g. "C", "F#", "Bb")
- mode — scale mode: "major" or "minor"

# Recipe

Return Call [[diatonic_scale]] with tonic=tonic, mode=mode.
