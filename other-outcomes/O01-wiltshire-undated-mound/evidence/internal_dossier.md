# R1-K02 lead dossier (lead_vetting_v1.1), Wiltshire, 2026-09-29

This summary is private and gives no coordinates; the location is only in `dossier.json` ([internal file]). It was
composed from local files only; no web or browser tool was used. Sources: browser passes B06 and B09 (2026-09-29, both
within the LR-CMP-1 budget, 57/60 each); R1's [internal file], its receipt
[internal file] and its saved Gateway lookup; CX0928's [internal file]
ledgers and the CX0928-N audit; and the independent challenge (`CHALLENGE.md`, phase 1 44/45 calls, phase 2 30/30,
no disallowed tools, transcript sha256 recomputed). Snapshot: `*_v1_prechallenge.*`.

**Validator:** `python [internal file] [internal file] gives class
**unvetted**, 0 errors, `contact_ready=false`. The challenge receipt is recorded; the lead stays unvetted because Q2
is UNRESOLVED.

| Question | Status | One-line basis |
|---|---|---|
| Q1: is the terrain feature real? | REAL | Two independent EA LiDAR surveys (2016 tiles, 2018 NLP) measure the same 0.42-0.43 m dome; a pale soil disc sits on it from 2011 |
| Q2: is it plausibly archaeological? | UNRESOLVED | Plough-spread barrow form, but a natural chalk rise, an old dump and a documented, unfixed deserted farm fit the same evidence |
| Q3: does it match existing records? | NEARBY_DISTINCT (low, provisional) | Records read are distinct (outfarm 288 m; ring ditches 487, 586, 717 m; 1.09 km); three area records' extents unread; challenger's UNRESOLVED not adopted |

## Q1: REAL (not tested by the web-only challenger)

- **Detection DTM = 2018 survey.** At the point the EA 1 m composite equals the National LiDAR Programme survey of
  25 Feb 2018 (SAME_SURVEY, rms 0.0 m). 0.43 m above a plane fitted at 15-30 m, 89 m3, annulus SD 0.039 m (about
  11 times the background). Ring relief against a 21 m mean falls smoothly from +0.14 m with no rim hollow.
- **Independent epoch.** The EA LiDAR tiles survey flown 25 Nov 2016 gives 0.42 m and 88 m3, 0.059 m rms from the
  composite over 150 m (receipt entry matched on survey date and heights; C-key not opened).
- **Imagery.** Esri Wayback, 7 images on 5 dates 2011-2022: pale disc at the centre in 4, differential growth in 2;
  bare soil in July 2011 shows a pale patch 15-20 m across; no ring in any image. Field-edge activity lies 33-39 m away.
- **Limits.** Both DTMs are EA ground-filtered products; plan shape and diameter are unmeasured (22 m is a model
  estimate); no hollow search beyond 30 m; the 1940 NARA frame is unregistered and the 1944 HE frame unviewed.

## Q2: UNRESOLVED (archaeological reading: plough-spread round barrow)

For: a regular dome over an unusually flat surround; the pale disc; nothing drawn on the six-inch or the first three
25-inch editions; ring ditches at 487, 586 and 717 m, a ~20 m ring ditch at 1.09 km, scheduled barrows from 2.07 km.
Against: very low relief; no ditch in the DTM rings or in any image; the pale disc does not separate a spread barrow
from a natural rise or a spread heap.

**Documented farm activity added by the challenge, none fixed at the point.** VCH places the deserted Cold Berwick
Farm (possibly early 17th century; gone by 1822; an 1822 fair near its former site) "on Cold Berwick Hill c. 1 km NW
of the church". The lead is 956 m from the church at 307 degrees: consistent with that rounded placement, not fixed
by it. Three demolished 19th-century outfarms are titled NW of Berwick Farm (county points beyond the 500 m square),
and a dairy was built in 1980 on a levelled site at an unstated position.

| Ordinary explanation | For | Against / status |
|---|---|---|
| Natural chalk or solution rise | R1's strongest competitor; Seaford Chalk, no superficial deposit mapped; low relief | Regular, concentric, confined within ~10-15 m; untested |
| Old ploughed-out dump or heap | R1's other competitor; Cold Berwick Farm rubble or yard debris; 1980 dairy levelling spoil; outfarms 288 m and 500 m+ away | Maps rarely draw heaps; the farm is placed only approximately; post-1980 spoil would be absent from a registered 1940 or 1944 frame; untested (Q4) |
| Chalk or marl pit spoil | B09's list; chalk outcrops over the parish; Lime Pit Copse named | No pit drawn; no hollow within 30 m; weakly against |
| Platform of a farmstead building, rick yard, stack stand or field building | Cold Berwick Farm's consistent placement; outfarms nearby; B09's list | Nothing drawn 1844-1939; farm site unfixed; untested before the 1880s and after 1939 (Q4) |
| Field-system component (lynchet junction, clearance heap) | MWI3402 extent unknown; MWI3421 field system and MWI3417 droveways unread; MWI3399 "perhaps a barrow or a field lynchet corner" | Concentric relief; no Gateway geometry within 250 m; plan shape unmeasured; untested |
| Recent field-edge activity | Structure and objects 2016-2022 | 33-39 m away; mound in the 2016 survey and 2011 soil disc: excluded |

Not PLAUSIBLE while the named competitors are untested; not ORDINARY_EXPLANATION_LIKELY because no source fixes a
heap, pit, structure, farmstead or natural feature at the spot.

## Q3: NEARBY_DISTINCT (confidence low, provisional)

No record read describes a mound at the lead. The county search returned no monument in its ±200 m square (the
setting selects display points in a square, C10), and R1's saved Gateway lookup, now read, measured every geometry
of the 35 records in a ±1 km box: none within 250 m, none containing the lead.

| Record | Distance | Form | Comparison |
|---|---|---|---|
| MWI65114 | 288 m N | demolished 19th-c. outfarm | distinct; bears on the dump and platform explanations |
| MWI3418 | 487 m ESE | ring ditch, 1971 county vertical, size not stated | distinct by position; transcription precision unknown |
| MWI3409 | 586 m NE | ring ditch; "existing NGR is accepted", Cambridge photograph not consulted | distinct by position: the weakest separation |
| MWI3410 | 717 m ENE | second ring ditch on Cold Berwick Hill, 210 m from MWI3409; source unread | distinct by position |
| HE 1624737 | 1.09 km SE | ring ditch ~20 m across (HE 2018 obliques) | similar size class, different position |
| MWI3402 | centroid 1.25 km W | field system W and NW of Hindon, extent unknown, no mound mentioned | distinct in form; extent unlikely to reach the lead |
| NHLE barrows and enclosures; HE [coordinate removed]; MWI666 | 1.82-3.70 km | barrows, enclosures, ring ditches | distinct by position |

**Why the challenger's UNRESOLVED is not adopted (D1).** Under PROTOCOL.md and the R1-K10/R1-K19 standard, a
partial HIT is a record read in full whose form class and size fit the lead and whose offset lies within plausible
plotting error for a stated reason. None of the three reasons meets that.
1. **Area records MWI3417, MWI3421, MWI3419.** Titles only, so not HITs. Their display points lie outside the 500 m
   square, and no Gateway geometry lies within 250 m. Droveways and a field system titled N and NE of the village
   would not document a round dome unless their descriptions name one (the R1-K07 standard); the unclassified
   earthworks could. The residual is an extent the Gateway holds only as a point: open item O10 and half of Q4.
2. **Cold Berwick Farm.** An ordinary explanation (Q2), not a record of a barrow. A fixed position at the lead would
   end the discovery case through Q2.
3. **MWI3409's unchecked grid reference.** The offset is 586 m on both axes: no digit slip gives it, and it is 2.5-3
   times R1-K19's partial offsets and 5 times R1-K10's. A second ring ditch lies 210 m from it; no ring shows at the
   lead in seven images (weak). Its photograph stays an open test (O4).

A trigger was fixed before any lookup: Q3 moves to UNRESOLVED if any record's extent reaches within 50 m of the lead
with a form that could be the mound, or if a ring-ditch photograph places its ring at the lead.

**Why low and provisional**
1. MWI3417, MWI3421 and MWI3419 extents and descriptions are unread (O10). MWI3411, a third ring-ditch title, has
   an unread position beyond the 500 m square (O4).
2. The 35 Gateway box records are measured but not named; B06's box has 4 of 7 unnamed (O1). All 72 county 2 km
   titles are read.
3. MWI3402's extent and Stead 2026 are unlocated; Cook 2025 names the services site about 1.4 km WNW (O2, O3).
4. Planning rows are web-indexed only (ADS blocked); maps after 1939, the tithe, Andrews and Dury and the inclosure
   award are unread; aerial rows are index rows only; Grinsell's gazetteer was not reached (O5-O7).

### Ledger by family (60 rows, plus one B06 search kept outside the ledger for lack of any URL)

| Family | Rows | HIT | SCOPED_NULL | ACCESS_FAILURE | Notes |
|---|---|---|---|---|---|
| national_inventory | 11 | 5 (all distinct) | 4 | 2 | NHLE scheduled layer at 250 m, +/-1 (B06 and challenger), +/-2, +/-3 km; Gateway keyword lists; HE 1624737, [coordinate removed] |
| regional_record | 11 | 8 (all distinct) | 2 | 1 | R1 lookup read; county 200/500/1000/2000 m squares; six full records or display points; challenger re-runs failed |
| planning_grey_literature | 7 | 0 | 5 | 2 | web-indexed and ADS term searches; services site located; AC Archaeology address; ADS blocked |
| historic_maps | 7 | 0 | 2 | 5 | six-inch and KYP 25-inch 1st-3rd read; NLS (three passes), old-maps, tithe, parish map failed |
| aerial_index | 11 | 0 | 5 | 6 | index rows only; AIM coverage gap confirmed with endpoints; no image resolves the spot |
| literature | 13 | 0 | 12 | 1 | VCH Berwick St Leonard and Chicklade read; web results; community histories; Grinsell not reached |

- **Merged with the challenge:** NHLE ±1 km (NI-02), county 500 m and 2 km (RR-03, RR-04), MWI65114, MWI3418,
  MWI3409, MWI3402 (RR-05 to RR-08), NLS six-inch (HM-02). **Added:** RR-10, RR-11, PL-06, PL-07, AI-11, LT-08 to
  LT-13. Earlier merges and relabels are listed in the changelog.

## Q4: the single decision-changing question (rule fixed 2026-09-29, before any lookup)

**Does any source place a documented feature within 50 m of the lead: the mapped extent or description of the
droveways on Cold Berwick Hill (MWI3417), the field system N and NE of Berwick St Leonard (MWI3421) or the
unclassified earthworks at Chicklade Bottom (MWI3419), or the site of Cold Berwick Farm on the inclosure award
(c. 1818-22), the six-inch sheet LVIII (1889) or Andrews and Dury (1773)?**

Tolerance 50 m from the lead's centre to the nearest mapped edge. A "within" or "beyond" answer needs an HER geometry
or a source registered to three control points with residuals of 20 m or less. Andrews and Dury can only exclude
(symbol more than 500 m away) or be inconclusive.

| Answer | Action |
|---|---|
| Farmstead, yard, building, pit or heap within 50 m | Drop as a discovery lead; Q2 to ORDINARY_EXPLANATION_LIKELY; keep as a detection case |
| Barrow, ring ditch, mound, cairn, clearance heap or unclassified earthwork within 50 m | Drop as a discovery lead; Q3 RECORDED if a mound or barrow is described there with 50 m precision, else UNRESOLVED with a conservative hold (as R1-K10) |
| None within 50 m: three extents read, farm placed beyond 50 m | Keep; Q3 firms. Then register the 1940 NARA frame (also tests the 1980 dairy spoil), the 1944 HE frame by ordinary order (owner approves any charge), then a field check with permission |
| Not answerable publicly (extent HER-only; award not digitised) | No status change; run the Q2 image test meanwhile; the named item becomes a specific item for a History Centre copy or, if the gate then holds, a narrow HER request |

- **Not decision-relevant:** the outfarm records' display points lie outside the 500 m square, so they cannot fall
  within 50 m (D4). The ring-ditch photographs are the separate O4 test.
- **Answerable by:** one browser pass (Gateway and county pages for the three records; a re-run of R1's frozen
  lookup helper with a 1000 m keep distance, an argument change only; online copies of the inclosure award and
  Andrews and Dury, never searched; the six-inch once the owner clears NLS verification).
- **Contact: not justified.** Gate 1 fails (public routes remain). Gate 2: items are identified (three extents;
  EA/158) but public routes come first. Gate 5 is met by the challenge receipt.

## Challenge pass (2026-09-29): verdicts and disagreements

Verdicts: point-level null SUPPORTED, extents UNVERIFIABLE; Cook 2025 at the services and the 2004 item as an
address SUPPORTED; ring-ditch positions SUPPORTED, mis-plot UNVERIFIABLE; farm placement consistent, unfixed;
literature partly SUPPORTED as a null. Accepted: MWI3410; the three area records; the outfarms and dairy; the square
search; the misaimed Q4; the farm wording. Disagreements (`challenge_disagreements`):

- **D1** Q3 stays NEARBY_DISTINCT: the three reasons are open items or Q2 evidence, not partial HITs.
- **D2** Extents were partly available: R1's saved lookup measured every Gateway geometry in the box beyond 250 m.
- **D3** The square is adopted as a working reading; a larger circle also fits the two test records.
- **D4** The outfarm display points are already bounded beyond the 500 m square by the challenger's own search.
- **D5** "No online copy" of Andrews and Dury, the award or the tithe: no call in the transcript searched for them.
- **D6** The challenger's list omits MWI3411 (ring ditch) and MWI65187 (outfarm) from its own 2 km results.

## Conflicts (full list in `conflicts`)

- **C1** Q3: B06 NEARBY_DISTINCT; B09 SCOPED_NULL with HIT rows (not allowed); challenger UNRESOLVED; kept
  NEARBY_DISTINCT by protocol definition and D1.
- **C2, C3** Keyword lists are title-level nulls. Box counts: 7 and 35 are different boxes; R1's lookup also counts 35.
- **C4, C6** Coverage and the HE image outage: differences of route, not of fact.
- **C5, C7, C8** Maps were read by R1 and CX0928, not the passes; records before images; present parish Hindon,
  pre-1934 parish unverified.
- **C10** County "radius": nominal radius (v1), extent-based (CX0928), square on display points (challenger).
  Square adopted as the simplest reading; every reading covers display points within 200 m and none tests extents.
- **C11** Cold Berwick Farm: "not aligned" (v1) against "consistent" (challenger). Both hold: consistent, unfixed.

## Correspondence: held (pre-protocol, unsent, unchanged; owner decides drop or revive)

1. **Wiltshire & Swindon HER Gmail draft** (K02 + K19), revised 2026-09-28. CX0928: HOLD.
2. **HE Archive five-location Gmail draft** (LOC231 5026 for this lead). CX0928: DROP.
3. **Local R1 letters** and the optional assessor pack `assessor_pack/K02/` (no send recorded). Bodies not opened.

## Next

1. Q4 browser pass under the fixed rule: three record pages, lookup re-run, inclosure award and Andrews and Dury
   searches, six-inch once verification is cleared. No correspondence.
2. Register the held 1940 NARA frame (Q2 origin and the post-1980 spoil test).
3. Open: ring-ditch photographs (O4), MWI3402 and its reports (O2, O3), Grinsell (O7), plan shape (O9).

- 2026-10-02 18:30:31Z: the owner SENT the combined follow-up reply in the HER thread (message [message id removed]). It contains the measurements, map and imagery research, three questions, Fig1 and Fig2. Codex removed the quoted history beforehand. Verified from Sent by the coordinator at 19:06Z. Awaiting the HER reply; this is evidence, not confirmation.
