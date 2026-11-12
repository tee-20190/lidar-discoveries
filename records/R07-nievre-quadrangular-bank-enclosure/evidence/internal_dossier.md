# Current amendment — CAG 58 consulted, 29 September 2026

**The two named commune entries are read; Q4 is answered at book scope.** Q1 LIKELY_REAL,
Q2 UNRESOLVED and Q3 NEARBY_DISTINCT (moderate) remain. The lead stays unvetted and contact
is not ready. Free Chrome consultation succeeds; no library visit or purchase is needed.
[Consultation receipt](cag58_2026-09-29/RESULT.md) records exact pages, comparison limitations
and the OCR correction. JSON rows LT-17–20 supersede the historical CAG access failures.

The conditional Q2 history branch is now applicable. Forest identity and the missing full
plan are already documented in the existing forest-history receipt; naming that gap again
is not progress. Exact archive shelfmark/copy quote remain missing. No correspondence/order,
new position/terrain measurement or archaeological-origin assertion occurred.

The dated narrative below is preserved as history; its unread-CAG and library-only statements
are superseded by this amendment. Prior bytes are in cag58_2026-09-29/dossier_before.json and
DOSSIER_before.md. Neither those files nor the SRA extract is staged for Git.

## Earlier dossier narrative, retained

# L1 lead dossier (lead_vetting_v1.1), 2026-09-29, after the challenge, B11 and the 1827 registration

This summary is private and gives no coordinates. The location is only in `dossier.json` ([internal file]).
It was composed from local files only; no web or browser tool was used. It cites the SRA commune extract, which is
internal-use only: never copy extract contents into a committed file.

- **Snapshots:** `dossier_v1_prechallenge.*` (before the challenge) and `dossier_v2_prechange.*` / `DOSSIER_v2_prechange.md`
  (before the 1827 registration).
- **Receipts:**
  - challenge: `CHALLENGE.md` (transcript sha256 `488d1de6…`, which matches the receipt);
  - research pass B11: [internal file];
  - 1827 registration: `cadastre_1827/RESULT.md`, with its private overlays.

