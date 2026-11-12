# R1-K02 challenge pass receipt

- Brief: [internal file]. Web and in-app browser tools only; phase 1 on case inputs only,
  phase 2 (dossier summary + priority claims) sent afterwards in the same agent context.
- Transcript: `challenge_transcript.jsonl`, sha256 `bae1f534deb8dc703e20d01fd5c787fa2cd4714392c4115a6a3067ac9b4b555a`. Counts below are mechanical ([internal file]); batched actions count as calls.
- Phase 1: 44 calls (budget 45); deviations: none.
- Phase 2: 30 calls (budget 30); deviations: none.

## Phase 1 report (verbatim)

P1_FINDINGS:
1. **Wiltshire & Swindon HER, radius search.** Form at https://services.wiltshire.gov.uk/HistoryEnvRecord with Easting [coordinate removed], Northing [coordinate removed] and radius 500 m. It returned 3 records:
   - **MWI3409 (ST93SW613), "Ring Ditch, Cold Berwick Hill".** https://services.wiltshire.gov.uk/HistoryEnvRecord/Home/ViewHERItem?HER=MWI3409. An undated ring ditch "visible on aerial photographs". Source: Cambridge University Aerial Photograph Unit, ref E/RC8 BK 61 (SWI8608). The record says the primary aerial photograph could not be consulted, so the existing NGR was accepted. The record page shows no grid reference, size or parish.
   - **MWI3418 (ST93SW622), "Ring Ditch, North West of Berwick Farm".** https://services.wiltshire.gov.uk/HistoryEnvRecord/Home/ViewHERItem?HER=MWI3418. An undated ring ditch visible on an aerial photograph. Source: Wiltshire County Council 1971, A10/[coordinate removed] (SWI14437). The page shows no grid reference; I checked with both WebFetch and an in-browser text find.
   - **MWI65114, "Site of Outfarm, South of Chicklade".** https://services.wiltshire.gov.uk/HistoryEnvRecord/Home/ViewHERItem?HER=MWI65114. Parish Hindon. A demolished 19th-century outfarm: one isolated structure, all historic buildings lost. Sources: Lake & Edwards 2014 and Edwards 2014 (Wiltshire Farmsteads Mapping Project). The page shows no grid reference.
   - **Radius behaviour and positions: unverified.** Re-running the search at 200 m and 100 m showed the same 3 rows, with identical element refs, and I could not confirm the table had refreshed. So all 3 records sit within 500 m only if the form honours its radius. I could not obtain their positions or distances. **Form comparison:** a ring ditch is a ditch cropmark and the LiDAR shows a mound with no ditch. A ploughed barrow could show both, so either ring ditch would record this feature only if its position coincides with it, and that is unresolved.
2. **Historic England Aerial Investigation & Mapping (ArcGIS REST, EPSG:27700).**
   - Monument_Extents (layer 1), envelope [coordinate removed]–[coordinate removed] E / [coordinate removed]–[coordinate removed] N (±600 m): features [].
   - Project_Area (layer 2), point query at [coordinate removed],[coordinate removed]: features [].
   - The point is outside any mapping project area, so the empty result says nothing about whether a feature exists here.
