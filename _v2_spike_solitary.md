---
type: action
description_hash: 94bc5d899dfad17c9b76062278bc2d4870f92673d3682ccaa9d62ebd9d4c3a93
recipe_hash: daa610f887eed10e376309a265a42e8eaf4eccddc119841498f013cb05960de8
python_hash: 9d6bef6c44603c3be9522d2e6c140fc5fbed22c4e3eec807595f3ff18ef08bd4
recipe_derived_from_source_hash: 94bc5d899dfad17c9b76062278bc2d4870f92673d3682ccaa9d62ebd9d4c3a93
python_derived_from_source_hash: 94bc5d899dfad17c9b76062278bc2d4870f92673d3682ccaa9d62ebd9d4c3a93
source_facet: synced
recipe_derived_from_description_hash: 94bc5d899dfad17c9b76062278bc2d4870f92673d3682ccaa9d62ebd9d4c3a93
python_derived_from_recipe_hash: daa610f887eed10e376309a265a42e8eaf4eccddc119841498f013cb05960de8
sync_state: synced
---

# Description

A minimal solitary pattern — kick on beats 1 and 3 of a single bar. V2 spike
test. Renders as a drum-kit score with audio playback.

## Inputs

(none)

# Recipe

Let part = Call [[play_at_beats]] with instrument=[[kick]], beats=[1, 2, 3].
[[show_score]] part.
Return part.

# Python

```python
def compute(context):
  part = play_at_beats(instrument=kick(), beats=[1, 2, 3])
  show_score(part)
  return part

```
