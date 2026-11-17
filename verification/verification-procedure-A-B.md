# Verification procedure — handover-pack files A and B

Written 19 Oct 2026 in ASD-STE100 (Simplified Technical English). Applies to `A-what-validated.md` (version of 7 Oct 2026, evening) and `B-per-pilot-sheet.md` (version of 7 Oct 2026, evening).

> **Update 13 Nov 2026.** The repository was reorganised on 4 Nov 2026 after this procedure was written. Dates were removed from the deliverable file names, the papers moved to `papers/` under descriptive names, and the register moved to private project notes (available on request). The paths in sections 4.2 and 6.6 are corrected to the new names. The claims in files A and B did not change, with one exception: B's D5.2 page numbers were corrected on 4 Nov, because the D5.2 OCR file has an empty leading chunk, so OCR chunk N is printed page N−1. Round 6 of the vault check (4 Nov, private project notes (available on request)) found three page drifts that bear on these files: D2.2 p.32 not p.33 (STREMODO 0.84, row P14); D6.2 p.80 not p.81; D1.4 p.24 not p.23. The vault's own tracking is in private project notes (available on request); record a completed round of this procedure there too.

---

## 1. Purpose

1.1 This procedure tells you how to examine files A and B.

1.2 Files A and B are agent output. Each fact in them has no value until you compare it with its source.

1.3 The Sentient Futures AI-use policy makes you responsible for each fact that goes into the founder brief. You sign an attestation for these facts.

1.4 When you complete this procedure, you can say: "I compared each fact in the brief with its primary source."

---

## 2. Definitions

| Term | Meaning in this procedure |
|---|---|
| Claim | One fact in file A or file B. One table cell can contain more than one claim. |
| Primary source | The document that first gives the fact: a deliverable PDF, a paper PDF, or a live web page. |
| Secondary source | A file in `handover-pack/` or a `.md` file in the root folder. A secondary source is **not** sufficient. |
| Text file | A file in `deliverables/text/`. It is a search aid. It is not a primary source. |
| Page N | The Nth page of the PDF file, as the PDF viewer shows it in its page box. It is **not** the number printed on the page. |
| Verbatim quote | Words in quotation marks in file A or file B. |
| Negative claim | A claim that says "not stated", "nothing found", "no document", or "no hits". |

Note: Page N in the text file is the Nth block between form-feed characters. On 19 Oct 2026, a comparison of D1.8 p.30, Catalogue p.62 and D2.2 p.33 showed that text page N is equal to PDF page N.

---

## 3. Result codes

Give each claim one result code.

| Code | Meaning | Action |
|---|---|---|
| OK | The source has the claim, at the cited page, with the same words or figures. | No change. |
| PAGE | The source has the claim, but at a different page. | Correct the page in A or B. |
| EDIT | The source has the claim, but the words or figures are different. | Correct the claim. Write the correct text. |
| WRONG | The source does not support the claim. | Remove the claim, or mark it "not supported". |
| SECOND | The claim cites only a secondary source. | Find the primary source. Then give a second code. |
| OPEN | You cannot get the source. | Write why. Do not put the claim in the brief. |

---

## 4. Equipment and sources

### 4.1 Tools

- A PDF viewer with a page box and a text search function.
- The `pdftotext` tool (it is in `/mingw64/bin/`). Use it only to search.
- A web browser. Use it for DOIs, CORDIS, Zenodo and vendor web sites.
- A log file. Make the file `handover-pack/verification-log-A-B.md`.

### 4.2 Primary sources in this repository

Use the PDF with the **descriptive name** (the name that agrees with the text file). Some deliverables have a second PDF with the web-site name. The second PDF can be a different version.

Example: the two D1.6 PDFs have different checksums. The text file is from `deliverables/D1.6 Practice abstracts batch 1.pdf`.

