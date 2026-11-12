# LC3-K52 challenge pass receipt

- Brief: [internal file]. Web and in-app browser tools only; phase 1 on case inputs only,
  phase 2 (dossier summary + priority claims) sent afterwards in the same agent context.
- Transcript: `challenge_transcript.jsonl`, sha256 `82104dfe33dfeffb2b2db7e5da597a6ba43bf880bac577340fb87e7aca73c1ce`. Counts below are mechanical ([internal file]); batched actions count as calls.
- Phase 1: 45 calls (budget 45); deviations: none.
- Phase 2: 29 calls (budget 30); deviations: none.

## Phase 1 report (verbatim)

P1_FINDINGS:

**Route 1: Norfolk Heritage Explorer spatial search** (public NHER, advanced search on grid reference [grid reference removed])
- The 1 km search returned 3 records: [query URL with coordinates removed]
  - NHER 12587, Roman coin (findspot). Grid reference not retrieved.
  - NHER 29008, Neolithic axehead (findspot). Grid reference not retrieved.
  - NHER 54586 (see below).
  - No mound, barrow, warren, military or clump record falls inside this search. The "Range" works as a square box: NHER 31524, 2.43 km away diagonally, came back in the 2 km run. So the 1 km run covered the whole 1 km circle. It searches by each record's grid point, so a large-area record whose centre lies more than 1 km away would be missed.
- The 2 km search (same URL with Range=2000) returned 41 records. The relevant ones are below.

**Records found**
- **NHER 54586, "Earthworks of a probable section of the Peddars Way Roman road"** (Harling parish)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF61548-Earthworks-of-a-probable-section-of-the-Peddars-Way-Roman-road
  - Printed location: [grid reference removed]. The text says "[grid reference removed]", a typo for TL.
  - Distance: about 356 m north. The easting is within 25 m of the lead's.
  - Form: a linear earthwork bank on the recorded road line, which is also the Harling–Brettenham parish boundary. Not a round mound.
  - Source: Norfolk NMP mapping, February 2011, from RAF 1946 and OS 1975 aerial photographs. That mapping covered this immediate area and recorded no mound at the lead's position.
  - Inferred, not checked on a map: the lead may lie on or near the line of the Peddars Way, close to where the Harling/Brettenham boundary meets Riddlesworth.
- **NHER 33622, "Possible Bronze Age round barrow"** (Harling)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF33622
  - Printed location: [grid reference removed]. Distance: about 1.40 km NNE.
  - Form: "Large circular mound, 40m diameter, 1.5m high" (1998 Rapid Earthwork Identification Survey, Forestry Commission compartment 8096). The lead is the same kind of mound but smaller: about 28 m across at 10% of centre height, 19–22 m at half height, 1.1 m high. Different location, so not the same feature.
- **NHER 37174, "Possible Bronze Age barrow"** (Harling)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF41413-Possible-Bronze-Age-barrow
  - Printed location: [grid reference removed]. Distance: about 1.45 km NNE.
  - Form: "said to resemble adjacent monument NHER 33622". Recorded in a 2002 survey before stump removal; the Forestry Commission agreed not to remove the stumps. No dimensions given. Not the same feature.
- **NHER 15755, "Undated mound"** (Harling)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF15755
  - Printed location: [grid reference removed]. Distance: about 2.00 km north.
  - Form: long mound, 26 × 10 m, 1.2–1.75 m high, aligned east–west. A 1996 assessment called it "a later dump of material immediately pre-afforestation". Indexed as butts, pillow mound and rabbit warren; cited in Mason 2009, *The Archaeology of the Warrens of Thetford Forest*.
  - It is elongated, while the lead's footprint is nearly round (20 × 18 m). It is the local precedent for the forestry-dump and warren explanations.
- **NHER 31524, "Possible Bronze Age barrow"** (West Harling Heath)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF31524
  - Printed location: [grid reference removed]. Distance: about 2.43 km NE.
  - Form: about 0.5 m high, 15 × 10 m, "not convincing as a barrow". Smaller and lower than the lead.
