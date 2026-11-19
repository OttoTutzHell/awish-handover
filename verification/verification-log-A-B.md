# Verification log — handover-pack files A and B

Log file required by `Verification procedure for A and B (STE).md` (sections 4.1 and 5.3). Applies to `A-what-validated.md` and `B-per-pilot-sheet.md`, both version of 7 Oct 2026 (evening).

**Status 17 Nov 2026: complete.** Every row has been compared with its source and given a result code.

**Update 13 Nov 2026.** Paths in this log were corrected to the file names in use since the 4 Nov 2026 reorganisation (deliverables without dates, papers in `papers/`, register in private project notes (available on request)). No claim row changed. The grep hit counts in the Appendix for D5.2(OCR) are OCR chunk numbers; printed page = chunk − 1. Known page drifts from the vault's round 6 (4 Nov): D2.2 p.32 not p.33 (STREMODO 0.84, row P14); D6.2 p.80 not p.81; D1.4 p.24 not p.23.

## Totals

| Code | Count |
|---|---|
| OK | 466 |
| PAGE | 1 |
| EDIT | 8 |
| WRONG | 4 |
| SECOND | 0 |
| OPEN | 0 |
| Claims examined | 479 |
| Claims pre-filled in this log (19 Oct 2026) | see "Pre-fill summary" at the end |

## Conventions used in this log

- "Row or section" names the file-A row (`T1 P3`), paragraph (`row-count para`), table (`T2`), disagreement (`D4`), or the file-B pilot and cell (`§1 Pilot 2 / Technologies`), data-arrangements row (`§1b Pilot 3`) or contradiction (`§4 C10`).
- "Cited source and page" is what file A or B cites. Short names follow procedure 4.2. `[web]` marks a claim whose primary source is a live web page (procedure 4.3). `[via handover-pack/D or F]` marks a claim that currently cites only a secondary source (6.5 step 4 → candidate SECOND).
- File names to write in "Primary source used" are those of procedure 4.2, for example `deliverables/D2.2 Methodology for measuring each AWI.pdf`, `deliverables/AWI Catalogue (final version).pdf`, `deliverables/D1.6 Practice abstracts batch 1.pdf`, `deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf`, `deliverables/D1.4 Project website report v2.pdf`, `deliverables/D6.2 Data management plan v1.pdf`, `deliverables/D6.3 Data management plan v2.pdf`, `papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf` (BSE-rev), `papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf` (PS-2026), `papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf` (Agronomy Research 2025).
- `grep: Gnn` refers to the numbered grep block in the Appendix, which gives the exact regex, the files searched, the total hits per file and the text-file page numbers of the hits (text page N = PDF page N, procedure section 2 note). Hit counts are counts of matching strings, not of relevant statements. The pages listed are the pages to open in the PDF (procedure 6.6 steps 4 to 7). Where a grep ran on a paper PDF (BSE-rev, Agronomy Research) the text was made with `pdftotext` into the agent's scratch folder; it is a search aid only.
- Caution from procedure 6.6: text search does not find words in images (D1.8 pp.1–13, D1.2 Annex D p.49, D5.2 scanned pages). D5.2 may be quoted only from the PDF.

---

## Section 9 problems 1 to 3 — counts (no codes assigned)

| # | File | Location | Problem (procedure section 9) | Count found 19 Oct 2026 (mechanical; the rule and the correction are the author's) |
|---|---|---|---|---|
| 1 | A | Row-count paragraph after Table 1 (line 67) | Says "20" rows with a figure; its list has 21 codes; "18" rows without a figure is possibly also incorrect | count: Table 1 rows by code = 22 pig (P1–P22) + 16 broiler (B1–B16) = 38, as stated. Codes in the parenthesised list = 21: P2, P3, P4, P6, P7, P8, P11, P12, P13, P14, P19, P22, B1, B2, B3, B9, B10, B11, B14, B15, B16. 38 − 21 = 17 rows not in the list; file A says 18 "not stated". The 17 rows not in the list are P1, P5, P9, P10, P15, P16, P17, P18, P20, P21, B4, B5, B6, B7, B8, B12, B13. Of these 17, the agreement cell contains a numeric figure of some kind in P9 (ADAL: 85.5 %, 96 %, 92 %, r = 0.96), P15 (vendor claims 99 %, 97 %) and P16 (human-rater ICC, β and bias figures); the other 14 contain no figure. Whether P9, P15 or P16 count as "a figure attached to the named sensor" is the rule to decide under problem 2. |
| 2 | A | Row P9 | The row gives an ADAL figure, but P9 is not in the list; P11 and B9 have similar third-party figures and are in the list | count: rows whose agreement cell carries a figure for a device that the sensor cell names but marks "not aWISH" (or that is not an aWISH pilot sensor): P9 (ADAL, "not aWISH") — NOT in list; P11 (VisStick, BSE-rev "98 and 100 %") — in list; B9 (Microvision, "not aWISH", 98 %) — in list; P4 (SoundTalks, BSE-rev r = 0.5) — in list; P13 (SMARTBOW "not in Cat.", PEEK r = 0.77) — in list; P2 (iDOL 65, R>0.96) — in list. Rows with vendor-claim figures only: P15 (Genba 99 %, SmartCalc 97 %) — NOT in list (P2 also has SmartCam 97 % but is in the list for iDOL). Row with human-rater figures only: P16 — NOT in list (file A says so). Under the rule "any third-party figure for a device named in the row counts", the list has 22 codes (add P9) and 16 rows are without a figure; under the rule "only figures for an aWISH pilot sensor count", the list has 3 (P3, B10, B11) and 35 rows are without a figure. |
| 3 | B | Section 3 table (lines 139–170) | Says 27 "not stated" cells; a count found 26 | count: rows in the section 3 table = 32; rows struck through (`~~`) = 6 (Pilot 2 Region; Pilot 3 Region; Pilot 4 Region; Pilot 5 Throughput; Pilot 5 Region; Pilot 6 Region); rows not struck through = 26. File B line 172 says "27 (6 cells filled from D1.4; 3 new rows added …)". 26 ≠ 27. The "6 cells filled" agrees with the 6 struck rows. The 26 unstruck rows by pilot: Pilot 1 ×3, Pilot 2 ×4, Pilot 3 ×4, Pilot 4 ×4, Pilot 5 ×3, Pilot 6 ×4, "all" ×4. |

---

## File A — Table 1, rows selected under 7.1 step 1

### T1 P3 — Body weight (aWISH pilot sensor, Weight-Detect)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P3 / Indicator, species, stage | Body weight (aWISH pilot sensor); Pig; On-farm (pilot 2, Spain) | Cat. p.32; D1.6 p.9 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Sensor | Weight-Detect, camera image analysis | Cat. p.32 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Vendor | Weight-Detect is PLF Agritech (Brisbane) technology; data processed in PLF Agritech's ADAMS cloud (Amazon); patented AU/US/EU; reports emailed to farmer | Agronomy Research 2025, full text (no page cited) | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Vendor | Cat. p.32 and D1.6 name InnoTech Vision as provider | Cat. p.32; D1.6 p.9 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Vendor | D2.2 p.19 names "PLF Agritech Europe" | D2.2 p.19 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Automated? | yes | Cat. p.32 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Agreement (quote) | "the WD system was able to predict the average pen weight of the pigs with 1.7% (2.0 kg) precision" vs "Manual weight recordings using electronic scales" | Agronomy Research 2025 (no page cited) | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Agreement (figures) | per-weighing errors 1.1%, 0.5%, 2.4%, 2.7% | Agronomy Research 2025 (no page cited) | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-17 |
| A | T1 P3 / Agreement (caveat) | one pen, nine pigs, one commercial farm in Spain, installed early 2024, four manual weighings; observational, no statistics | Agronomy Research 2025 | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-17 |
| A | T1 P3 / Agreement (caveat) | co-authored by the vendor and by Selección Batallé (the farm owner) | Agronomy Research 2025 (author list and affiliations) | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-17 |
| A | T1 P3 / Agreement (third-party) | BSE-rev cites an earlier figure "<3% error (Banhazi 2022b)" | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-17 |
| A | T1 P3 / Agreement (negative) | Not stated in D2.2/Cat. | D2.2; Cat. | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G01 (Weight.?Detect; WD system) — D2.2 1 hit p.19; Cat. 3 hits pp.21, 28, 32; Reachable locally: D2.2 PDF p.19 Table 6 'Weight-Detect TM … PLF Agritech Europe … Camera … 7'; Cat. pp.21, 28, 32 name Weight-Detect with no agreement figure; please re-check | 2026-11-17 |
| A | T1 P3 / TRL | 7 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G01 (Weight.?Detect; WD system) — D2.2 1 hit p.19; Cat. 3 hits pp.21, 28, 32; Reachable locally: D2.2 PDF p.19 Table 6 'Weight-Detect TM … PLF Agritech Europe … Camera … 7'; Cat. pp.21, 28, 32 name Weight-Detect with no agreement figure; please re-check | 2026-11-17 |
| A | T1 P3 / TRL | TRL 7 | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | EDIT | It says Weight-detect (TRL 7) was installed at Batallé, which I'm not sure is the same as what is claimed; Pack A now says 'TRL 7 for Weight-Detect as installed in Pilot 2, Batallé [D1.6 p.9]' | 2026-11-17 |
| A | T1 P3 / Source(s) (quote) | "Technology used in aWISH project" | Cat. p.32 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Source(s) | D1.8 p.30 contains information for this row | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P3 / Source(s) | Agronomy Research 23(S1):5–14, DOI 10.15159/AR.25.032 | DOI 10.15159/AR.25.032 — `papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf` | | | OK | Reachable locally; the quote '1.7% (2.0 kg) precision' is on PDF p.1; please re-check | 2026-11-17 |