| Short name in A and B | Primary source |
|---|---|
| D1.1, D1.2, D1.4, D1.5, D1.6, D1.8, D2.1, D2.2, D4.3, D6.2, D6.3 | `deliverables/<descriptive name>.pdf` |
| Cat. / Catalogue | `deliverables/AWI Catalogue (final version).pdf` |
| CORDIS listing | `deliverables/CORDIS listing 101060818.pdf` |
| PS-2026 (van Staaveren et al., Poultry Science) | `papers/van Staaveren 2026 PSJ - ChickenCheck footpad and hock burn validation.pdf` |
| BSE-rev (Ramon-Perez et al., Biosystems Engineering) | `papers/Ramon-Perez 2025 BiosystEng - pig welfare technologies at slaughter review.pdf` |
| Agronomy Research 2025 (Banhazi et al., Weight-Detect) | `papers/Banhazi 2025 AgronRes - Weight-Detect sub-clinical respiratory infection.pdf` |
| Animal Frontiers 2025 (Tuyttens et al.) | `papers/Tuyttens 2025 AnimFront - comprehensive animal welfare label framework.pdf` |
| SUIS 207 | `papers/Ramon-Perez 2024 SUIS - sensors and AI for pig welfare, Spanish.pdf` |
| Polskie Drobiarstwo (Siwek, Marchewka) | `papers/Siwek 2023 Polskie Drobiarstwo - poultry welfare in Poland, Polish.pdf` |
| Register | private project notes (available on request) (your own file; use it only for the question numbers) |

### 4.3 Primary sources on the web

| Claim | Primary source |
|---|---|
| "WEL2BE — Participation ended", "BY-NUNASOLUTIONS SL" | CORDIS project page for grant 101060818, participants list (cordis.europa.eu) |
| "NunaSolutions, is a brand of Teknologisk Institute" | The Nuna Solutions web site |
| Pilots page text, "Tear staining system (ILVO)", "Animal Sense (Bitgear, BioSense)" | www.awish-project.eu, pilots page |
| Publication list | www.awish-project.eu/journal-papers/ and /conference-papers/ |
| Zenodo records 17786812, 17630315, 17475673, 17475558, 18549284, 17628730, 17629216, 13969485, 13991423, 17803862 | zenodo.org/records/<number> |
| Figshare 25897855 | doi.org/10.6084/m9.figshare.25897855 |

Caution: Web pages change. For each web claim, save the page as PDF. Write the date and the URL in the log.

---

## 5. Preparation

5.1 Pull the latest version of the repository (`git pull`).

5.2 Make a new branch for the corrections. Example name: `verify-a-b`.

5.3 Make the log file `handover-pack/verification-log-A-B.md`. Use this table:

| File | Row or section | Claim (short) | Cited source and page | Primary source used | Page found | Result code | Correction | Date |
|---|---|---|---|---|---|---|---|---|

5.4 Open file A, file B and the log side by side.

5.5 Do not edit file A or file B before you write the result in the log.

---

## 6. General method for one claim

Use this method for each claim. Sections 7 and 8 tell you which claims to examine.

### 6.1 Verbatim quote

1. Find the cited source in the table in 4.2 or 4.3.
2. Open the PDF at the cited page.
3. Find the quoted words on the page. Use the search function of the viewer.
4. Compare each word, figure, unit and symbol.
5. If the words are not on the cited page, examine the page before and the page after.
6. If the words are not on these three pages, search the full PDF.
7. Write the result code in the log.

Note: The spot-check of 7 Oct 2026 found that page numbers in A can be 1 page incorrect. Thus the code PAGE is possible.

### 6.2 Figure from a paper (kappa, R, r, sensitivity, specificity, accuracy, error)

1. Open the paper PDF.
2. Find the figure in the results section or in the table. Do not use the abstract only.
3. Make sure that the figure is for the same indicator, the same sensor and the same comparison (for example, camera against the median of the human raters).
4. Make sure that the confidence interval, the sample size and the unit agree with file A.
5. Make sure that the caveats in file A are in the paper (for example: "one author is a CLK employee").
6. Write the section or table number in the log.

