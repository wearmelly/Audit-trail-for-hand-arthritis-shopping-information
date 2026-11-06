# Public data dictionary

Encoding: UTF-8. Delimiter: comma. The opening CSV row contains column names; there is no disclosure preamble. Values with embedded newlines use standard CSV quotation. Compilation license: CC BY 4.0; see LICENSE. Editor: Muhammed Veysel Erin.

## v3-reddit-hand-arthritis-heat-terms.csv

| Column | Meaning |
|---|---|
| bucket | Aggregate selection key; not a person or a post. |
| definition | Case-insensitive matching or selection rule, applied to title plus newline plus body. |
| record_count | Count of distinct post/comment records in this bucket. |
| account_count | Distinct nonempty, nondeleted author-label count; identities are not exported. Blank means no published account total. |
| evidence_id | Internal claim keys retained as public references, separated by a semicolon. |

Selection communities: rheumatoid, rheumatoidarthritis, osteoarthritis, psoriaticarthritis, thritis, lupus, arthritis, thumbarthritis. Hand filter: `\bhands?\b|finger|knuckle|thumb|wrist|\bgrip|\bjars?\b`. Deduplicate by record type and identifier, retaining the longest title-plus-body before filtering. These procedures describe the source operation; no source record identifiers are released. Buckets overlap and must not be added. Glove-only 21/19 differs from the deduplicated glove-or-warmer union 47/45. Discussion counts do not verify age, location, diagnosis, adoption or efficacy. Full method: V3-rapor.md.

## v4-maker-disclosure-audit.csv

| Column | Meaning |
|---|---|
| product_id | Stable product key from the accepted audit. Adjacent product keys begin with v3. |
| brand | Manufacturer/brand label from the sampling inventory. |
| product | Product name from the same inventory. |
| product_group | hand_massager or adjacent_product. |
| field | Original accepted field identifier; see field glossary below. |
| value | English rendering of the accepted coded value; limited maker-page summaries of at most 25 words, without adjudication notes or new claims about current terms. |
| status | stated, not-stated, conflict, or inaccessible. A restriction can be stated. |
| source_url | Historical maker-page reference; multiple references may share a cell. |
| captured_date | Historical capture date normalized to 2026-10-18. |

There are 447 accepted cells: 407 across 11 massagers, 40 across 8 adjacent products. Each massager has 37 fields and each adjacent product has 5; the combined vocabulary has 41 fields. This is not a full product-by-field rectangle. No source quotations, reviewer notes, extraction-pass columns or local capture filenames are exported. Not-stated does not mean absent. Full interpretation: V4-rapor.md.

## evidence-public.csv

| Column | Meaning |
|---|---|
| kanit_id | Claim reference used by the reports. |
| sayi | Original evidence value as text; includes counts, fractions, currency, dates and administrative values. |
| ifade | Exact scope of the claim, or a public administrative description. |
| public_file_column_filter | Published filename and column/filter, or a report section when the underlying observation is not attached. |

Retired double-count planning references are excluded. This lookup preserves original claim values, but a report-only locator is an attributed observation, not a reproducible raw-data export. V5 classified answers and the later separate analysis are not attached. V3 account totals cannot be independently reconstructed from aggregates.

## AI report provenance

V5-rapor.md describes separate historical collections. The public evidence lookup locates these claims in that report; underlying answer classifications, later analysis captures and AI source-log tables are not attached to this release. Those entries are attributed summaries, not independently recalculable observations.

## Audit field glossary

- `agirlik`: Weight.
- `ambalaj_sarti`: Packaging required for return.
- `ayri_parmak_odasi`: Separate individual finger chambers.
- `basinc_sayisal`: Pressure expressed in physical units.
- `basparmak`: Thumb coverage.
- `beden_tablosu`: Hand-size chart.
- `bilek_anilir`: Whether the wrist is mentioned.
- `bilek_isi`: Statement about wrist heating.
- `denenmis_iade`: Conditions for returning a tried/opened item.
- `diger_kesinti`: Other return deductions.
- `fiyat_usd`: Listed USD amount.
- `garanti`: Warranty terms.
- `geri_odeme_zamani`: Refund timing.
- `hazirlik_talimati`: Preparation instructions.
- `iade_adresi_ulke`: Country of return address.
- `iade_baslangic`: Return-window starting event.
- `iade_gun`: Return-window duration.
- `iade_kargo`: Who pays return freight and applicable conditions.
- `iade_kargo_tutari`: Return-shipping charge amount.
- `ic_olcu`: Internal hand dimensions.
- `isi_kademe`: Heat levels.
- `isi_tavan_f`: Maximum stated Fahrenheit temperature.
- `isi_tek_basina`: Heat operation without compression.
- `isi_var`: Heat availability.
- `kablosuz`: Cordless operation.
- `kontrol_tipi`: Physical control/interface description.
- `kutu_icerigi`: Box contents.
- `mod_sayisi`: Mode count.
- `noropati_uyarisi`: Warning concerning neuropathy or reduced sensation.
- `otomatik_kapanma_dk`: Automatic stop interval in minutes.
- `parmak_kapsami`: Finger coverage.
- `pil_suresi_dk`: Battery operation time in minutes.
- `sarj_portu`: Charging port.
- `sarj_suresi_dk`: Charging duration in minutes.
- `sarjda_kullanim`: Operation during charging.
- `sertifika_beyani`: Stated certification information, not independent verification.
- `ses_db`: Stated noise in dB.
- `uyku_uyarisi`: Warning about use while sleeping.
- `yeniden_stoklama`: Restocking deduction.
- `yogunluk_kademe`: Compression/intensity level count.
- `zorunlu_sarf`: Required consumables.

## Release metadata and layout references

Editor: Muhammed Veysel Erin. Evidence CSV format: column headers occupy the opening row [V4-99]. The original report preparation and recorded official-rule reading date was 2026-11-05 [V4-90]; this date is not a source-page publication date.

The recorded OSF Project transition notice gives 2026-11-16 as the last date for creating new Projects/Components [V4-92], and 2027-02-19 as the date existing Projects become read-only [V4-93]. These observations concern Projects, not every OSF service, and are preserved from the recorded rule check.

The documented Pinterest layout reference is a 2:3 vertical canvas, 1000 x 1500 pixels [V4-94]. It describes artwork formatting, not a dataset observation. No artwork is attached to this release.