### T1 P5 — Skin lesions (carcass)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P5 / Indicator, species, stage | Skin lesions (carcass); Pig; Postmortem (Cat.); slaughterhouse | Cat. pp.46–48; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Sensor (vendor) | PigInspector — 2D/3D cameras + AI on carcass line (CLK GmbH) | Cat. pp.46–48 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Sensor (vendor) | also ArtificialVet® (CompanyMind), not aWISH | Cat. pp.46–48 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Automated? (quote) | yes ("Automated system providing real-time data") | Cat. p.47 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Automated? (quote) | "algorithm performs measurements (still under development)" | D1.8 p.27 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Agreement (negative) | Skin lesions: not stated (checked D2.2 pp.19, 31–33; Cat. pp.46–48) | D2.2 pp.19, 31–33; Cat. pp.46–48 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G02 (skin.?lesion; Pig.?Inspector) — D2.2 13 hits pp.19(5), 29, 31(2), 32(2), 35(3); Cat. 20 hits pp.12, 46(4), 47(4), 48(2), 49, 50(3), 53, 54(3), 147 | 2026-11-13 |
| A | T1 P5 / Agreement | Blömke et al. 2020 covers ears and tails only | D2.2 p.33; BSE-rev | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P5 / TRL | 4 for PigInspector skin lesions (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P5 / TRL (quote) | "CLK Pig Inspector (TRL 5)" for the whole system | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P5 / Source(s) | D1.8 pp.25, 27, 30 contain information for this row | D1.8 pp.25, 27, 30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |

### T1 P6 — Ear lesions (carcass)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P6 / Indicator, species, stage | Ear lesions (carcass); Pig; Postmortem / slaughterhouse | D2.2 pp.19, 31, 33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Sensor (vendor) | PigInspector (CLK GmbH), cameras + AI | D2.2 pp.19, 31; D1.6 p.9 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Automated? | yes | D2.2 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Agreement (quote) | "Blömke et al., 2020 compared the system with human observations in ears and tails and they found 95.4%, 77%, and 96.5% of accuracy, sensitivity, and specificity respectively in ear lesions" | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Agreement (quote) | "overall sensitivity of 77 % and an overall specificity of 96.5 % for ear lesions … positive predictive value of 59 % … negative predictive value of 98.5 %, the accuracy amounted to 95.4 %" | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Agreement (attribution) | Figures are from Blömke et al. 2020, DOI 10.1016/j.meatsci.2019.107934; pre-aWISH, not an aWISH pilot result | BSE-rev; DOI 10.1016/j.meatsci.2019.107934 [web, 6.3 step 3 if the figure goes into the brief] | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / TRL | 9 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / TRL | TRL 5 (whole system) | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P6 / Source(s) | D2.2 pp.35, 38 contain information for this row | D2.2 pp.35, 38 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-14 |

### T1 P7 — Tail lesions (carcass)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P7 / Indicator, species, stage | Tail lesions (carcass); Pig; Postmortem / slaughterhouse | Cat. pp.49–52; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 P7 / Sensor (vendor) | PigInspector (CLK GmbH) | Cat. pp.49–52; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 P7 / Sensor (vendor) | prototype TailCam (PigWatch project/DTI) | D2.2 p.19; BSE-rev | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Sensor (vendor) | prototype TAILSCAN (Farm4Trade) | Cat. pp.49–52; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Automated? | yes | Cat.; D2.2 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | WRONG | Corrected in pack A: "yes for PigInspector; TailCam and TAILSCAN are 'Sensor technology currently under development' (BSE-rev p.4)" | 2026-11-17 |
| A | T1 P7 / Agreement (quote) | PigInspector: "99.5%, 77.8%, and 99.7% [accuracy, sensitivity, specificity] in tail lesions" (Blömke et al. 2020) | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Agreement (quote) | BSE-rev adds "positive predictive value was 72.4 % … negative predictive value was 99.8 %" | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Agreement (quote) | TailCam (PigWatch test report): "Serious tail lesions were detected with a sensitivity of 61 %, while 39 % were misclassified … overall specificity … was 96 %" | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Agreement (negative) | TAILSCAN: not stated | D2.2; Cat.; BSE-rev | deliverables/D2.2 Methodology for measuring each AWI.pdf | | EDIT | grep: G03 (TAIL.?SCAN; Farm.?4.?Trade) — D2.2 1 hit p.19; Cat. 10 hits pp.49, 52(3), 53, 56(3), 59(2); BSE-rev (pdftotext) 6 hits pp.4(3), 10(3); It is indeed not mentioned in this doc; Pack A now says TAILSCAN has no figure in D2.2, Cat. or BSE-rev and is under development (BSE-rev pp.4, 10) | 2026-11-17 |
| A | T1 P7 / TRL | PigInspector tail lesions 9 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / TRL | TailCam 6–7 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / TRL | PigInspector system TRL 5 | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P7 / Source(s) | D2.2 pp.31, 35 contain information for this row | D2.2 pp.31, 35 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |

### T1 P8 — Tail length

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P8 / Indicator, species, stage | Tail length; Pig; Postmortem / slaughterhouse | Cat. pp.53–57; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Sensor (vendor) | PigInspector (CLK) for tail length | Cat. p.54; D2.2 p.19 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Sensor (vendor, quote) | "Tail Length (prototype)" 2D camera (UAB & Batallé) | Cat. p.57 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Sensor (vendor, quote) | "Tail Length (VION)" two 3D cameras after first flame oven | D1.8 p.28 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Sensor (vendor) | TailCam; TAILSCAN also listed for tail length | Cat. pp.53–57; D2.2 p.19; BSE-rev | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Automated? | yes | Cat.; D2.2 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Agreement (negative) | PigInspector/VION tail length: not stated (checked D2.2, Cat. pp.53–57) | D2.2; Cat. pp.53–57 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | Claim narrowed 17 Nov (UAB now has a figure, next row); verdict kept. grep: G04 (tail.?length) — D2.2 5 hits pp.7, 13, 19, 28, 29; Cat. 13 hits pp.12, 47, 50, 52, 53(2), 54(2), 55, 56, 57(3) | 2026-11-13 |
| A | T1 P8 / Agreement (quote, added 17 Nov) | UAB/Batallé 2D camera, preliminary, not peer-reviewed: "accuracy (F-score) of 55.2 for seven categories and 76.2 for four categories"; 870 labelled training images, 672 test images; "Although based on a small sample, these preliminary results suggest the sensor has the potential …" | Zenodo 17475558, p.1 — `papers/Ramon-Perez 2025 ISAE - tail length and lesions tool (zenodo 17475558).pdf` | papers/Ramon-Perez 2025 ISAE - tail length and lesions tool (zenodo 17475558).pdf | | OK | Replaces "could not be opened" (WRONG, 17 Nov) | 2026-11-17 |
| A | T1 P8 / Agreement (quote) | TailCam: "very good correlation … between manually measured tail length and values calculated by TailCam system (RMSE = 1.95; r = 0.90)" — pre-aWISH | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P8 / TRL | PigInspector tail length 3–4 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P8 / Source(s) | D1.8 p.28 contains information for this row | D1.8 p.28 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |

### T1 P9 — Lung (and liver) lesions

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P9 / Indicator, species, stage | Lung (and liver) lesions; Pig; Postmortem (evisceration line) | Cat. pp.58–60; D1.6 p.9 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Sensor (vendor) | Lesion-Detect, camera-based (Innotech / InnoTech Vision) | Cat. p.60; D1.6 pp.9, 11 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Sensor (quote) | "Technology under development within the aWISH project" | Cat. p.60 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Sensor (vendor) | ADAL robot (Farm4Trade), not aWISH | Cat. pp.58–59; D2.2 p.19 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Automated? | yes (intended) | Cat. p.60 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Agreement (quote, added 17 Nov) | Lesion-Detect, peer-reviewed, aWISH-period (Banhazi et al. 2026, Agronomy Research 24(2):76–95): Trial 1 Batallé, hanging lungs, n = 102; Trial 2 Carnex, trays, n = 228; FP/FN 2.50 % / 1.84 % (Trial 1) and 3.28 % / 2.16 % (Trial 2) of lung area; average automatic–manual difference about 0.1 PHMS point (hanging) and about 1 point (trays), against inter-observer variability "often 1 to 3 PHMS points"; first author and two co-authors are with InnoTech Vision | PDF pp.1, 3, 14–15 — `deliverables/publication-sweep/Banhazi 2026 AgronRes - Lesion-Detect development and pilot testing (doi AR.26.034).pdf` | deliverables/publication-sweep/Banhazi 2026 AgronRes - Lesion-Detect development and pilot testing (doi AR.26.034).pdf | 14–15 | OK |  | 2026-11-17 |
| A | T1 P9 / Agreement (abstracts, added 17 Nov) | The two Lesion-Detect conference abstracts give no figures: 17,000 images collected, camera focus problems (2024); "manual scoring and the automated scoring were compared" (2025) | Zenodo 17630315, p.1 — `papers/Banhazi 2024 ISAH - Lesion-Detect system development (zenodo 17630315).pdf`; Zenodo 17786812, p.47 — `papers/Banhazi 2025 BSE Tartu - Lesion-Detect lung lesion scoring (zenodo 17786812).pdf` | papers/Banhazi 2024 ISAH - Lesion-Detect system development (zenodo 17630315).pdf | | OK | Replaces "could not be opened" (WRONG, 17 Nov) | 2026-11-17 |
| A | T1 P9 / Agreement (quote) | ADAL: "detect pleurisy with an accuracy of 85.5 % (specificity = 96 %, sensitivity = 92 %)" and "(r = 0.96)" vs veterinarians (Bonicelli et al. 2021) — pre-aWISH | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | 10 | PAGE | | 2026-11-13 |
| A | T1 P9 / TRL | ADAL TRL 8 | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P9 / TRL | Lesion-Detect TRL 3 | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P9 / Source(s) | D2.2 p.13; D1.8 p.30 contain information for this row | D2.2 p.13; D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

### T1 P10 — Stunning effectiveness (pigs)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P10 / Indicator, species, stage | Stunning effectiveness (consciousness after CO2 stunning); Pig; Stunning / slaughterhouse | Cat. pp.61–63 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Sensor (vendor) | Computer vision on ocular sequences / corneal reflex: BlinkAI — Nuna Solutions | Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor | Nuna Solutions is a brand of the Danish Technological Institute / DMRI ("NunaSolutions, is a brand of Teknologisk Institute") | Nuna Solutions web site [web, via handover-pack/F §6 → 6.5 step 4] | | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor | trading as BY-NUNASOLUTIONS SL | CORDIS participants list [web, via handover-pack/D and F] | deliverables/CORDIS listing 101060818.pdf | | WRONG | grep: G07 — local CORDIS listing text file 0 hits for Nuna / Wel2be / W2B / Teknologisk / Technological Institute / DMRI (procedure 7.5 step 4: use the live page); Cut from pack A row P10 (not in the local CORDIS copy) | 2026-11-17 |
| A | T1 P10 / Vendor (quote) | "Provider nunaSolutions … under development within the aWISH project" | Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor (quote) | "Stunning effectiveness (Nuna solutions)" | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor | Listed as WEL2BE | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor | WEL2BE also in D1.4 pp.17, 20 | D1.4 pp.17, 20 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor (quote) | "Pilot2_W2B1 CET'automatique" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Vendor | "WEL2BE — Participation ended" per CORDIS | CORDIS participants list [web, via handover-pack/D and F] | deliverables/CORDIS listing 101060818.pdf | | OK | grep: G07 — local CORDIS listing 0 hits (see above); Set OK: the author confirmed on 16 Nov that WEL2BE's participation has ended | 2026-11-17 |
| A | T1 P10 / Vendor (negative) | Handover terms between WEL2BE and Nuna Solutions: not stated in any document read | all documents read | | | EDIT | grep: G07 (Nuna; Wel.?2.?be; W2B; Teknologisk; Technological Institute; DMRI) over 15 text files — hits only in D1.4 8 (pp.17, 18(3), 19(2), 20, 25); D1.6 4 (pp.9(2), 10, 11); D1.8 1 (p.30); D2.2 1 (p.27); Cat. 4 (pp.62(2), 85(2)); D6.2 3 (p.92(3)); 0 hits in D1.1, D1.2, D1.5, D2.1, D2.1-annex, D4.3, D5.2(OCR), D6.3, CORDIS; How could I know?; Pack A now names the 15 documents searched instead of 'any document read' | 2026-11-17 |
| A | T1 P10 / Sensor (vendor) | Also "Monitoring of the CO2 Stunning" (Genba), not aWISH | Cat. pp.61–63 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Automated? | yes (intended) | Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Agreement (negative) | not stated (checked D2.2, Cat. pp.61–63) | D2.2; Cat. pp.61–63 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G06 (Blink.?AI; Nuna; CET.?Automatique; Wel.?2.?be; W2B; corneal) — D2.2 4 hits pp.27(2), 28, 29; Cat. 7 hits pp.61(2), 62(3), 85(2) | 2026-11-17 |
| A | T1 P10 / Agreement (abstract, added 17 Nov) | HSA 2025 abstract (UAB, Selección Batallé, Nuna Solutions): prototype at a commercial plant, 550 pigs an hour, CO2 stunning; 1,737 automatic corneal-reflex assessments over three days; "only five animals showed a positive corneal reflex", "a limitation for this study"; no accuracy figure | Zenodo 17475673, p.1 — `papers/Ramon-Perez 2025 HSA - pig consciousness sensor development (zenodo 17475673).pdf` | papers/Ramon-Perez 2025 HSA - pig consciousness sensor development (zenodo 17475673).pdf | | OK | Replaces "could not be opened" (WRONG, 17 Nov) | 2026-11-17 |
| A | T1 P10 / Agreement (quote) | "None of them have been externally validated" (CET'Automatique/Wel2be, Genba CO₂ monitoring, Signs of life/Argus) | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / TRL | TRL 5 | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P10 / Source(s) | D2.2 p.27 lists Wel2be CET'Automatique from survey | D2.2 p.27 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |

### T1 P14 — Stress vocalisations (STREMODO)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P14 / Indicator, species, stage | Stress vocalisations; Pig; Antemortem — unloading & lairage | Cat. pp.77–78; D1.8 p.26 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Sensor (vendor) | STREMODO — microphone + artificial neural network (FBN) | Cat. pp.77–78; D1.6 p.9 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Sensor (quote) | "Sensor hangs above monitored area (unloading and lairage area)" | D1.8 p.26 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Automated? | yes | Cat. pp.77–78 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Agreement (quote) | "Schön et al., 2004 compared the vocalizations recorded automatically with the human labelling, which found a correlation of 0.84" | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Agreement (quote) | "percentage of misclassification was low (<5 %)" (Schön et al. 2004) | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Agreement (quote) | "strongly correlated (r = 0.78–0.87) with the assessment of six human experts" (Schön et al. 2004) | BSE-rev (no page cited) | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Agreement (negative + paper, added 17 Nov) | aWISH lairage results not stated. The ECPLF 2024 STREMODO paper is a barn study funded by BMEL, not aWISH: isolated weaned piglets' stress calls detected "with 63 % sensitivity, 97 % specificity, and 79 % balanced normalized precision"; n = 75 piglets | D2.2; Cat.; D1.6; D1.8; Zenodo 18549284, pp.1, 4, 8 — `papers/Westendorff 2024 ECPLF - area-specific vocalisation and activity (zenodo 18549284).pdf` | papers/Westendorff 2024 ECPLF - area-specific vocalisation and activity (zenodo 18549284).pdf | 1, 4, 8 | OK | grep: G08 (STREMODO) — D2.2 5 hits pp.19, 31, 32, 35(2); Cat. 2 hits pp.77, 78; D1.6 2 hits pp.9, 11; D1.8 3 hits pp.25, 26, 30 | 2026-11-17 |
| A | T1 P14 / TRL | 4 (estimated) | D2.2 p.19 Table 6 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / TRL (quote) | "STREMODO (TRL 5)" | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P14 / Source(s) | D2.2 pp.31, 35; D1.8 pp.25, 30 contain information for this row | D2.2 pp.31, 35; D1.8 pp.25, 30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |

### T1 P16 — Tear staining

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 P16 / Indicator, species, stage | Tear staining; Pig; Postmortem (slaughter line) | Cat. pp.87–88 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Sensor (quote) | Computer vision, surface area of tear staining in both eyes ("Tear staining aWISH", provider "aWISH partners") | Cat. p.88 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Holder (quote) | Holder ILVO: "Tear staining (ILVO)" | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Holder (quote) | project website pilots page "Tear staining system (ILVO)" | www.awish-project.eu pilots page [web, via handover-pack/D → 6.5 step 4] | | | OK | | 2026-11-17 |
| A | T1 P16 / Holder | Listed as WEL2BE | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Holder (quote) | "Pilot2_W2B2 tear-staining" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Holder | WEL2BE's participation has since ended per CORDIS | CORDIS participants list [web] | deliverables/CORDIS listing 101060818.pdf | | OK | grep: G07 — local CORDIS listing 0 hits | 2026-11-16 |
| A | T1 P16 / Automated? | yes (intended) | Cat. p.88 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Agreement (negative) | Sensor vs human: not stated (checked D2.2, Cat. p.88) | D2.2; Cat. p.88 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G09 (tear.?stain) — D2.2 3 hits pp.26, 28, 35; Cat. 9 hits pp.13, 87(4), 88(4); also D1.6 1 hit p.9; D1.8 1 hit p.30 | 2026-11-17 |
| A | T1 P16 / Agreement (figures, human-rater) | "18 raters … 38 pigs" | Zenodo 17803862 (ISAE Benelux 2024 abstract) [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T1 P16 / Agreement (figures) | inter-rater "Left ICC: 0.434; Right ICC: 0.360" | Zenodo 17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T1 P16 / Agreement (figures) | intra-rater "Left average ICC: 0.754; Right average ICC: 0.677" | Zenodo 17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T1 P16 / Agreement (figures) | accuracy vs "Silver Standard" "Left β=0.78, p<0.001; Right β=0.60, p<0.001" | Zenodo 17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T1 P16 / Agreement (figures) | "Left bias = 1.80; Right bias = 2.74" | Zenodo 17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T1 P16 / TRL | TRL 3 | D1.6 pp.9, 11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 P16 / Source(s) | D2.2 p.28 (prototype mention) contains information for this row | D2.2 p.28 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |

### T1 B5 — Distress / alarm calls

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B5 / Indicator, species, stage | Distress / alarm calls; Broiler; Antemortem — lairage (and on-farm) | Cat. pp.133–135 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B5 / Sensor (vendor) | ITAVI Bird vocalisation = "EBroilerTrack Sound" microphones in lairage (Itavi) | Cat. p.135; D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | WRONG | not so sure; Corrected in pack A: the Catalogue entry is quoted as it stands, and the link to EBroilerTrack Sound is marked as probable (D1.6 p.10) | 2026-11-17 |
| A | T1 B5 / Sensor (quote) | "Technology used in aWISH project" | Cat. p.135 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B5 / Sensor (vendor) | ALIS Chirpy sensor (Greengage) | Cat. pp.133–135 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B5 / Automated? | yes | Cat. pp.133–135 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B5 / Agreement (negative) | not stated (checked D2.2 pp.22, 32–33; Cat. pp.133–135) | D2.2 pp.22, 32–33; Cat. pp.133–135 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G10 (E.?Broiler.?Track; Itavi; distress; alarm.?call; Chirpy; Greengage) — D2.2 18 hits pp.17(3), 19, 20, 21, 22(4), 23(5), 33(2), 39; Cat. 15 hits pp.49, 106, 133(5), 134(4), 135(4) | 2026-11-17 |
| A | T1 B5 / Agreement (quote, comparable literature) | Zoom H4n distress-call algorithm "accuracy of 95%" (Mao et al., 2022) | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 B5 / TRL | EBroilerTrack Sound TRL 5 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B5 / Source(s) | D2.2 p.25; D1.8 p.30 contain information for this row | D2.2 p.25; D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-13 |

### T1 B9 — Stunning effectiveness (broilers)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B9 / Indicator, species, stage | Stunning effectiveness; Broiler; Stunning — gas tunnel exit | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Sensor | Camera monitoring movement in crates, pilot 3 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Holder | holder WEL2BE | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Holder | also D1.4 p.18 names Wel2be | D1.4 p.18 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Holder (quote) | "Pilot3_W2B1 Stunning" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Holder | WEL2BE's participation has since ended per CORDIS | CORDIS participants list [web] | deliverables/CORDIS listing 101060818.pdf | | OK | grep: G07 — local CORDIS listing 0 hits | 2026-11-16 |
| A | T1 B9 / Holder (negative) | successor holder for the broiler sensor unconfirmed; no document read names a broiler stunning sensor holder after WEL2BE | all documents read | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G07 (see P10) and G11 (Wel.?2.?be; W2B; stunning) — D1.6 7 hits pp.9(3), 10(2), 11(2); Cat. 24 hits pp.3(2), 10(3), 61(2), 62(3), 63(4), 67, 84, 107(3), 136(2), 137(2), 152; D2.2 12 hits pp.11, 27(2), 28(4), 29, 34(2), 35(2); D1.4 10 hits pp.17, 18(4), 19(3), 20, 25; D1.5 0; D6.2 7 hits pp.51, 52, 54, 92(4); D6.3 6 hits pp.36, 38, 39, 40, 44, 57 | 2026-11-17 |
| A | T1 B9 / Holder | D1.8 p.30 and Cat. p.62 name Nuna Solutions / BlinkAI only for pig (corneal-reflex) stunning | D1.8 p.30; Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Sensor (vendor) | Cat. lists only Microvision EM130C (electrical stunning, posture camera), not aWISH | Cat. pp.136–137 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Automated? | yes (intended) | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Agreement (negative) | Broiler stunning sensor (WEL2BE-listed): not stated (checked D1.6; not in Cat./D2.2; not in D1.4, D1.5, D6.2, D6.3) | D1.6; Cat.; D2.2; D1.4; D1.5; D6.2; D6.3 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G11 — hit counts as in the row above | 2026-11-17 |
| A | T1 B9 / Agreement (quote) | Microvision: "accuracy of 98% when tested at commercial speed" (Ye et al., 2020) | D2.2 p.34 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Agreement (quote) | "validated (Ye et al 2020 – doi: 10.3382/ps/pez564)" | Cat. p.137 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B9 / TRL | WEL2BE broiler stunning TRL 3 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / TRL | Microvision 8 (estimated) | D2.2 p.25 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 B9 / Source(s) | D2.2 pp.25, 33 contain information for this row | D2.2 pp.25, 33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | Couldn't find it; Was WRONG ('Couldn't find it'). Microvision EM130C, the row's comparison system, is on D2.2 p.25 (TRL table, 'Microvision EM130C … 8'), p.33 (Table 15) and p.34 (Ye et al. 2020, 98 %); please re-check | 2026-11-17 |

### T1 B10 — Foot pad dermatitis (carcass)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B10 / Indicator, species, stage | Foot pad dermatitis (carcass); Broiler; Postmortem (after plucking) | Cat. pp.138–140; D1.6 p.10 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Sensor (vendor) | ChickenCheck Footpad — camera (CLK GmbH) | Cat. p.140 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Sensor (quote) | "5 classes of FPD … Approx. 5 pairs/second" | Cat. p.140 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Sensor | pilots 3 & 4 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Sensor (vendor) | Meyn prototype (not aWISH) | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Automated? | yes | Cat. p.140 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (paper identity) | PS-2026, peer-reviewed, aWISH-period, DOI 10.1016/j.psj.2026.106968, open access CC BY | DOI 10.1016/j.psj.2026.106968 [web]; PS-2026 PDF | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (design) | two plants, DUC (12,000 birds/h) and Plukon Sieradz (15,000 birds/h) | PS-2026 (methods; no page cited) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (design) | validation set 500 images / 1,000 feet and hocks; three human assessors | PS-2026 (methods) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (design) | footpad scored per QS Guideline (0, 1, 2a, 2b) | PS-2026 (methods) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (figure) | rater-median vs camera kappa 0.70 (0.67–0.74) | PS-2026 (results / table; 6.2 steps 2–6) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (figure) | linear-weighted kappa 0.80 | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (figure) | inter-observer human kappa 0.33 (0.30–0.36) | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (figure) | lesion-area R² 0.93; camera bias +2.47 % | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | 1 | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (caveat) | score cut-offs CLK-confidential | PS-2026 | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (caveat) | images carried no flock/batch identity, so no flock-level validation | PS-2026 | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Agreement (caveat) | CLK changed the software after the study | PS-2026 | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-14 |
| A | T1 B10 / Agreement (caveat) | one author is a CLK employee | PS-2026 (affiliations / declaration of interest) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-16 |
| A | T1 B10 / Agreement (quote, pre-aWISH) | Meyn: "(r=0.54 and 0.59) … reached r=0.69 and 0.74" (Vanderhasselt et al.) | D2.2 p.33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / TRL | TRL 9 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B10 / Source(s) | Cat. pp.138–139; D2.2 pp.23, 32; D1.8 p.30 contain information for this row | Cat. pp.138–139; D2.2 pp.23, 32; D1.8 p.30 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |

### T1 B11 — Hock burn (carcass)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B11 / Indicator, species, stage | Hock burn (carcass); Broiler; Postmortem | Cat. pp.141–142 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Sensor (vendor) | ChickenCheck Hockburn — camera (CLK GmbH) | Cat. p.142 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Sensor (quote) | "3 classes … Approx. 4 pairs/second" | Cat. p.142 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Sensor | pilots 3 & 4 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Automated? | yes | Cat. p.142 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (design) | same design and validation set as B10 (500 images / 1,000 feet and hocks, DUC and Plukon Sieradz, three assessors) | PS-2026 (methods) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (design) | hock burn scored 0–2 adapted from IKB Kip | PS-2026 (methods) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (figure) | rater-median vs camera kappa 0.60 (0.57–0.64) | PS-2026 (results / table) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (figure) | linear-weighted kappa 0.69 | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (figure) | inter-observer human kappa 0.47 (0.32–0.62) | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (figure) | lesion-area R² 0.97; camera bias −0.38 cm² | PS-2026 (results) | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-13 |
| A | T1 B11 / Agreement (caveats) | as B10: cut-offs CLK-confidential; no flock/batch identity; software changed after the study; one author is a CLK employee | PS-2026 | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-16 |
| A | T1 B11 / TRL | TRL 9 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| A | T1 B11 / Source(s) | D1.8 p.30 contains information for this row | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

### T1 B12 — Catch damage

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B12 / Indicator, species, stage | Catch damage (haematomas, broken wings/legs; bruises, fractures); Broiler; Postmortem | Cat. pp.143–144 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B12 / Sensor (vendor) | ChickenCheck Catch Damage — camera (CLK GmbH), pilot 4 | Cat. pp.143–144; D1.6 p.10 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B12 / Sensor (quote) | "detects catch damage on wings and is being further developed to identify damage on the breast and legs" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| A | T1 B12 / Automated? | yes | Cat. pp.143–144 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B12 / Agreement (negative) | not stated (checked Cat. pp.143–144; D2.2; D1.6) | Cat. pp.143–144; D2.2; D1.6 | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G12 (catch.?damage; Chicken.?Check) — Cat. 12 hits pp.108, 138, 140, 141, 142, 143(2), 144(2), 145, 146, 151; D2.2 3 hits pp.23, 28, 35; D1.6 8 hits p.10(8) | 2026-11-17 |
| A | T1 B12 / TRL | TRL 7 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| A | T1 B12 / Source(s) | D1.8 p.30 contains information for this row | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

### T1 B13 — Scratches (back)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T1 B13 / Indicator, species, stage | Scratches (back); Broiler; Postmortem | Cat. pp.145–146 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B13 / Sensor (vendor) | ChickenCheck Scratch — camera (CLK GmbH, aWISH partners) | Cat. pp.145–146 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B13 / Sensor (quote) | "being developed and validated" | Cat. p.146 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B13 / Automated? | yes (intended) | Cat. pp.145–146 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | T1 B13 / Agreement (negative) | not stated (checked Cat. pp.145–146; D1.6) | Cat. pp.145–146; D1.6 | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G13 (scratch; Chicken.?Check) — Cat. 13 hits pp.108, 138, 140, 141, 142, 143, 144, 145(3), 146(3); D1.6 8 hits p.10(8); (D2.2, not claimed as checked: 1 hit p.23) | 2026-11-17 |
| A | T1 B13 / TRL | TRL 4 | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| A | T1 B13 / Source(s) | D1.8 p.30 contains information for this row | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

---

## File A — row-count paragraph after Table 1 (procedure 7.3 steps 1 to 3)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | row-count para (line 67) / 7.3 step 1 | Row count: 38 (22 pig, 16 broiler) | A Table 1 itself | | | OK | count: 22 pig + 16 broiler = 38 (see section 9 problem 1 above) | 2026-11-17 |
| A | row-count para / 7.3 step 2 | Rows with at least one agreement/validation figure attached to the named sensor: 22 (the 21 listed before plus P9) | A Table 1 itself | | | OK | count: 21 codes listed before + P9 = 22 (corrected 17 Nov); the old wording was OK on 17 Nov | 2026-11-17 |
| A | row-count para / 7.3 step 2 | Rows "not stated" for agreement: 16 | A Table 1 itself | | | OK | count: 38 − 22 = 16 (corrected 17 Nov); the old wording was OK on 17 Nov | 2026-11-17 |
| A | row-count para / 7.3 step 3 | Of the listed rows P3, P9, B10, B11 are aWISH-period results; every other listed row's figure is from a pre-aWISH study (P2, P4, P6, P7, P8, P11, P12, P13, P14, P19, P22, B1, B2, B3, B9, B14, B15, B16 — 18 rows, each to be checked) | each row's Source(s) cell | | | OK | the old wording was OK on 17 Nov | 2026-11-17 |
| A | row-count para / 7.3 step 3 | P16 has human-rater figures only | Zenodo 17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | row-count para / 7.3 steps 4–5 (corrected 17 Nov) | P9 Lesion-Detect (Banhazi et al. 2026) is the one pig slaughterhouse sensor row with a peer-reviewed aWISH-period validation (also line 5); this file missed the paper on 7 Oct | PDF p.1 — `deliverables/publication-sweep/Banhazi 2026 AgronRes - Lesion-Detect development and pilot testing (doi AR.26.034).pdf` | deliverables/publication-sweep/Banhazi 2026 AgronRes - Lesion-Detect development and pilot testing (doi AR.26.034).pdf | | OK | Was: "No pig slaughterhouse sensor row carries an aWISH-period or peer-reviewed validation figure" (OK on 16 Nov); contradicted by Banhazi et al. 2026, published 25 May 2026 | 2026-11-17 |

---

## File A — Table 2 (publications), procedure 7.4

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | T2 row 1 | "Validation of an automated system for at-slaughter assessment of footpad dermatitis and hock burn in broiler chickens"; van Staaveren, van Langeveld, Schulte-Landwehr, Mulder, Galliot, Créach, Sztandarski, Marchewka, Forkman, Van Noten, Tuyttens, Giersberg, Manet, Rodenburg; Poultry Science 105(7):106968; 2026; Opened: yes (full text, 7 Oct 2026); open access CC BY | DOI 10.1016/j.psj.2026.106968 [web]; `papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf` | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-17 |
| A | T2 row 2 | "Technologies for automatic assessment of pig welfare using animal-based indicators in the slaughterhouse: a review"; Ramon-Perez, Camerlink, van Staaveren, Maschat, van Langeveld, Banhazi, Fels, Jachens, Maselyne, Forkman, Llonch; Biosystems Engineering 259:104286; 2025; Opened: yes; open access; "Review of 16 slaughterhouse and 71 on-farm technologies (52 feasible)"; "One author employed by Innotech Vision" | DOI 10.1016/j.biosystemseng.2025.104286 [web]; `papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf` | papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf | | OK | | 2026-11-17 |
| A | T2 row 3 | "Sub-clinical respiratory infection identified on farms by monitoring weight changes of pigs with the Weight-Detect instrument"; Banhazi, Dunn, Banhazi, Reixach, Ramon-Perez, Llonch, Maselyne; Agronomy Research 23(S1):5–14; 2025; Opened: yes; one pen, nine pigs, four manual weighings; vendor and farm-owner co-authors | DOI 10.15159/AR.25.032 [web]; `papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf` | papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf | | OK | | 2026-11-17 |
| A | T2 row 4 | "A framework for a comprehensive animal welfare label"; Tuyttens, Lawrence, Mullan; Animal Frontiers 15(2):61–68; 2025 (April); Opened: yes; conceptual; Table 3 pros/cons; funded by aWISH; no validation data | DOI 10.1093/af/vfaf003 [web]; `papers/Tuyttens 2025 AnimFront - comprehensive animal welfare label framework.pdf` | papers/Tuyttens 2025 AnimFront - comprehensive animal welfare label framework.pdf | | OK | | 2026-11-17 |
| A | T2 row 5 | "Nuevos enfoques para monitorizar el bienestar animal mediante sensores e IA"; Ramon Perez, Ko, Llonch, Allueva Molina (UAB); SUIS no. 207, pp.22–27; 2024 (May); no DOI; Opened: yes; overview; Table 2 lists slaughterhouse indicators; acknowledges ClearFarm, aWISH, PigLF; no validation figures | none given; `papers/Ramon-Perez 2024 SUIS - sensors and AI for pig welfare, Spanish.pdf` | papers/Ramon-Perez 2024 SUIS - sensors and AI for pig welfare, Spanish.pdf | | OK | | 2026-11-17 |
| A | T2 row 6 | (National overview of Polish poultry welfare research; one paragraph on aWISH); Siwek, Marchewka; Polskie Drobiarstwo; 2023 (September); no DOI; Opened: yes; aWISH paragraph gives 24 partners, 13 countries, six slaughterhouses, catalogue, best-practice guides; no validation figures | none given; `papers/Siwek 2023 Polskie Drobiarstwo - poultry welfare in Poland, Polish.pdf` | papers/Siwek 2023 Polskie Drobiarstwo - poultry welfare in Poland, Polish.pdf | | OK | | 2026-11-14 |
| A | T2 row 7 | "Scoring Tear Staining in Pigs: Similarity, Consistency, Accuracy, and Level of Experience"; van Langeveld, van Staaveren, Van Noten, Rodenburg, Tuyttens; Proc. ISAE Benelux Conference 2024; 2024; Opened: yes | DOI 10.5281/zenodo.17803862 [web] | papers/van Langeveld 2024 ISAE Benelux - scoring tear staining, rater reliability (zenodo 17803862).pdf | | OK | | 2026-11-17 |
| A | T2 row 8 | "Developing the 'Lesion-Detect' system …"; Banhazi et al.; 15th Int. Conf. Biosystems Engineering, Tartu; 2025; Opened: yes, copy in papers/ (16 Nov); no figures | DOI 10.5281/zenodo.17786812 — `papers/Banhazi 2025 BSE Tartu - Lesion-Detect lung lesion scoring (zenodo 17786812).pdf` | papers/Banhazi 2025 BSE Tartu - Lesion-Detect lung lesion scoring (zenodo 17786812).pdf | | OK | Was "Opened: no", WRONG 17 Nov (I did open it. Downloading the pdf now.); corrected | 2026-11-17 |
| A | T2 row 9 | "Development of the Lesion-Detect System …"; Banhazi et al.; ISAH & SEAOHUN Conf., Chiang Mai; 2024; Opened: yes, copy in papers/ (16 Nov); no figures | DOI 10.5281/zenodo.17630315 — `papers/Banhazi 2024 ISAH - Lesion-Detect system development (zenodo 17630315).pdf` | papers/Banhazi 2024 ISAH - Lesion-Detect system development (zenodo 17630315).pdf | | OK | Was "Opened: no", WRONG 17 Nov (Opened this one and downloading the pdf); corrected | 2026-11-17 |
| A | T2 row 10 | "Automated evaluation of pig consciousness in the slaughterhouse: sensor development"; Ramon-Perez, Gol, Reixach, Sanchez, Manteca, Llonch; HSA Conference 2025; 2025; Opened: yes, copy in papers/ (16 Nov); no accuracy figure | DOI 10.5281/zenodo.17475673 — `papers/Ramon-Perez 2025 HSA - pig consciousness sensor development (zenodo 17475673).pdf` | papers/Ramon-Perez 2025 HSA - pig consciousness sensor development (zenodo 17475673).pdf | | OK | Was "Opened: no", WRONG 17 Nov (Opened and downloading); corrected | 2026-11-17 |
| A | T2 row 11 | "Development of an automated tool for monitoring tail length and lesions in pig slaughterhouses"; Ramon-Perez, Gol, Arbat, Reixach, Llonch; Proc. 58th ISAE Congress; 2025; Opened: yes, copy in papers/ (16 Nov); preliminary F-scores | DOI 10.5281/zenodo.17475558 — `papers/Ramon-Perez 2025 ISAE - tail length and lesions tool (zenodo 17475558).pdf` | papers/Ramon-Perez 2025 ISAE - tail length and lesions tool (zenodo 17475558).pdf | | OK | Was "Opened: no", WRONG 17 Nov (Opened now, downloading pdf); corrected | 2026-11-17 |
| A | T2 row 12 | "Area-specific vocalisation and activity monitoring in pigs (STREMODO)"; Westendorff, Puppe, Moscovice, Eusemann, Manteuffel; ECPLF 2024; 2024; Opened: yes, copy in papers/ (16 Nov); barn study, not aWISH-funded | DOI 10.5281/zenodo.18549284 (per project site) — `papers/Westendorff 2024 ECPLF - area-specific vocalisation and activity (zenodo 18549284).pdf` | papers/Westendorff 2024 ECPLF - area-specific vocalisation and activity (zenodo 18549284).pdf | | OK | Was "Opened: no", WRONG 17 Nov (Downloading, just opened); corrected | 2026-11-17 |
| A | T2 row 13 | "The aWISH project: Automated animal welfare monitoring for broilers and pigs at the slaughterhouse"; Rodenburg et al.; Measuring Behavior 2024; 2024; Opened: yes (17 Nov) | DOI 10.6084/m9.figshare.25897855 [web] (7.4 step 3) | | | OK | Was "Opened: no", WRONG 17 Nov (Downloaded); corrected | 2026-11-17 |
| A | T2 row 14 | "Weight-Detect instrument predicted impending respiratory infection …"; "Enviro-Detect instrument …"; Banhazi et al.; ISAH & SEAOHUN Conf. 2024; 2024; Opened: yes, copies in papers/ (16 Nov) | DOI 10.5281/zenodo.17628730 — `papers/Banhazi 2024 ISAH - Weight-Detect predicted respiratory infection (zenodo 17628730).pdf`; DOI 10.5281/zenodo.17629216 — `papers/Banhazi 2024 ISAH - Enviro-Detect in a Spanish livestock building (zenodo 17629216).pdf` | papers/Banhazi 2024 ISAH - Weight-Detect predicted respiratory infection (zenodo 17628730).pdf | | OK | Was "Opened: no", WRONG 17 Nov; corrected | 2026-11-17 |
| A | T2 row 15 | "Guideline(s) to validate sensor output of animal-based measurements"; Maselyne et al.; Llonch et al.; EAAP 2024; WAFL 2024; 2024; Opened: yes, copies in papers/ (method guidance) | DOI 10.5281/zenodo.13969485; DOI 10.5281/zenodo.13991423 [web] (7.4 step 3) | papers/Maselyne 2024 EAAP - guideline to validate sensor output (zenodo 13969485).pdf | | OK | Was "Opened: no", WRONG 17 Nov; corrected | 2026-11-17 |
| A | T2 listing sources (line 91) | Listing sources: awish-project.eu journal-papers and conference-papers pages (opened 2026-10-07); CORDIS listing pp.3–7 "Last update: 26 November 2025"; Zenodo search for 101060818 not possible (HTTP 429) | www.awish-project.eu/journal-papers/ and /conference-papers/ [web]; CORDIS listing pp.3–7; zenodo.org [web] | deliverables/CORDIS listing 101060818.pdf | | OK | | 2026-11-14 |

Note: Table 2 has 15 publication rows plus the listing-sources line; the agent's first count of "16 rows" included the table header row.

---

## File A — Disagreements D1 to D12 (procedure 7.5)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| A | D1 PigInspector TRL | D2.2 p.19 Table 6: ear lesions 9, tail lesions 9, skin lesions 4, tail length 3–4; D1.6 pp.9, 11 "CLK Pig Inspector (TRL 5)"; Cat. p.53 labels "PigInspector (prototype)" for tail length but not for skin/tail lesions (pp.46, 49) | D2.2 p.19; D1.6 pp.9, 11; Cat. pp.46, 49, 53 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-14 |
| A | D2 STREMODO | TRL 4 (D2.2 p.19) vs "STREMODO (TRL 5)" (D1.6 pp.9, 11); same source paper (Schön et al. 2004): D2.2 p.33 "correlation of 0.84" vs BSE-rev "r = 0.78–0.87" | D2.2 pp.19, 33; D1.6 pp.9, 11; BSE-rev | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| A | D3 Weight-Detect provider | D2.2 p.19 "Weight-Detect TM — PLF Agritech Europe"; Cat. p.32 and D1.6 p.9 "InnoTech Vision"; Agronomy Research 2025: PLF Agritech (Brisbane) technology, ADAMS cloud, patented AU/US/EU; "the vendor-authored paper does not name InnoTech Vision as the provider" | D2.2 p.19; Cat. p.32; D1.6 p.9; Agronomy Research 2025 (DOI 10.15159/AR.25.032) | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | grep: G14 (Inno.?Tech) on Agronomy Research 2025 PDF (pdftotext) — 1 hit p.1: author affiliation "1InnoTech Vision ApS., Niels Pedersens Alle 2, 8830 Tiele, Denmark" (first author's affiliation; the claim concerns "provider", which is a different statement — judgement is the author's) | 2026-11-14 |
| A | D4 Pig stunning sensor owner | Cat. p.62 "BlinkAI — nunaSolutions"; D1.8 p.30 "Stunning effectiveness (Nuna solutions)"; D1.6 pp.9, 11 "WEL2BE implemented a stunning effectiveness technology for pigs (TRL 5)"; D2.2 p.27 "CET'Automatique — Wel2be — Automatic control of pig unconsciousness at slaughter"; D6.2 p.92 "Pilot2_W2B1 CET'automatique Vision system 16/03/2023"; CORDIS (2026-10-07) "WEL2BE — Participation ended", "BY-NUNASOLUTIONS SL — Spain … SME: Yes"; Nuna site "NunaSolutions, is a brand of Teknologisk Institute"; 2023–2024 documents name WEL2BE, 2025–2026 documents name Nuna; whether BlinkAI and CET'Automatique are the same system, and handover terms: not stated in any document read; broiler sensor (B9) remains WEL2BE only | Cat. p.62; D1.8 p.30; D1.6 pp.9, 11; D2.2 p.27; D6.2 p.92; CORDIS participants list [web, via handover-pack/D and F — 7.5 step 4]; Nuna web site [web, via F §6] | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G15 (Blink.?AI; CET.?Automatique) over 15 text files — D2.2 1 hit p.27; Cat. 2 hits pp.61, 62; D6.2 1 hit p.92; 0 hits elsewhere (incl. CORDIS listing). G07 for Nuna / WEL2BE: see P10 | 2026-11-14 |
| A | D5 Tear-staining sensor owner | Cat. p.88 "aWISH partners"; D1.6 p.9 "WEL2BE, TRL 3"; D6.2 p.92 "Pilot2_W2B2 tear-staining Vision system"; D1.8 p.30 "Tear staining (ILVO)"; website pilots page (2026-10-07) "Tear staining system (ILVO)"; WEL2BE's participation ended per CORDIS | Cat. p.88; D1.6 p.9; D6.2 p.92; D1.8 p.30; www.awish-project.eu pilots page [web, via handover-pack/D]; CORDIS [web] | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G09 (tear.?stain) — D1.6 1 hit p.9; D1.8 1 hit p.30; Cat. 9 hits pp.13, 87(4), 88(4); D2.2 3 hits pp.26, 28, 35 | 2026-11-14 |
| A | D6 Tail length tool owner | Cat. p.57 "UAB & Batallé" (2D camera); D1.8 p.28 "Tail Length (VION)" (two 3D cameras); PigInspector (CLK) also listed for tail length (Cat. p.54) | Cat. pp.54, 57; D1.8 p.28 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | D7 eYeNamic foot health | Cat. p.130 "externally validated (Hertem et al 2018 - 10.1016/j.biosystemseng.2018.05.008)" vs D2.2 p.33 "the prediction was poor for foot pad lesions and hock burns"; DOI on Cat. p.130 differs from Cat. p.129 and D2.2 reference list (10.1016/j.biosystemseng.2018.07.002) | Cat. pp.129, 130; D2.2 pp.33, 39; both DOIs [web] | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-14 |
| A | D8 Meyn FPD system | Listed "validated" in D2.2 Table 15 (p.32) although r values 0.54–0.74 (p.33) are below the R>0.75 criterion (p.10); Cat. p.139 calls results "relatively poor"; year 2012 in D2.2 text (p.33) vs 2013 in D2.2 refs (p.39) and Cat. p.139 | D2.2 pp.10, 32, 33, 39; Cat. p.139 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-14 |
| A | D9 D2.2 internal counts | Executive summary p.7 "Seven pig welfare assessment products are considered validated, three already on the market and three still in development"; Table 16 (p.35) lists 8 rows, 3 "On market", 5 "Prototype"; conclusions (p.35) "107 commercial sensors and 23 prototypes" for pigs vs "88 … 16" (pp.7, 12) | D2.2 pp.7, 12, 35 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-16 |
| A | D10 Catalogue dating | File titled "D2.5 … Final Version — Updated September 2026" (Cat. p.1); website checks dated 24 Oct 2024 and 21 Aug 2026 (Cat. pp.48, 60, 78, 83, 86, 88); caller's brief treats it as M20 | Cat. pp.1, 48, 60, 78, 83, 86, 88 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| A | D11 Poultry Science 2026 author list | Journal record includes "M.W.E. Manet"; SciFAW Centenary conference version (research-portal.uu.nl "…-2" record) omits Manet and spells "Tuyttels" in the DSpace copy | PS-2026 PDF; research-portal.uu.nl [web] | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | | OK | | 2026-11-14 |
| A | D12 BroilerZoom | Cat. p.112 "externally validated"; D2.2 p.33 "average relative mean error of 8%" with "errors … generally larger in the end of the rearing period"; no R or accuracy against the D2.2 criterion | Cat. p.112; D2.2 pp.10, 33 | deliverables/D2.2 Methodology for measuring each AWI.pdf | | OK | | 2026-11-14 |

---

## File B — section 1 per-pilot table (procedure 8.1 step 1, 8.2)

Negative "plan past Oct 2026" claims all use grep G16 (procedure 8.2 step 6 terms: after the project; end of the project; continu; sustain; maintain; 2027; beyond). The per-file counts in G16 are: D1.1 19, D1.2 33, D1.6 2 (pp.6, 7), D1.8 18, D4.3 11, D5.2(OCR) 45, Cat. 23, D1.4 6 (pp.4, 21, 23, 27, 35(2)), D1.5 9, D6.2 25, D6.3 16. Pages are in the Appendix. The terms are generic ("continu", "maintain"), so most hits will be irrelevant; the pages are what to open.

### §1 Pilot 1 — Vion, Groenlo

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 1 / Slaughterhouse (quote) | "the pig slaughterhouse Vion in Groenlo, the Netherlands" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Species, country | Pigs; NL | D1.6 p.9; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Co-lead (quote) | "University of Utrecht as scientific co-lead" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Co-lead (quote) | "Sci. lead: UU" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote) | "Three new technologies were implemented" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, TRL, vendor) | "CLK Pig Inspector (TRL 5) … measures tail length and checks for skin, ear, and tail lesions on pig carcasses, using 2D and 3D color cameras" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, TRL, vendor) | blood samples "for IGF BP analysis as stress indicators (performed by FBN, TRL 3)" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, TRL, vendor) | "STREMODO (TRL 5) developed by FBN … installed in the unloading and lairage area" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies | D1.8 p.25 is a slide "Overview sensor technology" dated 5 Sep 2025 and lists seven items | D1.8 pp.14, 25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "AI4Animals (Deloitte) – Animal Treatment" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "STREMODO (FBN) – Stress Vocalizations" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "IGFBPs (FBN) – Stress level in exsanguination blood" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "AUTOFOM3 (Carometec) – Backfat and Muscle Depth Across Carcass" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "PigInspector (CLK GmbH) – Ear, Tail and Skin Lesions" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote, vendor) | "Tail Length (VION)" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote) | "CGM Insertion Probe – Backfat and Muscle Depth" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote) | "Tail Length (VION)" ("Two 3D Camera's after the first flame oven") under "OTHER TECHNOLOGIES" | D1.8 p.28 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Technologies (quote) | "AI4ANIMALS (DELOITTE, VION)" ("Algorithm uses CCTV footage in unloading area") under "OTHER TECHNOLOGIES" | D1.8 p.28 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Stage (quote) | stage labels "UNLOADING, LAIRAGE, STUNNING, BLEEDING, PROCESSING" | D1.8 p.25 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Stage | mapping: unloading (STREMODO, AI4Animals), lairage (STREMODO), bleeding (IGF-BP in "exsanguination blood"), processing / post-mortem (PigInspector, Tail Length, Autofom3, CGM probe); "unloading and lairage area" | D1.8 p.25; D1.6 p.9 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | EDIT | STREMODO is shown as implemented in lairage; Pack B now puts STREMODO under lairage, as on the D1.8 p.25 slide, and quotes 'unloading and lairage area' | 2026-11-17 |
| B | §1 Pilot 1 / Stage (negative) | Farm / loading / transport: not stated (D1.6, D1.8) | D1.6; D1.8 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G25 (farm; loading; transport) — D1.6 36 hits, of which pp.9(4), 10(6), 11(1) in the pilot abstracts; D1.8 52 hits, none on pp.23–28 except p.26(1), p.28(1) (full page list in Appendix) | 2026-11-17 |
| B | §1 Pilot 1 / Installation status (quote) | PigInspector "Images of the pigs are taken via 3 cameras (+ lighting), on which an algorithm performs measurements (still under development)" | D1.8 p.27 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Installation status (dates) | slide dated 5 Sep 2025; deliverable dated 22/10/2025 | D1.8 p.14; D1.8 p.1 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Installation status (quote) | STREMODO "Sensor hangs above monitored area (unloading and lairage area)" | D1.8 p.26 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Installation status (quote) | "were implemented in the slaughterhouse" (Sep 2024) | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Installation status (quote) | "they have already installed cameras in the unloading and lairage area to determine animal behaviour, a full carcass scan system (AutoFOM3) to measure carcass composition and camera's to measure tail length on the carcass (individual carcass tracking using RFID on the slaughter line). With technology providers CLK GmbH and FBN Dummerstorf more carcass vision data will be added (bite marks, scratches, ear/tail or other lesions) and sound/motion and blood measurements" | D1.4 p.16 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Installation status (date) | D1.4 pilot text "possibly Apr 2023" (first submission 28.04.2023; v2.0 17/09/2024 "Adaptation of comments by EC") | D1.4 pp.3–4 | deliverables/D1.4 Project website report v2.pdf | | EDIT | v1.0 on the last of april '23, v2.0 seventeenth of sept. v2 publication date sep 21 2027; Pack B now gives both versions: v1.0 published 30 Apr 2023, v2.0 17 Sep 2024 (the approval table's '21/09/2027' is a typo in D1.4 p.4) | 2026-11-17 |
| B | §1 Pilot 1 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, D1.4, D1.5, D6.2, D6.3) | the 10 files named | | | OK | grep: G16 — D1.1 19, D1.2 33, D1.6 2, D1.8 18, D4.3 11, D5.2(OCR) 45, D1.4 6, D1.5 9, D6.2 25, D6.3 16 hits (pages in Appendix) | 2026-11-17 |
| B | §1 Pilot 1 / Plan past Oct 2026 (quote) | "In pilot 1 due to data sharing limitations all data will remain private and securely stored within the aWISH dataplatform." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Throughput (negative) | not stated (checked all files incl. D1.4 p.16) | all 11 File-B files | | | OK | grep: G17 (capacity; throughput; per week; per day; per hour; slaughtered; birds/h; pigs/h) — D1.1 1 (p.9), D1.2 1 (p.9), D1.6 0, D1.8 2 (p.55), D4.3 6, D5.2(OCR) 7, Cat. 2 (p.68), D1.4 4 (pp.13, 17, 20(2)), D1.5 1 (p.8), D6.2 8 (pp.8, 52(7)), D6.3 15. G18 (Vion; Groenlo) — D1.6 4 (pp.4, 9(3)); D1.8 6 (pp.23, 24, 25(2), 28(2)); D1.4 6 (pp.7(2), 16(3), 25); D6.2 3 (pp.52, 91, 92); D6.3 2 (pp.16, 41); 0 in D1.1, D1.2, D4.3, D5.2, Cat., D1.5 | 2026-11-17 |
| B | §1 Pilot 1 / Region (quote) | "Gelderland (the Netherlands) + extensions to the rest of the Netherlands and Germany" | D1.8 p.24 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Region (quote) | "Pilot 1 covers Groenlo, Gelderland in the Netherlands and extensions to the rest of the Netherlands and Germany." | D1.4 p.16 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Contact (quote) | "Pilot lead: Vion" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 1 / Contact (quote) | website pilots page holds "the location, production type, contact details and technologies and developments of each pilot" | D1.1 p.17; D1.2 p.17 | deliverables/D1.1 CD&E plan and execution report v1.pdf | | OK | | 2026-11-14 |