- **NHER 6102 and 6103, "Bronze Age round barrow on West Harling Heath"**: inside the 2 km box (so within about 2.8 km). Not opened, so no grid references.
- **NHER 54569, "Earthworks of a possible World War Two firing range"** (Shadwell Park, Brettenham)
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF61416-Earthworks-of-a-possible-World-War-Two-firing-range
  - Printed location: [grid reference removed]. Distance: about 2.14 km NW.
  - Form: banks and trenches forming a butt and target stand. Not a round mound. It is the nearest recorded military feature.
- **NHER 30519, "Riddlesworth Park and multi-period finds"**
  - URL: https://www.heritage.norfolk.gov.uk/record-details?MNF30519-Riddlesworth-Park-and-multi-period-finds=
  - Printed location: [grid reference removed] (centre of the park). Distance: about 1.71 km east.
  - Content: the park was laid out about 1792 and covered about 160 ha on Faden's 1794 map, with "clumps of woodland in the western area" (also on the 1840 tithe map). After the Second World War the parkland was ploughed and the clumps reduced.
  - It supports the estate-clump explanation in general, but locates no clump at the lead.
- **Parish summary TNF1491**: http://www.heritage.norfolk.gov.uk/record-details?TNF1491-Riddlesworth-%28Parish-Summary%29=
  - It lists 31 NHER numbers and mentions no mound, barrow, warren, clump or military feature.

**Route 2: Historic England research records** (Heritage Gateway, keyword "Riddlesworth", 13 results)
- Only one barrow-type record came back: **HE Monument [coordinate removed]**, also NMR TL 98 SE 5 and Norfolk SMR 6109.
  - URL: https://historicengland.org.uk/listing/heritage-gateway/results/record/0d636742-8028-4a8c-8b7c-e1f9aaf2d338/65b3e6a1-e86e-4228-b07e-90dfa43a4e0d
  - Printed location: [grid reference removed]. Distance: about 4.08 km east.
  - Form: a double ring-ditch cropmark. The 1977 field visit saw no mound or ditch. Not the lead.
  - The Megalithic Portal's "Riddlesworth Tumulus" at [grid reference removed] (seen only in a search summary) is the same site.
- The other 12 results are buildings, churches, findspots, deserted settlements and Devils Ditch. None is a mound.

**Access failures**
- Direct WebFetch of Heritage Gateway returned HTTP 403. The browser worked instead. The old Heritage Gateway uid=[coordinate removed] link now resolves to an unrelated Shropshire record.
- The NLS six-inch OS map viewer showed a "Human Verification" bot check. I did not bypass it, so I viewed no historic map of the spot.
- The Breckland Society *Warrens of Breckland* PDF came back as unreadable binary through WebFetch.
- Not reached within the budget:
  - Norfolk Map Explorer (1946 RAF, tithe and Faden map layers).
  - National Heritage List map search. Any scheduled monument would also be in the NHER, and none falls within 1 km.
  - Historic England's Aerial Archaeology Mapping Explorer.
  - Lawson, Martin and Priddy 1981 (East Anglian Archaeology 12), consulted directly. Norfolk's barrow records are in the NHER, and none is within 1 km.
  - The Suffolk HER, which lies across the Little Ouse.

P1_BEST_READING: No prior record of this feature was found in the sources searched.
- No NHER or Historic England research record describes a mound within about 1 km of [grid reference removed].
- The nearest recorded mounds are 1.40–2.00 km away. Two are probable barrows, similar in kind but larger (NHER 33622, 40 m; NHER 37174). The third is a long mound interpreted as a pre-afforestation dump or possible pillow mound (NHER 15755), which has a different shape.
- The 2011 Norfolk NMP mapping of this immediate area, from 1946 and 1975 aerial photographs, recorded the Peddars Way bank 356 m away but no mound here. Possible reasons: the mound was not visible on those photographs (for example under trees), was judged not archaeological, or was formed after 1975. It is present in the 2009 survey.
- No source examined accounts for it with an ordinary explanation. Local analogues exist for each:
  - estate clumps: Riddlesworth Park's western clumps, park centre 1.7 km east;
  - dumping before afforestation and warren features: NHER 15755, 2 km north;
  - WWII military use: Shadwell Park, 2.1 km NW.
