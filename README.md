# The Psalms verse by verse in three public-domain English texts

**Site: [psalms-and-prayers.at01.io](https://psalms-and-prayers.at01.io/)** · Download: [latest release](https://github.com/JasonTKG/psalms-and-prayers/releases/latest)

Archived on Zenodo: [doi:10.5281/zenodo.24496794](https://doi.org/10.5281/zenodo.24496794) · also on [Kaggle](https://www.kaggle.com/datasets/jasontkg/the-psalms-verse-by-verse-kjv-asv-web) and [Hugging Face](https://huggingface.co/datasets/lakerguy16/psalms-and-prayers)

All 150 psalms, verse by verse, in three public-domain English texts, and one index row per psalm. Psalms and Prayers prints these texts side by side.

## Files

| File | Rows |
|---|---|
| `psalms_verses.csv` | 2,461 |
| `psalms_index.csv` | 150 |

## Columns

**`psalms_verses.csv`**

- `psalm`: psalm number, Hebrew (Protestant) numbering
- `verse`: verse number as in the King James Version
- `kjv`: King James Version, standard text of 1769, markup removed
- `asv`: American Standard Version (1901)
- `web`: World English Bible

**`psalms_index.csv`**

- `psalm`: psalm number
- `book`: book of the Psalter, 1 to 5
- `superscription_kjv`: the psalm's superscription in the King James Version; blank where it has none
- `verses`: number of verses in the King James Version
- `kjv_words`: words in the King James text, counted by the site
- `selah_count`: times the word Selah occurs in the King James text

## Sources

| Source | URL | Terms | Retrieved |
|---|---|---|---|
| King James (Authorized) Version, eBible.org file eng-kjv2006 | https://ebible.org/Scriptures/eng-kjv2006_usfm.zip | Public domain (in the United Kingdom the Crown's letters patent still restrict printing it) | 2026-11-24 |
| American Standard Version (1901), eBible.org file eng-asv | https://ebible.org/Scriptures/eng-asv_usfm.zip | Public domain | 2026-11-24 |
| World English Bible, eBible.org file engwebp | https://ebible.org/Scriptures/engwebp_usfm.zip | Public domain; the name is a trademark of eBible.org | 2026-11-24 |

## How it was checked

The texts are copied by program from eBible.org's USFM files; wording and spelling are never changed. Markup is removed (word tags, Strong's numbers, footnotes, line and paragraph marks). A separate program, with its own USFM reader, compares every verse on the site with the saved source files before each release, and a test with hand-made wrong edits confirms that it catches a changed word.

## Left out

The site also prints the JPS 1917 text, the Douay-Rheims, Brenton's Septuagint, the Westminster Leningrad Codex and the Clementine Vulgate, which follow other verse numberings and are not in this release. The prayers are not included: they come from several prayer books, among them the 1662 Book of Common Prayer, whose extracts the site prints under terms limited to non-commercial use. OpenBible.info cross-references (CC BY 4.0) are not included either.

## Licence

The three texts are in the public domain. The index figures and this arrangement are dedicated to the public domain under CC0 1.0 (see `LICENSE`).

## Maintainer

Built and maintained by [JasonTKG](https://github.com/JasonTKG); corrections and questions: open an issue.

Exported 2026-11-24 from the data the site's pages are generated from.