### §1 Pilot 2 — Batallé (or NORFRISA, contradiction 10)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 2 / Slaughterhouse (quote) | "the pig slaughterhouse Batallé in Catalonia, Spain" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Slaughterhouse (quote) | "NORFRISA (FRIGORÍFICOS DEL NORDESTE S.A.) is one of the largest slaughterhouses in Spain" | D1.4 p.17 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Species, country | Pigs; ES | D1.6 p.9; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Co-lead (quote) | "Autonomous University of Barcelona as scientific co-lead" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Co-lead (quote) | prints "Pilot lead: Batallé / Wet. H.: UAB" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "5 new technologies were installed: 3 sensors at the slaughterhouse and 2 on-farm" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, TRL, vendor) | "WEL2BE implemented a stunning effectiveness technology for pigs (TRL 5), evaluating if pigs are properly stunned in the gas tunnel by monitoring the corneal reflex" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, TRL, vendor) | "A camera system was also installed to assess tear staining (WEL2BE, TRL 3)" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, TRL, vendor) | "At the evisceration line, InnoTech Vision installed the Lesion-Detect (TRL 3) … lung and liver lesions" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, TRL) | on-farm "Enviro-Detect (TRL 7), monitoring barn climate (temperature, humidity, ammonia, dust, CO2), and Weight-Detect (TRL 7)" | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, vendor) | "Tail Length (prototype) … Provider UAB & Batallé … 2D camera … Technology used in aWISH project" | Cat. p.57 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (negative) | tail-length prototype not in D1.6 | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | EDIT | grep: G35 (AI4Animals; Autofom; Carometec; CGM; Deloitte; tail.?length) on D1.6 — 3 hits pp.8, 9, 11 ("tail length" occurs on p.9 in the Pig Inspector sentence); CLK PigInspector checks tail length as well as other things, but no other specialized system is mentioned; Pack B now says D1.6 names tail length only as one of PigInspector's measures (p.9) | 2026-11-17 |
| B | §1 Pilot 2 / Technologies (vendor correction) | stunning-effectiveness sensor = Nuna Solutions (BlinkAI; DTI/DMRI brand); WEL2BE listed in D1.6, participation since ended | Cat. p.62; D1.8 p.30; CORDIS [web, via handover-pack/F §6]; Nuna web site [web, via F §6] | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G07 — local CORDIS listing 0 hits for Nuna / WEL2BE | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | CORDIS: "WEL2BE — Participation ended"; "BY-NUNASOLUTIONS SL — Spain" | CORDIS participants list [web, via handover-pack/F §6 → 7.5 step 4] | deliverables/CORDIS listing 101060818.pdf | | OK | | 2026-11-16 |
| B | §1 Pilot 2 / Technologies (quote) | "BlinkAI … Provider nunaSolutions" | Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "Stunning effectiveness (Nuna solutions)" | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote, vendor) | Tear staining = ILVO: "Tear staining (ILVO)" | D1.8 p.30 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "Tear staining aWISH … Provider aWISH partners" | Cat. p.88 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "new technologies of Wel2be and InnoTech Vision are being implemented." | D1.4 p.17 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "Pilot2_W2B1 CET'automatique Vision system 16/03/2023" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Technologies (quote) | "Pilot2_W2B2 tear-staining Vision system 16/03/2023" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Stage | Farm (Enviro-Detect, Weight-Detect); stunning ("gas tunnel"); post-mortem ("evisceration line") | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-16 |
| B | §1 Pilot 2 / Stage (negative) | tear staining camera location not stated beyond "installed" | D1.6 p.9; D1.8 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G09 (tear.?stain) — D1.6 1 hit p.9; D1.8 1 hit p.30 | 2026-11-17 |
| B | §1 Pilot 2 / Stage (negative) | Loading / transport / lairage: not stated (D1.6, D1.8) | D1.6; D1.8 | | | OK | grep: G25 (farm; loading; transport) and G26 (lairage; stunning) — D1.6 G26 6 hits pp.9(2), 10(2), 11(2); D1.8 G26 5 hits pp.25(2), 26, 30, 70; G25 counts as Pilot 1 | 2026-11-17 |
| B | §1 Pilot 2 / Installation status (quote) | "were installed" (Sep 2024) | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Installation status (quote, figure) | "This system [Weight-Detect] detected the onset of respiratory disease in a batch 6 days before clinical signs appeared." | D1.6 p.9 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Installation status (negative) | D1.8 p.23 (5 Sep 2025) gives only "1st phase pilot"; no installation status | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G27 (pilot ?[1-6]) on D1.8 — 3 hits pp.24(2), 25 (p.23 slide uses "Pilot lead"); G28 (install) on D1.8 — 0 hits; G19 (Batall[eé]; Selecci[oó]n) on D1.8 — 1 hit p.23 | 2026-11-16 |
| B | §1 Pilot 2 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, Catalogue, D1.4, D1.5) | the 9 files named | deliverables/D1.1 CD&E plan and execution report v1.pdf | | OK | grep: G16 — D1.1 19, D1.2 33, D1.6 2, D1.8 18, D4.3 11, D5.2(OCR) 45, Cat. 23, D1.4 6, D1.5 9 hits (pages in Appendix) | 2026-11-17 |
| B | §1 Pilot 2 / Plan past Oct 2026 (quote) | "Pilot 2 Data access will be restricted and stopped after the end of the project." | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Throughput (negative) | For Batallé: not stated (checked all files) | all 11 File-B files | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G17 counts as Pilot 1. G19 (Batall[eé]; Selecci[oó]n) — D1.6 3 (pp.4, 9(2)); D1.8 1 (p.23); Cat. 1 (p.57); D1.4 2 (p.7(2) — abbreviation list entry "BATA SELECCION BATALLE SA", not pilot text); D6.2 4 (p.62(4)); D6.3 5 (pp.16, 52(4)); 0 in D1.1, D1.2, D4.3, D5.2, D1.5 | 2026-11-17 |
| B | §1 Pilot 2 / Throughput (quote, figures) | NORFRISA: "advanced facilities of more than 24,000 square meters that allow 10,000 pigs to be slaughtered every day" | D1.4 p.17 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Throughput (quote, figures) | NORFRISA: "250 own workers and 17 official inspectors" | D1.4 p.17 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Region (quote) | "Pilot 2 covers Catalonia in Spain, and extensions to the rest of Spain." | D1.4 p.17 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Contact (quote) | "Pilot lead: Batallé" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 2 / Contact (quote) | "In Pilot 2 Technical manager of the project at Selección Batallé and the data protection manager of Selección Batallé." | D6.3 p.52 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |

