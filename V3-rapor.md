We sell Melly, the hand massager mentioned on this page.

# Reddit language audit: warmth and hand-related arthritis discussions

## Research question and scope

This report counts selected language in an existing Reddit archive. It asks what people mention, without treating mentions as evidence of effectiveness, product adoption, or representative demand. The editorial context is shopping information for U.S. adults with hand arthritis. The source records were not restricted to that demographic.

## Archive and selection

The read-only reconstruction returns **28,931 distinct records [V3-17]** before topic selection. The analysis loader combines the local downloaded search archive, paginated comment captures, and the project's stored Reddit records. A duplicate is the same record type and record ID; when copies differ, the longer title-plus-body version is retained. This is record-level deduplication, not deduplication of people or cross-posted language.

The selected community names are `rheumatoid`, `rheumatoidarthritis`, `osteoarthritis`, `psoriaticarthritis`, `thritis`, `lupus`, `arthritis`, and `thumbarthritis`, using a case-insensitive exact match. Including the lupus community is part of the inherited selection rule, not a verified arthritis diagnosis.

The hand filter is the case-insensitive expression `\bhands?\b|finger|knuckle|thumb|wrist|\bgrip|\bjars?\b`. It runs on title, a newline, and body. Selection yields **3,499 records [V3-01]** and **2,005 account labels [V3-02]**. Wrist, grip, and jar wording can qualify a record without an explicit description of hand arthritis.

## Definitions and results

A record is a post or comment. An account count is the distinct author-label count inside the selected bucket, with blank and deleted labels excluded. Account labels are used only for counting and never supplied in the public output. The categories below describe the words sought in each record.

| Language bucket | Matching records | Distinct account labels | Source expression |
|---|---:|---:|---|
| Paraffin or wax | 109 [V3-03] | 81 [V3-04] | `paraffin`, `wax bath`, or the word `wax` |
| Warm water, dishwater, sink, or hand soaking | 70 [V3-05] | 58 [V3-06] | Hot or warm water, dishwater, sink, or hand-soaking wording |
| Heating pads | 66 [V3-07] | 65 [V3-08] | `heating pad`, `heat pad`, `electric pad` |
| Massagers or hand spas | 57 [V3-09] | 50 [V3-10] | Hand massager, massage device or machine, hand spa, or unqualified `massager` |
| Heated gloves or mitts | 21 [V3-11] | 19 [V3-12] | Heated gloves, heated mitts or mittens, or battery-and-glove wording |
| Hand warmers | 28 [V3-18] | 28 [V3-19] | `hand warmer` or `handwarmer` |
| Heated-glove or hand-warmer terms, deduplicated union | 47 [V3-20] | 45 [V3-21] | Logical OR of the preceding expressions |
| Broad pressure/glove discomfort flag | 77 [V3-13] | 75 [V3-14] | Pressure or glove terms near discomfort or intolerance wording |

The entire heated-glove expression is `heated glove|heated mitt|heat(ed|ing) mittens?|battery.{0,15}gloves?`. Its bounded wildcard is syntax, not a separate empirical result. The remaining matching expressions are specified in the reproduction instructions below.

The pressure flag searches for pressure, compression, squeezing, tightness, gloves, or rings near discomfort or inability-to-tolerate language within a sentence fragment. It is deliberately broad. Describing the flagged accounts as people who cannot tolerate an electric device would overstate the coding.

## Counting overlapping glove and warmer language

The heated-glove selection produces **21 records [V3-11] / 19 labels [V3-12]**; a distinct hand-warmer search finds **28 records [V3-18] / 28 labels [V3-19]**. These categories overlap. Their union, with each record and account counted once, contains **47 records [V3-20] / 45 labels [V3-21]**. Keep the glove-only result separate from this broader union.

## Reproduction from the archived records

- Start with the archived search results, paginated comments, and saved Reddit captures. Combine title and body for matching. Within each record type and identifier, retain the longest available text.
- Restrict community membership to the names listed above, ignoring capitalization. Then apply the hand-related expression already given.
- For water language, use `hot water|warm water|dishwater|dish water|sink|soak\w* (my )?hands`. For massager language, use `hand massager|massager|massage (device|machine)|hand ?spa`. Apply the other topic expressions shown in the table and the glove expression following it.
- For discomfort matching, search within a sentence fragment for a pressure-related word followed by pain or intolerance wording. Also admit inability-to-wear language preceding gloves, compression, tightness, or rings, and pain preceding putting on or wearing compression or gloves. Apply the original proximity bounds documented with the discomfort evidence references [V3-13] [V3-14]; these filters cover more than powered massagers.
- Run all expressions case-insensitively. Count records per match set and unique author labels after removing blank or deleted labels. Combine glove and warmer results with logical OR before deduplication.
- Compare aggregates against the bracketed references in the results. Author-count verification needs the lawful source captures; aggregate releases contain no account identities.

## Interpretation limits

Archive coverage depends on prior searches and collection choices. Repeated contributors, community selection, broad word matches, deleted content, and missing demographic verification limit inference. Categories are neither exclusive nor collectively exhaustive. No percentage is presented as a population rate. No quote is used to establish a product effect. The delivery contains aggregates only; researchers needing to validate author deduplication must have lawful access to the original local captures.

## Materials behind the counts

The inputs are previously collected Reddit search captures and comment records, existing topic annotations, and the associated archive-count summaries. Topic annotations help inspect language coding, while distinct-author checks require the original captures. Assistant-search diagnostics are a separate source and contribute no Reddit observations. Each result retains an evidence key for its counting rule and provenance.

Editor: Muhammed Veysel Erin

### Product safety statement

Heat is a constant 108°F (42°C). Skin can burn with prolonged heat contact, especially with reduced sensation.

If you have numbness, reduced sensation or neuropathy, keep the heat off or do not use this product.

Do not use on a hot, swollen joint.

This is not a treatment. If your hands go numb at night, or symptoms keep coming back, talk to your doctor.

Related reading: https://wearmelly.com/blogs/guides/hand-arthritis-reddit-records?utm_source=report&utm_medium=report&utm_campaign=artrit-dagitim