3. **NHLE Scheduled Monuments (layer 6 of National_Heritage_List_for_England_NHLE_v02_VIEW).** Envelope [coordinate removed]–[coordinate removed] E / [coordinate removed]–[coordinate removed] N (±1 km): features []. No scheduled monument found in that square.
4. **Victoria County History, Wilts vol. 13, Berwick St Leonard.** https://www.british-history.ac.uk/vch/wilts/vol13/pp100-105
   - Cold Berwick Farm stood on Cold Berwick Hill about 1 km north-west of the church. It was possibly built in the early 17th century and gone by 1822 (inclosure records). An 1822 fair is described as near its former site. Cited sources: Andrews & Dury 1773, the OS 6-inch map Wiltshire LVIII (1889 onwards), and the inclosure award (W.R.O. EA/158, 135/27).
   - Church of St Leonard, NHLE 1318783: NGR [grid reference removed] (E [coordinate removed], N [coordinate removed]), taken from the NHLE REST layer 0.
   - The point lies 956 m from the church at a bearing of about 307° (north-west). That is a plane Euclidean distance on the OSGB grid, with no coordinate conversion needed, and it matches "about 1 km NW".
   - The VCH position is only a rounded distance and compass direction, so it could be several hundred metres out. It is a candidate ordinary explanation (the platform or debris of a deserted farmstead), not a position match.
   - Cold Berwick Farm was gone by 1822, so it is not the same site as the 19th-century outfarm MWI65114.
   - The same page also documents late-18th-century farm buildings about 1 km west of the church (land later in Hindon). By 1983 that site held a mid-20th-century house among 19th- and 20th-century farm buildings. By the same grid arithmetic that is about 620 m from the point, taking the rounded "1 km W" at face value.
   - It also documents Berwick Hill Dairy, built in 1980 on a levelled site beside the Hindon–Chicklade Bottom Farm road; exact position not given. Cold Berwick Hill was downland, enclosed around 1818–22.
5. **ACCESS_FAILURE: NLS historic OS maps.** maps.nls.uk/geo/explore at the point served a "confirm you are human" check. I did not attempt it and could not view the 1889 OS 6-inch sheet. The Wiltshire HER map also gave no readable positions: page text extraction returned only navigation.
6. **Web search.** "Cold Berwick Hill" with ring ditch/barrow/mound, and Berwick St Leonard/Chicklade with ring ditch/barrow/tumulus: no record specific to this feature found.

P1_BEST_READING: **UNRESOLVED.**
- Two undated aerial-photograph ring ditches (MWI3409 "Cold Berwick Hill", MWI3418 "NW of Berwick Farm") are returned by a 500 m HER search, but I could not get their positions. Either could document this mound as a ploughed barrow if its grid reference falls on it.
- No scheduled monument lies within the ±1 km square (NHLE). The AIM result is empty, but mapping does not cover this area.
- An ordinary explanation is documented in approximate form only: VCH places the deserted 17th-century Cold Berwick Farm, gone by 1822, about 1 km NW of the church, and the point is 956 m NW of it.
- Also documented, positions not resolved: a demolished 19th-century outfarm (MWI65114, Hindon parish), later farm buildings about 1 km W of the church, and the 1980 levelled dairy site.
- None of these is tied to this feature's position.
- Next checks: the NGRs of MWI3409, MWI3418 and MWI65114, and the OS 6-inch Wiltshire LVIII (1889) at [grid reference removed].

CALLS: 44

## Phase 2 report (verbatim)

P2_CLAIMS:
1. **"No record within about 200–250 m": SUPPORTED for record points; UNVERIFIABLE for area extents.**
   - Search: HER form at https://services.wiltshire.gov.uk/HistoryEnvRecord, centred on E [coordinate removed], N [coordinate removed].
   - **The radius setting searches a square around each record's single point, not a circle.** At 500 m it returned MWI3409 at 586 m (dE 487, dN 325). It did not return MWI3410 at 717 m (dE 677). So "200 m" means a ±200 m box.
   - The nearest record point in the 2000 m list is MWI65114 at 288 m N, outside the ±200 m box, which fits the dossier's null result.
   - Record pages show only a single point: MWI3402's map shows one marker and no polygon. Large-area records therefore cannot be tested this way.
   - Area records in the 2000 m list that the dossier does not address, extents and descriptions unread:
     - MWI3417 (ST93SW621), "Undated Droveways, Cold Berwick Hill";
     - MWI3421 (ST93SW625), "Undated Field System, North & North East of Berwick St Leonard";
     - MWI3419 (ST93SW623), "Undated Earthworks, Chicklade Bottom".