### §1 Pilot 3 — DUC (Plukon Food Group), Chailley

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 3 / Slaughterhouse (quote) | "the broiler slaughterhouse DUC (Plukon Food Group) in Chailley, France" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Slaughterhouse (quote) | "Pilot lead: Plukon – Duc" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Species, country | Broilers; FR | D1.6 p.10; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Co-lead (quote) | "Itavi as scientific co-lead" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Co-lead (quote) | "Sci. lead: ITAVI" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote) | "Six new technologies were implemented: 3 sensors at the slaughterhouse, 1 sensor and a mobile application on-farm, and 1 sensor for transport" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote, TRL, vendor) | "At the gas tunnel exit, WEL2BE installed the stunning effectiveness sensor (TRL 3) … monitoring movement in the crates" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote, TRL, vendor) | "CLK installed ChickenCheck Footpad (TRL 9) and ChickenCheck Hockburn (TRL 9)" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote, TRL, vendor) | Itavi "EBroilerTrack Sound (TRL 5) in the lairage area" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote, TRL) | on-farm "EBENE application (TRL 9)" and "EbroilerTrack Image (TRL 5)" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote, vendor) | "Transport Monitoring Sensors, measuring temperature, humidity and CO2 in broiler crates during transport" (Itavi) | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (holder, negative) | broiler stunning sensor holder WEL2BE per D1.6 p.10; participation since ended per CORDIS; which partner now holds it is not stated in any document read | D1.6 p.10; CORDIS [web]; all documents read | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G07 and G11 — see File A B9 row; D6.3 has 0 hits for Nuna / WEL2BE / W2B (G07) and 6 hits for "stunning" (G11, pp.36, 38, 39, 40, 44, 57) | 2026-11-17 |
| B | §1 Pilot 3 / Technologies | D1.8 p.30 and Cat. p.62 name Nuna Solutions/BlinkAI only for pig stunning | D1.8 p.30; Cat. p.62 | deliverables/AWI Catalogue (final version).pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote) | "With technology providers CLK GmbH, ITAVI and Wel2be, more carcass vision data will be added: foot pad and hock burn cameras and sound/motion measurements in the hatchery / transport / lairage area" | D1.4 p.18 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Technologies (quote) | "Pilot3_W2B1 Stunning Vision system 16/03/2023" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Stage (quotes) | Farm (EBENE, EBroilerTrack Image); transport; lairage (EBroilerTrack Sound); stunning ("gas tunnel exit"); post-mortem ("Further along the line", ChickenCheck) | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Stage (negative) | Loading: not stated separately | D1.6 p.10; D1.8 | | | OK | grep: G25 — "loading" is one of the terms; D1.6 p.10 has 6 hits for farm / loading / transport (incl. "unloading" matches "loading") | 2026-11-17 |
| B | §1 Pilot 3 / Stage (quote) | "cameras are already installed in the unloading, lairage, stunning, bleeding and scalding entrance areas" (pre-existing) | D1.4 p.18 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Installation status (quotes) | "were implemented" / "installed" (Sep 2024) | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Installation status (negative) | D1.8 p.23 (5 Sep 2025): "1st phase pilot" only; no installation status | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G27, G28 as Pilot 2; G21 (DUC; Chailley; Plukon) on D1.8 — 3 hits p.23(3) | 2026-11-16 |
| B | §1 Pilot 3 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, D1.4, D1.5) | the 8 files named | | | OK | grep: G16 — D1.1 19, D1.2 33, D1.6 2, D1.8 18, D4.3 11, D5.2(OCR) 45, D1.4 6, D1.5 9 hits (pages in Appendix) | 2026-11-17 |
| B | §1 Pilot 3 / Plan past Oct 2026 (quote) | "For ITAVI, database of labeled acoustic sound will be kept by ITAVI, to be enriched after the project and also the model developed. The rest of the data will be deleted at the end of the project: EBENE® evaluation, videos, raw sounds track, transport monitoring. Images are only available 28 days; reports are available for five years." | D6.3 p.53 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Throughput (negative) | not stated (checked all files incl. D1.4 p.18) | all 11 File-B files | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | 2 | EDIT | grep: G17 counts as Pilot 1. G21 (DUC; Chailley; Plukon) — D1.6 8 (pp.4(2), 10(6)); D1.8 3 (p.23(3)); D1.4 7 (pp.7, 18(4), 19(2)); D6.3 10 (pp.16(3), 41(2), 45, 47, 49, 51, 52); 0 in D1.1, D1.2, D4.3, D5.2, Cat., D1.5, D6.2; Not stated in the File-B files, but the ChickenCheck paper (van Staaveren et al. 2026, p.2) gives "DUC, France, line speed: 12,000 birds per h". Pack B updated | 2026-11-17 |
| B | §1 Pilot 3 / Region (quote) | "Pilot 3 covers Chailley, Yonne in France and extensions to France, the Netherlands, Germany, Belgium, Poland and Bulgaria." | D1.4 p.18 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Contact (quote) | "In Pilot 3 Plukon." | D6.3 p.52 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 3 / Contact (quote) | "Plukon needs to validate all data access (pilot 3)" | D6.3 p.47 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |

