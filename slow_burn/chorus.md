---
type: action
description_hash: 60d69be29dcc358d5013b4257c78fec5d1739fd51b26e5e93a6d3628663a9235
recipe_hash: 1f29c2e7526303b05483a2b3993137828ee85ea1f0c6fde8f20df526993e5119
python_hash: 94cde7d260b1b6aa50e5d09eed9b8ece0dd13403b572251fc5e6251c1114c2af
recipe_derived_from_source_hash: 60d69be29dcc358d5013b4257c78fec5d1739fd51b26e5e93a6d3628663a9235
python_derived_from_source_hash: 60d69be29dcc358d5013b4257c78fec5d1739fd51b26e5e93a6d3628663a9235
source_facet: synced
recipe_derived_from_description_hash: 60d69be29dcc358d5013b4257c78fec5d1739fd51b26e5e93a6d3628663a9235
python_derived_from_recipe_hash: 1f29c2e7526303b05483a2b3993137828ee85ea1f0c6fde8f20df526993e5119
---

# Description

One 12-bar vocal chorus of the blues — the basic repeating unit of
the song. AAB lyric arc: a four-bar phrase that sets up the line,
the same phrase repeated for weight, then the four-bar answer that
resolves it. Sung over the harmonic frame from [[form]]. Twelve
bars in 12/8, slow blues feel, around 70 BPM with an eighth-note
triplet swing.

The phrases lean weary and sparse — lots of rest space, sighing
through the line — with the answer landing more firmly on the
tonic at the end.

## Inputs

(none)

# Recipe

Let form_score = Call [[form]].
Let phrase_a1 = Call [[vocal_phrase_a]].
Let phrase_a2 = Call [[vocal_phrase_a]].
Let phrase_b = Call [[vocal_phrase_b]].
Let vocal_line = Call [[sequence_list]] with sections=[phrase_a1, phrase_a2, phrase_b].
Return Call [[voices_list]] with sections=[form_score, vocal_line].

# Python

```python
def compute(context):
    # v0.7.0: form / vocal_phrase_a / vocal_phrase_b are now library
    # notes in forge.music.lib; called directly instead of via
    # context.compute.
    form_score = form()
    phrase_a = vocal_phrase_a()
    phrase_b = vocal_phrase_b()

    vocal_line = sequence(repeat(phrase_a, 2), phrase_b)
    return voices(form_score, vocal_line)
```

# Dependencies

*Synced from Python. Edit the Python and regenerate, or run "Forge: Sync edges" to refresh.*

[[form]] [[vocal_phrase_a]] [[vocal_phrase_b]] [[sequence_list]] [[voices_list]]
