A fret is a straight bar across the neck, so it stops **all** the strings at exactly the same distance from the nut. Each fret leaves the sounding length multiplied by 2^(−1/12) ≈ 0.9439 — one equal-tempered semitone, a shade under 17/18 — on every string alike. That single ratio, repeated, is the whole fretboard.

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
">Table 1 — Where equal-tempered frets fall.</div>

<div style="
  font-size:12px;
  color:#555555;
  margin:2px 0 10px;
">The sounding length left after a fret, on any string, beside the simple ratio it nearly matches.</div>

<table style="width:100%; border-collapse:collapse;">
<tr>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Fret</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Length left</th>
  <th style="text-align:left; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">Nearest simple ratio</th>
  <th style="text-align:right; padding:4px 8px; color:#2B2B2B; border-bottom:1px solid #666666;">From nut (mm)</th>
</tr>
<tr>
  <td style="text-align:right; padding:4px 8px; color:#555555;">3</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">0.8409</td>
  <td style="padding:4px 8px; color:#555555;">5/6 = 0.8333</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">103.4</td>
</tr>
<tr>
  <td style="text-align:right; padding:4px 8px; color:#555555;">4</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">0.7937</td>
  <td style="padding:4px 8px; color:#555555;">4/5 = 0.8000</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">134.1</td>
</tr>
<tr>
  <td style="text-align:right; padding:4px 8px; color:#555555;">5</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">0.7492</td>
  <td style="padding:4px 8px; color:#555555;">3/4 = 0.7500</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">163.1</td>
</tr>
<tr>
  <td style="text-align:right; padding:4px 8px; color:#555555;">7</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">0.6674</td>
  <td style="padding:4px 8px; color:#555555;">2/3 = 0.6667</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">216.2</td>
</tr>
<tr>
  <td style="text-align:right; padding:4px 8px; color:#555555;">12</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">0.5000</td>
  <td style="padding:4px 8px; color:#555555;">1/2 = 0.5000</td>
  <td style="text-align:right; padding:4px 8px; color:#555555;">325.0</td>
</tr>
</table>

</div>

Read the table against the [[monochord]]; distances are for a 650 mm scale length. Fret 12 is exactly half the string, an octave. Frets 5 and 7 land almost on the 3/4 and 2/3 points, the pure fourth and fifth. But fret 4 misses the pure major third (4/5) by enough to sound about 14 cents sharp, and that is the problem: the ratio is fixed, so every string, in every key, gets the same compromise, with no way to make one chord purer at the cost of another. Try it: on the monochord, stop the string at 4/5 and then at fret 4's 0.7937, and listen for the difference. See [[thirds_and_fifths]] for the intervals involved.

## Do The Problem

The [[lute]]'s frets were loops of gut, not soldered metal — retie one under a different rule and it can end up somewhere else entirely. Below is a full six-course lute, starting fretted by the Rule of Eighteen. Switch the dropdown to Equal temperament and every fret stays one straight bar, just slid to a new spot. Switch to Pythagorean or Well temperament and watch the SAME fret break into a zigzag instead — one straight bar can't land in the right place for six strings that don't all open on the same pitch class at once. That zigzag, impossible to actually build, is the problem with frets made visible: a fretted instrument gets exactly one physical compromise per fret, and the moment a tuning stops being perfectly symmetric, that one compromise stops being right for more than one string.

```html-embed
music_instruments/resources/html/lute_fretboard.html
380
```

## History

On the [[lute]] the frets were loops of gut tied around the neck, so a player could nudge them to suit a piece. Around 1581 Vincenzo Galilei proposed one fixed rule for all of them, 17/18 of the remaining length per fret — see [[rule_of_eighteen]] — which is only about a cent per fret away from the exact ratio that Simon Stevin worked out, c. 1585–1608, as [[equal_temperament]].

The guitar's fixed metal frets locked that compromise into the instrument. A [[piano]] tuner can still choose how to spread the [[pythagorean_comma|comma]], and a [[viola]] player, with no frets at all, chooses every note by ear.