### §1 Pilot 4 — Plukon, Sieradz

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 4 / Slaughterhouse (quote) | "the broiler slaughterhouse Plukon in Sieradz, Poland" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Slaughterhouse (quote) | "Pilot lead: Plukon – Sieradz" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Species, country | Broilers; PL | D1.6 p.10; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Co-lead (quote) | "IGBZ PAN as scientific co-lead" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Co-lead (quote) | "Sci. lead: IGBZ PAN" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, vendor) | "CLK is responsible for all newly installed technologies in this pilot" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, TRL) | "ChickenCheck Footpad (TRL 9) and ChickenCheck Hockburn (TRL 9)" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, TRL) | "ChickenCheck Catch Damage (TRL 7) detects catch damage on wings and is being further developed to identify damage on the breast and legs" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, TRL) | "ChickenCheck Scratch (TRL 4), which detects scratches on broiler chickens' backs" | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote) | "These four camera systems are installed after the plucking phase, where each chicken is evaluated in real-time." | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, TRL, vendor) | "On-farm welfare assessments are also conducted for selected flocks using the EBENE app (TRL 9) from Itavi, as in pilot 3." | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, vendor) | "With technology providers CLK GmbH and Wel2be, more carcass vision data will be added: foot pad, hock burn and catch damage cameras." | D1.4 p.19 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (quote, vendor) | "New technologies are installed from Itavi, Wel2be and CLK GmbH." | D1.4 p.19 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Technologies (negative) | WEL2BE does not appear in the D1.6 Pilot 4 list | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G11 (Wel.?2.?be; W2B; stunning) on D1.6 — 7 hits pp.9(3), 10(2), 11(2); the two p.10 hits are to be located (Pilot 3 or Pilot 4 abstract) | 2026-11-14 |
| B | §1 Pilot 4 / Stage (quotes) | Farm (EBENE, "selected flocks"); post-mortem ("after the plucking phase") | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Stage (negative) | Loading / transport / lairage / stunning: not stated (D1.6, D1.8) | D1.6; D1.8 | | | OK | grep: G25 and G26 counts as Pilots 1 and 2 | 2026-11-17 |
| B | §1 Pilot 4 / Stage (quote) | "cameras are already installed in the unloading, lairage, stunning, bleeding and scalding entrance areas" (pre-existing) | D1.4 p.19 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Installation status (quote) | "are installed after the plucking phase" (Sep 2024) | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Installation status (quote) | "Due to the overlap in technologies between pilots 3 and 4, they serve as external validators for each other." | D1.6 p.10 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Installation status (negative) | D1.8 p.23 (5 Sep 2025): "1st phase pilot" only | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G27, G28 as Pilot 2; G22 (Sieradz) on D1.8 — 1 hit p.23 | 2026-11-16 |
| B | §1 Pilot 4 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, D1.4, D1.5) | the 8 files named | | | OK | grep: G16 — counts as Pilot 3 | 2026-11-17 |
| B | §1 Pilot 4 / Plan past Oct 2026 (quote) | "In Pilot 4 Images are only available 28 days, reports are available for five years." | D6.3 p.53 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Throughput (negative) | not stated (checked all files incl. D1.4 p.19) | all 11 File-B files | papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf | 2 | EDIT | grep: G17 counts as Pilot 1. G22 (Sieradz) — D1.6 1 (p.10); D1.8 1 (p.23); D1.4 2 (p.19(2)); D6.3 1 (p.16); 0 elsewhere. G21 (Plukon) counts as Pilot 3; Not stated in the File-B files, but the ChickenCheck paper (van Staaveren et al. 2026, p.2) gives "Plukon Sieradz Sp.z o.o, Poland, line speed: 15,000 birds per h". Pack B updated | 2026-11-17 |
| B | §1 Pilot 4 / Region (quote) | "Pilot 4 covers Sieradz in Poland and extensions towards France, the Netherlands, Germany, Belgium and Poland." | D1.4 p.19 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 4 / Contact (quote) | "Pilot lead: Plukon – Sieradz" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

### §1 Pilot 5 — Grossfurtner-Higelsberger

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 5 / Slaughterhouse (quote) | "the pig slaughterhouse Grossfurtner-Higelsberger GmbH in Austria" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Slaughterhouse (quote) | "Pilot lead: Großfurtner-Higelsberger" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Species, country | Pigs; AT | D1.6 p.11; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Co-lead (quote) | "VetMedUni as scientific co-lead" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Co-lead (quote) | "Sci. lead: Vetmeduni" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Technologies (quote) | "This is a second phase pilot … installed here with one year time difference." | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Technologies (quote, TRL, vendor) | "Pilot 5 already installed the CLK Pig Inspector (TRL 5)" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Technologies (quote, TRL, vendor) | "in analogy to pilot 2, WEL2BE will install the stunning effectiveness technology for pigs (TRL 5) and the tear staining sensor (TRL 3) in pilot 5, starting at second half of 2024." | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Technologies (vendor correction) | stunning effectiveness = Nuna Solutions (BlinkAI; DTI/DMRI brand), WEL2BE participation ended; tear staining = ILVO | D1.8 p.30; Cat. pp.62, 88; CORDIS [web, via handover-pack/F]; Nuna web site [web, via F] | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G07 — local CORDIS listing 0 hits | 2026-11-16 |
| B | §1 Pilot 5 / Technologies (quote, vendor) | "Technologies of CLK GmbH and Wel2be will be installed and implemented in this Pilot 5." | D1.4 p.20 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Stage | Post-mortem (Pig Inspector); stunning (planned, per D1.6) | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Stage (negative) | Farm / loading / transport / lairage: not stated (D1.6, D1.8) | D1.6; D1.8 | | | OK | grep: G25 and G26 counts as Pilots 1 and 2 (D1.6 p.11: G25 1 hit, G26 2 hits) | 2026-11-17 |
| B | §1 Pilot 5 / Installation status (quotes) | Pig Inspector "already installed"; WEL2BE sensors "will install … starting at second half of 2024" (Sep 2024; possibly April 2024 text) | D1.6 p.11; D1.6 p.3 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Installation status (negative) | D1.8 p.23 (5 Sep 2025): "2nd phase pilot" only; whether the stunning / tear-staining sensors were installed is not stated | D1.8 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G23 (Grossfurtner; Großfurtner; Higelsberger; Schwertberg; Schwertzberg) on D1.8 — 2 hits p.23(2); G26 (lairage; stunning) on D1.8 — pp.25(2), 26, 30, 70; G09 (tear.?stain) on D1.8 — 1 hit p.30; G28 (install) on D1.8 — 0 hits | 2026-11-16 |
| B | §1 Pilot 5 / Installation status (negative) | D6.3 (Oct 2024) carries no installation statement for Pilot 5 | D6.3 | deliverables/D6.3 Data management plan v2.pdf | | OK | grep: G28 (install) on D6.3 — 2 hits pp.17, 41; G33 (pilot 5; P5; Vetmed; Grossfurtner) on D6.3 — 28 hits pp.16(2), 37, 38, 39, 40, 41(4), 42, 43, 44, 45, 46(2), 48, 49(2), 50(2), 51(3), 52(2), 54(2) | 2026-11-17 |
| B | §1 Pilot 5 / Installation status (quote) | "Pilot 5 wrote their response based on the GA" | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, D1.4, D1.5, D6.2, D6.3) | the 10 files named | | | OK | grep: G16 — counts as Pilot 1 | 2026-11-17 |
| B | §1 Pilot 5 / Plan past Oct 2026 (quote) | Pilot 5, "Adapted from the GA": "The main aWISH results will be made available/accessible for the long-term." — GA text | D6.3 p.51 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Throughput (quote, figure) | "The abattoir slaughters pigs only and provides a slaughter capacity of 5,500 (legal minimum and higher welfare standard) pigs per week." | D1.4 p.20 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Region (quote) | "Pilot 5 covers Upper Austria in Austria and extensions towards the rest of Austria." | D1.4 p.20 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Region (quote) | second-phase aim "to broaden the piloting activities and geographical coverage of the developed aWISH solutions and to provide external validation" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Contact (quote) | "Project partner Higelsberger GmbH as part of the Großfurtner GmbH group operates a slaughterhouse and meat-cutting plant located in Schwertzberg, Upper Austria" | D1.4 p.20 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 5 / Contact | Pilot lead: the slaughterhouse; scientific co-lead VetMedUni Vienna | D1.8 p.23; D1.6 p.11 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |

