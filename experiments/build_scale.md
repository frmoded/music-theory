---
type: action
inputs: []
recipe_version: 1
source_facet: description
---

# Description

Return the major scale for a given tonic as ascending pitch names, tonic to tonic inclusive. Given a tonic note name (e.g. "C", "F#", "Bb"), return the eight pitch names of one ascending octave of the major scale — from the tonic up to the tonic an octave above. Pitch names use music21 spelling with octave designations (flats written with `-`, e.g. "B-4").

## Inputs

- tonic — tonic note name string (e.g. "C", "F#", "Bb")

# Recipe

Return Call [[diatonic_scale]] with tonic=tonic.