- None of these is evidenced at the lead's position, and the historic-map check that would test them failed.
- Possible extra context to test: the lead may sit on or near the recorded line of the Peddars Way and a parish boundary junction. This is inferred from coordinates only.

Calls used: 45 web and browser calls (out of 45), plus one ToolSearch to load WebSearch and WebFetch. The browser tab I opened (tab-9) is closed.

## Phase 2 report (verbatim)

P2_CLAIMS:
Direct quotes are limited by copyright rules, so the source text is paraphrased except for one quote (on KNE 020).

**Q1 REAL** (two EA surveys, the measurements, flight dates, rms 0.109 m, stability): **UNVERIFIABLE.** These are the project's own measurements, and no public route to re-measure them was in scope. The composite figures (1.11 m, 233 m³, 0.97 m, 22 × 19 m) and the 2009 figures (1.06 m, 227 m³, 0.91 m) match the phase-1 case data exactly. The 2009 widths and the flight dates were not checked.

**Q2 PLAUSIBLE, sub-claims:**
- **River-terrace sand and gravel: SUPPORTED.** The BGS 1:50,000 superficial-deposits WMS, queried at the lead, returns River Terrace Deposits, 1 (sand and gravel).
- **Scheduled Rushford Heath bowl barrow about 411 m away: SUPPORTED (417–423 m).**
  - https://heritage.suffolk.gov.uk/Designation/DSF15346 (SM 31107): [grid reference removed], 417 m. Its title places it "180m west of Peddar's Way". About 1.5 m high, up to about 34 m across, with a buried ditch about 3 m wide.
  - https://heritage.suffolk.gov.uk/Monument/MSF7186 (EUN 002): [grid reference removed], 423 m. On the 1905 OS 25-inch map; 90 ft × 6 ft in 1969; 26 m × 1.39 m in 1976.