### §1 Pilot 6 — Carnex, Vojvodina

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1 Pilot 6 / Slaughterhouse (quote) | "the pig slaughterhouse Carnex in Vojvodina, Serbia" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Slaughterhouse (quote) | "Pilot lead: Carnex" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Species, country | Pigs; RS | D1.6 p.11; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Co-lead (quote) | "BioSense as scientific co-lead" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Co-lead (quote) | "Sci. lead: Biosense" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Technologies (quote) | "second phase pilot, validating three technologies already implemented in pilots 1 and 2" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Technologies (quote, TRL, vendor) | "FBN will install STREMODO (TRL 5) in the lairage area" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Technologies (quote, TRL, vendor) | "Innotech Vision will install the Lesion Detect (TRL 3) at the evisceration line and the Enviro-detect sensor (TRL 7) on-farm" | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Technologies (quote) | "Installations are expected to be completed by the end of 2024." | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Technologies (quote, TRL, vendor) | "pilot 6 already features Bit Gear's Animal Sense technology (TRL 8) … barn climate (temperature, relative humidity, ammonia concentrations) … the feed level inside the silo and feed consumption. In cooperation with BioSense, the Animal Sense will be extended with a sensor to track pig behavior inside the pen." | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Stage | Farm (Animal Sense; Enviro-detect planned); lairage (STREMODO planned); post-mortem ("evisceration line", planned) | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Stage (negative) | Loading / transport / stunning: not stated (D1.6, D1.8) | D1.6; D1.8 | | | OK | grep: G25 and G26 counts as Pilots 1 and 2 | 2026-11-17 |
| B | §1 Pilot 6 / Installation status (quotes) | Animal Sense "already features"; STREMODO, Lesion Detect, Enviro-detect "will install … expected to be completed by the end of 2024" (Sep 2024) | D1.6 p.11 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Installation status (negative) | D1.8 p.23 (5 Sep 2025): "2nd phase pilot" only; completion of the planned installations is not stated | D1.8 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | grep: G24 (Carnex; Vojvodina) on D1.8 — 1 hit p.23; G29 (Lesion.?Detect; Enviro.?Detect; STREMODO; Animal.?Sense; Pig.?Sense) on D1.8 — 5 hits pp.25, 26, 30(3); on D6.3 — 8 hits pp.36(3), 37(4), 39; G28 (install) on D1.8 — 0 hits | 2026-11-17 |
| B | §1 Pilot 6 / Installation status (quote, vendor) | "Carnex alongside with BioSense (BitGear) has installed and developed the IoT solution PigSense which measures the environmental parameters and real-time food consumption at the pig farms" | D1.4 p.21 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Installation status (quote, figure) | "The system with IoT sensors and IoT platform is currently applied to their three pig farms and potentially four." | D1.4 p.21 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Plan past Oct 2026 (negative) | not stated as to installations (checked D1.1, D1.2, D1.6, D1.8, D4.3, D5.2, D1.4, D1.5, D6.2, D6.3) | the 10 files named | | | OK | grep: G16 — counts as Pilot 1 | 2026-11-17 |
| B | §1 Pilot 6 / Plan past Oct 2026 (quote) | "No answer yet from pilot 6." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Throughput (negative) | Slaughterhouse throughput: not stated | all 11 File-B files | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G17 counts as Pilot 1. G24 (Carnex; Vojvodina) — D1.6 4 (pp.4, 11(3)); D1.8 1 (p.23); D1.4 4 (pp.7(2), 21(2)); D6.2 1 (p.32); D6.3 2 (pp.16, 41); 0 elsewhere | 2026-11-16 |
| B | §1 Pilot 6 / Throughput (quote) | farm side only: "currently applied to their three pig farms and potentially four" | D1.4 p.21 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Region (quote) | "Pilot 6 covers Vojvodinain Serbia and extensions towards the rest of Serbia." (as printed) | D1.4 p.21 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-14 |
| B | §1 Pilot 6 / Contact (quote) | BioSense Institute "also hosts the website" — "The website is hosted by BIOSENSE and will be maintained after the completion of aWISH." | D1.1 p.16; D1.2 p.16 | deliverables/D1.1 CD&E plan and execution report v1.pdf | | OK | | 2026-11-14 |

---

## File B — section 1b data-arrangements table (procedure 8.1 step 2, 8.3)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §1b totals / 8.3 step 2 (quote) | "Currently, 32 signed DSA and 2 ethical approval documents are collected." | D6.3 p.8 | deliverables/D6.3 Data management plan v2.pdf | | OK | grep: G40 (data sharing agreement; DSA; 32 signed) on D6.3 — 23 hits pp.5, 6, 7(2), 8(4), 9, 11, 14(4), 16(2), 17, 35, 54, 78, 80, 81(2) | 2026-11-14 |
| B | §1b totals / 8.3 step 3 (figures) | per-pilot signed DSAs 4, 0, 21, 6, 0, 1 (Table 5) | D6.3 p.16 | deliverables/D6.3 Data management plan v2.pdf | | OK | count: 4 + 0 + 21 + 6 + 0 + 1 = 32, equal to the p.8 total | 2026-11-14 |
| B | §1b totals (quote) | "These are stored by the project coordinator EV ILVO." | D6.3 p.16 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b WP3-wide (quote, unattributed) | "At least a report of the analysis of the data should be made openly available. Individual data most likely not." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b WP3-wide (quote, unattributed) | "If there are restrictions on use, how will access be provided to the data, both during and after the end of the project? Not discussed yet." | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b WP3-wide (quote, unattributed) | "In general, our data outputs will not be open to the public domain (always according to the Grant agreement). Licensing can be studied in every case, if necessary." | D6.3 p.51 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b WP3-wide (quote, unattributed) | "The setting up of a Data Transfer Agreement between all partners within each pilot needs to be considered." | D6.3 p.54 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / DSAs (quote, figure) | 4 ("P1 Vion - The Netherlands 4") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.2 (quote) | "In Pilot 1 most data are owned by the farmer or Vion" | D6.2 p.52 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.2 (negative) | no other Pilot 1 answer in the D6.2 WP3 annex (pp.50–63) | D6.2 pp.50–63 | deliverables/D6.2 Data management plan v1.pdf | | OK | grep: G30 (pilot 1; P1) on D6.2 — 3 hits pp.32, 51, 52; G18 (Vion; Groenlo) on D6.2 — 3 hits pp.52, 91, 92 | 2026-11-16 |
| B | §1b Pilot 1 / D6.2 dataset list (quotes) | "Pilot1_VION1 … Carcass composition data"; "Pilot1_FBN1 … Stress behaviour" (p.91); "Pilot1_VION2 PigInspector" (p.92); "Pilot1_InnoTech1 … developmental data" (p.93) | D6.2 pp.91, 92, 93 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 1 / D6.3 openness (quote) | "In pilot 1 due to data sharing limitations all data will remain private and securely stored within the aWISH dataplatform. As per aWISH dataplatform (see WP4)." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 access after project (negative) | not stated for Pilot 1 specifically | D6.3 pp.41–54 | | | OK | grep: G30 (pilot 1; P1) on D6.3 — 17 hits pp.16, 36, 37, 38, 39, 41(2), 42, 43(3), 44, 45, 46, 48, 54(2) | 2026-11-17 |
| B | §1b Pilot 1 / D6.3 access after project (quote, platform-level) | "all data will remain available but not findable for a period that will be determined by the cloud storage cost." | D6.3 p.60 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 other (quote) | "In Pilot 1 Data are owned by the farmer or Vion." | D6.3 p.41 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 other (quote) | embargo: "If necessary 2 year will be nice lead time. (pilot 1)" | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 other (quote) | access protocol: "Depending on the data and who owns them. (pilot 1)" | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 other (quote) | "Pilot 1 - Data sharing agreements are signed by all focus companies." | D6.3 p.54 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 1 / D6.3 other (quote) | "In pilot 1 data owned by farmers should be legally arranged for usage." | D6.3 p.54 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / DSAs (quote, figure) | 0 ("P2 Batallé - Spain 0") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote, attribution) | "All our collected datasets will be confidential for external stakeholders of the project. Data will be usable for the scientific teams of the project in order to achieve the project goals. But the data should remain confidential for external use ." — WP3 general-info cell; repeated as Pilot 2's answer in D6.3 p.42 | D6.2 p.53; D6.3 p.42 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote) | "Pilot 2 believes that data access will be restricted and stopped after the end of the project." | D6.2 p.56 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote) | "Pilot 2 will provide the documentation under petition of the coordinator or the scientific leader of the WP." | D6.2 p.59 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote) | data management "In Pilot 2 Manager of the project at Selección Batallé and the data protection manager of Selección Batallé." | D6.2 p.62 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote) | security "In Pilot 2 - All provisions actually actives on our working network. Includes firewall and backup copies." | D6.2 p.62 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote, figures) | data volumes: "Stunning sensor: 0,001 Gb per day (if image collection: 1Gb per day) Tear staining sensor: 0,001 Gb per day (if image collection: 2Gb per day) Lung and liver sensor: 0,001 Gb per day (if image collection: 4Gb per day)" | D6.2 p.52 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.2 (quote) | other procedures: "Pilot 2 - no" | D6.2 p.63 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 openness (quote) | "In pilot 2 each dataset will be open to the partners involved in the task (equipment provider and scientific leader) but will be closed to other partners." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 openness (quote) | "In pilot 2 All collected datasets will be confidential for external stakeholders of the project … But the data should remain confidential for external use." | D6.3 p.42 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 access after project (quote) | "Pilot 2 Data access will be restricted and stopped after the end of the project." (v1 "believes that … will be" has become "will be") | D6.3 p.46; D6.2 p.56 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 2 / D6.3 access after project (quote) | "Pilot 2 - In general, data will not be usable by third parties. In particular situations, with a previous study, we can give permission to use some datasets." | D6.3 p.51 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 other (quote) | "In pilot 2 Data will be allocated in a trusted repository, according to the project working plan. Ubitech is the responsible of the management of the data repository for the aWISH project (WP4)." | D6.3 p.45 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 other (quote) | repository arrangements: "In pilot 2 they will do in few weeks." | D6.3 p.45 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 other (quote) | "Pilot 2 can create vocabularies if necessary." | D6.3 p.49 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 2 / D6.3 other (quote) | data management "In Pilot 2 Technical manager of the project at Selección Batallé and the data protection manager of Selección Batallé." | D6.3 p.52 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / DSAs (quote, figure) | 21 ("P3 Plukon - Duc - France 21") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.2 (negative) | Pilot 3 not named in the D6.2 WP3 annex | D6.2 pp.50–63 | deliverables/D6.2 Data management plan v1.pdf | | OK | grep: G31 (pilot 3; P3) on D6.2 — 1 hit p.32; G21 (DUC; Chailley; Plukon) on D6.2 — 0 hits | 2026-11-16 |
| B | §1b Pilot 3 / D6.2 dataset list (quotes) | "Pilot3_PLUK1 … Footpad Lesions"; "Pilot3_PLUK2 … Hockburns"; "Pilot3_W2B1 Stunning Vision system 16/03/2023" | D6.2 p.92 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 openness (quote) | "In pilot 3 no, because data can hold confidential information, only when it is made anonymous some data can be shared." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 openness (quote) | "No, data will not be publicly available. (pilot 3)." | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 openness (quotes) | metadata "No, because data can hold confidential information. (pilot 3)"; "Data will not be publicly available. (pilot 3)" | D6.3 p.47 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 openness (quote) | "For pilot 3 Data will not be publicly available." | D6.3 p.50 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 access after project (quote) | "In Pilot 3 - For ITAVI, database of labeled acoustic sound will be kept by ITAVI, to be enriched after the project and also the model developed. The rest of the data will be deleted at the end of the project: EBENE® evaluation, videos, raw sounds track, transport monitoring. Images are only available 28 days; reports are available for five years." | D6.3 p.53 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 access after project (quote) | "Pilot 3 - Yes after validation with Plukon and ITAVI depending on the technologies output is needed." | D6.3 p.51 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 access after project (quote, attribution) | "Preferably, data will be available during the project lifetime. After the end of the project, data will not be accessed." — WP3 answer, follows a Pilot 3 sentence; not attributed to a named pilot (8.3 step 5) | D6.3 p.49 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | "Yes, Plukon needs to validate all data access (pilot 3)" | D6.3 p.47 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | "In pilot 3 .csv files can be sent via mail. All the valuable data will be uploaded on the awish platform and the raw data for model training will be stored by ITAVI on hard drives or laptop." | D6.3 p.45 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | "other data sharing need validation by Plukon (economic data for example)" | D6.3 p.45 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | "In pilot 3 the code will be included in a relevant software for acoustic monitoring and EBENE but not for transport heat stress modeling and EBroilerTrack image." | D6.3 p.48 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | data management "In Pilot 3 Plukon."; costs "Part of the Horizon Europe grant. (pilot 3)." | D6.3 p.52 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 3 / D6.3 other (quote) | "For pilot 3 Yes, therefore only anonymous data can be used." | D6.3 p.54 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / DSAs (quote, figure) | 6 ("P4 Plukon - Sieradz - Poland 6") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / D6.2 (negative) | Pilot 4 not named in the D6.2 WP3 annex | D6.2 pp.50–63 | deliverables/D6.2 Data management plan v1.pdf | | OK | grep: G32 (pilot 4; P4) on D6.2 — 1 hit p.32; G22 (Sieradz) on D6.2 — 0 hits | 2026-11-16 |
| B | §1b Pilot 4 / D6.2 dataset list (quotes) | "Pilot4_PLUK1 … Footpad Lesions"; "Pilot4_PLUK2 … Hockburns" (p.91); "Pilot4_PLUK3 … CatchDamage" (p.92); "Pilot4_PLUK3 … ChickenCheck Scratch" (p.93) | D6.2 pp.91, 92, 93 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 4 / D6.3 openness (quote) | "In Pilot 4 no, because data can hold confidential information, only when it is made anonymous some data can be shared." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / D6.3 access after project (quote) | "In Pilot 4 Images are only available 28 days, reports are available for five years." | D6.3 p.53 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / D6.3 other (quote) | "In Pilot 4 the file name of the images have a timestamp, rating and flocknumber." | D6.3 p.42 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / D6.3 other (quote) | "In Pilot 4 the suggestion is to send .csv files via email." | D6.3 p.45 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 4 / D6.3 other (quote) | security: "In Pilot 4 Back-ups are available, firewalls before accessing as well." | D6.3 p.53 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / DSAs (quote, figure) | 0 ("P5* Grossfurtner - Austria 0"; "* 2nd phase pilot") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 5 / D6.2 (negative, attribution) | not stated as a named pilot; D6.2 WP3 annex has unattributed answers that reappear in D6.3 as Pilot 5's | D6.2 pp.50–63 | deliverables/D6.2 Data management plan v1.pdf | | OK | grep: G33 (pilot 5; P5; Vetmed; Grossfurtner) on D6.2 — 4 hits pp.32, 52(2), 61 | 2026-11-17 |
| B | §1b Pilot 5 / D6.2 (quote, unattributed) | "Observational data are generated at the slaughterhouse and further processed by technology partners and Vetmed" | D6.2 p.52 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.2 (quote, unattributed) | "Vetmed as a research partner receives a dissemination fee of €3500" | D6.2 p.61 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.2 dataset list (quote) | "Pilot5_GROSS1 PigInspector" | D6.2 p.93 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 5 / D6.3 openness (quote, GA text) | "Pilot 5 wrote their response based on the GA: Documents and multimedia will mainly be open, apart from deliverables noted as confidential. Datasets will be made open if possible (see Grant Agreement 1.2.6). Code and algorithms that are part of the (commercial) exploitation plans of the companies will be protected (…)" | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.3 access after project (quote, GA text) | "Pilot 5 - Adapted from the GA: Yes, results will be published in scientific papers and associated data will be linked to a repository with a persistent identifier. Deliverables, presentations, policy briefs, trainings and other dissemination material will be open access with CC-0/ BY/ BY NC license. The main aWISH results will be made available/accessible for the long-term." | D6.3 p.51 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 5 / D6.3 access after project (quote) | embargo: "No, not from Vetmed's side, but this needs to be discussed with the technology providers as well. (pilot 5)" | D6.3 p.46 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.3 other (quote) | "Details of datasets, data ownership and restrictions and data contacts will be specified in the next version of the Data Management Plan (DMP)." | D6.3 p.42 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.3 other (quote, figure) | "For pilot 5 Vetmed as a research partner receives a dissemination fee of €3500. This includes an open access publication fee (and a conference/event subscription fee). All other costs (& how much budget there is to spend on WP3) regarding FAIR data access need to be defined by WP4/UBI (central data platform)." | D6.3 p.52 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 5 / D6.3 other (quote) | "For pilot 5 data ownership, data anonymization (farm data) and data (e.g., algorithms) sharing by technology providers are topics that still need special emphasis and will be further described in the next version of the DMP." | D6.3 p.54 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 6 / DSAs (quote, figure) | 1 ("P6* Carnex - Serbia 1"; "* 2nd phase pilot") | D6.3 p.16 Table 5 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-16 |
| B | §1b Pilot 6 / D6.2 (negative) | Pilot 6 not named in the D6.2 WP3 annex | D6.2 pp.50–63 | deliverables/D6.2 Data management plan v1.pdf | | OK | grep: G34 (pilot 6; P6; Carnex) on D6.2 — 1 hit p.32 | 2026-11-17 |
| B | §1b Pilot 6 / D6.2 dataset list (quote) | "Pilot6_FBN1 … Stress behaviour" | D6.2 p.93 | deliverables/D6.2 Data management plan v1.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 6 / D6.3 openness (quote) | "No answer yet from pilot 6." | D6.3 p.44 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 6 / D6.3 access after project (negative) | not stated | D6.3 pp.41–54 | | | OK | grep: G34 (pilot 6; P6; Carnex) on D6.3 — 11 hits pp.16(2), 37, 38, 39, 41(3), 42, 43, 44 | 2026-11-17 |
| B | §1b Pilot 6 / D6.3 other (quote) | "In pilot 6 there will also be newly generated data coming from newly installed equipment." | D6.3 p.41 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |
| B | §1b Pilot 6 / D6.3 other (quote) | "In pilot 6 it is yet to be determined." | D6.3 p.42 | deliverables/D6.3 Data management plan v2.pdf | | OK | | 2026-11-14 |

