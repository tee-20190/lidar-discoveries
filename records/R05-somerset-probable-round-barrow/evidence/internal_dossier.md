# R1-K07 lead dossier (lead_vetting_v1.1), Somerset, 2026-09-29, after the challenge and the B10 merge

This summary is private and gives no coordinates; the location is only in `dossier.json` ([internal file]). It
merges local evidence only; no web or browser tool was used to compose it. Sources: B04 and B10 browser research
passes (arm identities not recorded); R1 dossier `K07.md`; CX0928 Codex ledgers (`SOMERSET.md`, `HE_ARCHIVE_K.md`) and
saved receipts; challenge receipt `CHALLENGE.md`. Pre-challenge snapshots: `dossier_v1_prechallenge.json` and
`DOSSIER_v1_prechallenge.md`, unchanged.

**Validator:** `python [internal file] [internal file] gives class
**unvetted**, 0 errors, `contact_ready=false`. The lead stays unvetted because Q2 is UNRESOLVED, even with a challenge
receipt.

| Question | Before challenge | Now |
|---|---|---|
| Q1: real terrain feature? | LIKELY_REAL | LIKELY_REAL (not tested by the challenge) |
| Q2: plausibly archaeological? | UNRESOLVED | UNRESOLVED: deer-park and military readings added; planting clump weakened |
| Q3: already documented? | NEARBY_DISTINCT (moderate, provisional) | NEARBY_DISTINCT (moderate, provisional). Challenger says SCOPED_NULL (C6); B10 says UNRESOLVED |

## Q1: LIKELY_REAL (unchanged)

One EA 1 m composite DTM shows a discrete circular rise on a summit: 1.41 m above a plane fitted at 15-30 m, but only
+0.34 m of local relief in the 0-5 m ring. Independent imagery (2006, 2011-2022) shows a persistent uncut island or
disc at the spot. It is not REAL: the imagery shows vegetation marks, not relief; an uncut grass island may leave DTM
residue; there is no second LiDAR epoch. New route (O9): the Somerset HER map's EA lidar layer, product and epoch
unknown.

## Q2: UNRESOLVED

The archaeological reading is a small round barrow. Jack's Castle lies 926 m ESE: B10 read its entry as "Selwood
Barrow", flat-topped, 21 m across and 3 m high, excavated by Colt Hoare. A "Barrow" field name lies 2.18 km NW.

| Explanation | For | Against / status |
|---|---|---|
| Clearance or spoil heap | Arable field; a hollow 40-150 m away | Mark unchanged 2011-22; untested before 2006 |
| Feeder or trampling | Pale patch round a 2-3 m object (2018, 2021) | Explains the patch, not the rise |
| Natural summit knoll | Summit convexity | Discrete rise within about 10 m; no mapped drift |
| Coal-trial or clay-pit spoil | Coal shaft 19476, 944 m N (100 m precision, dug from 1804); Haven brickyard within 1 km | Nothing marked at the spot; other trial sites unlocated (Torrens unread) |
| Planting clump (Stourhead) | Hilltop; Alfred's Tower and the park's Somerset part within 1 km | **Weakened:** the tithe shows area woodland, not a clump; empty field c.1888; outside the registered park |
| Woodland-clearance heap | Woodland c.1840 across the whole crop; open field by c.1888 | A barrow left in a cleared wood gives the same sequence |
| Buried modern structure | Dished top; central object | No record within 500 m |
| Military (new) | 1944 aircraft strike on Alfred's Tower (55478) | Recorded at the tower, not the lead; no military record within 500 m |

Other archaeological readings to rule in or out (new): a **deer-park feature** (pillow mound, lodge, boundary bank
or prospect mound) and a **windmill mound**. The 1251 park boundary runs "towards Kingsettle along the old ditch",
McGarvie 1980 cites a "massive bank to N", and the park's extent is UNVERIFIABLE (O12). These readings would be
archaeological, but not a barrow. A 1940s image or a field check decides.

## Q3: NEARBY_DISTINCT (moderate, provisional)

No record lies within 500 m in any working search. The null rests on CX0928's county radius search (0 at 250 m and
500 m, with saved lists) and is corroborated by the challenger's visual map-overlay check. Every record compared is
distinct:

| Record | Distance (reference) | Form |
|---|---|---|
| HE [coordinate removed] = HER 53578/15185 (Cook's Farm) | 816-818 m NNE (grid refs) | c.1.8-acre enclosure; on RAF CPE/UK/1924, 1947 |
| HER 37541; NHLE 1005642 Jack's Castle | about 892 m NW; 926 m ESE (3 passes) | lidar-recorded enclosure; 21 m bell barrow, Wiltshire |
| HER 19476 | 944 m N (100 m precision) | coal-trial shaft, dug from 1804 |
| HER 28626 (registered-park part), 53591, 55478, others | 500-1000 m band | park (lead outside it), 1 m cross socket, tower |
| NT MNA193177; HER 15790; HER 16938 | about 1.13; 1.14; 1.33 km | linear banks; settlement earthworks; 33 m platform |
| HE [coordinate removed]; HE [coordinate removed]; HER 53581 | about 1.5 (1 km precision); 1.47; 1.48 km (centre) | possible temple; farm track; deer park, no extent |

**Not SCOPED_NULL (C6).** PROTOCOL.md reserves SCOPED_NULL for a ledger with no HIT rows at all. These rows are
position and form comparisons made to exclude a mislocated alias, so they are HITs. PROTOCOL.md sets no distance for
"nearby"; the wording adopts the challenger's substance ("nothing within 500 m; nothing competes"). Relabelling the
rows to reach a status is barred, and the counting class is the same either way.

**Why provisional**

1. **Main caveat: no Wiltshire & Swindon HER result.** Two challenger attempts at 500 m gave no readable output.
   The boundary is estimated at about 0.8-1 km E. The same form worked for M052.
2. **Deer-park extent UNVERIFIABLE (O12).** A park record is not a record of the mound; McGarvie 1980 could map a
   feature at the lead.
3. **SANHS Somerset Archaeology 1977 (O14), search summary only.** It reportedly notes "a large, well-preserved round
   mound on a prominent hill overlooking Bruton", probably a barrow. The location is unknown and the PDF has no text
   layer. It is **not a match**, but it is the only open route to RECORDED. HER 56089 "Barrow field name, NE of
   Bruton" is also unread; its point lies beyond the 3 km setting.
4. **Other open items.** NT MNA192015 was not found. HER 28626 was checked only visually. Planning rows are
   web-indexed. Aerial rows are coverage nulls: no AIM project covers the lead (four queries).

### Ledger by family (66 rows: 44 v1 + 13 challenge + 9 B10; 5 reads merged into existing rows)

| Family | Rows | HIT (all distinct) | SCOPED_NULL | ACCESS_FAILURE | Added after v1 |
|---|---|---|---|---|---|
| national_inventory | 15 | 6 | 6 | 3 | NI-11 NHLE 2 km; NI-12 registered park at the point; NI-13/14 HE [coordinate removed], [coordinate removed]; NI-15 (B10) |
| regional_record | 20 | 9 | 5 | 6 | RR-12 map overlays (VISUAL ONLY); RR-13 Wiltshire HER (failed twice); RR-14 19476; RR-15 MNA192015 (not found); RR-16 to RR-20 (B10) |
| planning_grey_literature | 6 | 0 | 5 | 1 | PL-06 (B10, search results only) |
| historic_maps | 8 | 0 | 4 | 4 | HM-08 HER-map OS layer did not load |
| aerial_index | 12 | 0 | 8 | 4 | AI-09 to AI-11 AIM (challenge); AI-12 AIM (B10) |
| literature | 5 | 0 | 4 | 1 | LT-04 challenger search (results only); LT-05 SANHS 1977 (summary only; PDF unreadable) |

**Merged, not duplicated:** HER 53581 (CX0928, B04, challenger); HER 19476 (challenger, B10); NHLE 1005642 entry
(CX0928, B10); the county 1 km query (CX0928, B10: same 11 IDs); NLS direct (R1, B04, B10). **Schema mappings:** two
unread items (RR-20, LT-05) and one invalid route (RR-19) are recorded as ACCESS_FAILURE, so they cannot count as
coverage; B10's AIM NOT_APPLICABLE became SCOPED_NULL.

## Tithe clump: provenance finding

The claim comes from SOMERSET.md line 32 (CX0928, 2026-09-28). Codex viewed the Somerset HER tithe raster at the
point and saved `titheazure_z8_5x5.png` and the tithe panel of `k07_layer_comparison_z8.png`. I re-viewed both saved
images at CX0928's computed pixel position. Tree symbols are spread evenly over the whole ~186 m crop, the woodland
convention; none is concentrated at the point, which falls on blank ground between symbols. **Verified reading:** the
spot lay inside mapped woodland c.1840, with no clump and no mound symbol. The v1 phrase "planting clump (c.1840
tithe tree symbols at the spot)" overstated this, so the planting clump is weakened, not strengthened (C8).
Registration is unmeasured, but the whole crop is woodland; the parcel name is unassigned (O10).

## Q4: the single decision-changing question

**What does the earliest 1940s vertical that resolves a 12-14 m feature show at the spot?** Routes, cheapest first:

(1) a free HE footprint check: do RAF CPE/UK/1924 frames 2260-2261 (16 Jan 1947; cited by HE [coordinate removed] for the enclosure
816 m away; local prints at the Somerset HER) cover the point? (2) The Aerial Photo Explorer, once restored, for those
frames and LOC231 5014-5015 (1944). (3) Ordinary orders; NCAP GX/10313 0349 (1940) is likely unreadable and comes last.

| Answer | Action |
|---|---|
| Mound or uncultivated island in open ground | Keep (excludes a post-1940s heap, feeder or structure); then a field check or qualified assessment |
| Open ground, no mound, with a similar-size open-ground feature resolved in the same frame | Drop; Q2 to ORDINARY_EXPLANATION_LIKELY |
| Trees, clump, heap, pit or works | Downgrade; keep only if an earthwork shows independent of it |
| Unreadable, or no coverage | No change; take the next route |

- **Record precheck (first, cheapest).** Does the SANHS 1977 note or HER 56089 describe the lead? Yes → Q3
  RECORDED, class known_site; stop discovery-oriented work. No, or location not given → continue with Q4.
- **Already done / controls.** CX0928 viewed the free Somerset layers: tithe (woodland), OS c.1888 (empty field),
  RAF c.1946 (inconclusive), 2006 (mark). Jack's Castle is tree-covered in 1946-48, so it serves only if open (C7).
- **Contact: not justified.** Gate 5 now holds (challenge receipt), but gate 1 fails: free and ordinary routes remain.

## Challenge pass (CHALLENGE.md; transcript hash recomputed, matches)

- **Call counts.** Phase 1 was blind, 45 of 45 calls, clean. Phase 2 used 31 of 30 calls, **one over budget**; the
  report's own count says 30, and the mechanical count governs. No disallowed tools.
- **Adopted:** the lead is outside the Stourhead registered park; AIM is a coverage gap; HE [coordinate removed] and [coordinate removed] are
  distinct; 19476's location is confirmed; the deer park is UNVERIFIABLE and deer-park features are added to Q2;
  CPE/UK/1924 is added to Q4; the tithe claim needed checking.
- **Where I disagree:** the SCOPED_NULL label (C6); that the tithe would favour a clump (C8); that the free Somerset
  layers are still pending (they were already viewed); that "a mound in open ground c.1888" could come from a map;
  Jack's Castle as a ready control (C7); that a deer-park extent alone would move Q3 (only a mapped feature at the lead
  would).

## Conflicts, open items and correspondence

- **Conflicts** (full list in `conflicts`): C1 Jack's Castle at 926 m, confirmed by three passes, missed by B04's
  South Somerset list; C2 B04's UI search failed where CX0928's radius search worked; C3 HE [coordinate removed]'s "barrow to the
  south" may be Jack's Castle; C4 B04 and B10 gave UNRESOLVED without CX0928's evidence; C5 size estimates differ;
  C6 to C10 the Q3 label, the Jack's Castle control, the tithe claim, the deer park, the basis of the HER null.
- **New open items:** O12 deer-park extent and features; O13 "Kingsettle Camping Retreat, South Brewham", a
  search-result title in the challenge transcript, not reported or opened, location unknown (a possible modern-use
  context); O14 SANHS 1977 and HER 56089. O1 is resolved for the registered park and 28626; O2 (Wiltshire) and O3
  (MNA192015) are narrowed but open.
- **Correspondence: held** (unchanged, unsent; the owner decides). This covers the Somerset HER Gmail draft, the HE
  five-location Gmail draft, the local R1 letters and the assessor pack. The Somerset HER's locally held prints are no
  reason to revive its draft: HE holds the sortie, and coverage of the lead is unverified.

## Changelog (`changelog`, 28 entries: 3 composition, 18 challenge integration, 7 B10 merge)

**Challenge integration:** snapshot and challenge object; Q3 label kept with reasoning; deer park UNVERIFIABLE and
deer-park readings added; tithe verified as woodland; registered park excluded; Wiltshire failures recorded; HE [coordinate removed]
and [coordinate removed] read; NHLE and AIM rows added; 19476 confirmed; visual HER check marked as such; HM-08 and LT-04 added; Q4
routes revised; Q1 note; O13; correspondence note. **B10 merge:** rows merged and added; SANHS 1977 recorded as
summary-only; 28626 and 53591 resolved from the saved entries; 56089 placed beyond 3 km; Jack's Castle dimensions
confirmed; military reading added; route reclassifications.

## Next checks (post-challenge priorities)

1. **Record precheck:** read SANHS 1977 (page images or OCR) and HER 56089. This is the only route to RECORDED.
2. **Wiltshire & Swindon HER:** retry the 500 m search; it is the main provisional caveat.
3. **Deer park:** McGarvie 1980 and OS card ST 73 SW 9, for the park's extent and any feature at the lead.
4. **Q4 images:** the free HE footprint check for CPE/UK/1924 2260-2261, then APE or ordinary orders (owner approval
   for any charge).
5. **Q1:** detrended profiles and a vegetation-residue test; the product and epoch of the Somerset HER EA lidar layer.
