# Potts Swedenborg Concordance

Digitized text from the 5,700 pages of [Rev. John Faulkner Potts' Swedenborg Concordance](https://www.newchurchhistory.org/funfacts/indexf5a4.html?p=358) (1900, six volumes).

Although the volumes have been [scanned and made public](https://archive.org/search?query=swedenborg+concordance), the scans contain numerous OCR errors—for example, superscripts used for Swedenborg section numbers are often misread, and italic Latin principal phrases are frequently scrambled.

This edition was corrected by the staff of [New Christian Bible Study](https://newchristianbiblestudy.org/) and a team of over two dozen volunteers. The concordance is available online at [newchristianbiblestudy.org/concordance](https://newchristianbiblestudy.org/concordance) and includes later supplemented by Rev. Donald Rose.

## Repository layout

| Path | Description |
|------|-------------|
| [`text/`](text) | Concordance slices as `.swconcord` plain text (~31 MiB total) |
| [`json/`](json) | Structured JSON for each text slice (~164 MiB total) |
| [`allPotts-explicated.swconcord`](allPotts-explicated.swconcord) | Single file with all slices; reference shorthand expanded (e.g. `AC[123], --[456]` → `AC[123], AC[456]`) |
| [`concord-serialized.schema.json`](concord-serialized.schema.json) | JSON Schema for files in `json/` |
| [`docs/`](docs) | Grammar, abbreviations, and reference tables |

Text is split into many slice files so it can be processed in chunks. Alternatively, use the single combined file when you need the full concordance at once.

## Documentation

- [Concordance grammar](docs/grammar.md) — syntax and semantics of `.swconcord` text
- [Miscellaneous abbreviations](docs/misc-abbreviations.md) — keys from Potts (Comp., Def., Ex., etc.)
- [Bible book names](docs/bible-book-names.md)
- [Swedenborg works abbreviations](docs/swedenborg-works-info.csv) — updated to modern usage (CSV)

Potts's original introduction is in [`text/Concordance Introduction.md`](text/Concordance%20Introduction.md).