### 6.3 Figure that a review cites from an older study

File A cites many figures from D2.2 or BSE-rev. These figures come from older studies (for example, Blömke et al. 2020).

1. Make sure that D2.2 or BSE-rev gives the figure. Use 6.1.
2. Make sure that file A marks the figure as "pre-aWISH" or "third-party".
3. If the figure goes into the brief, open the original study by its DOI. Compare the figure.

### 6.4 TRL value

1. Find the source: D2.2 p.19 (pigs), D2.2 p.25 (broilers), or D1.6 pp.9–11.
2. Make sure that the TRL is for the same sensor and the same indicator.
3. For a D2.2 TRL, make sure that file A says "estimated". D2.2 pp.19 and 25 have a disclaimer that the TRLs are estimates.

### 6.5 Vendor or holder name

1. Find each source that file A or B cites for the name.
2. Write the date of each source in the log.
3. Make sure that the newest source gives the name in file A or B.
4. If the claim cites `handover-pack/D` or `handover-pack/F`, give the code SECOND. Then open the primary web source (4.3).

### 6.6 Negative claim ("not stated", "no hits", "nothing found")

A negative claim is easy to make and difficult to prove. Do these steps for each negative claim that goes into the brief.

1. Write down the list of documents that the claim says were checked.
2. Search each text file for the terms. Use the command below. Change the terms for the claim.

```bash
grep -n -i -E "Lesion.?Detect|lung|liver" "deliverables/text/D2.2 Methodology for measuring each AWI.txt"
```

3. Use spelling variants: with and without hyphens, spaces, capital letters and accents. Examples: `ChickenCheck` and `Chicken Check`; `Großfurtner` and `Grossfurtner`; `Batallé` and `Batalle`.
4. Search the PDF also. Tables, figures and slides can be absent from the text file.
5. Look at the pages that are only images. Examples: D1.8 pp.1–13 and D1.2 Annex D (p.49). Text search does not find words in images.
6. If you find the information, give the code WRONG. Write the page.
7. If you do not find the information, give the code OK. Write the search terms in the log.

Caution: Do not quote D5.2 from its OCR text. Quote D5.2 only from the PDF.

---

## 7. Procedure for file A

### 7.1 Select the rows

1. Examine all claims in these rows. These rows carry the main conclusions.

| Rows | Why |
|---|---|
| P3, B10, B11 | The only aWISH-period validation figures. The brief and the register quote them (1.7 %, κ 0.70, κ 0.60). |
| P5, P6, P7, P8, P9, P10, P14, P16 | aWISH pig slaughterhouse sensors. They support the claim "no peer-reviewed validation of any aWISH pig slaughterhouse sensor". |
| B5, B9, B12, B13 | aWISH broiler sensors with "not stated" results. |
| Each other row that goes into the brief | Policy requirement (1.3). |

2. For the remaining rows, examine 1 row in 5. Select the rows before you start. Do not select rows because they look correct. Example: put the remaining row numbers in a list, and select each fifth row.

3. If a sampled row has a result WRONG or EDIT, examine all remaining rows.

### 7.2 Examine each selected row

Do these steps for each cell of the row.

1. **Indicator, species, stage.** Compare with the Catalogue pages and the D2.2 pages in the "Source(s)" column.
2. **Measurement method / sensor (vendor).** Use 6.5.
3. **Automated?** Make sure that the cited page supports "yes", "no" or "partly".
4. **Reported agreement.** Use 6.1, 6.2 or 6.3. For "not stated", use 6.6.
5. **TRL.** Use 6.4.
6. **Source(s).** Make sure that each cited page contains information for this row.

### 7.3 Examine the main conclusions of file A