- **Knettishall Heath barrows at 1.5–2 km: SUPPORTED.**
  - KNE 001, Hut Hill (https://heritage.suffolk.gov.uk/Monument/MSF7403): [grid reference removed], 1,473 m. Recorded as about 100 ft × 7 ft (1962) and 30.5 m × 2.1 m (1969). The dossier's 2.39 m height was not found.
  - KNE 019 (https://heritage.suffolk.gov.uk/Monument/MSF15688): [grid reference removed], 1,967 m. A covert boundary bank around the SM 31106 barrow.
- **No record places a heap, pit, structure or military feature at the point: SUPPORTED for records.**
  - The NHE ±1 km search holds only three records. NHER 54586 is at 356 m. NHER 29008 (axehead, [grid reference removed]) is at 696 m. NHER 12587 (Roman coin found in a yard at Riddlesworth Stud, [grid reference removed]) is at 704 m.
  - An NHE keyword search (camp, warren, clump, military, Nissen, spoil) within ±3 km returned 13 records. None is nearer than Riddlesworth Park (1.7 km) and NHER 15755 (2.0 km).
- **1880s OS map shows open rough ground, no clump at the point: UNVERIFIABLE.** The NLS map viewer was behind a "Human Verification" check, which I did not bypass.
- **RAF 1946 mosaic woodland/scrub; 1988 forestry ride: UNVERIFIABLE.** I did not reach Norfolk Map Explorer or the HE Aerial Photo Explorer.
  - Indirect support: the 2011 Norfolk NMP used RAF 1946 and OS 1975 photographs here (sources of NHER 54586) and recorded nothing at the point.
- **No warren at Riddlesworth or Knettishall in the Breckland Society survey; nearest Snarehill about 5.7 km.**
  - The part about the Society's survey is **UNVERIFIABLE**: both of its PDFs came back as unreadable binary, and the project page carries no gazetteer.
  - The implied nearest-warren distance is **CONTRADICTED**. KNE 020 (https://heritage.suffolk.gov.uk/Monument/MSF15689), [grid reference removed], centre about 1.54 km SE, describes a bank that "Appears to be subsumed within indistinct bank around the `rabbit warren'". It links to the bank around KNE 009.
  - https://leapinghare.org/businesses/places-to-see/knettishall-heath/ also refers to an 18th-century rabbit warren on Knettishall Heath.
  - NHER 15755, 2.0 km north, is indexed as pillow mound and rabbit warren.
- **Riddlesworth Park record point 1.7 km, with tree clumps: SUPPORTED.** NHER 30519 is at [grid reference removed], 1,708 m. Clumps are recorded in the park's western area on the 1794 and 1840 maps.
- **1942 army camp of Nissen huts in Riddlesworth Park, extent not given: SUPPORTED.**
  - https://www.polishresettlementcampsintheuk.co.uk/PRC/riddlesworth.htm: a large camp on requisitioned park land, built of Nissen huts. It gives no location within the park.
  - NHER 6119 (Riddlesworth Hall, [grid reference removed]) does not mention it.

**Q3 NEARBY_DISTINCT (low), sub-claims:**
- **Peddars Way line about 105 m: UNVERIFIABLE directly, consistent.** I did not view the NHE line. Interpolating between the SM 31107 title ("180m west") and the NHER 54586 bank centre puts the road about 85–100 m west of the lead.
  - NHER 1289 (https://www.heritage.norfolk.gov.uk/record-details?MNF1289-The-Peddars-Way) does not describe this stretch.
  - The stretch it cites, NHER 54566 ([grid reference removed]), lies 2.86 km north at the River Thet.
- **Earthwork section about 300 m: SUPPORTED, approximately.** NHER 54586 (MNF61548) is centred at [grid reference removed], 356 m away. It is a bank along the Roman road line, which is also a parish boundary.
- **Rushford Heath barrow at 411–417 m: SUPPORTED** (see above).
- **Knettishall barrows at 1.47–2.0 km: SUPPORTED** (see above).
- **Park record point 1.7 km: SUPPORTED** (see above).
- **Double ring ditch at 4.0 km: SUPPORTED.** HE Monument [coordinate removed] / NHER 6109 is at [grid reference removed], 4,075 m (the dossier says 4,046 m). It is a cropmark with no mound, recorded 1977.
- **NHE map shows nothing else within about 350 m: SUPPORTED.** The nearest point records are at 696 m and 704 m.
- **OS six-inch, 1:25,000 and 1880s maps show no label at the point: UNVERIFIABLE** (NLS check).
- **Parish summaries name no mound or warren here: SUPPORTED for Riddlesworth (TNF1491).** The Breckland Society survey part is UNVERIFIABLE.
- **EAA 12 unreadable: SUPPORTED.**
  - https://eaareports.org.uk/publication/report12/ returns "Website Builder 404".
  - The ADS EAA contents page returned a Cloudflare "Just a moment..." challenge, which I did not bypass.
- **Gazetteer's Norfolk entries were compiled from the county record: UNVERIFIABLE.**
  - The Suffolk HER does carry EAA 12 into its barrow records: KNE 001 cites Lawson, Martin and Priddy 1981.
  - The Norfolk barrow records I opened (NHER 33622, 37174, 31524) post-date 1981 and do not cite it.

P2_MISSED:
- **NHER 33622** ([grid reference removed], 1.40 km NNE): large circular mound, 40 m across, 1.5 m high, probable barrow. Found by a 1998 Rapid Earthwork Identification Survey of a Forestry Commission compartment.
- **NHER 37174** ([grid reference removed], 1.45 km NNE): mound said to resemble 33622. Found by a 2002 survey before stump removal.
  - These two are the nearest Norfolk-side analogues, both in plantation. The forestry pre-planting and stump-removal survey reports (SCCAS 98/25 and 2002/126) are a source family the dossier did not use.
- **NHER 15755** ([grid reference removed], 2.0 km N): long mound, 26 × 10 m. A 1996 assessment called it probably a dump of material made just before afforestation. Indexed as butts, pillow mound and rabbit warren, and cited in Mason 2009. It is local precedent for both the forestry-dump and warren explanations.
- **NHER 31524** (2.43 km): possible barrow, judged unconvincing.
- **Knettishall warren:** KNE 020 and KNE 009, with the warren itself at about 1.2–1.5 km SE across the river.
- **Norfolk NMP 2011 coverage:** it recorded Second World War features nearby (NHER 54569 firing range, 2.14 km; NHER 54570 camp, 2.66 km; NHER 54576 weapons pits, 3.02 km) but nothing at the lead.
- **The camp's later history:** it became a Polish resettlement camp in 1946 (602 residents). No NHER record of the Riddlesworth camp exists within ±3 km, so its footprint is unknown.
- **Riddlesworth Stud** is about 700 m away (NHER 12587).
- **Explanations not considered:**
  - a road- or boundary-related mound, since the lead lies about 90 m from the Peddars Way line, which is also a parish boundary;
  - a forestry stump heap formed before 2009.

P2_OVERSTATED:
- **"Nearest Snarehill, about 5.7 km":** recorded warren evidence lies 1.2–2.0 km away (KNE 020 and KNE 009; NHER 15755). "Warren not supported by sources" should become: untested at the spot.
- **"Stable between the surveys, so not … a recent heap":** this excludes only heaps formed after 2009. A forestry heap or a heap from clearing the 1942–46 camp is still possible.
- **"Partial surrounding hollow":** the supplied ring metric is 0.018 m deep over a 49 m ring. Any hollow is unquantified.
- **The gazetteer-provenance sentence** is stated as fact without EAA 12 having been read.
- **Smaller points:** the 105 m figure is given more precisely than the evidence supports (about 85–100 m is derivable). The 2.39 m height for Hut Hill was not found. 4,046 m against 4,075 m for the ring ditch.

P2_STATUS_SURVIVES: yes.
- No record documents the lead in the NHER (±1 km), the HE research records ("Riddlesworth", 13 results) or the Suffolk HER (nearest is SM 31107 at 417 m, a larger, distinct mound south of the river).
- Every record the dossier missed is 1.4 km or more away and distinct.
- Low confidence remains right, because EAA 12, the historic maps and the aerial mosaics are unverified.

P2_Q4_SURVIVES: yes, narrowed.
- The HER half is effectively answered already: the online NHER has no mound or barrow record within ±1 km.
- Only EAA 12 itself remains, and it is still unreadable. It is unlikely to hold a barrow absent from the HER, but that is not proven.
- Its "warren, clump, military or spoil" branch can hardly fire, because a barrow gazetteer does not judge those explanations.
- Questions with more value, for the Norfolk Historic Environment Service or another qualified person: did the forestry earthwork surveys or the NMP cover this compartment, and did the 1942–46 camp extend here?

LIMITS:
- The Q1 measurements and flight dates could not be checked.
- The NLS map viewer and the ADS site both presented bot checks.
- Norfolk Map Explorer, the HE Aerial Photo Explorer, and the Faden, Hodskinson and tithe maps were not reached.
- Both Breckland Society PDFs were unreadable.
- I did not open the KNE 009 warren record, so its edge distance is unknown.
- The Riddlesworth camp's location is unknown.
- The Barnham barrow cluster and the CNW 003, KNE 002 and KNE 006 rows were not rechecked.
- Correction to phase 1: the NHE search may not be a square box. NHER 6119, with a point 1.99 km east, was missing from the 2 km run. The ±1 km result still holds for records whose points lie within 1 km.

Phase 2 calls used: 29 of 30. tab-10 is closed.