2. **MWI3402 and its reports.**
   - **Extent covers the point: UNVERIFIABLE, and unlikely.** Record: https://services.wiltshire.gov.uk/HistoryEnvRecord/Home/ViewHERItem?HER=MWI3402, titled "Undated Field System, West and North West of Hindon". Its centroid is E [coordinate removed], N [coordinate removed], 1245 m due W of the point.
   - The record's own sources include SWI13104 (Grinsell et al. 1957, VCH Wilts I.1), SWI31818 (Stead 2026, "Land at Chicklade", Magnitude Surveys geophysics) and SWI31822 (Cook 2025, "Chicklade Services, A303", PCA evaluation).
   - **Cook 2025 is at the A303 services, not this field: SUPPORTED by location.** Chicklade Services sits at [grid reference removed] (https://commons.wikimedia.org/wiki/File:Chicklade_Services,_A303,_Wiltshire_-_geograph.org.uk_-_55958.jpg, "600m W of the small village of Chicklade"). That is about 1.39 km WNW of the point, to ±100 m.
   - **Where Stead 2026 surveyed: UNVERIFIABLE** (no public text found).
   - **The 2004 AC Archaeology "Chicklade" item is probably an address, not a site: SUPPORTED.** AC Archaeology's office is "Manor Farm Stables, Chicklade, Hindon, Salisbury SP3 5SU" (https://www.ukpostcodecheck.com/address/6b1b230f/a-c-archaeology_manor-farm-stables_chicklade_hindon_salisbury_sp3-5su). I did not open the 2004 item itself.
3. **Ring-ditch positions: SUPPORTED. Whether either is the lead mis-plotted: UNVERIFIABLE.** Coordinates are the E/N fields on each HER record page; distances are straight-line on the OSGB grid.

   | Record | Grid ref (E, N) | Distance, bearing | Stated source |
   |---|---|---|---|
   | MWI3418 (ST93SW622), "Ring Ditch, North West of Berwick Farm" | [coordinate removed], [coordinate removed] | 487 m, 117° (ESE) | "Ring ditch is visible on an aerial photograph"; WCC 1971 A10/[coordinate removed] (SWI14437) |
   | MWI3409 (ST93SW613), "Ring Ditch, Cold Berwick Hill" | [coordinate removed], [coordinate removed] | 586 m, 56° (NE) | CUCAP E/RC8 BK 61 (SWI8608); "existing NGR is accepted", primary photo not consulted |
   | MWI3410 (ST93SW614), second "Ring Ditch, Cold Berwick Hill" | [coordinate removed], [coordinate removed] | 717 m, 71° (ENE) | not read; 210 m from MWI3409 |

   MWI3409 was plotted without anyone checking the photograph, so a mis-plot cannot be excluded. An error of 586 m would be unusually large, and no ring ditch record sits west of the pair. It would take the CUCAP frame to settle.
4. **Mapped heap, pit, yard, rick stand, building or lynchet at the point: UNVERIFIABLE.**
   - The NLS six-inch viewer serves a "Let's confirm you are human" page (phase 1), which I did not attempt. I found no online copy of Andrews & Dury 1773, the inclosure award (W.R.O. EA/158) or the tithe map.
   - Cold Berwick Farm: VCH Berwick St Leonard (https://www.british-history.ac.uk/vch/wilts/vol13/pp100-105) gives only "on Cold Berwick Hill c. 1 km NW of the church", gone by 1822. The church is at NHLE 1318783, [grid reference removed]. The point is 956 m from it at 307°, which matches the rounded description but is not a fixed position.
   - Nearest building site actually located: MWI65114, a demolished 19th-century outfarm (E [coordinate removed], N [coordinate removed]), 288 m N.
5. **Barrow at or near the spot in the literature: partly SUPPORTED as a null; the key sources are UNVERIFIABLE.**
   - VCH Chicklade (https://www.british-history.ac.uk/vch/wilts/vol13/pp105-114) notes "few archaeological finds" and names no barrow. VCH Berwick St Leonard names no barrow either.
   - Grinsell's 1957 gazetteer (VCH Wilts I.1, pp. 21–279) has no public online text I could reach; one web search failed. VCH Hindon (vol. 11) was not read.
   - The 2000 m HER list, which folds in Grinsell as a source (SWI13104 on MWI3402), shows no barrow record on Cold Berwick Hill. The barrows it does list are SW of Hindon (MWI3397/3398/3399) and on Two Mile Down (MWI666).

P2_MISSED:
- A second ring ditch, MWI3410, 717 m ENE, making two ring ditches recorded on Cold Berwick Hill.
- Area and linear records inside the 2 km box with unknown extents: droveways on Cold Berwick Hill (MWI3417), a field system N and NE of Berwick St Leonard (MWI3421), and unclassified earthworks at Chicklade Bottom (MWI3419).
- Three demolished 19th-century outfarm sites "North West of Berwick Farm" (MWI65172, MWI65173, MWI65174), positions unread. They are ordinary-explanation candidates of the building or yard type.
- A local precedent: MWI3399 is recorded as "perhaps a barrow or a field lynchet corner" (SW of Hindon).
- The search box is square, so a "500 m" search reaches up to 707 m at the corners.
- The Aerial Investigation & Mapping result is empty only because the point lies outside every project area (phase 1). It is not evidence of absence.
- VCH Berwick St Leonard records Berwick Hill Dairy (1980), built on a levelled site beside the Hindon–Chicklade Bottom Farm road, position unknown. Levelling there is a possible source of spoil.
- Cold Berwick Farm's VCH position (about 1 km NW of the church) matches the point's 956 m at 307°.

P2_OVERSTATED:
- "No monument under 200 m" is true only of single record points. It says nothing about the extents of area records.
- The weight Q4 puts on MWI3402 and its two reports is misplaced. The field system is titled W/NW of Hindon with its centroid 1.25 km W, and Cook 2025 is the services site about 1.4 km WNW.
- Calling Cold Berwick Farm "not located relative to the lead" understates it. The only published placement is consistent with the point, although it is still unfixed.
- NEARBY_DISTINCT treats the ring-ditch positions as reliable, but MWI3409's grid reference was accepted without anyone checking the photograph.

P2_STATUS_SURVIVES:
- NEARBY_DISTINCT holds only for record points: nothing lies within the ±200 m box, and the nearest point records are 288 m (outfarm) and 487–717 m (three ring ditches).
- The overall Q3 status should be UNRESOLVED for three reasons:
  - three area or linear records (MWI3417, MWI3421, MWI3419) have unread extents and descriptions;
  - the deserted Cold Berwick Farm has a published position that matches the point but is unfixed;
  - MWI3409's position is unchecked against its photograph.
- Status is not RECORDED, because no source places a mound, barrow or ring ditch at the point.

P2_Q4_SURVIVES:
- Partly: the yes/no drop rule stands, but the candidate list is aimed at the wrong items.
- Proposed Q4: does any of MWI3417, MWI3421, MWI3419 or MWI65172–4 (via the E/N fields on each record page and its description), or Cold Berwick Farm (placed on Andrews & Dury 1773, the inclosure award EA/158 or the 1889 six-inch sheet LVIII), place a mound, farmstead, yard or heap within about 50 m of E [coordinate removed], N [coordinate removed]?
  - If a farmstead or yard falls on the point: an ordinary explanation is documented, so downgrade or drop the lead.
  - If a barrow or ring ditch falls on it: RECORDED.
  - If neither: keep the lead and move to the 1940/1944 aerial-frame tests.
- Stead 2026 (SWI31818) moves to a narrow HER request only if its location is shown to be near the point.

LIMITS:
- NLS blocked by the human-verification page, which I did not attempt.
- Andrews & Dury, the inclosure award, the tithe map, Grinsell 1957 and VCH Hindon were not read.
- HER record pages give only a point, so no extents were available.
- The phase-1 re-runs at 200 m and 100 m were inconclusive because the results table may not have refreshed. The square-box behaviour is inferred from two records at the 500 m setting.
- The Chicklade Services position is only a six-figure grid reference.
- I did not re-check HE 1624737 or the dossier's Heritage Gateway lookups.

CALLS: 30 in phase 2 (44 in phase 1; 74 in total).
