# BK-Score dataset – evidence ratings for 520 supplements, peptides and biohacking practices

**Version 1.0.0 · as of 8 November 2026 · Licence CC BY 4.0 · Source: [biohackingkompakt.de](https://biohackingkompakt.de)**

The BK-Score rates how much is actually known about a substance or practice, on five axes from 0 to 10. It rates the state of knowledge, not the substance itself. The dataset covers 520 entries: supplements, peptides and experimental drugs, treatments and diagnostics, lifestyle practices and Khavinson bioregulator peptides. Each rating comes with a written rationale in German that names its studies.

## Key figures (version 1.0.0, 520 entries)

- **37 entries (7.1 %)** reach the label "Gut belegt" (well supported).
- **102 entries (19.6 %)** were either never studied in humans (53) or are marketed far ahead of the evidence (49).
- **264 entries (50.8 %)** have a hype gap of 3 or less out of 10. For every second entry, the marketing promise is well ahead of the data. That share is 60 % for peptides and experimental drugs, 42 % for supplements, 33 % for lifestyle practices and 13 of 14 Khavinson bioregulators.
- **38 entries** are well supported but heavily overhyped – real compounds with inflated promises, such as vitamin D3, B12 or iron.

## Files

| File | Content |
|---|---|
| `data/bk-score.csv` | One row per entry, UTF-8, comma-separated |
| `data/bk-score.json` | Same data plus axis definitions, disclaimer and the German rationale (`beleg`) |

### Columns (CSV)

| Column | Meaning |
|---|---|
| `id` | Stable identifier (same as the URL slug) |
| `name` | Name (German) |
| `category` | Supplement · Peptides & experimental · Treatments & diagnostics · Lifestyle practices · Bioregulator peptides (Khavinson) |
| `label` | Overall label (German), derived from the five axes by fixed rules |
| `human_evidence` | 0–10: how much good data exists in humans |
| `mechanism` | 0–10: how well the mechanism is understood |
| `safety_data` | 0–10: how well safety has been studied (not: how safe it is) |
| `hype_gap` | 0–10: 10 = the marketing stays level with the data; low values = large gap |
| `track_record` | 0–10: documented use in humans (since when, how broadly). Does not measure whether it works |
| `direction` | positive · negative · mixed · open – what the data say about the advertised effect |
| `url` | Entry page with all sources |
| `rationale_de` | Written rationale for every axis (German) |

## Method

The rules for each axis and label are published at [biohackingkompakt.de/methodik.html](https://biohackingkompakt.de/methodik.html). Ratings are based on primary sources (PubMed/Europe PMC, ClinicalTrials.gov, EMA, FDA, BfArM, EFSA). Every entry page lists its sources. Entries are updated when new trials, approvals or retractions appear. A running changelog is kept on the website.

## Disclaimer

Subjective assessment by Biohacking Kompakt based on published rating rules. Not a scientific consensus, not a medical recommendation. No dosing information for unapproved substances.

## Citation

Höser, P. (2026). *BK-Score dataset: evidence ratings for 520 supplements, peptides and biohacking practices* (Version 1.0.0) [Data set]. Biohacking Kompakt. https://github.com/phoeser/bk-score-dataset

## Licence

[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). You may share and adapt the data, including commercially, as long as you credit "Biohacking Kompakt" and link to biohackingkompakt.de.

---

## Deutsch

Der BK-Score bewertet auf fünf Achsen von 0 bis 10, wie viel über ein Mittel bekannt ist – nicht das Mittel selbst. Der Datensatz enthält 520 Einträge mit Begründung und Quellenlink. Kennzahlen: 37 gut belegt (7,1 %), 102 nie am Menschen untersucht oder weit vor den Daten beworben (19,6 %), bei 264 Einträgen (50,8 %) liegt das Werbeversprechen deutlich über den Daten (Hype-Abstand höchstens 3 von 10). Lizenz CC BY 4.0, Quellenangabe „Biohacking Kompakt“ mit Link auf biohackingkompakt.de.
