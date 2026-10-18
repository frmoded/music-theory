---
type: action
description_hash: e3b8959cd6a325b60ad7e498b92e956a8df49897c7599db8bce8e8bc37766621
recipe_hash: 922910256aaa5942de8598c45fb4e0ae53a96acc22dd39d0f4ad00a8ed39e6b2
python_hash: 28f734b84e38334bf3b3ade17db0a46a75411fd9cdb9634ea11aa210fe28ce3b
recipe_derived_from_source_hash: e3b8959cd6a325b60ad7e498b92e956a8df49897c7599db8bce8e8bc37766621
python_derived_from_source_hash: e3b8959cd6a325b60ad7e498b92e956a8df49897c7599db8bce8e8bc37766621
source_facet: synced
recipe_derived_from_description_hash: e3b8959cd6a325b60ad7e498b92e956a8df49897c7599db8bce8e8bc37766621
python_derived_from_recipe_hash: 922910256aaa5942de8598c45fb4e0ae53a96acc22dd39d0f4ad00a8ed39e6b2
---

# Description

The instrumental chorus — 12 bars, no vocal. The electric guitar
takes the lead in minor pentatonic with blue notes; the harmonic
frame from [[form]] continues underneath. The moment the song
stops singing about the feeling and just shows it, sitting between
the second and third vocal choruses. 12/8, eighth-note triplet
feel, around 70 BPM. Denser than the vocal choruses — the
emotional arc going up rather than across.

## Inputs

(none)

# Recipe

Let harmonic_frame = Call [[form]].
Let solo_line = Call [[guitar_solo_chorus]].
Return Call [[voices_list]] with sections=[harmonic_frame, solo_line].

# Python

```python
def compute(context):
    # v0.7.0: form / guitar_solo_chorus are now library notes in
    # forge.music.lib; called directly instead of via context.compute.
    harmonic_frame = form()
    solo_line = guitar_solo_chorus()
    return voices(harmonic_frame, solo_line)
```

# Dependencies

*Synced from Python. Edit the Python and regenerate, or run "Forge: Sync edges" to refresh.*

[[form]] [[guitar_solo_chorus]] [[voices_list]]