1. Count the rows in Table 1. File A says 38 rows: 22 pig and 16 broiler.
2. Count the rows that have an agreement figure. File A says 20. Then count the row codes in the list in the same paragraph.
3. Make sure that only P3, B10 and B11 have aWISH-period figures. For each other row with a figure, make sure that the figure is from a pre-aWISH study.
4. Do a new search for aWISH validation papers. The search of 7 Oct 2026 can be out of date. Use these sources:
   - the aWISH journal-papers page and conference-papers page;
   - CORDIS, "Results" for grant 101060818;
   - Zenodo, search "101060818";
   - Google Scholar, search "aWISH" with "slaughterhouse" and "pig".
5. Write each new paper in the log. If a new paper gives a pig slaughterhouse validation figure, the main conclusion is WRONG.

### 7.4 Examine Table 2 (publications)

1. Open each DOI at doi.org.
2. Compare the title, authors, journal, volume, pages and year.
3. Try again to open the Zenodo and figshare records that gave HTTP 429. Use your browser, not an agent.
4. If a record is now open, read it. Look for validation figures. Then change "Opened?" to "Yes" and write the date.

### 7.5 Examine the disagreements D1 to D12

1. For each disagreement, open the two (or more) sources.
2. Make sure that each source says what file A says.
3. Make sure that the disagreement is real. A disagreement is not real if the two sources are about different sensors, indicators or dates.
4. For D4 and D5 ("resolved"), make sure that the resolution has a primary source (4.3). The CORDIS listing file in the repository does not contain "Participation ended" or "NUNASOLUTIONS". Thus you must use the live CORDIS page.

### 7.6 Examine the "Could not find / not stated" list

1. Use 6.6 for items 1, 2, 3 and 7.
2. For item 9, use 7.4 step 3.

---

## 8. Procedure for file B

### 8.1 Select the claims

1. Examine all claims in the per-pilot table (section 1).
2. Examine all claims in the data-arrangements table (section 1b).
3. Examine the chronology (section 2) only where it adds a claim that is not in section 1 or 1b.
4. Examine all 13 contradictions (section 4).

### 8.2 Examine the per-pilot table (section 1)

Do these steps for each pilot (1 to 6).

1. **Slaughterhouse, species, country.** Compare with D1.6 pp.9–11 and D1.8 p.23.
2. **Research co-lead.** Compare with D1.6 pp.9–11 and D1.8 p.23.
3. **Technologies installed.** Use 6.1 for each quote. Use 6.5 for each vendor.
4. **Stage of chain.** Make sure that the cited page gives the location (for example, "gas tunnel", "evisceration line").
5. **Latest installation status.** Write the date of the source. Make sure that the claim does not say "installed" when the source says "will install".
6. **Plan past Oct 2026.** This cell is a negative claim. Use 6.6 with these terms: `after the project`, `end of the project`, `continu`, `sustain`, `maintain`, `2027`, `beyond`.
7. **Throughput, region of extension.** Use 6.1.

### 8.3 Examine the data-arrangements table (section 1b)

1. Open D6.3 p.16. Compare the number of signed Data Sharing Agreements for each pilot (4, 0, 21, 6, 0, 1).
2. Open D6.3 p.8. Make sure that it says "32 signed DSA".
3. Add the six numbers. Make sure that the total agrees with p.8, or write the difference in the log.
4. For each quote from D6.2 and D6.3, use 6.1.
5. Make sure that each quote is for the pilot that file B gives. Some answers in the WP3 annex are not attributed to a pilot (for example D6.3 p.49).
6. Make sure that file B marks the answers that are "GA text" (Pilot 5).

### 8.4 Examine the "not stated" list (section 3)

1. Count the rows that are not struck through. File B says 27. On 19 Oct 2026, a count of the table gave 26 rows that are not struck through. Find the correct number.
2. For each row, use 6.6.
3. For each struck row, make sure that the cited page fills the cell.

### 8.5 Examine the contradictions (section 4)

