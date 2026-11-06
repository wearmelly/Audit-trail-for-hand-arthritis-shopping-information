We sell Melly, the hand massager mentioned on this page.

# A dated audit of hand-care product documentation

## Objective

For an adult shopping in the United States with hand arthritis, a specification and a return policy answer different questions. This audit records whether selected manufacturer pages provided the relevant information. It does not score devices or infer a therapeutic outcome.

## Material and sampling

The input is an adjudicated manufacturer-documentation table, read alongside its field definitions and archived-page inventory. The sample contains **19 products [V4-03]**: **11 powered hand massagers [V4-01]** and **8 neighboring products [V4-02]**. Inclusion follows the historical category-audit selection, rather than a random sample of all products for sale.

The acquisition date is **October 18, 2026 [V4-21]**. Some access cells contain timestamps and others only the date. The underlying references are the sellers' own product pages, product data, return terms, support pages, and available manuals. Retailer listings and customer reviews are outside this audit's evidence base. Archived inaccessible pages remain marked as such.

## Shape of the accepted data

| Part of the table | Product count | Fields per product | Accepted records |
|---|---:|---:|---:|
| Powered hand massagers | 11 [V4-01] | 37 [V4-04] | 407 [V4-07] |
| Adjacent products | 8 [V4-02] | 5 [V4-05] | 40 [V4-08] |
| Combined compilation | 19 [V4-03] | 41 distinct field names overall [V4-06] | 447 [V4-09] |

The combined field vocabulary is not assigned to every product. Multiplying the combined product count by the combined field count would create cells that were never collected.

## Extraction and definitions

The original workflow saved source pages, extracted values in independent passes, compared the outputs, and resolved disputed or suspiciously empty cells against the captures. An earlier extraction summary covers neighboring products; it is process documentation rather than an additional observation set.

`stated` means the reviewed maker material supplies the field's value. `not-stated` means no supporting statement was found in the pages reviewed. `conflict` preserves inconsistent statements. `inaccessible` means the relevant material could not be read. A stated return restriction counts as documentation even when it prevents a requested type of return.

The accepted status totals are **226 stated [V4-15]**, **201 not-stated [V4-16]**, **11 conflict [V4-17]**, and **9 inaccessible [V4-18]** records. Their sum equals the accepted table's **447 rows [V4-09]**. The separate agreement report concerns extraction comparisons; its agreement total is not substituted for the accepted status counts.

## Descriptive findings

| Field in the accepted source | Explicitly documented among hand massagers | Interpretation |
|---|---:|---|
| Heat without compression | 0/11 [V4-10] | No explicit standalone-heat documentation was accepted. |
| Pressure in physical units | 0/11 [V4-11] | No numerical pressure value with a physical unit was accepted. |
| Heat availability | 11/11 [V4-12] | Heat availability was documented throughout this sample. |
| Maximum stated temperature | 8/11 [V4-13] | A temperature ceiling was stated; this is not skin-temperature evidence. |
| Return-window duration | 11/11 [V4-14] | A time window alone does not settle the rest of the policy. |
| Conditions for returning tried items | 10/11 [V4-19] | Text addressing tried-item conditions was found; this does not mean all accepted used returns. |
| Responsibility for return freight | 8/11 [V4-20] | A rule about who pays was explicit; payment need not be the seller's. |

The standalone-operation finding asks whether heat works without compression; it does not ask whether heat is mentioned at all. These observations concern archived maker disclosures. They establish neither current brand policies nor present-day prices.

## Reproducing the documentation counts

- Import the adjudicated product-field table with a CSV reader that handles quoted passages spanning several lines.
- Identify products using the table's product key and classify them as powered massagers or adjacent products using the accompanying schema.
- Within each group, count products, distinct field names, and accepted product-field observations separately. Check uniqueness of every product-and-field pair.
- Select each reader-facing field listed above. Count explicit statements among the massager observations for that field; retain its full massager denominator.
- Preserve the status distinctions: a restrictive return term remains a stated term. Count conflicts and unreadable references separately from undocumented values.
- Follow the source-page reference, saved passage, and capture date associated with each observation. Validate historical wording against saved material rather than assuming a current page is identical.
- Use the aggregate count summary as a cross-check. The extraction-agreement summary describes the review process and is not a substitute for the adjudicated observations.

## Limits and reuse

Some fields are broad or depend on interpretation of page wording. Unread pages and missing manuals can hide disclosures. The sample is small and selected, and policies can change after capture. This audit supports checking documentation gaps; it does not justify an absence claim about an entire market, a safety rating, or an effectiveness comparison.

## Evidence materials

The primary material is the accepted manufacturer-disclosure table. Supporting records include field definitions, an archived-page index, count summaries, and the extraction review with adjudication notes. The older public feature compilation supplies release context. Evidence keys connect the reported values to the relevant field, status, and capture-date selection.

Editor: Muhammed Veysel Erin

### Product safety statement

Heat is a constant 108°F (42°C). Skin can burn with prolonged heat contact, especially with reduced sensation.

If you have numbness, reduced sensation or neuropathy, keep the heat off or do not use this product.

Do not use on a hot, swollen joint.

This is not a treatment. If your hands go numb at night, or symptoms keep coming back, talk to your doctor.

Related reading: https://wearmelly.com/blogs/guides/how-to-choose-hand-massager-arthritis?utm_source=report&utm_medium=report&utm_campaign=artrit-dagitim
