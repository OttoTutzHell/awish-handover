[← Back to README](../README.md) · [Founder Brief (online)](https://ottotutzhell.github.io/awish-handover/founder-brief.html) · [Pack A: Validated sensors](A-what-validated.md) · [Glossary](../GLOSSARY.md)

# B. Per-pilot sheet

aWISH ran six pilots: four slaughterhouses in a first phase and two more in a second phase that served as external validation sites. For each pilot, this pack records what was installed, at which stage of the chain, its last stated status, and what any document says about the time after October 2026. [Pack A](A-what-validated.md) covers how well each technology has been validated.

**Contents:** [In brief](#in-brief) · [1. Per-pilot overview](#1-per-pilot-overview) · [1b. Data arrangements](#1b-data-arrangements-per-pilot) · [2. Chronology](#2-per-pilot-chronology) · [3. Points marked "not stated"](#3-points-marked-not-stated) · [4. Contradictions between documents](#4-contradictions-and-discrepancies-between-documents) · [Appendix: files read](#appendix-files-read)

## In brief

- **Six pilots:** four pig slaughterhouses ([Vion](#pilot-1-vion-groenlo-netherlands-pigs) in the Netherlands, [Batallé](#pilot-2-batallé-catalonia-spain-pigs) in Spain, [Grossfurtner-Higelsberger](#pilot-5-grossfurtner-higelsberger-austria-pigs) in Austria, [Carnex](#pilot-6-carnex-vojvodina-serbia-pigs) in Serbia) and two broiler slaughterhouses (Plukon's [DUC](#pilot-3-duc-plukon-food-group-chailley-france-broilers) in France and [Sieradz](#pilot-4-plukon-sieradz-poland-broilers) in Poland).
- **Nothing public says what happens to any installation after October 2026:** whether the sensors keep running, or who pays for them (§3).
- **The pilot data are mostly closed:**
	- Pilot 1's data stay private on the aWISH data platform.
	- Pilot 2 stops data access at the end of the project.
	- Pilot 3 deletes its data at the end of the project, except ITAVI's acoustic database and model; reports are kept five years.
	- Pilot 6 never answered (§1b).
- **Two vendors changed** from what D1.6 says (§4). Pig stunning effectiveness is now Nuna Solutions' BlinkAI, and tear staining is ILVO's. WEL2BE has left the project, and no one is named for its broiler stunning sensor at Pilot 3.
- **Installations announced for late 2024** at Pilots 5 and 6 are confirmed only for Lesion-Detect at Carnex.

**Method**
- Extraction with citations only.
- No synthesis, and no inference of continuation intent, installation status or payer.

**How to read the citations**
- Page numbers are PDF page numbers.
- Sources are footnotes. D5.2 has no text layer and was read through OCR; its footnotes say so and give the printed page number.
- The deliverables (D1.1, D6.3 and so on) are explained in [Pack A, "The sources"](A-what-validated.md#the-sources), and listed with their dates in the [appendix](#appendix-files-read). Because of copyright restrictions, the deliverables are not uploaded here; download them from the [aWISH project website](https://www.awish-project.eu/) or [CORDIS (grant 101060818)](https://cordis.europa.eu/project/id/101060818).
- D1.4's pilot descriptions are the project website's texts. D1.4 v1.0 was published 30 Apr 2023 and v2.0 on 17 Sep 2024 ("Adaptation of comments by EC")[^d14-3-4], so these texts date from one of the two. They are cited as "website text".
- **Q2, Q4, Q5** refer to the open handoff questions in Section 6 of the [Founder Brief](https://ottotutzhell.github.io/awish-handover/founder-brief.html#handoff):
	- **Q2:** what the 32 Data Sharing Agreements let a third party receive
	- **Q4:** per pilot, whether the kit stays running after October 2026, who pays, and named contact
	- **Q5:** research or nonprofit licence terms per vendor

---

## 1. Per-pilot overview

| Pilot | Slaughterhouse (country) | Species | Phase | Scientific co-lead | New technologies (vendor) |
|---|---|---|---|---|---|
| [1](#pilot-1-vion-groenlo-netherlands-pigs) | Vion, Groenlo (NL) | Pigs | 1st | Utrecht University | PigInspector (CLK); STREMODO and IGF-BP blood assay (FBN) |
| [2](#pilot-2-batallé-catalonia-spain-pigs) | Batallé, Catalonia (ES) | Pigs | 1st | UAB | Stunning effectiveness (Nuna Solutions, listed as WEL2BE); tear staining (ILVO, listed as WEL2BE); Lesion-Detect, Weight-Detect, Enviro-Detect (InnoTech Vision) |
| [3](#pilot-3-duc-plukon-food-group-chailley-france-broilers) | DUC (Plukon Food Group), Chailley (FR) | Broilers | 1st | Itavi | Broiler stunning (WEL2BE); ChickenCheck Footpad and Hockburn (CLK); EBroilerTrack Sound and Image, EBENE app, transport sensors (Itavi) |
| [4](#pilot-4-plukon-sieradz-poland-broilers) | Plukon, Sieradz (PL) | Broilers | 1st | IGBZ PAN | ChickenCheck Footpad, Hockburn, Catch Damage, Scratch (CLK); EBENE app (Itavi) |
| [5](#pilot-5-grossfurtner-higelsberger-austria-pigs) | Grossfurtner-Higelsberger (AT) | Pigs | 2nd | VetMedUni Vienna | PigInspector (CLK); stunning effectiveness and tear staining planned |
| [6](#pilot-6-carnex-vojvodina-serbia-pigs) | Carnex, Vojvodina (RS) | Pigs | 2nd | BioSense Institute | Animal Sense (Bit Gear); STREMODO, Lesion-Detect, Enviro-Detect planned |

Phase: D1.8[^d18-23]. The details and sources for every cell are in the pilot sections below.

### Pilot 1: Vion, Groenlo (Netherlands, pigs)

**Slaughterhouse and leads**
- Vion, Groenlo, the Netherlands[^d16-9]
- Pilot lead: Vion[^d18-23]
- Scientific co-lead: Utrecht University[^d16-9-d18-23]

**Technologies installed**
- New in aWISH, per D1.6:[^d16-9]
	1. PigInspector (CLK), TRL 5: tail length and skin, ear and tail lesions on carcasses, with 2D and 3D colour cameras
	2. IGF-BP blood analysis as a stress indicator (FBN), TRL 3
	3. STREMODO (FBN), TRL 5, in the unloading and lairage area
- D1.8 lists seven technologies:[^d18-25]
	- AI4Animals (Deloitte): animal treatment
	- STREMODO (FBN): stress vocalisations
	- IGFBPs (FBN): stress level in exsanguination blood
	- AUTOFOM3 (Carometec): backfat and muscle depth across the carcass
	- PigInspector (CLK): ear, tail and skin lesions
	- Tail Length (VION)
	- CGM insertion probe: backfat and muscle depth
- D1.8 labels two of them "other technologies":[^d18-28]
	- Tail Length (VION): two 3D cameras after the first flame oven
	- AI4Animals (Deloitte, Vion): an algorithm on CCTV footage of the unloading area

**Technologies at each stage of the chain**
- Unloading: AI4Animals
- Lairage and unloading: STREMODO
- Bleeding: IGF-BP in exsanguination blood
- Processing / post-mortem: PigInspector, Tail Length, AutoFOM3, CGM probe
- Farm, loading, transport: none named

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-27] PigInspector's measuring algorithm "still under development"
- D1.8 (5 Sep 2025):[^d18-26] STREMODO hangs above the unloading and lairage area
- D1.6 (Sep 2024):[^d16-9] the three new technologies "were implemented"
- D1.4 (website text):[^d14-16] already installed: cameras in the unloading and lairage area, the AutoFOM3 carcass scanner, and tail-length cameras with RFID carcass tracking. CLK and FBN measurements were to be added.

**After October 2026**
- Installations: not stated
- Data: kept private on the aWISH data platform.[^d63-44] See §1b.

**Throughput and region**
- Throughput: not stated
- Region: Gelderland, extending to the rest of the Netherlands and to Germany[^d18-24-d14-16]

**Open questions (Founder Brief §6):** Q4; Q5 (vendors CLK, FBN); Q2.

### Pilot 2: Batallé, Catalonia (Spain, pigs)

**Slaughterhouse and leads**
- Batallé, Catalonia, Spain[^d16-9]
- D1.4 names NORFRISA (Frigoríficos del Nordeste S.A.) instead.[^d14-17] **[unverified]**[^new] Norfrisa is a pig slaughterhouse of the Batallé group, in Girona; see §4 item 10.
- Pilot lead: Batallé[^d18-23]
- Scientific co-lead: Autonomous University of Barcelona (UAB)[^d16-9]. D1.8 prints "Wet. H.: UAB" where the other pilots print "Sci. lead".[^d18-23]
- Data management: the project's technical manager and the data protection manager at Selección Batallé (roles only)[^d63-52]

**Technologies installed**
- Per D1.6, three at the slaughterhouse and two on farm:[^d16-9]
	- Stunning effectiveness, TRL 5: checks the corneal reflex in the gas tunnel. D1.6 lists it as WEL2BE's; it is now Nuna Solutions' BlinkAI (a DTI/DMRI brand).[^d18-30-cat-62] WEL2BE's participation has ended.[^cordis]
	- Tear-staining camera, TRL 3. D1.6 lists it as WEL2BE's; D1.8 as ILVO's.[^d18-30]
	- Lesion-Detect (InnoTech Vision), TRL 3: lung and liver lesions at the evisceration line
	- On farm: Enviro-Detect, TRL 7 (barn temperature, humidity, ammonia, dust and CO2), and Weight-Detect, TRL 7
- A Tail Length prototype (UAB and Batallé, 2D camera) appears only in the Catalogue (contradiction 5).[^cat-57]
- D1.4 (website text) names Wel2be and InnoTech Vision.[^d14-17]

**Stage of chain**
- Farm: Enviro-Detect, Weight-Detect
- Stunning (gas tunnel): stunning-effectiveness sensor
- Post-mortem: Lesion-Detect at the evisceration line; the tear-staining camera's location is not stated
- Loading, transport, lairage: none named

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-23] listed as a first-phase pilot; no installation status
- D1.6 (Sep 2024):[^d16-9] "were installed"

**After October 2026**
- Installations: not stated
- Data: access restricted and stopped at the end of the project.[^d63-46] See §1b.

**Throughput and region**
- Throughput: not stated for Batallé. D1.4 gives 10,000 pigs a day for NORFRISA (contradiction 10).[^d14-17]
- Region: Catalonia, extending to the rest of Spain[^d14-17]

**Open questions (Founder Brief §6):** Q4; Q5 (Nuna Solutions, InnoTech Vision; ILVO for tear staining); Q2.

### Pilot 3: DUC (Plukon Food Group), Chailley (France, broilers)

**Slaughterhouse and leads**
- DUC (Plukon Food Group), Chailley, France[^d16-10]
- Pilot lead: Plukon – Duc[^d18-23]
- Scientific co-lead: Itavi[^d16-10-d18-23]
- Data management: Plukon, which must validate all data access[^d63-47-52]

**Technologies installed**
- Per D1.6, three at the slaughterhouse, two on farm and one for transport:[^d16-10]
	- Stunning effectiveness (WEL2BE), TRL 3: a camera at the gas-tunnel exit that monitors movement in the crates
	- ChickenCheck Footpad and ChickenCheck Hockburn (CLK), TRL 9
	- EBroilerTrack Sound (Itavi), TRL 5, in the lairage area
	- On farm: EBENE app, TRL 9, and EBroilerTrack Image, TRL 5 (Itavi)
	- Transport Monitoring Sensors (Itavi): temperature, humidity and CO2 in the crates
- **Broiler stunning sensor holder:** WEL2BE's participation has ended, and no document names a later holder. D1.8 and the Catalogue name Nuna Solutions only for pig stunning.[^d18-30-cat-62]
- D1.4 (website text) names CLK, Itavi and Wel2be.[^d14-18]

**Stage of chain**
- Farm: EBENE, EBroilerTrack Image
- Transport: Transport Monitoring Sensors
- Lairage: EBroilerTrack Sound
- Stunning: stunning-effectiveness sensor at the gas-tunnel exit
- Post-mortem: ChickenCheck
- Loading: none named
- Already in place: cameras in the unloading, lairage, stunning, bleeding and scalding-entrance areas[^d14-18]

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-23] listed as a first-phase pilot; no installation status
- D1.6 (Sep 2024):[^d16-10] "were implemented"

**After October 2026**
- Installations: not stated
- Data: ITAVI keeps its labelled acoustic database and model, to be enriched after the project. The other data (EBENE evaluations, videos, raw sound, transport monitoring) are deleted at the end. Images are kept 28 days, reports five years.[^d63-53] See §1b.

**Throughput and region**
- Throughput: 12,000 birds an hour (line speed)[^ps26-2]
- Region: Chailley, Yonne, extending to France, the Netherlands, Germany, Belgium, Poland and Bulgaria[^d14-18]

**Open questions (Founder Brief §6):** Q4; Q5 (CLK, Itavi; no holder of the broiler stunning sensor after WEL2BE); Q2.

### Pilot 4: Plukon, Sieradz (Poland, broilers)

**Slaughterhouse and leads**
- Plukon, Sieradz, Poland[^d16-10]
- Pilot lead: Plukon – Sieradz[^d18-23]
- Scientific co-lead: IGBZ PAN[^d16-10-d18-23]

**Technologies installed**
- All new technologies are CLK's, installed after the plucking phase, where each chicken is evaluated in real time:[^d16-10]
	- ChickenCheck Footpad and ChickenCheck Hockburn, TRL 9
	- ChickenCheck Catch Damage, TRL 7: wings, being extended to breast and legs
	- ChickenCheck Scratch, TRL 4: scratches on the back
- On farm: welfare assessments of selected flocks with Itavi's EBENE app, TRL 9[^d16-10]
- D1.4 (website text) names CLK, Itavi and Wel2be; D1.6 does not name WEL2BE for Pilot 4 (contradiction 11).[^d14-19]

**Stage of chain**
- Farm: EBENE, selected flocks
- Post-mortem: ChickenCheck, after plucking
- Loading, transport, lairage, stunning: none named
- Already in place: cameras in the unloading, lairage, stunning, bleeding and scalding-entrance areas[^d14-19]

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-23] listed as a first-phase pilot only
- D1.6 (Sep 2024):[^d16-10] installed after the plucking phase. Pilots 3 and 4 serve as external validators for each other.

**After October 2026**
- Installations: not stated
- Data: images are kept 28 days, reports five years.[^d63-53] See §1b.

**Throughput and region**
- Throughput: 15,000 birds an hour (line speed)[^ps26-2]
- Region: Sieradz, extending to France, the Netherlands, Germany, Belgium and Poland[^d14-19]

**Open questions (Founder Brief §6):** Q4; Q5 (CLK, Itavi); Q2.

### Pilot 5: Grossfurtner-Higelsberger (Austria, pigs)

**Slaughterhouse and leads**
- Grossfurtner-Higelsberger GmbH, Austria[^d16-11]: Higelsberger GmbH, part of the Großfurtner group, runs a slaughterhouse and cutting plant in Schwertzberg, Upper Austria[^d14-20]
- Pilot lead: Großfurtner-Higelsberger[^d18-23]
- Scientific co-lead: VetMedUni Vienna[^d16-11-d18-23]

**Technologies installed**
- A second-phase pilot, installed a year after the first phase, for wider coverage and external validation:[^d16-11]
	- PigInspector (CLK), TRL 5: already installed
	- Planned from the second half of 2024, as in Pilot 2: stunning effectiveness, TRL 5, and tear staining, TRL 3. D1.6 lists both as WEL2BE's; they are now Nuna Solutions' and ILVO's (see Pilot 2).
- D1.4 (website text) names CLK and Wel2be.[^d14-20]

**Stage of chain**
- Post-mortem: PigInspector
- Stunning: planned
- Farm, loading, transport, lairage: none named

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-23] listed as a second-phase pilot only. Whether the stunning and tear-staining sensors were installed is not stated.
- D6.3 (Oct 2024): no installation statement. Pilot 5's answers are based on the Grant Agreement.[^d63-44]
- D1.6 (Sep 2024, possibly April 2024 text; contradiction 9):[^d16-11] PigInspector already installed; the WEL2BE sensors to be installed from the second half of 2024

**After October 2026**
- Installations: not stated
- Data: D6.3's Pilot 5 answer, that results will stay "accessible for the long-term", is Grant Agreement text, not a pilot arrangement.[^d63-51] See §1b.

**Throughput and region**
- Throughput: 5,500 pigs a week[^d14-20]
- Region: Upper Austria, extending to the rest of Austria[^d14-20]

**Open questions (Founder Brief §6):** Q4; Q5 (CLK, Nuna Solutions; ILVO for tear staining); Q2.

### Pilot 6: Carnex, Vojvodina (Serbia, pigs)

**Slaughterhouse and leads**
- Carnex, Vojvodina, Serbia[^d16-11]
- Pilot lead: Carnex[^d18-23]
- Scientific co-lead: BioSense Institute[^d16-11-d18-23], which also hosts the project website[^d11-16-d12-16]

**Technologies installed**
- A second-phase pilot validating three technologies from Pilots 1 and 2, to be installed by the end of 2024:[^d16-11]
	- STREMODO (FBN), TRL 5, in the lairage area
	- Lesion-Detect (InnoTech Vision), TRL 3, at the evisceration line
	- Enviro-Detect (InnoTech Vision), TRL 7, on farm
- Already present: Animal Sense (Bit Gear), TRL 8, measuring barn climate (temperature, humidity, ammonia), silo feed level and feed consumption. With BioSense it is to be extended with a sensor for pig behaviour in the pen.[^d16-11]
- D1.4 calls the farm system PigSense, by BioSense (BitGear), running on three and potentially four farms (contradiction 12).[^d14-21]

**Stage of chain**
- Farm: Animal Sense; Enviro-Detect planned
- Lairage: STREMODO planned
- Post-mortem: Lesion-Detect at the evisceration line, installed in Serbia in late 2024 and tested on 228 lungs[^ar26-3-14]
- Loading, transport, stunning: none named

**Installation status, latest first**
- D1.8 (5 Sep 2025):[^d18-23] listed as a second-phase pilot only. Whether the planned installations were completed is not stated.
- D1.6 (Sep 2024):[^d16-11] Animal Sense in place; the other three to be completed by the end of 2024

**After October 2026**
- Installations: not stated
- Data: Pilot 6 had not answered D6.3's questions.[^d63-44] See §1b.

**Throughput and region**
- Slaughterhouse throughput: not stated
- Farms: three, potentially four[^d14-21]
- Region: Vojvodina, extending to the rest of Serbia[^d14-21]

**Open questions (Founder Brief §6):** Q4; Q5 (FBN, InnoTech Vision, Bit Gear); Q2.

### Statements that apply to all pilots

- Six broiler and pig production chains, in France, Poland, Spain, the Netherlands, Austria and Serbia[^d11-2-d12-2]
- Contacts: none named. The project website's pilots page is described as holding each pilot's contact details.[^d11-17-d12-17]
- D1.8: "Trainings and testing by 20 focus companies / pilot", with no pilot-specific detail.[^d18-33]
- The Best Practice Guides stay available via the project website and feedback tools after the project.[^d43-9] BioSense hosts the website and will maintain it after aWISH.[^d11-16-d12-16] Neither statement concerns the installations.
- No document read says anything about any installation, arrangement or payment after 31 Oct 2026.
- D1.4 carries one website description per pilot.[^d14-16-21] D1.5 has no pilot content. D6.2 and D6.3 cover data only (§1b).

---

## 1b. Data arrangements per pilot 

D6.3 is the second and latest data management plan. Its WP3 (pilots) annex answers pilot by pilot, to the EC template's questions.[^d63-41-54] "GA text" means the document marks the answer as taken or adapted from the Grant Agreement. Where D6.3 does not name a pilot, the cell reads "not stated". The earlier plan, D6.2 (Apr 2023), is summarised below the table.

| Pilot | Signed Data Sharing Agreements[^d63-16] | Openness | Access after the project, retention | Other pilot-specific facts |
|---|---|---|---|---|
| 1 (Vion) | 4 | Private, on the aWISH data platform, because of data-sharing limitations[^d63-44] | Not stated for Pilot 1. The platform-level (WP4) answer applies: data stay available but not findable, for a period set by "cloud storage cost"[^d63-60] | • Data owned by the farmer or Vion[^d63-41]<br>• Embargo: 2 years if necessary[^d63-46]<br>• Access depends on the data and who owns them[^d63-46]<br>• All focus companies have signed data sharing agreements[^d63-54]<br>• Farmer-owned data need a legal arrangement before use[^d63-54] |
| 2 (Batallé) | 0 | • Open to the partners in the task (equipment provider and scientific leader), closed to other partners[^d63-44]<br>• All datasets confidential to stakeholders outside the project[^d63-42] | • Access restricted and stopped after the project.[^d63-46] D6.2 gave this as what Pilot 2 "believes".[^d62-56]<br>• Not usable by third parties in general; "with a previous study", permission for some datasets[^d63-51] | • Data in the aWISH repository, managed by Ubitech (WP4)[^d63-45]<br>• Repository arrangements to be made "in few weeks"[^d63-45]<br>• Can create vocabularies if needed[^d63-49]<br>• Data management: the project's technical manager and the data protection manager at Selección Batallé[^d63-52] |
| 3 (DUC / Plukon) | 21 | • Only anonymised data can be shared, because data can hold confidential information[^d63-44]<br>• Not publicly available, metadata included[^d63-46-47-50] | • ITAVI keeps its labelled acoustic database and model, to be enriched after the project. The other data (EBENE evaluations, videos, raw sound, transport monitoring) are deleted at the end. Images are kept 28 days, reports five years.[^d63-53]<br>• Reuse after validation by Plukon and ITAVI[^d63-51]<br>• "After the end of the project, data will not be accessed": a WP3 answer that follows a Pilot 3 sentence but names no pilot[^d63-49] | • Plukon must validate all data access[^d63-47] and other sharing, such as economic data[^d63-45]<br>• .csv files by email; valuable data to the aWISH platform; raw training data kept by ITAVI on hard drives or laptops[^d63-45]<br>• Code to go into the acoustic-monitoring and EBENE software, not into transport heat-stress modelling or EBroilerTrack Image[^d63-48]<br>• Data management: Plukon. Costs: the Horizon Europe grant[^d63-52]<br>• Only anonymous data can be used[^d63-54] |
| 4 (Plukon Sieradz) | 6 | Only anonymised data can be shared, because data can hold confidential information[^d63-44] | Images kept 28 days, reports five years[^d63-53] | • Image file names carry a timestamp, rating and flock number[^d63-42]<br>• .csv files by email suggested[^d63-45]<br>• Back-ups and firewalls in place[^d63-53] |
| 5 (Grossfurtner-Higelsberger) | 0 (second-phase pilot) | GA text, not a pilot decision: documents mainly open; datasets open if possible; the companies' commercial code and algorithms protected[^d63-44] | • GA text: results in papers with data linked in a repository; dissemination material open access (CC-0, BY or BY NC); main results "accessible for the long-term"[^d63-51]<br>• Embargo: none from Vetmed's side, but to be discussed with the technology providers[^d63-46] | • Datasets, ownership, restrictions and contacts to be specified in the next DMP[^d63-42]<br>• Vetmed receives a €3,500 dissemination fee, covering open-access publication and conference fees. Other FAIR-data costs "need to be defined by WP4/UBI (central data platform)".[^d63-52]<br>• Data ownership, anonymisation of farm data and the technology providers' sharing of algorithms still need work, for the next DMP[^d63-54] |
| 6 (Carnex) | 1 (second-phase pilot) | No answer yet[^d63-44] | Not stated | • New data will come from newly installed equipment[^d63-41]<br>• "yet to be determined"[^d63-42] |

**WP3-wide statements in D6.3 that name no pilot**
- At least a report of the data analysis should be open; individual data most likely not.[^d63-44]
- How access will be provided, with restrictions, during and after the project: "Not discussed yet".[^d63-46]
- Outputs will in general not be open to the public domain; licensing can be studied case by case.[^d63-51]
- A Data Transfer Agreement between all partners in each pilot "needs to be considered".[^d63-54]
- 32 signed data sharing agreements and 2 ethical approval documents,[^d63-8] held by the coordinator, ILVO[^d63-16]

**The earlier plan, D6.2 (Apr 2023).** Its WP3 annex is largely "To be determined".[^d62-50-63] It names only Pilot 2, plus Pilot 1 once. Most of it reappears in D6.3, and its dataset list is in the chronology (§2).[^d62-91-93] Only in D6.2:
- Pilot 1: nothing beyond data ownership by the farmer or Vion,[^d62-52] which D6.3 repeats[^d63-41]
- Pilot 2:
	- Datasets confidential outside the project, usable by the project's scientific teams.[^d62-53] D6.3 repeats this as Pilot 2's answer.[^d63-42]
	- Documentation provided at the request of the coordinator or the WP leader[^d62-59]
	- Data management: the project manager and the data protection manager at Selección Batallé. Security: firewall and backup copies.[^d62-62]
	- Data volumes: 0.001 GB a day per sensor (stunning, tear staining, lung and liver), or 1, 2 and 4 GB a day with image collection[^d62-52]
	- Other procedures: none[^d62-63]
- Pilot 5: not named. Unattributed answers reappear in D6.3 as Pilot 5's: observational data processed by the technology partners and Vetmed,[^d62-52] and Vetmed's €3,500 dissemination fee.[^d62-61] D6.2 does not state the attribution.
- Pilots 3, 4 and 6: not named.

---

## 2. Per-pilot chronology 

What each deliverable says about each pilot, oldest first. Dates: D6.2 Apr 2023 · D1.4 Apr 2023 or Sep 2024 (website text) · D1.1 and D1.6 Sep 2024 (D1.6 v1.0 Apr 2024) · D1.2, D4.3, D5.2 and D6.3 Oct 2024 · D1.8 slides 5 Sep 2025. D1.5 (May 2023) has no pilot content.

### Pilot 1 — Vion, Groenlo
- D6.2 (Apr 2023):
	- data owned by the farmer or Vion[^d62-52]
	- datasets for carcass composition and stress behaviour,[^d62-91] PigInspector[^d62-92] and InnoTech development data[^d62-93]
- D1.4 (website text): unloading and lairage cameras, the AutoFOM3 scanner and tail-length cameras already installed; CLK and FBN to add more[^d14-16]
- D1.6 (Sep 2024): PigInspector (TRL 5), IGF-BP analysis (TRL 3) and STREMODO (TRL 5) implemented[^d16-9]
- D1.2 (Oct 2024): the third newsletter covered Pilots 1, 2 and 5,[^d12-22] but its content is an image and cannot be read[^d12-49]
- D6.3 (Oct 2024):
	- 4 signed data sharing agreements[^d63-16]
	- data private on the aWISH platform[^d63-44]
	- agreements signed by all focus companies[^d63-54]
	- data owned by the farmer or Vion[^d63-41]
- D1.8 (5 Sep 2025):
	- first-phase pilot, led by Vion, scientific lead UU[^d18-23]
	- region: Gelderland, extending to the rest of the Netherlands and Germany[^d18-24]
	- seven technologies, adding AI4Animals, AUTOFOM3, Tail Length (VION) and a CGM probe[^d18-25]
	- PigInspector's algorithm "still under development"[^d18-27]
	- Tail Length (VION) and AI4Animals labelled "other technologies"[^d18-28]
- Nothing in D1.1 beyond the country code (NL),[^d11-2] D4.3 or D5.2.

### Pilot 2 — Batallé
- D6.2 (Apr 2023):
	- datasets "Pilot2_W2B1 CET'automatique" and "Pilot2_W2B2 tear-staining", both vision systems dated 16 Mar 2023,[^d62-92] and InnoTech weight and environmental data[^d62-93]
	- Pilot 2 "believes" access will be restricted and stopped after the project[^d62-56]
	- data volumes per sensor[^d62-52]
	- data-management roles at Selección Batallé[^d62-62]
- D1.4 (website text): names NORFRISA (10,000 pigs a day), not Batallé, with Wel2be and InnoTech Vision as technology providers[^d14-17]
- D1.6 (Sep 2024): five technologies installed[^d16-9]
	- stunning effectiveness (TRL 5) and tear staining (TRL 3), both listed as WEL2BE's. Later documents name other vendors (§4 items 1 and 2).
	- Lesion-Detect (TRL 3) at the evisceration line
	- Enviro-Detect and Weight-Detect (TRL 7) on farm
- D1.2 (Oct 2024): the third newsletter covered Pilot 2; content not readable[^d12-22]
- D6.3 (Oct 2024):
	- 0 signed data sharing agreements[^d63-16]
	- data open only to the task's partners[^d63-44]
	- access restricted and stopped after the project[^d63-46]
	- not usable by third parties in general[^d63-51]
	- repository arrangements "in few weeks"[^d63-45]
- D1.8 (5 Sep 2025):
	- first-phase pilot, led by Batallé, "Wet. H.: UAB"; no installation statement[^d18-23]
	- stunning effectiveness credited to Nuna Solutions, tear staining to ILVO[^d18-30]
- Catalogue (Sep 2026, the latest document): Tail Length prototype by UAB and Batallé, 2D camera[^cat-57]
- Nothing in D1.1 beyond the country code (ES),[^d11-2] D4.3 or D5.2.

### Pilot 3 — DUC (Plukon Food Group), Chailley
- D6.2 (Apr 2023): datasets for footpad lesions, hock burns and the stunning vision system (16 Mar 2023).[^d62-92] No Pilot 3 answer in the WP3 annex.
- D1.4 (website text): cameras already in the unloading, lairage, stunning, bleeding and scalding-entrance areas; CLK, ITAVI and Wel2be to add footpad and hock-burn cameras and sound and motion measurements[^d14-18]
- D1.6 (Sep 2024): six technologies implemented[^d16-10]
	- WEL2BE stunning effectiveness (TRL 3) at the gas-tunnel exit
	- ChickenCheck Footpad and Hockburn (TRL 9)
	- EBroilerTrack Sound (TRL 5) in lairage
	- EBENE app (TRL 9) and EBroilerTrack Image (TRL 5) on farm
	- Transport Monitoring Sensors
- D1.2 (Oct 2024): not mentioned; the third newsletter covered Pilots 1, 2 and 5 only[^d12-22]
- D6.3 (Oct 2024):
	- 21 signed data sharing agreements[^d63-16]
	- only anonymised data can be shared[^d63-44]
	- Plukon validates all data access[^d63-47]
	- ITAVI keeps its acoustic database; other data deleted at the end; images kept 28 days, reports five years[^d63-53]
- D1.8 (5 Sep 2025): first-phase pilot, led by Plukon – Duc, scientific lead ITAVI; no installation statement.[^d18-23] WEL2BE is not named, and no later holder of the broiler stunning sensor is.
- Nothing in D1.1 beyond the country code (FR),[^d11-2] D4.3 or D5.2.

### Pilot 4 — Plukon, Sieradz
- D6.2 (Apr 2023): datasets for footpad lesions and hock burns,[^d62-91] catch damage[^d62-92] and ChickenCheck Scratch.[^d62-93] No Pilot 4 answer in the WP3 annex.
- D1.4 (website text): cameras already in place from unloading to the scalding entrance; CLK and Wel2be to add footpad, hock-burn and catch-damage cameras; technologies installed from Itavi, Wel2be and CLK[^d14-19]
- D1.6 (Sep 2024): all new technologies are CLK's, installed after plucking[^d16-10]
	- ChickenCheck Footpad and Hockburn (TRL 9)
	- Catch Damage (TRL 7), being extended to breast and legs
	- Scratch (TRL 4)
	- EBENE app on farm for selected flocks
	- Pilots 3 and 4 validate each other
- D1.2 (Oct 2024): not mentioned. It notes Poland is "notably underrepresented" in communications, which is about outreach, not the pilot.[^d12-41]
- D6.3 (Oct 2024):
	- 6 signed data sharing agreements[^d63-16]
	- only anonymised data can be shared[^d63-44]
	- images kept 28 days, reports five years[^d63-53]
- D1.8 (5 Sep 2025): first-phase pilot, led by Plukon – Sieradz, scientific lead IGBZ PAN; no installation statement[^d18-23]
- Nothing in D1.1 beyond the country code (PL),[^d11-2] D4.3 or D5.2.

### Pilot 5 — Grossfurtner-Higelsberger
- D6.2 (Apr 2023): dataset "Pilot5_GROSS1 PigInspector".[^d62-93] Answers that D6.3 later labels as Pilot 5's appear here unattributed.[^d62-52-61]
- D1.4 (website text): Higelsberger GmbH, part of the Großfurtner group, in Schwertzberg, Upper Austria; 5,500 pigs a week; CLK and Wel2be technologies to be installed[^d14-20]
- D1.6 (Sep 2024): second-phase pilot[^d16-11]
	- PigInspector (TRL 5) already installed
	- WEL2BE stunning effectiveness (TRL 5) and tear staining (TRL 3) to follow from the second half of 2024
- D1.2 (Oct 2024): the third newsletter covered Pilot 5; content not readable[^d12-22]
- D6.3 (Oct 2024): no installation statement
	- 0 signed data sharing agreements; second-phase pilot[^d63-16]
	- answers based on the Grant Agreement[^d63-44]
	- no embargo from Vetmed's side, but to be discussed with the technology providers[^d63-46]
	- GA text: main results "accessible for the long-term"[^d63-51]
	- the technology providers' sharing of algorithms still to be worked out[^d63-54]
- D1.8 (5 Sep 2025): second-phase pilot, led by Großfurtner-Higelsberger, scientific lead Vetmeduni.[^d18-23] Whether the stunning and tear-staining sensors were installed is not stated.
- Nothing in D1.1 beyond the country code (AT),[^d11-2] D4.3 or D5.2.

### Pilot 6 — Carnex, Vojvodina
- D6.2 (Apr 2023): dataset "Pilot6_FBN1 … Stress behaviour".[^d62-93] No Pilot 6 answer in the WP3 annex.
- D1.4 (website text): PigSense, by Carnex with BioSense (BitGear), measures farm environment and feed use on three, potentially four, farms; FBN and InnoTech Vision named as new technology providers[^d14-21]
- D1.6 (Sep 2024): second-phase pilot[^d16-11]
	- STREMODO (TRL 5), Lesion-Detect (TRL 3) and Enviro-Detect (TRL 7) to be installed by the end of 2024
	- Bit Gear's Animal Sense (TRL 8) already in place, to be extended with a pig-behaviour sensor with BioSense
- D1.2 (Oct 2024): not mentioned. It notes Serbia is "notably underrepresented" in communications, which is about outreach, not the pilot.[^d12-41]
- D6.3 (Oct 2024): no installation statement
	- 1 signed data sharing agreement; second-phase pilot[^d63-16]
	- "No answer yet"[^d63-44]
	- "yet to be determined"[^d63-42]
	- new data expected from newly installed equipment[^d63-41]
- D1.8 (5 Sep 2025): second-phase pilot, led by Carnex, scientific lead Biosense.[^d18-23] Whether the end-2024 installations were completed is not stated.
- Nothing in D1.1 beyond the country code (RS),[^d11-2] D4.3 or D5.2.

---

## 3. Points marked "not stated"

| Pilot | Point | Note |
|---|---|---|
| 1 | After October 2026 (installations) | Data-only statements in §1b |
| 1 | Throughput | — |
| 1 | Stage: farm, loading, transport | — |
| 2 | After October 2026 (installations) | Data access stops at the end of the project[^d63-46] |
| 2 | Throughput (Batallé) | D1.4 gives 10,000 pigs a day for NORFRISA (contradiction 10)[^d14-17] |
| 2 | Installation status after Sep 2024 | D1.8 lists the pilot only[^d18-23] |
| 2 | Stage: loading, transport, lairage | — |
| 3 | After October 2026 (installations) | Data: ITAVI keeps its acoustic database; other data deleted[^d63-53] |
| 3 | Installation status after Sep 2024 | D1.8 lists the pilot only[^d18-23] |
| 3 | Holder of the broiler stunning sensor after WEL2BE | — |
| 4 | After October 2026 (installations) | Data: images 28 days, reports five years[^d63-53] |
| 4 | Installation status after Sep 2024 | D1.8 lists the pilot only[^d18-23] |
| 4 | Stage: loading, transport, lairage, stunning | — |
| 5 | After October 2026 (installations) | D6.3's Pilot 5 answer is Grant Agreement text[^d63-51] |
| 5 | Whether the stunning and tear-staining sensors were installed | Planned from the second half of 2024[^d16-11]; no later document confirms |
| 5 | Stage: farm, loading, transport, lairage | — |
| 6 | After October 2026 (installations) | No answer from Pilot 6 in D6.3[^d63-44] |
| 6 | Throughput (slaughterhouse) | Farm side: three, potentially four farms[^d14-21] |
| 6 | Whether STREMODO and Enviro-Detect were installed | Expected by the end of 2024[^d16-11]; no later document confirms. Lesion-Detect was installed in late 2024[^ar26-3-14] |
| 6 | Stage: loading, transport, stunning | — |
| all | Named contact | Not recorded. The website pilots page is described as holding contact details[^d11-17-d12-17] |
| all | Who pays for any installation after October | No payer named. Pilot 5's FAIR-data costs "need to be defined by WP4/UBI"[^d63-52]; platform retention depends on "cloud storage cost"[^d63-60] |
| all | D6.2 pilot-specific data statements for Pilots 3–6 | D6.2 names only Pilot 2, and Pilot 1 once[^d62-52] |
| all | D6.3 post-project data access for Pilots 1, 5, 6 | Pilot 1: platform-level answer only; Pilot 5: Grant Agreement text; Pilot 6: no answer |

Total "not stated" points: 24.

---

## 4. Contradictions and discrepancies between documents

1. **Stunning-effectiveness vendor: Nuna Solutions for pigs; open for broilers.**
	- D1.6 attributes the pig and broiler stunning-effectiveness sensors to WEL2BE[^d16-9-10-11]. So do D1.4[^d14-17-20] and D6.2[^d62-92] ("Pilot2_W2B1 CET'automatique"; "Pilot3_W2B1 Stunning"), both 2023 texts.
	- D1.8[^d18-30] (slide, 5 Sep 2025) lists "Stunning effectiveness (Nuna solutions)".
	- AWI Catalogue (Sep 2026):[^cat-62] "BlinkAI … Technology under development within the aWISH project to monitor the stunning effectiveness … Provider nunaSolutions … Technology used in aWISH project".
	- CORDIS: "WEL2BE — Participation ended | France".[^cordis]
	- **[unverified]**[^new] CORDIS also lists BY-NUNASOLUTIONS SL (Spain) among the participants.[^cordis-p]
	- Nuna Solutions' own site: "NunaSolutions, is a brand of Teknologisk Institute",[^packf-6] i.e. the Danish Technological Institute / DMRI.
	- **Conclusion:** the pig stunning-effectiveness sensor is Nuna Solutions' BlinkAI (a DTI/DMRI brand). WEL2BE is the earlier participant listed in D1.6, whose participation has since ended.
	- Not stated in any document read: the terms of any handover between WEL2BE and Nuna Solutions.
	- The **broiler** stunning sensor at Pilot 3 is attributed to WEL2BE only[^d16-10]. No document names a successor holder for it.
2. **Tear-staining vendor: ILVO.**
	- D1.6:[^d16-9-11] "WEL2BE, TRL 3". D6.2:[^d62-92] "Pilot2_W2B2 tear-staining" (2023).
	- D1.8:[^d18-30] "Tear staining (ILVO)".
	- Catalogue:[^cat-88] "Tear staining aWISH … Provider aWISH partners … in the development phase (accessed 21 August 2026)".
	- Project website pilots page: "Tear staining system (ILVO)".[^web-pilots]
	- **Conclusion:** tear staining is ILVO's[^d18-30-cat-88].
3. **Pilot 1 technology count.**
	- D1.6:[^d16-9] "Three new technologies".
	- D1.8:[^d18-25] seven items. Four of them do not appear in D1.6: AI4Animals (Deloitte), AUTOFOM3 (Carometec), Tail Length (VION) and CGM Insertion Probe. D1.8[^d18-28] labels two of them "OTHER TECHNOLOGIES".
	- Not necessarily a contradiction, since D1.6 says "new".
4. **Tail length attribution at Pilot 1 (internal to D1.8).**
	- D1.8[^d18-25] lists "PigInspector (CLK GmbH) – Ear, Tail and Skin Lesions" and, separately, "Tail Length (VION)".
	- D1.8[^d18-27] says PigInspector "Measures ear, tail, and skin lesions + tail length".
	- D1.6[^d16-9] says the Pig Inspector "measures tail length".
5. **Pilot 2 tail-length prototype.** Catalogue[^cat-57] lists "Tail Length (prototype) … Provider UAB & Batallé … Technology used in aWISH project". It is not in the D1.6 Pilot 2 list.[^d16-9] **[unverified]**[^new] The Meat Industry Event slides list a tail lesion and tail length classifier at Batallé (Ramon-Pérez et al., submitted).[^mie]
6. **Pilot 3 naming.** D1.6:[^d16-10] "DUC (Plukon Food Group) in Chailley"; D1.8:[^d18-23] "Plukon – Duc". Same site, different label.
7. **Co-lead label for Pilot 2.** D1.8[^d18-23] prints "Wet. H.: UAB" where the other pilots print "Sci. lead:". Quoted as printed; meaning not inferred.
8. **Partner count (project-level, not pilot-level).**
	- D1.8[^d18-18] slide: "28 partners 11 countries 6 pilots".
	- D1.4:[^d14-10] "involves 28 partners, including affiliated entities, from 11 European countries".
	- Siwek and Marchewka 2023 give "24 partners, 13 countries" (Pack A, Table 2).
	- **[unverified]**[^new] CORDIS lists the coordinator and 29 participants, 30 organisations in 12 countries. Four are marked "Third-party", and two, WEL2BE and Aghitech (Hungary), "Participation ended".[^cordis-p] Leaving out the two that ended gives 28 organisations in 11 countries, the figures in D1.4 and D1.8. No document says that is how they counted.
	- The 28 includes affiliated entities, but no document read gives the split.
9. **D1.6 dating.** D1.6's v1.0 is dated 29 Apr 2024. Its v2.0 (17 Sep 2024) is described only as "Adoption of comments by EC"[^d16-3]. The "Sep 2024" label on the installation statements may therefore overstate their currency: the status may be as of April 2024.
10. **Pilot 2 slaughterhouse name.**
	- D1.4 (website text; first submitted 28 Apr 2023, v2.0 17 Sep 2024):[^d14-17] "NORFRISA (FRIGORÍFICOS DEL NORDESTE S.A.) is one of the largest slaughterhouses in Spain … 10,000 pigs to be slaughtered every day".
	- D1.6:[^d16-9] "the pig slaughterhouse Batallé in Catalonia, Spain". D1.8:[^d18-23] "Pilot lead: Batallé". D6.3:[^d63-16] "P2 Batallé - Spain". D6.3:[^d63-52] "Selección Batallé".
	- Batallé does not occur in D1.4. Norfrisa does not occur in D1.6, D1.8, D6.2 or D6.3.
	- The aWISH documents do not explain the change.
	- **[unverified]**[^new] Business registers list Norfrisa (Frigoríficos del Nordeste, S.A.) as a pig slaughter-services company in Riudellots de la Selva, Girona, in the "CÁRNICA BATALLÉ" group, with members of the Batallé family as its presidents.[^norfrisa] D1.4 and the later documents therefore name companies of the same group. Which plant hosted the pilot is not stated.
	- Norfrisa is listed as a round-table panellist at the 8 Oct 2026 industry event.[^packe-17]
11. **Pilot 4 vendor list.**
	- D1.4:[^d14-19] "With technology providers CLK GmbH and Wel2be, more carcass vision data will be added"; "New technologies are installed from Itavi, Wel2be and CLK GmbH."
	- D1.6:[^d16-10] "CLK is responsible for all newly installed technologies in this pilot", plus the Itavi EBENE app. WEL2BE is not named for Pilot 4.
	- The D6.2 dataset list[^d62-91-93] has no W2B dataset for Pilot 4.
12. **Pilot 6 on-farm system name.**
	- D1.4:[^d14-21] "BioSense (BitGear) has installed and developed the IoT solution PigSense".
	- D1.6:[^d16-11] "Bit Gear's Animal Sense technology (TRL 8)".
	- Website pilots page (7 Oct 2026): "Animal Sense (Bitgear, BioSense)".
13. **Pilot 1 pre-existing technologies.**
	- D1.4 (website text):[^d14-16] "already installed cameras in the unloading and lairage area …, a full carcass scan system (AutoFOM3) … and camera's to measure tail length on the carcass (individual carcass tracking using RFID on the slaughter line)".
	- D1.8 lists "AUTOFOM3 (Carometec)"[^d18-25] and "Tail Length (VION)" under "OTHER TECHNOLOGIES".[^d18-28] D1.6[^d16-9] counts "Three new technologies".
	- D1.4 describes the AutoFOM3 and tail-length cameras as already installed before the project's additions. Not a contradiction between documents.

Apart from items 10–12, no document read contradicts another on slaughterhouse name, species, country or scientific co-lead institution.

---

## Appendix: files read

| Document | Date (from its title or summary page) | Per-pilot content found? |
|---|---|---|
| D1.1 Communication, dissemination and exploitation (CD&E) plan and execution report, v1 | Registered by the EC 21 Sep 2024[^d11-1] | No.<br>• Only the country list "FR, PL, ES, NL, AT, RS"[^d11-2] and a description of the website "Pilots" page[^d11-17]. |
| D1.6 Practice abstracts, batch 1 | v1.0 29 Apr 2024; v2.0 17 Sep 2024, submitted 21 Sep 2024[^d16-2-3]. v2.0 is "Adoption of comments by EC"[^d16-3], so pilot text may reflect April 2024 status. | Yes: one abstract per pilot[^d16-9to11] |
| D1.2 CD&E plan and execution report, v2 | Registered by the EC 28 Oct 2024, submitted 28 Oct 2024[^d12-1-3] | No per-pilot content.<br>• Mentions that "The third newsletter offered updates on Pilot 1, 2, and 5"[^d12-22]. The newsletters are in Annex D[^d12-49], which is an image and cannot be searched.<br>• Website "Pilots" page description[^d12-17]. |
| D4.3 Best practice guides, v1 | Registered by the EC 28 Oct 2024, submitted 30 Oct 2024[^d43-1-2] | No.<br>• No slaughterhouse, pilot or pilot-technology names.<br>• Only generic "the pilots"[^d43-9]. |
| D5.2 Value chain actors' needs, perceptions and constraints (read through OCR) | Registered by the EC 25 Oct 2024, submitted 29 Oct 2024[^d52-1-2] | No.<br>• No slaughterhouse names. Interviews are anonymised ("The written notes were anonymised")[^d52-19]. |
| D1.8 Policy briefs and policy workshop report, batch 1 | Registered by the EC 22 Oct 2025[^d18-1]. The pilot content sits in the slides of the "aWISH Policy Workshop … 05/09/2025"[^d18-14], so it is dated 5 Sep 2025. | Yes.<br>• Pilot overview slide[^d18-23]; Pilot 1 slides[^d18-24-28]; technology list[^d18-30].<br>• The policy brief[^d18-1-13] is image-only and cannot be searched. |
| AWI Catalogue (D2.5, final version, "Updated September 2026")[^cat-1] | Sep 2026 | One hit for a pilot name: "Provider UAB & Batallé"[^cat-57]. A few vendor pages that bear on contradictions are cited in §4. |
| D6.2 Data management plan, v1 | "Due date of delivery 30/04/2023 Submission date 28/04/2023"[^d62-2] | Yes, but thin.<br>• The WP3 annex[^d62-50-63] carries pilot-specific text only for Pilot 2[^d62-52-53-56-59-62-63] and one sentence for Pilot 1[^d62-52]. Pilots 3–6 are not answered individually.<br>• The dataset list names datasets per pilot.[^d62-91-93]<br>• See §1b and the chronology. |
| D6.3 Data management plan, v2 | "Due date of delivery 31/10/2024 Submission date 29/10/2024"[^d63-3] | Yes.<br>• Table 5[^d63-16]: signed Data Sharing Agreements per pilot.<br>• The WP3 annex[^d63-41-54] answers pilot by pilot.<br>• See §1b and the chronology. |
| D1.4 Project website report, v2 | "Submission date 28.04.2023"; revisions "21.09.2024"; "2.0 17/09/2024 Adaptation of comments by EC"[^d14-3-4]. The pilot descriptions[^d14-16-21] are the website texts. v2.0 is described only as adaptation of EC comments, so these texts may date from April 2023. | Yes.<br>• One website description per pilot[^d14-16-21], with region of extension and, for some pilots, throughput.<br>• Names vendors per pilot; differs from D1.6 in places (contradictions 10–12). |
| D1.5 Social media engagement strategy | "Due date of delivery 31.05.2023 Submission date 31.05.2023"[^d15-4] | No.<br>• No slaughterhouse names, vendor names or "pilot". |

<!-- Footnotes. GitHub and Obsidian both render these as numbered notes at the end of the page, in order of first use. -->

[^d14-3-4]: D1.4, pp.3–4.
[^d18-23]: D1.8, p.23.
[^d16-9]: D1.6, p.9.
[^d16-9-d18-23]: D1.6, p.9; D1.8, p.23.
[^d18-25]: D1.8, p.25.
[^d18-28]: D1.8, p.28.
[^d18-27]: D1.8, p.27.
[^d18-26]: D1.8, p.26.
[^d14-16]: D1.4, p.16.
[^d63-44]: D6.3, p.44.
[^d18-24-d14-16]: D1.8, p.24; D1.4, p.16.
[^d14-17]: D1.4, p.17.
[^new]: Added 22 Nov 2026 from aWISH deliverables, CORDIS, or public business registers. Not yet checked in the verification log (`verification/verification-log-A-B.md`).
[^d63-52]: D6.3, p.52.
[^d18-30-cat-62]: D1.8, p.30; Catalogue, p.62.
[^cordis]: CORDIS, aWISH project listing ([cordis.europa.eu/project/id/101060818](https://cordis.europa.eu/project/id/101060818)), accessed 7 Oct 2026.
[^d18-30]: D1.8, p.30.
[^cat-57]: Catalogue, p.57.
[^d63-46]: D6.3, p.46.
[^d16-10]: D1.6, p.10.
[^d16-10-d18-23]: D1.6, p.10; D1.8, p.23.
[^d63-47-52]: D6.3, pp.47, 52.
[^d14-18]: D1.4, p.18.
[^d63-53]: D6.3, p.53.
[^ps26-2]: van Staaveren et al. 2026, *Poultry Science* 105(7):106968, DOI [10.1016/j.psj.2026.106968](https://doi.org/10.1016/j.psj.2026.106968), p.2.
[^d14-19]: D1.4, p.19.
[^d16-11]: D1.6, p.11.
[^d14-20]: D1.4, p.20.
[^d16-11-d18-23]: D1.6, p.11; D1.8, p.23.
[^d63-51]: D6.3, p.51.
[^d11-16-d12-16]: D1.1, p.16; D1.2, p.16.
[^d14-21]: D1.4, p.21.
[^ar26-3-14]: Banhazi et al. 2026, *Agronomy Research* 24(2):76–95, DOI [10.15159/AR.26.034](https://doi.org/10.15159/AR.26.034), PDF pp.3, 14.
[^d11-2-d12-2]: D1.1, p.2; D1.2, p.2.
[^d11-17-d12-17]: D1.1, p.17; D1.2, p.17.
[^d18-33]: D1.8, p.33.
[^d43-9]: D4.3, p.9.
[^d14-16-21]: D1.4, pp.16–21.
[^d63-41-54]: D6.3, pp.41–54.
[^d63-16]: D6.3, p.16.
[^d63-60]: D6.3, p.60.
[^d63-41]: D6.3, p.41.
[^d63-54]: D6.3, p.54.
[^d63-42]: D6.3, p.42.
[^d62-56]: D6.2, p.56.
[^d63-45]: D6.3, p.45.
[^d63-49]: D6.3, p.49.
[^d63-46-47-50]: D6.3, pp.46, 47, 50.
[^d63-47]: D6.3, p.47.
[^d63-48]: D6.3, p.48.
[^d63-8]: D6.3, p.8.
[^d62-50-63]: D6.2, pp.50–63.
[^d62-91-93]: D6.2, pp.91–93.
[^d62-52]: D6.2, p.52.
[^d62-53]: D6.2, p.53.
[^d62-59]: D6.2, p.59.
[^d62-62]: D6.2, p.62.
[^d62-63]: D6.2, p.63.
[^d62-61]: D6.2, p.61.
[^d62-91]: D6.2, p.91.
[^d62-92]: D6.2, p.92.
[^d62-93]: D6.2, p.93.
[^d12-22]: D1.2, p.22.
[^d12-49]: D1.2, p.49.
[^d18-24]: D1.8, p.24.
[^d11-2]: D1.1, p.2.
[^d12-41]: D1.2, p.41.
[^d62-52-61]: D6.2, pp.52, 61.
[^d16-9-10-11]: D1.6, pp.9, 10, 11.
[^d14-17-20]: D1.4, pp.17–20.
[^cat-62]: Catalogue, p.62.
[^cordis-p]: CORDIS, aWISH project page, participant list ("Participants (29)"), read 22 Nov 2026; page last updated 26 Nov 2025. https://cordis.europa.eu/project/id/101060818
[^packf-6]: Nuna Solutions' website (accessed Oct 2026).
[^d16-9-11]: D1.6, pp.9, 11.
[^cat-88]: Catalogue, p.88.
[^web-pilots]: aWISH project website pilots page ([www.awish-project.eu](https://www.awish-project.eu/)), accessed 7 Oct 2026.
[^d18-30-cat-88]: D1.8, p.30; Catalogue, p.88.
[^mie]: aWISH Meat Industry Event, 8 Oct 2026, slide deck (uploaded to aWISH website Nov 2026), slides 25 and 83.
[^d18-18]: D1.8, p.18.
[^d14-10]: D1.4, p.10.
[^d16-3]: D1.6, p.3.
[^norfrisa]: Alimarket company record for Frigoríficos del Nordeste, S.A. (Norfrisa): group "CÁRNICA BATALLÉ"; "Matadero de servicios de porcino"; Riudellots de la Selva, Girona. https://www.alimarket.es/alimentacion/empresa/225356/frigorificos-del-nordeste--s-a---norfrisa--225356. BORME entries (Registro Mercantil de Girona) shown by InfoNIF: presidents Pere Batalle Deulonder (to Dec 2024), Josep Batalle Deulonder (Dec 2024) and Josep Batalle Carbones (from 25 Mar 2025), as printed. https://infonif.economia3.com/ficha-empresa/frigorificos-del-nordeste-sa. Both read 22 Nov 2026.
[^packe-17]: aWISH Meat Industry Event programme (8 Oct 2026).
[^d11-1]: D1.1, p.1.
[^d11-17]: D1.1, p.17.
[^d16-2-3]: D1.6, pp.2–3.
[^d16-9to11]: D1.6, pp.9–11.
[^d12-1-3]: D1.2, pp.1, 3.
[^d12-17]: D1.2, p.17.
[^d43-1-2]: D4.3, pp.1–2.
[^d52-1-2]: D5.2, pp.1–2 (OCR; printed page).
[^d52-19]: D5.2, p.19 (OCR; printed page).
[^d18-1]: D1.8, p.1.
[^d18-14]: D1.8, p.14.
[^d18-24-28]: D1.8, pp.24–28.
[^d18-1-13]: D1.8, pp.1–13.
[^cat-1]: Catalogue, p.1.
[^d62-2]: D6.2, p.2.
[^d62-52-53-56-59-62-63]: D6.2, pp.52, 53, 56, 59, 62, 63.
[^d63-3]: D6.3, p.3.
[^d15-4]: D1.5, p.4.