1. For each contradiction, open each source. Make sure that each source says what file B says.
2. **Contradiction 10 (Batallé or NORFRISA)** has the highest priority. The README says that you must solve it before the sheet goes to a person. Do these steps:
   1. Open D1.4 p.17 in the PDF. Make sure that it names NORFRISA for Pilot 2. (A text search on 19 Oct 2026 found "NORFRISA" on text page 17.)
   2. Open D1.6 p.9, D1.8 p.23, D6.3 p.16 and D6.3 p.52. Make sure that they name Batallé.
   3. Open the live aWISH pilots page. Write which name it gives for Pilot 2.
   4. Open the CORDIS participants list. Write if Selección Batallé, Norfrisa, or both, are participants.
   5. If the sources do not solve the contradiction, put this question in the questions for ILVO: "Which slaughterhouse is the Pilot 2 site: Batallé or NORFRISA?"
   6. Until the contradiction is solved, write "Pilot 2 slaughterhouse: Batallé (D1.6, D1.8, D6.3) or NORFRISA (D1.4); not solved" in each text that goes to a person.
3. **Contradictions 1 and 2** use CORDIS and the Nuna web site. Use 7.5 step 4.

---

## 9. Problems found before the procedure

On 19 Oct 2026, a short examination found these problems. Examine and solve each problem during the procedure.

| # | File | Location | Problem | Action |
|---|---|---|---|---|
| 1 | A | Row-count paragraph after Table 1 | It says "20" rows with a figure, but its list has 21 row codes. The "18" rows without a figure is possibly also incorrect. | Use 7.3 steps 1–2. Correct the numbers. |
| 2 | A | Row P9 | The row gives an ADAL figure, but P9 is not in the list of rows with a figure. Rows P11 and B9 have similar third-party figures and are in the list. | Use one rule for all rows. Then correct the list. |
| 3 | B | Section 3 | It says 27 "not stated" cells. A count found 26. | Use 8.4 step 1. |
| 4 | A, B | Rows P10, P16, B9; contradictions 1, 2 | The claims "Participation ended" and "BY-NUNASOLUTIONS SL" are not in the local CORDIS listing. They cite `handover-pack/D` and `F` (secondary). | Use 7.5 step 4. Save the live CORDIS page as PDF. |
| 5 | A, B | Each citation of the Catalogue, D1.6, D1.8 | Two PDFs exist for some deliverables. They can be different versions. | Use the PDF in 4.2. Write the file name in the log. |
| 6 | Brief | private project notes (available on request) line 203 (the 7 Oct handover brief; the founder brief is `aWISH Founder Brief.md`) | It says file B has "9 contradictions". File B now has 13. | After the procedure, update the brief. |

---

## 10. Completion

10.1 Complete these steps when you have examined all selected claims.

1. Count the result codes in the log. Write the totals at the top of the log.
2. Make the corrections in file A and file B. Mark each correction "[verified 2026-MM-DD]".
3. Do not put a claim with the code WRONG or OPEN into the brief.
4. Update the status of A and B in `handover-pack/README.md`. Write the date and the number of claims examined.
5. Update the facts in `aWISH Founder Brief.md`, in the vault entity notes and in the register (private project notes (available on request)) that come from A or B.
6. Add one line to the AI-use log in `handover-pack/README.md`. Write what the agents did and what you examined.
7. Commit the changes on your branch.

10.2 Sign the attestation only when these conditions are true:

- Each claim in the brief that comes from A or B has the code OK, PAGE or EDIT in the log.
- Each correction is in the file.
- Each web claim has a saved PDF with a date.

---

## 11. Time estimate

| Task | Approximate time |
|---|---|
| Preparation (section 5) | 15 minutes |
| File A, rows in 7.1 step 1 (15 rows) | 3 to 4 hours |
| File A, sample and sections 7.3 to 7.6 | 2 hours |
| File B, sections 8.2 and 8.3 (6 pilots) | 3 hours |
| File B, sections 8.4 and 8.5 | 1.5 hours |
| Completion (section 10) | 1 hour |
