# Noor Hadith Data Pack

Data pack for the **Noor** Quran & prayer app — served via CDN (jsDelivr) and downloaded by the app on demand.

## Contents
- `index.json` — collections, books, counts
- `bukhari/<book>.json` — Sahih al-Bukhari, per book (97 books + introduction entries)
- `muslim/<book>.json` — Sahih Muslim, per book (57 books)
- `links.json` — Muttafaq Alayh cross-references (hadith present in both collections, with both numbers)

Each hadith: `n` = hadith number, `ib` = number within book, `ar` = Arabic text, `ur` = Urdu translation.

## Source & verification
Compiled from the open hadith-api dataset (fawazahmed0/hadith-api, itself sourced from sunnah.com data).
Counts: Bukhari 7,589 entries, Muslim 7,564 entries. Known gaps (being filled in pack v2):
Urdu missing for 570 Bukhari and 105 Muslim entries; Arabic missing for 9 Bukhari and 204 Muslim entries
(mostly chain-only cross-reference entries in Muslim). Muttafaq links are high-confidence algorithmic
matches (normalized-Arabic containment, mutual-best), spot-verified against known pairs.
