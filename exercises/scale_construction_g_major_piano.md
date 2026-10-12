---
type: action
inputs:
  - student_pitches
input_widgets:
  student_pitches: piano
description_hash: 703303d396896f9e2a56c18e8cfe5905ea7691788a49d0aeb67dde7a373bc34e
recipe_hash: 89bb0583e16bc3d4a5b50f9f3312589f1342b76e53dbb9805cd1d5d0e3e367be
python_hash: e5d1a4fc162f7e942b790e395406201fb6b83935dfe1843a475fc8837c15f097
recipe_derived_from_source_hash: 703303d396896f9e2a56c18e8cfe5905ea7691788a49d0aeb67dde7a373bc34e
source_facet: description
recipe_derived_from_description_hash: 703303d396896f9e2a56c18e8cfe5905ea7691788a49d0aeb67dde7a373bc34e
---

# Description

Click the seven notes of the G major scale on the piano, from the tonic
(G3) up to the seventh (F#4). Then click Forge to grade your attempt.

Same W-W-H-W-W-W-H pattern as C major, transposed to start on G — which
forces exactly one black key. Find it.

## Inputs

- student_pitches — the notes you play, picked on an interactive piano-keyboard widget; graded against the G major scale

# Recipe

Return Call [[scale_construction_exercise]] with tonic="G3", mode="major", student_pitches=student_pitches, widget_type="piano".

# Python

```python
def compute(context):
    return None
```
