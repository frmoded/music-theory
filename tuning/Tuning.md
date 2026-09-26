Tuning is the practical question behind every note name: which exact frequency does each pitch get? Because twelve pure fifths never quite close into seven octaves (see [[why_12_notes]] and the [[pythagorean_comma]]), every instrument has to settle the leftover gap somewhere, and different eras settled it differently. For the physics of why string length and tension set the pitch, see [[frequency]].

This chapter covers how different eras handled the [[pythagorean_comma|Pythagorean comma]] once they'd found it — four systems, each choosing a different place to put the same unavoidable gap, plus one practical shortcut invented along the way. Compare the two ends of the spectrum yourself: read [[pythagorean_tuning]] (pure fifths, everything else pays) against [[equal_temperament]] (every step identical, nothing is pure).

- [[pythagorean_tuning]] — build every note from stacked pure fifths; simplest, and the one that surfaces the comma in the first place.
- [[meantone]] — spread the gap evenly across most fifths, at the cost of one unplayable "wolf" interval.
- [[rule_of_eighteen]] — Vincenzo Galilei's practical 16th-century approximation to equal temperament, built for fretted instruments before the mathematics of equal temperament existed.
- [[well_temperament]] — spread it unevenly instead, so every key is at least playable.
- [[equal_temperament]] — spread it with total mathematical evenness, abandoning rational ratios entirely.

## How close is each system to the others?

**Metric:** take each system's twelve chromatic pitches as cents above C (a cent is 1/100 of an equal-tempered semitone), then compute the **root-mean-square (RMS) difference** between two systems' twelve-note vectors — the standard way tuning systems get compared quantitatively. A small RMS means the two systems place their twelve notes almost identically; a large one means real, audible disagreement across the octave.

For [[pythagorean_tuning]] and [[meantone]] the table below uses each system's own well-known conventional cent values (built from the nearest fifths in either direction), not the deliberately one-directional twelve-fifth chain from [[why_12_notes]] — that chain exists specifically to expose the comma, not to represent how either tuning is actually built in practice, and mixing the two would compare different things under the same name. Rows and columns are in chronological order, as in the timeline under History.

<div style="
  background:#FDFCFA;
  border-radius:6px;
  padding:14px 16px;
  margin:8px 0;
">

<div style="
  font-size:15px;
  font-weight:600;
  color:#2B2B2B;
">Table 1 — How far apart the tuning systems sit.</div>

<div style="
  font-size:12px;
  color:#555555;
  margin:2px 0 10px;
">RMS difference between two systems' twelve-note tunings, in cents: smaller means more alike.</div>

<table style="width:100%; border-collapse:collapse;">
<tr>
  <th style="text-align:left; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;"></th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Pythagorean</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Meantone</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Rule of 18</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Well temp.</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Equal</th>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><strong>Pythagorean</strong></td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">—</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">22.9¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">13.3¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">15.1¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">8.3¢</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><strong>Meantone</strong></td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">22.9¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">—</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">12.3¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">9.9¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">14.6¢</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><strong>Rule of 18</strong></td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">13.3¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">12.3¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">—</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">4.7¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">6.8¢</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><strong>Well temp.</strong></td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">15.1¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">9.9¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">4.7¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">—</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">7.7¢</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><strong>Equal</strong></td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">8.3¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">14.6¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">6.8¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">7.7¢</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">—</td>
</tr>
</table>

</div>

A few things worth reading off the table: [[well_temperament|well temperament]] and [[rule_of_eighteen|the Rule of Eighteen]] sit closest to each other (4.7¢) — both were independently built as approximations to universal playability, one by ear and compromise, one by a single repeated ratio. [[pythagorean_tuning|Pythagorean]] and [[meantone]] sit furthest apart (22.9¢) — the two most philosophically opposed choices, pure fifths versus pure-ish thirds. Of the historical systems, [[equal_temperament|equal temperament]] itself sits closest to [[rule_of_eighteen|the Rule of Eighteen]] (6.8¢) — which makes sense, since Galilei's rule was already reaching for exactly what equal temperament later formalized.

## History

<div style="
  background:#FDFCFA;
  border-radius:6px;
  padding:14px 16px;
  margin:8px 0;
">

<div style="
  font-size:15px;
  font-weight:600;
  color:#2B2B2B;
">Table 2 — When each system entered use.</div>

<div style="
  font-size:12px;
  color:#555555;
  margin:2px 0 10px;
">In roughly chronological order.</div>

<table style="width:100%; border-collapse:collapse;">
<tr>
  <th style="text-align:left; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">System</th>
  <th style="text-align:left; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">When</th>
  <th style="text-align:left; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Notes</th>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><a class="internal-link" data-href="pythagorean_tuning" href="pythagorean_tuning">Pythagorean tuning</a></td>
  <td style="padding:4px 8px; color:#555555;">Legendary origin ~6th century BCE; rigorously formalized by Euclid's <em>Sectio Canonis</em>, c. 300 BCE</td>
  <td style="padding:4px 8px; color:#555555;">Dominant through the medieval period</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><a class="internal-link" data-href="meantone" href="meantone">meantone</a></td>
  <td style="padding:4px 8px; color:#555555;">Spreading from the late 15th century; standard through the 16th–17th centuries</td>
  <td style="padding:4px 8px; color:#555555;">—</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><a class="internal-link" data-href="rule_of_eighteen" href="rule_of_eighteen">Rule of Eighteen</a></td>
  <td style="padding:4px 8px; color:#555555;">c. 1581 (Vincenzo Galilei)</td>
  <td style="padding:4px 8px; color:#555555;">For fretted instruments specifically</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><a class="internal-link" data-href="well_temperament" href="well_temperament">well_temperament</a></td>
  <td style="padding:4px 8px; color:#555555;">Flourished 17th–18th centuries; Werckmeister's schemes published 1691, Bach's <em>Well-Tempered Clavier</em> 1722</td>
  <td style="padding:4px 8px; color:#555555;">—</td>
</tr>
<tr>
  <td style="padding:4px 8px; color:#555555;"><a class="internal-link" data-href="equal_temperament" href="equal_temperament">equal_temperament</a></td>
  <td style="padding:4px 8px; color:#555555;">Mathematically derived by Simon Stevin, c. 1585–1608; the de facto keyboard standard by the 19th century, universal by the 20th</td>
  <td style="padding:4px 8px; color:#555555;">—</td>
</tr>
</table>

</div>