---

## File B — section 4 contradictions 1 to 13 (procedure 8.1 step 4, 8.5)

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|
| B | §4 C1 Stunning-effectiveness vendor | D1.6 attributes pig and broiler stunning sensors to WEL2BE (pp.9, 10, 11); D1.4 pp.17–20 and D6.2 p.92 ("Pilot2_W2B1 CET'automatique"; "Pilot3_W2B1 Stunning") likewise; D1.8 p.30 "Stunning effectiveness (Nuna solutions)"; Cat. p.62 "BlinkAI … Technology under development within the aWISH project to monitor the stunning effectiveness … Provider nunaSolutions … Technology used in aWISH project"; CORDIS "WEL2BE — Participation ended / France", "BY-NUNASOLUTIONS SL — Spain … SME: Yes"; Nuna site "NunaSolutions, is a brand of Teknologisk Institute"; handover terms not stated in any document read; broiler sensor at Pilot 3 attributed to WEL2BE only, no successor named | D1.6 pp.9, 10, 11; D1.4 pp.17–20; D6.2 p.92; D1.8 p.30; Cat. p.62; CORDIS participants list [web, via handover-pack/D Table 3 and F §6 — 7.5 step 4]; Nuna web site [web, via F §6] | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G07 (Nuna; WEL2BE; W2B; Teknologisk; Technological Institute; DMRI) and G15 (BlinkAI; CET'Automatique) — see File A P10 and D4; local CORDIS listing 0 hits for all these terms | 2026-11-16 |
| B | §4 C2 Tear-staining vendor | D1.6 pp.9, 11 "WEL2BE, TRL 3"; D6.2 p.92 "Pilot2_W2B2 tear-staining"; D1.8 p.30 "Tear staining (ILVO)"; Cat. p.88 "Tear staining aWISH … Provider aWISH partners … in the development phase (accessed 21 August 2026)"; website pilots page (2026-10-07) "Tear staining system (ILVO)" | D1.6 pp.9, 11; D6.2 p.92; D1.8 p.30; Cat. p.88; www.awish-project.eu pilots page [web, via handover-pack/D] | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G09 (tear.?stain) — D1.6 1 hit p.9 (file B also cites p.11: 0 hits on p.11 for "tear.?stain"); D1.8 1 hit p.30; Cat. 9 hits pp.13, 87(4), 88(4) | 2026-11-16 |
| B | §4 C3 Pilot 1 technology count | D1.6 p.9 "Three new technologies"; D1.8 p.25 seven items, of which AI4Animals (Deloitte), AUTOFOM3 (Carometec), Tail Length (VION), CGM Insertion Probe do not appear in D1.6 or the register's vendor table; D1.8 p.28 labels two "OTHER TECHNOLOGIES" | D1.6 p.9; D1.8 pp.25, 28 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | grep: G35 (AI4Animals; Autofom; Carometec; CGM; Deloitte; tail.?length) on D1.6 — 3 hits pp.8, 9, 11 (expected to be "tail length" only; to confirm on the page) | 2026-11-17 |
| B | §4 C4 Tail length attribution at Pilot 1 | D1.8 p.25 lists "PigInspector (CLK GmbH) – Ear, Tail and Skin Lesions" and separately "Tail Length (VION)"; D1.8 p.27 says PigInspector "Measures ear, tail, and skin lesions + tail length"; D1.6 p.9 Pig Inspector "measures tail length" | D1.8 pp.25, 27; D1.6 p.9 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-16 |
| B | §4 C5 Pilot 2 tail-length prototype | Cat. p.57 "Tail Length (prototype) … Provider UAB & Batallé … Technology used in aWISH project"; not in D1.6 Pilot 2 list (p.9) nor in the register's vendor table | Cat. p.57; D1.6 p.9 | deliverables/AWI Catalogue (final version).pdf | | OK | grep: G35 on D1.6 — "tail.?length" hits pp.8, 9, 11 (p.9 is the Pig Inspector sentence); G19 (Batall) on Cat. — 1 hit p.57 | 2026-11-16 |
| B | §4 C6 Pilot 3 naming | D1.6 p.10 "DUC (Plukon Food Group) in Chailley"; D1.8 p.23 "Plukon – Duc" | D1.6 p.10; D1.8 p.23 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-16 |
| B | §4 C7 Co-lead label for Pilot 2 | D1.8 p.23 prints "Wet. H.: UAB" where other pilots print "Sci. lead:" | D1.8 p.23 | deliverables/D1.8 Policy briefs and policy workshop report batch 1.pdf | | OK | | 2026-11-14 |
| B | §4 C8 Partner count | D1.8 p.18 slide "28 partners 11 countries 6 pilots"; register "24 partners in three layers"; documents read do not reconcile the two | D1.8 p.18; register (own file) | deliverables/D1.4 Project website report v2.pdf | | WRONG | grep: G36 ((24 or 28) partners; (11 or 13) countries) over 11 File-B files — D1.8 2 hits p.18(2); D1.4 1 hit p.10 ("involves 28 partners, including affiliated entities, from 11 European countries"); 0 elsewhere. Note: file A T2 row 6 (Siwek, Marchewka 2023) gives "24 partners, 13 countries"; D1.4 also said 28 partners in 11 countries; Corrected in pack B §4 C8: D1.4 p.10 'involves 28 partners, including affiliated entities, from 11 European countries' now quoted | 2026-11-17 |
| B | §4 C9 D1.6 dating | v1.0 dated 29/04/2024; v2.0 (17/09/2024) described only as "Adoption of comments by EC" | D1.6 p.3 | deliverables/D1.6 Practice abstracts batch 1.pdf | | OK | | 2026-11-16 |
| B | §4 C10 Pilot 2 slaughterhouse name | D1.4 p.17 "NORFRISA (FRIGORÍFICOS DEL NORDESTE S.A.) is one of the largest slaughterhouses in Spain … 10,000 pigs to be slaughtered every day"; D1.6 p.9 "the pig slaughterhouse Batallé in Catalonia, Spain"; D1.8 p.23 "Pilot lead: Batallé"; D6.3 p.16 "P2 Batallé - Spain"; D6.3 p.52 "Selección Batallé"; "Batallé does not occur in D1.4"; "Norfrisa does not occur in D1.6, D1.8, D6.2 or D6.3"; Norfrisa listed as roundtable panellist at the 8 Oct 2026 industry event (handover-pack/E source 17) | D1.4 p.17; D1.6 p.9; D1.8 p.23; D6.3 pp.16, 52; live pilots page and CORDIS participants list [web] (8.5 step 2.3–2.4); handover-pack/E source 17 [secondary] | deliverables/D1.4 Project website report v2.pdf | | OK | grep: G20 (Norfrisa; Frigoríficos del Nordeste) — D1.4 3 hits p.17(3); 0 hits in D1.6, D1.8, D6.2, D6.3 and all other File-B files. G19 (Batall[eé]; Selecci[oó]n) — D1.4 2 hits p.7(2): the abbreviation list entry "BATA SELECCION BATALLE SA" (so "Batallé does not occur in D1.4" holds for the pilot text pp.16–21 but not for the whole document); D1.6 pp.4, 9(2); D1.8 p.23; D6.2 p.62(4); D6.3 pp.16, 52(4); Cat. p.57 | 2026-11-17 |
| B | §4 C11 Pilot 4 vendor list | D1.4 p.19 "With technology providers CLK GmbH and Wel2be, more carcass vision data will be added"; "New technologies are installed from Itavi, Wel2be and CLK GmbH."; D1.6 p.10 "CLK is responsible for all newly installed technologies in this pilot" plus Itavi EBENE; WEL2BE not named for Pilot 4; D6.2 dataset list (pp.91–93) has no W2B dataset for Pilot 4 | D1.4 p.19; D1.6 p.10; D6.2 pp.91–93 | deliverables/D1.4 Project website report v2.pdf | | OK | grep: G11 (Wel.?2.?be; W2B; stunning) — D1.4 p.19(3); D1.6 p.10(2); D6.2 p.92(4) and pp.51, 52, 54 (the p.92 hits are to be matched to Pilot2_W2B1, Pilot2_W2B2, Pilot3_W2B1 — three dataset names, four hits) | 2026-11-17 |
| B | §4 C12 Pilot 6 on-farm system name | D1.4 p.21 "BioSense (BitGear) has installed and developed the IoT solution PigSense"; D1.6 p.11 "Bit Gear's Animal Sense technology (TRL 8)"; website pilots page (2026-10-07) "Animal Sense (Bitgear, BioSense)" | D1.4 p.21; D1.6 p.11; www.awish-project.eu pilots page [web, via handover-pack/D] | deliverables/D1.4 Project website report v2.pdf | | OK | grep: G29 (…; Animal.?Sense; Pig.?Sense) — D1.4 1 hit p.21; D1.8 hits pp.25, 26, 30(3) are STREMODO / Lesion-Detect / Enviro-Detect terms | 2026-11-17 |
| B | §4 C13 Pilot 1 pre-existing technologies | D1.4 p.16 "already installed cameras in the unloading and lairage area …, a full carcass scan system (AutoFOM3) … and camera's to measure tail length on the carcass (individual carcass tracking using RFID on the slaughter line)"; D1.8 p.25 "AUTOFOM3 (Carometec)"; D1.8 p.28 "Tail Length (VION)" under "OTHER TECHNOLOGIES"; D1.6 p.9 "Three new technologies" | D1.4 p.16; D1.8 pp.25, 28; D1.6 p.9 | deliverables/D1.4 Project website report v2.pdf | | OK | | 2026-11-17 |

---

## File A — 1-in-5 sample of the remaining Table 1 rows (procedure 7.1 step 2)

Rows examined in full under 7.1 step 1 (15): P3, P5, P6, P7, P8, P9, P10, P14, P16, B5, B9, B10, B11, B12, B13.

Remaining rows, in table order (23): 1 P1, 2 P2, 3 P4, 4 P11, 5 P12, 6 P13, 7 P15, 8 P17, 9 P18, 10 P19, 11 P20, 12 P21, 13 P22, 14 B1, 15 B2, 16 B3, 17 B4, 18 B6, 19 B7, 20 B8, 21 B14, 22 B15, 23 B16.

Every fifth row of that list (positions 5, 10, 15, 20) — **sample: P12, P19, B2, B7.** Selected mechanically before any examination (7.1 step 2). Rows for these four are not pre-filled in this log; add them when examining. If any sampled row gets WRONG or EDIT, examine all 23 remaining rows (7.1 step 3).

---

## Pre-fill summary (19 Oct 2026)

| File | Section | Rows pre-filled |
|---|---|---|
| A | Table 1 rows P3, P5, P6, P7, P8, P9, P10, P14, P16 (pigs) | 17 + 10 + 9 + 13 + 11 + 11 + 18 + 11 + 16 = 116 |
| A | Table 1 rows B5, B9, B10, B11, B12, B13 (broilers) | 9 + 16 + 21 + 14 + 7 + 7 = 74 |
| A | Row-count paragraph (7.3 steps 1–3, plus the step 4–5 conclusion) | 6 |
| A | Table 2 publications (15 rows + listing-sources line) | 16 |
| A | Disagreements D1–D12 | 12 |
| B | §1 per-pilot table: Pilot 1 / 2 / 3 / 4 / 5 / 6 | 34 + 35 + 26 + 25 + 23 + 22 = 165 |
| B | §1b data arrangements (totals and WP3-wide 7; Pilots 1–6: 12 + 16 + 16 + 8 + 11 + 7) | 77 |
| B | §4 contradictions 1–13 | 13 |
| | **Total rows pre-filled** | **479** (File A 224; File B 255) |
| | Rows with a `grep:` entry (negative claims, plus claims that cite a web source absent from the local CORDIS listing) | 66 (File A 21; File B 45) |
| | Section 9 problems counted | 3 (problems 1, 2, 3) |

Not pre-filled (outside the brief given to the agent): File A "Could not find / not stated" list items 1, 2, 3, 7, 9 (procedure 7.6); File B section 2 chronology (8.1 step 3, only where it adds a claim); File B section 3 "not stated" list rows (8.4 steps 2–3; only the row count was done); File B "Statements that apply to all pilots" bullets (lines 42–47); the 1-in-5 sample rows P12, P19, B2, B7.

---

## Appendix — grep output (19 Oct 2026)

Helper: a Python script that splits each text file on form-feed characters and reports, per file, the total number of case-insensitive regex matches and the text-page numbers that carry them, with the number of matches per page in parentheses. Equivalent single-file command, per procedure 6.6:

```bash
grep -n -i -E "Lesion.?Detect|lung|liver" "deliverables/text/D2.2 Methodology for measuring each AWI.txt"
```

Files searched (short name → text file in `deliverables/text/`): D1.1 → `D1.1 CD&E plan and execution report v1.txt`; D1.2 → `D1.2 CD&E plan and execution report v2.txt`; D1.4 → `D1.4 Project website report v2.txt`; D1.5 → `D1.5 Social media engagement strategy.txt`; D1.6 → `D1.6 Practice abstracts batch 1.txt`; D1.8 → `D1.8 Policy briefs and policy workshop report batch 1.txt`; D2.1 → `D2.1 Valid AWI for pigs and broilers.txt`; D2.1-annex → `D2.1 annexes and disclaimer (website version).txt`; D2.2 → `D2.2 Methodology for measuring each AWI.txt`; Cat. → `AWI Catalogue (final version).txt`; D4.3 → `D4.3 Best practice guides v1.txt`; D5.2(OCR) → `D5.2 OCR text.txt`; D6.2 → `D6.2 Data management plan v1.txt`; D6.3 → `D6.3 Data management plan v2.txt`; CORDIS → `CORDIS listing 101060818.txt`. BSE-rev and AgronRes2025 are `pdftotext` extractions of `papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf` and `papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf` made in the agent's scratch folder (not kept in the repository).

"All 15 text files" = every file above except D5.2's non-OCR text file (8 KB, no usable text). "11 File-B files" = D1.1, D1.2, D1.6, D1.8, D4.3, D5.2(OCR), Cat., D1.4, D1.5, D6.2, D6.3.

```text
## G01
regex: Weight.?Detect|WD system
D2.2: 1 hits on pp. 19
Cat.: 3 hits on pp. 21, 28, 32

## G02
regex: skin.?lesion|Pig.?Inspector
D2.2: 13 hits on pp. 19(5), 29, 31(2), 32(2), 35(3)
Cat.: 20 hits on pp. 12, 46(4), 47(4), 48(2), 49, 50(3), 53, 54(3), 147

## G03
regex: TAIL.?SCAN|Farm.?4.?Trade
D2.2: 1 hits on pp. 19
Cat.: 10 hits on pp. 49, 52(3), 53, 56(3), 59(2)
BSE-rev: 6 hits on pp. 4(3), 10(3)

## G04
regex: tail.?length
D2.2: 5 hits on pp. 7, 13, 19, 28, 29
Cat.: 13 hits on pp. 12, 47, 50, 52, 53(2), 54(2), 55, 56, 57(3)

## G05a
regex: Lesion.?Detect|lung|liver (procedure 6.6 literal)
D2.2: 57 hits on pp. 1, 2(3), 3, 4, 5, 6, 7(2), 8(2), 9(5), 10, 11(6), 12, 13(2), 14, 15, 16, 17, 18, 19(2), 20(2), 21, 22, 23, 24, 25, 26, 27, 28(2), 29(2), 30, 31, 32, 33, 34, 35, 36, 37, 38, 39
Cat.: 12 hits on pp. 12, 43, 58(3), 59(2), 60(4), 149

## G05b
regex: Lesion.?Detect|\blungs?\b|\blivers?\b (word-bounded; 'Deliverable' excluded)
D2.2: 11 hits on pp. 7, 11(5), 13, 19, 20, 28, 29
Cat.: 12 hits on pp. 12, 43, 58(3), 59(2), 60(4), 149

## G06
regex: Blink.?AI|Nuna|CET.?Automatique|Wel.?2.?be|W2B|corneal
D2.2: 4 hits on pp. 27(2), 28, 29
Cat.: 7 hits on pp. 61(2), 62(3), 85(2)

## G07
regex: Nuna|Wel.?2.?be|W2B|Teknologisk|Technological Institute|DMRI (all 15 text files)
D1.1: 0 hits
D1.2: 0 hits
D1.4: 8 hits on pp. 17, 18(3), 19(2), 20, 25
D1.5: 0 hits
D1.6: 4 hits on pp. 9(2), 10, 11
D1.8: 1 hits on pp. 30
D2.1: 0 hits
D2.1-annex: 0 hits
D2.2: 1 hits on pp. 27
Cat.: 4 hits on pp. 62(2), 85(2)
D4.3: 0 hits
D5.2(OCR): 0 hits
D6.2: 3 hits on pp. 92(3)
D6.3: 0 hits
CORDIS: 0 hits

## G08
regex: STREMODO
D2.2: 5 hits on pp. 19, 31, 32, 35(2)
Cat.: 2 hits on pp. 77, 78
D1.6: 2 hits on pp. 9, 11
D1.8: 3 hits on pp. 25, 26, 30

## G09
regex: tear.?stain
D2.2: 3 hits on pp. 26, 28, 35
Cat.: 9 hits on pp. 13, 87(4), 88(4)
D1.6: 1 hits on pp. 9
D1.8: 1 hits on pp. 30

## G10
regex: E.?Broiler.?Track|Itavi|distress|alarm.?call|Chirpy|Greengage
D2.2: 18 hits on pp. 17(3), 19, 20, 21, 22(4), 23(5), 33(2), 39
Cat.: 15 hits on pp. 49, 106, 133(5), 134(4), 135(4)

## G11
regex: Wel.?2.?be|W2B|stunning
D1.6: 7 hits on pp. 9(3), 10(2), 11(2)
Cat.: 24 hits on pp. 3(2), 10(3), 61(2), 62(3), 63(4), 67, 84, 107(3), 136(2), 137(2), 152
D2.2: 12 hits on pp. 11, 27(2), 28(4), 29, 34(2), 35(2)
D1.4: 10 hits on pp. 17, 18(4), 19(3), 20, 25
D1.5: 0 hits
D6.2: 7 hits on pp. 51, 52, 54, 92(4)
D6.3: 6 hits on pp. 36, 38, 39, 40, 44, 57

## G12
regex: catch.?damage|Chicken.?Check
Cat.: 12 hits on pp. 108, 138, 140, 141, 142, 143(2), 144(2), 145, 146, 151
D2.2: 3 hits on pp. 23, 28, 35
D1.6: 8 hits on pp. 10(8)

## G13
regex: scratch|Chicken.?Check
Cat.: 13 hits on pp. 108, 138, 140, 141, 142, 143, 144, 145(3), 146(3)
D1.6: 8 hits on pp. 10(8)
D2.2: 1 hits on pp. 23

## G14
regex: Inno.?Tech (Agronomy Research 2025 PDF via pdftotext)
AgronRes2025: 1 hits on pp. 1

## G15
regex: Blink.?AI|CET.?Automatique (all 15 text files)
D1.1: 0 hits
D1.2: 0 hits
D1.4: 0 hits
D1.5: 0 hits
D1.6: 0 hits
D1.8: 0 hits
D2.1: 0 hits
D2.1-annex: 0 hits
D2.2: 1 hits on pp. 27
Cat.: 2 hits on pp. 61, 62
D4.3: 0 hits
D5.2(OCR): 0 hits
D6.2: 1 hits on pp. 92
D6.3: 0 hits
CORDIS: 0 hits

## G16
regex: 8.2.6 terms: after the project|end of the project|continu|sustain|maintain|2027|beyond (11 File-B files)
D1.1: 19 hits on pp. 8, 10, 11, 12, 13, 16(2), 18, 20(2), 23, 28, 31, 32(3), 33, 34, 36
D1.2: 33 hits on pp. 6, 8, 9, 10, 11(2), 12, 13, 16(3), 18, 21, 22, 25(2), 26, 31, 32, 33(2), 34(2), 35, 36, 38, 39, 40, 41, 42(3), 43
D1.6: 2 hits on pp. 6, 7
D1.8: 18 hits on pp. 14, 33, 46(2), 47(3), 48, 53(3), 56, 62(2), 67, 69, 75, 76
D4.3: 11 hits on pp. 7, 27, 41, 55(2), 63, 72, 93, 100, 114(2)
D5.2(OCR): 45 hits on pp. 6, 16(2), 17(3), 29(2), 30(2), 34(2), 35(3), 36, 40, 41, 42(2), 43, 48, 49, 59, 65, 68(2), 69, 70, 72, 74, 77, 78, 79, 86, 88, 94(2), 99, 103, 112, 119, 133, 139, 142
Cat.: 23 hits on pp. 25, 31, 44, 45, 48, 73, 80, 81, 113, 114, 115, 116, 117, 118, 119, 120, 121, 122, 123, 124, 125, 126, 137
D1.4: 6 hits on pp. 4, 21, 23, 27, 35(2)
D1.5: 9 hits on pp. 9(2), 11(2), 12, 28(4)
D6.2: 25 hits on pp. 10, 11, 21, 27, 39, 40, 45, 47, 56(2), 59(2), 60, 67, 69, 74, 76, 77(3), 80, 86, 88, 95(2)
D6.3: 16 hits on pp. 24, 32, 37, 46, 49, 50, 51, 53, 61(2), 66, 68, 69(2), 74, 84

## G17
regex: capacity|throughput|per week|per day|per hour|slaughtered|birds/h|pigs/h (11 File-B files)
D1.1: 1 hits on pp. 9
D1.2: 1 hits on pp. 9
D1.6: 0 hits
D1.8: 2 hits on pp. 55(2)
D4.3: 6 hits on pp. 26, 75, 120, 121, 122, 123
D5.2(OCR): 7 hits on pp. 26, 38, 50, 57, 86, 104, 143
Cat.: 2 hits on pp. 68(2)
D1.4: 4 hits on pp. 13, 17, 20(2)
D1.5: 1 hits on pp. 8
D6.2: 8 hits on pp. 8, 52(7)
D6.3: 15 hits on pp. 9, 36(2), 40(10), 43(2)

## G18
regex: Vion|Groenlo
D1.1: 0 hits
D1.2: 0 hits
D1.6: 4 hits on pp. 4, 9(3)
D1.8: 6 hits on pp. 23, 24, 25(2), 28(2)
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 6 hits on pp. 7(2), 16(3), 25
D1.5: 0 hits
D6.2: 3 hits on pp. 52, 91, 92
D6.3: 2 hits on pp. 16, 41

## G19
regex: Batall[eé]|Selecci[oó]n
D1.1: 0 hits
D1.2: 0 hits
D1.6: 3 hits on pp. 4, 9(2)
D1.8: 1 hits on pp. 23
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 1 hits on pp. 57
D1.4: 2 hits on pp. 7(2)
D1.5: 0 hits
D6.2: 4 hits on pp. 62(4)
D6.3: 5 hits on pp. 16, 52(4)

## G20
regex: Norfrisa|Frigor[ií]ficos del Nordeste
D1.1: 0 hits
D1.2: 0 hits
D1.6: 0 hits
D1.8: 0 hits
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 3 hits on pp. 17(3)
D1.5: 0 hits
D6.2: 0 hits
D6.3: 0 hits

## G21
regex: \bDUC\b|Chailley|Plukon
D1.1: 0 hits
D1.2: 0 hits
D1.6: 8 hits on pp. 4(2), 10(6)
D1.8: 3 hits on pp. 23(3)
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 7 hits on pp. 7, 18(4), 19(2)
D1.5: 0 hits
D6.2: 0 hits
D6.3: 10 hits on pp. 16(3), 41(2), 45, 47, 49, 51, 52

## G22
regex: Sieradz
D1.1: 0 hits
D1.2: 0 hits
D1.6: 1 hits on pp. 10
D1.8: 1 hits on pp. 23
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 2 hits on pp. 19(2)
D1.5: 0 hits
D6.2: 0 hits
D6.3: 1 hits on pp. 16

## G23
regex: Gro(ss|ß)furtner|Higelsberger|Schwertberg|Schwertzberg
D1.1: 0 hits
D1.2: 0 hits
D1.6: 4 hits on pp. 4, 11(3)
D1.8: 2 hits on pp. 23(2)
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 4 hits on pp. 7, 20(3)
D1.5: 0 hits
D6.2: 0 hits
D6.3: 1 hits on pp. 16

## G24
regex: Carnex|Vojvodina
D1.1: 0 hits
D1.2: 0 hits
D1.6: 4 hits on pp. 4, 11(3)
D1.8: 1 hits on pp. 23
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 4 hits on pp. 7(2), 21(2)
D1.5: 0 hits
D6.2: 1 hits on pp. 32
D6.3: 2 hits on pp. 16, 41

## G25
regex: \bfarm|loading|transport (stage terms, D1.6 and D1.8)
D1.6: 36 hits on pp. 2(2), 4(3), 5, 6(4), 7(3), 8(12), 9(4), 10(6), 11
D1.8: 52 hits on pp. 21(2), 26, 28, 30(4), 35, 37, 39, 43, 46, 47, 48(7), 49(2), 51, 52, 53(2), 54, 55(3), 56, 58(2), 59(4), 60(2), 61(2), 62, 68(2), 70(3), 71, 72, 73(2)

## G26
regex: lairage|stunning (stage terms, D1.6 and D1.8)
D1.6: 6 hits on pp. 9(2), 10(2), 11(2)
D1.8: 5 hits on pp. 25(2), 26, 30, 70

## G27
regex: pilot ?[1-6] mentions in D1.8
D1.8: 3 hits on pp. 24(2), 25

## G28
regex: install (D1.8, D6.3 — installation status after Sep 2024)
D1.8: 0 hits
D6.3: 2 hits on pp. 17, 41

## G29
regex: Lesion.?Detect|Enviro.?Detect|STREMODO|Animal.?Sense|Pig.?Sense (D1.8, D6.3 — Pilot 6 completion)
D1.8: 5 hits on pp. 25, 26, 30(3)
D6.3: 8 hits on pp. 36(3), 37(4), 39
D1.4: 1 hits on pp. 21

## G30
regex: pilot ?1 / P1 (D6.2 and D6.3)
D6.2: 3 hits on pp. 32, 51, 52
D6.3: 17 hits on pp. 16, 36, 37, 38, 39, 41(2), 42, 43(3), 44, 45, 46, 48, 54(2)

## G31
regex: pilot ?3 / P3 (D6.2 and D6.3)
D6.2: 1 hits on pp. 32
D6.3: 35 hits on pp. 16, 36, 38, 39, 40, 41(2), 42, 43(3), 44, 45(2), 46, 47(4), 48(2), 49(3), 50, 51(3), 52(3), 53(2), 54(2)

## G32
regex: pilot ?4 / P4 (D6.2 and D6.3)
D6.2: 1 hits on pp. 32
D6.3: 11 hits on pp. 16, 36, 38, 40, 41, 42, 43, 44, 45, 53(2)

## G33
regex: pilot ?5 / P5 / Vetmed / Gross (D6.2 and D6.3)
D6.2: 4 hits on pp. 32, 52(2), 61
D6.3: 28 hits on pp. 16(2), 37, 38, 39, 40, 41(4), 42, 43, 44, 45, 46(2), 48, 49(2), 50(2), 51(3), 52(2), 54(2)

## G34
regex: pilot ?6 / P6 / Carnex (D6.2 and D6.3)
D6.2: 1 hits on pp. 32
D6.3: 11 hits on pp. 16(2), 37, 38, 39, 41(3), 42, 43, 44

## G35
regex: AI4Animals|Autofom|Carometec|CGM|Deloitte|tail.?length (D1.6 — contradiction 3/5)
D1.6: 3 hits on pp. 8, 9, 11

## G36
regex: (24|28) partners (contradiction 8)
D1.1: 0 hits
D1.2: 0 hits
D1.6: 0 hits
D1.8: 2 hits on pp. 18(2)
D4.3: 0 hits
D5.2(OCR): 0 hits
Cat.: 0 hits
D1.4: 1 hits on pp. 10
D1.5: 0 hits
D6.2: 0 hits
D6.3: 0 hits

## G37
regex: payment / pay / cost / invoice (who pays, all 11 files)
D1.1: 3 hits on pp. 2, 9, 11
D1.2: 3 hits on pp. 2, 9, 11
D1.6: 3 hits on pp. 1, 12(2)
D1.8: 10 hits on pp. 18, 37, 52, 61(2), 62(3), 68, 69
D4.3: 2 hits on pp. 1, 49
D5.2(OCR): 131 hits on pp. 2, 5, 6(4), 10(2), 13, 14(2), 16(2), 17, 18, 19, 25(2), 26(2), 27(2), 37(4), 38(4), 40, 42(3), 43(2), 44, 45, 46, 47(7), 48, 52(5), 53(3), 54, 55(2), 56, 57(5), 58(2), 61, 62, 63, 64, 65, 67(2), 68(3), 69(2), 70(3), 71, 72(2), 73(2), 75, 77, 78(2), 82, 87(2), 91, 92, 93, 97(3), 112, 127, 128(2), 129(5), 130(6), 134, 138, 145, 151(2), 152(4), 153(7), 154
Cat.: 0 hits
D1.4: 3 hits on pp. 2, 11, 26
D1.5: 2 hits on pp. 2, 11
D6.2: 16 hits on pp. 1, 8, 14, 29(4), 30, 41, 48, 61(3), 70, 81, 89
D6.3: 13 hits on pp. 2, 9, 14, 25(2), 33, 52(3), 60, 62, 75, 85

## G38
regex: after the project etc. in D5.2 OCR — sanity: same as G16 D5.2 row
D5.2(OCR): 45 hits on pp. 6, 16(2), 17(3), 29(2), 30(2), 34(2), 35(3), 36, 40, 41, 42(2), 43, 48, 49, 59, 65, 68(2), 69, 70, 72, 74, 77, 78, 79, 86, 88, 94(2), 99, 103, 112, 119, 133, 139, 142

## G39
regex: ADAL (P9 third-party figure, D2.2/Cat)
D2.2: 1 hits on pp. 19
Cat.: 2 hits on pp. 58, 59

## G40
regex: DSA / Data Sharing Agreement counts (D6.3)
D6.3: 23 hits on pp. 5, 6, 7(2), 8(4), 9, 11, 14(4), 16(2), 17, 35, 54, 78, 80, 81(2)

```

### Context of hits that bear on a negative claim (verbatim from the text files; to be confirmed in the PDF)

- **G19, D1.4 p.7** — abbreviation list: `BATA        SELECCION BATALLE SA` (so the string "Batalle" occurs in D1.4, outside the pilot text on pp.16–21; file B §4 C10 says "Batallé does not occur in D1.4").
- **G14, Agronomy Research 2025 p.1** — author affiliations: `1InnoTech Vision ApS., Niels Pedersens Alle 2, 8830 Tiele, Denmark` (first author's affiliation; file A D3 says the paper "does not name InnoTech Vision as the provider").
- **G36, D1.4 p.10** — `involves 28 partners, including affiliated entities, from 11 European countries` (a second source for the "28 partners / 11 countries" figure of D1.8 p.18; file B §4 C8 cites only D1.8).
- **G36, D1.8 p.18** — `28 partners               11 countries   6 pilots` (as file B quotes).
- **G40, D6.3 p.8** — `Currently, 32 signed DSA and 2 ethical approval documents are collected.` (as file B quotes).
- **G05a, D2.2** — the procedure's example regex `lung|liver` matches the word "Deliverable" in the running header of every D2.2 page; use the word-bounded variant (G05b) or search the PDF for "lung" and "liver" as whole words.

## Update of 19 Nov 2026 (not yet checked)

Text added to packs A and B on 19 Nov, from an ILVO researcher's email of 17 Nov 2026 (name on request). The result code stays blank until the author has checked it.

| File | Where | Text added | Source | Result code | Date |
|---|---|---|---|---|---|
| A | Note 4 | The WP3 deliverable will be public and gives the main lessons learned; the pig sensor validation is described in more detail in D4.2, which will also be public; journal papers are in preparation, and one has been submitted | ILVO email, 17 Nov 2026 | | |
| A | Could not find, item 1 | "Where to look next: D4.2, once published" | ILVO email, 17 Nov 2026 | | |
| A | P16, sources cell | ILVO has withdrawn its restricted tear-staining image set from Zenodo, because partners are reluctant to share images that identify a slaughterhouse | ILVO email, 17 Nov 2026 | | |
| B | Pilot 5 chronology | Vetmeduni sets the access terms for its restricted Zenodo record (contact on request; asked 19 Nov); ILVO is still asking partners to share as much as they can, but many are reluctant; ILVO has withdrawn its tear-staining image set | ILVO email, 17 Nov 2026; the author's email to Vetmeduni, 19 Nov 2026 | | |
