---
type: action
inputs:
  - tonic
recipe_version: 2
sync_state: stale-python
description_hash: 70f866bc1a1c6ee782a7d01f94a1461468bb46999e2fd8935e8592f6e69c405b
recipe_hash: 25cf6418814c1158bfb59d3f0fb8ab81e396fcfc15016f97ab4a8d6ec3e03de1
python_hash: 738f4aacd2a562e7b0174668651c572a26c9f160b1a28c5f61db34dbacb459ad
recipe_derived_from_source_hash: 70f866bc1a1c6ee782a7d01f94a1461468bb46999e2fd8935e8592f6e69c405b
python_derived_from_source_hash: 70f866bc1a1c6ee782a7d01f94a1461468bb46999e2fd8935e8592f6e69c405b
source_facet: recipe
recipe_derived_from_description_hash: 70f866bc1a1c6ee782a7d01f94a1461468bb46999e2fd8935e8592f6e69c405b
english_hash: e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855
python_derived_from_recipe_hash: 25cf6418814c1158bfb59d3f0fb8ab81e396fcfc15016f97ab4a8d6ec3e03de1
---

# Description

Return the three notes of the major triad rooted at a given tonic — root, third, and fifth — as a list of pitch names. Given a tonic note name (e.g. "C", "F#", "Bb"), return the three pitch-class names of the major triad built on it: the root, the major third above it, and the perfect fifth above it. Pitch names use music21 spelling (flats written with `-`, e.g. "B-").

## Inputs

- tonic — tonic note name string (e.g. "C", "F#", "Bb")

# Recipe
Return {{ [major_scale(tonic)[i] for i in [0, 2, 4]] }}.

# Python

```python
def compute(context, tonic):
  return [music21.pitch.Pitch(tonic).transpose(iv).name for iv in ['P1', 'M3', 'P5']]

```