**Validator:** `python [internal file] [internal file] gives class **unvetted**,
0 errors, `contact_ready=false`. The lead stays unvetted because Q2 is UNRESOLVED.

| Question | Before challenge | After challenge and B11 (v2) | Now (after the 1827 plan) |
|---|---|---|---|
| Q1: is the terrain feature real? | LIKELY_REAL | LIKELY_REAL | LIKELY_REAL |
| Q2: is it plausibly archaeological? | UNRESOLVED | UNRESOLVED | **UNRESOLVED**: the boundary and plot-limit explanations are contradicted for 1827 and today; a woodland compound is untested |
| Q3: does it match existing records? | UNRESOLVED | NEARBY_DISTINCT (moderate, provisional) | NEARBY_DISTINCT (moderate, provisional; CAG 58 remains) |

## The 1827 cadastre (HM-20; `cadastre_1827/RESULT.md`)

- **Registration.** Sheet C2 (1:2500) was registered to the modern cadastre with a similarity transform on 14
  control points (commune-limit bends and the apexes of plot 157). RMS is 4.0 m (leave-one-out 5.4 m; affine and
  subset fits 2.5-4.3 m). The error against the LiDAR boundary ditch near the lead is 5-12 m, within the 15 m
  tolerance.
- **Containing plot.** The whole enclosure lies inside **plot C 157 "Les 91 Arpens"**, one undivided wood lot of
  about 37 ha. No separate plot, building, symbol or name is drawn at or next to it.
- **Nearest plot line.** The only plot line within about 75 m is the **commune limit**: 33 m away in the cadastral
  frame (about 22-28 m on the ground), on one side, about 9° off the south side. It is stable at 30.9-33.1 m across
  four models and has not moved since 1827.
- **Lines that are not limits.** Two lines cross the enclosure: a red grid line labelled "Méridienne" and a pencil
  construction band. The east-side linear seen in the LiDAR has no 1827 counterpart.
- **Land use.** Woodland, moderate confidence ("Bois" on the assembly plan; wood names all round). The état de
  sections is not on disk.
- **Decision.** The rule branch is "neither" → **KEEP**.
- **Limits.** A plain area on an ownership plan is weak evidence of absence and does not date the earthwork.

## Q1: LIKELY_REAL

- **Terrain evidence.** A closed angular bank of 88.3 x 71.1 m (maximum span 110.1 m). The west bank is 0.3 m above
  its inner foot and 1.1 m above its outer foot, and the interior slopes.
- **Independent readings.** The challenge agent (Q1-E5, footprint containing 99% of the trace) and B11 (Q1-E6) read
  the same feature on the LiDAR HD hillshade.
- **Why not REAL.** Every view is of one survey product.

## Q2: UNRESOLVED (re-derived from PROTOCOL.md definitions)

| Ordinary explanation | Status | Basis |
|---|---|---|
| Commune-boundary jog | **CONTRADICTED** (1827 and today) | footprint wholly in C0202 (K6); 1827 limit 22-42 m away on one side, course unchanged (HM-20); earlier two-commune hits were bbox artefacts (K6, K7) |
| Cadastral parcel banks and rides | **CONTRADICTED** for ownership limits | no plot limit on any side in 1827 or today; east-side linear post-1827 or non-cadastral; forest-parcel line 22/23 oblique, 35-80 m N |
| Post-medieval plot or pen | **WEAKENED**, not excluded | no such parcel in 1827, plot wooded (moderate); a pen built inside a wood lot is not excluded |
| **Woodland compound** (nursery, game or stock enclosure, forestry works; before or after 1827) | **OPEN, untested**, now the main one | public forest (parcel 23); plan records ownership, not earthworks; post-1827 linear joins the east side; no source documents a compound |
| Charcoal or industry; pits; pond; quarry; kiln; karst | disfavoured | positive angular bank; no pit, face, basin or chamber |
| Military works | OPEN, unsupported | nothing in readable aerials |

- **Why not ORDINARY_EXPLANATION_LIKELY:** nothing documents a compound.
- **Why not PLAUSIBLE:** the compound explanation stands untested, and an explanation weakening is not evidence for
  archaeology.
- **Archaeological reading.** Le Châtelet (Chevrier 2009 site 4) is the same class, with far stronger relief.
- **What would settle Q2:** the forest management plan and forest records (O7), and dating evidence from a field check.

## Q3: NEARBY_DISTINCT (moderate, provisional; unchanged by the 1827 plan)

**Every HIT is distinct by position.**
- Le Châtelet (Chevrier site 4 and Wiki58 (a)): 1,556 m from the published point. The challenger and B11 see a
  visible enclosure 1.49 km away.
- Wiki58 "La Forêt" at 6.2 km and "La Rolande" at 8.0 km ESE, with different forms.
- Mérimée PA00112843 (Chartreuse buildings) at 2,994 m.

**Supporting nulls.** The SRA CAN extract (nearest entity 3,333 m) covers the lead's commune for the whole footprint.
Chevrier's full text has no other entry for either commune. The 1827 plan has no earthwork name.

**Residuals.** CAG 58 is unread (LT-11); a Châteauneuf-Val-de-Bargis extract is a minor check. SCOPED_NULL is barred
because HIT rows exist.

### Ledger by family (58 rows: 31 original, 15 challenge, 11 B11, 1 registration; 7 searches without URL)

| Family | Rows | HIT (all distinct) | SCOPED_NULL | ACCESS_FAILURE |
|---|---|---|---|---|
| national_inventory | 9 | 1 | 4 | 4 |
| regional_record | 4 | 0 | 3 | 1 |
| planning_grey_literature | 3 | 0 | 3 | 0 |
| historic_maps | 20 | 0 | 16 | 4 |
| aerial_index | 8 | 0 | 5 | 3 |
| literature | 14 | 4 | 6 | 4 |

- **New row HM-20.** Local registration of the archives.nievre.fr sheet C2 image; the receipt is
  `cadastre_1827/RESULT.md`. HM-09 and HM-17 are annotated as superseded for the question.
- **Precision.** Screenshot-derived positions carry about ±5 m (footprint corners) or about ±50 m (État-major
  registration). Helper-summarised WFS results are marked; only their counts and IDs are reliable.
- **Earlier corrections kept.** B11 rows are merged as passes where they repeated searches. Its POP Sainte-Colombe
  "zero" is a failed read (C15), and its commune-boundary claim is corrected (C16).

## Q4: the single decision-changing question

**Does the Carte archéologique de la Gaule 58 (Bigeard 1996, print) list an entity for Sainte-Colombe-des-Bois or
Châteauneuf-Val-de-Bargis at or near the lead? Check by lieu-dit ("Les 91 Arpens" / "Quatre-Vingts Arpents", Bois
Volerin, Le Gouleau, Couthion) or by a described enclosure in these woods.**

| Answer | Action |
|---|---|
| An entry fits the lead by lieu-dit or description | Q3 RECORDED: a known-site detection; stop discovery work on L1 |
| All entries lie elsewhere or clearly differ | Q3 stays NEARBY_DISTINCT (may rise to high); next: identify the forest and read its management plan (Q2 test) |
| An entry mentions an unlocated enclosure in these woods | Q3 UNRESOLVED; follow the entry's cited source; an SRA fiche would then face the contact gate |
| No library copy can be consulted | No change; record ACCESS_FAILURE; go on to the management plan |

- **Route.** A library copy. CAG 58 is a published book, so this is a library route, not a custodian contact.
  **Contact: not justified** (gate conditions 1 and 2 fail).
- **Next.** (1) CAG 58 in a library. (2) If Q3 holds: identify the forest (Sainte-Colombe communal or Bellary state)
  and read its management plan through public routes. Only an unpublished specific plan would make an ONF or commune
  request a gate candidate. (3) A field check paired with Le Châtelet, at the owner's decision.
- **History (`q4.question_history`).**
  - v1: the boundary question; its present-day half was answered by the challenge and K6.
  - v2: the 1827 plan, answered with the "neither" → KEEP branch.

## Challenge pass (unchanged)

- **Run.** Phase 1 (blind) reached NEARBY_DISTINCT in 43 of 45 calls; phase 2 used 30 of 30. No disallowed tools.
- **Procedural note (minor).** Two phase-1 calls went to a guessed tab id and failed harmlessly.
- **Disagreements** (`challenge_disagreements`): the path strip is partly a 10 m cadastral misfit (C11); the E0717
  envelope detail is wrong, though the artefact conclusion stands (C12); "non-wooded" is contested and the 1827 plan
  now favours wooded (C10); the 1827 sheets were already local; SCOPED_NULL is impossible because HITs exist.
- **Partly withdrawn.** My own "parallel" against the challenger's "oblique": both overstate. The angle is 3-9° by
  method (C13).

## Changelog (`changelog`, 33 entries: 15 challenge, 7 B11, 11 registration)

**Registration entries:** (1) Q4 v2 answered: KEEP, plot C 157, no limit on any side; (2) boundary jog contradicted
for 1827; (3) cadastral banks contradicted for 1827, and the east-side linear is post-1827 or non-cadastral;
(4) post-medieval plot or pen weakened; (5) woodland compound now the main untested explanation, Q2 stays
UNRESOLVED; (6) K6 "parallel" withdrawn: 3-9° (C13); (7) C10 gains the 1827 "wooded" evidence, O15 narrowed; (8) O14:
a boundary ditch is seen 5-12 m from the registered limit; (9) Q3's 1827-name residual resolved, Q3 unchanged;
(10) Q4 replaced by the CAG 58 question; (11) HM-20 added, HM-09 and HM-17 annotated, O1 and O5 closed, and the
Méridienne and pencil lines recorded as non-limits.

## Open items and conflicts (full lists in `open_items`, `conflicts`)

- **Closed:** O1 (no limit on any side), O3 (Wiki58 positions), O5 (sheet registered), O11 (État-major line).
- **Narrowed:** O2 (minor Châteauneuf residual), O4 (CAG 58 only), O14 (boundary ditch seen) and O15 (1827
  woodland; the État-major was not re-read).
- **Open:** O6 no aerial frame viewed; O7 forest identity and management plan (the next Q2 test); O8 Atlas, BSR,
  ADLFI; O9 no second Q1 source; O13 Le Châtelet's position against Chevrier's point.
- **Conflicts.** C10 (land use; 1827 favours wooded), C11 (double line), C12 (E0717 envelope), C13 (angle 3-9°),
  C14 (1950-65 reading; 1827 does not settle it), C15 (POP zero), C16 (B11's boundary claim), C17 (SW dotted line).
  C1 and C2 are resolved.

## Correspondence: held (unchanged)

- **Local drafts mentioning L1 (4):** [internal file], and under
  [internal file]: `SRA_REPLY_DRAFT.md`, `SRA_REPLY_DRAFT_VARIANT_B.md` and
  `SRA_REPLY_DRAFT_A2_2026-09-26.md`.
- **Live Gmail SRA draft.** It was revised to L2 only on 2026-09-28 (not re-checked here).
- None was edited, sent or withdrawn; the owner decides. Nothing about L1 has been sent.

## Residual attack surface

1. **CAG 58 (Q4).** The only unread inventory that could make Q3 RECORDED.
2. **Forest history.** Which forest holds the lead, and whether its management plan or records place a nursery,
   pen or compound here. This is the test that could drop the lead through Q2.
3. **The registration itself.** It rests on the modern cadastre, which has a 10 m misfit between the communes, and on
   reading the LiDAR ditch as the physical boundary. A 15 m error would not change the "neither" branch: the nearest
   limit is still 22 m or more away and on one side only.
4. **Dating.** Nothing yet dates the earthwork. The plan shows only that no ownership plot matched it in 1827.

## Bounded ONF source check, 29 September 2026

Bellary state forest F25196B, parcel 23 is confirmed by actual polygon containment (FH-01). The two available management orders were read in full (FH-02); they do not locate or date the enclosure. Q1/Q2/Q3 and the CAG 58 question remain unchanged. See [forest-history receipt](forest_history_2026-09-29/RESULT.md).
