# FR2-S13 lead dossier (lead_vetting_v1.1), 2026-10-02, before the challenge pass

Private summary without coordinates; the location is only in `dossier.json` ([internal file]).

**Validator:** `python [internal file] [internal file] gives class **unvetted**, 0 errors, `contact_ready=false`.

Commune: Garchy (58122). Review codes: N092. Feature: Round mound about 19 m across at half height and 1.0-1.35 m high in broadleaf woodland, with pits 40-70 m to the south-west.

| Question | Status | Basis (first sentence) |
|---|---|---|
| Q1: is the terrain feature real? | LIKELY_REAL | A compact round mound with a steep core stands clear of the slope in renders and four profiles of one IGN LiDAR HD DTM (leaf-off flight). |
| Q2: is it plausibly archaeological? | PLAUSIBLE | A compact round mound fits a tumulus or the rubble of a small building; the lieu-dit Les Chazeaux (87 m; a name often derived from old buildings) and BD TOPO ruins (138 m) point to former buildings nearby. |
| Q3: does it match existing records? | NEARBY_DISTINCT | Positioned records are distinct: the SRA site list reproduced in the commune carte communale (2017) names nine sites, the nearest being Les Saules (Gallo-Roman occupation, 1.2 km) and the Vallee du Bois Mollet anomalies (1.4 km); the CAG 58 items of the commune are 4.9 km away or finds without a findspot (two bronze bracelets). |

## Q1: LIKELY_REAL

A compact round mound with a steep core stands clear of the slope in renders and four profiles of one IGN LiDAR HD DTM (leaf-off flight). Orthophotos are non-diagnostic under canopy (canopy height about 18-20 m), so REAL is not earned.

- **Q1-E1** (records-screen render: multi-direction hillshade, hillshade 315/25, local relief and residual from an annulus plane): Isolated round mound with a steep core and a faint skirt; pits or hollows lie 40-70 m to the south-west and south.
- **Q1-E2** (four detrended profiles (0, 45, 90, 135 deg), refined-centre profiles and a 1 m radial profile): Detrended DTM values within 22 m: radial mean about the review mark +0.67 m at the centre, half height at 9.5 m radius, lowest -0.01 m at 26.5 m; S-N (refined centre): centre +1.27 m, highest +1.34 m at -1 m, lowest +0.28 m at +21 m; W-E (refined centre): centre +1.02 m, highest +1.14 m at +2 m, lowest +0.11 m at -22 m; SW-NE: centre +0.73 m, highest +0.86 m at +2 m, lowest +0.24 m at +21 m; NW-SE: centre +1.35 m, highest +1.63 m at -4 m, lowest +0.50 m at -20 m.
- **Q1-E3** (canopy height within 5 m and 30 m of the lead): MNH within 5 m: mean 17.53 m, max 28.71 m; within 30 m: mean 19.47 m, 88 % above 2 m.
- **Q1-E4** (300 m and 100 m windows centred on the lead): Woodland in 1957, 2002 and 2023; the mound cannot be seen; non-diagnostic.

Dimensions: {"half_height_diameter_m": 19.0, "base_diameter_m": 38.0, "height_above_trend_m": 1.25}

## Q2: PLAUSIBLE

A compact round mound fits a tumulus or the rubble of a small building; the lieu-dit Les Chazeaux (87 m; a name often derived from old buildings) and BD TOPO ruins (138 m) point to former buildings nearby. The spot was open land on the etat-major map, beside a road, and wooded by 1949, so spoil from the nearby pits and clearance remain open.

| Ordinary explanation | For | Against | Status |
|---|---|---|---|
| spoil from the pits 40-70 m south-west | Pits and hollows nearby. | The mound is separated from the pits by about 40 m. | OPEN |
| rubble of a ruined building | Les Chazeaux and BD TOPO ruins nearby. | No building at the spot on the etat-major map or the 1949 map. | OPEN |
| field-clearance cairn | Open land in the 19th century. | A single mound 1.25 m high. | OPEN |
| vegetation residue in the DTM | Tall canopy. | Smooth convex form in four profiles from a leaf-off flight. | DISFAVOURED |

## Q3: NEARBY_DISTINCT

Positioned records are distinct: the SRA site list reproduced in the commune carte communale (2017) names nine sites, the nearest being Les Saules (Gallo-Roman occupation, 1.2 km) and the Vallee du Bois Mollet anomalies (1.4 km); the CAG 58 items of the commune are 4.9 km away or finds without a findspot (two bronze bracelets). The neighbouring commune boundary is 94 m away; its unpositioned CAG item (La Colline, a tumuliform stone heap) is assigned to that commune, not to this one. The CAN remains restricted.

| Family | Rows |
|---|---|
| national_inventory | NI-01 SCOPED_NULL; NI-02 ACCESS_FAILURE |
| regional_record | RR-01 HIT; RR-02 ACCESS_FAILURE; RR-03 ACCESS_FAILURE |
| planning_grey_literature | PL-01 SCOPED_NULL; PL-02 SCOPED_NULL; PL-03 SCOPED_NULL; PL-04 SCOPED_NULL; PL-06 ACCESS_FAILURE; PL-07 ACCESS_FAILURE |
| historic_maps | HM-01 SCOPED_NULL; HM-02 SCOPED_NULL; HM-03 SCOPED_NULL; HM-04 SCOPED_NULL; HM-05 SCOPED_NULL |
| aerial_index | AI-01 SCOPED_NULL; AI-02 SCOPED_NULL; AI-03 SCOPED_NULL; AI-04 SCOPED_NULL; AI-05 ACCESS_FAILURE; AI-06 SCOPED_NULL |
| literature | LT-01 HIT; LT-02 SCOPED_NULL; LT-03 SCOPED_NULL; LT-04 SCOPED_NULL; LT-05 SCOPED_NULL; LT-06 SCOPED_NULL; LT-07 SCOPED_NULL; LT-08 SCOPED_NULL; LT-09 ACCESS_FAILURE; LT-10 SCOPED_NULL; LT-12 ACCESS_FAILURE |

| Row | Source | Outcome | Note |
|---|---|---|---|
| NI-01 | Ministry of Culture Merimee dataset (local copy [internal file], sha256 65c493db...) | SCOPED_NULL | No record within 2 km; nearest record in the five communes: PA00112989 (chapelle, commune 58215) at 4,138 m. Merimee holds protected monuments and inventory files, not the Carte archeologique nationale. |
| NI-02 | Carte archeologique nationale (Patriarche), Ministry of Culture / SRA Bourgogne-Franche-Comte | ACCESS_FAILURE | The CAN is restricted; the project holds no SRA extract for this commune. A blank public query never establishes absence from the CAN. |
| RR-01 | SRA site list reproduced in the Garchy carte communale (approved 2017-09-27), rapport pp. 30-31 ("Patrimoine archeologique") with its map | HIT (Garchy SRA list site 1, Les Saules: Gallo-Roman occupation; 1217 m; distinct) | The lead lies at the western tip of the commune, outside every mapped site; Vallee du Bois Mollet (7) 1.4 km; all others 2.9 km or more. |
| RR-02 | SRA Bourgogne-Franche-Comte commune extract of the CAN | ACCESS_FAILURE | The project holds an SRA extract for another commune only (2026-09-10); none for this commune. Not requested here (no correspondence in this pass). |
| RR-03 | Archaeological presumption zones (ZPPA): IGN Geoplateforme WFS catalogue and Atlas des patrimoines | ACCESS_FAILURE | The only ZPPA layer in the national WFS catalogue is zppa_cvl_executoire_2025 (Centre-Val de Loire), which does not cover the Nievre. |
| PL-01 | Carte communale of Garchy (DU_58122, approved 2017-09-27): rapport de presentation (GPU) | SCOPED_NULL | Only the archaeology section (RR-01) concerns sites. |
| PL-02 | IGN API Carto GPU module: document, zone and sector at the lead | SCOPED_NULL | CC 58122_CC_20170927 applies; zone or sector N; no archaeological zone or prescription at the point. |
| PL-03 | IGN API Carto GPU module: servitudes, information and prescription layers | SCOPED_NULL | Features within 200 m: espace boisé classé. No heritage servitude (AC1/AC4), archaeological information zone or heritage prescription. |
| PL-04 | IGN API Carto GPU module: zones, information and prescriptions within 1.5 km | SCOPED_NULL | No archaeology-flagged zone or information layer within 1.5 km. Prescriptions and information features: espace boisé classé (87 m). Each endpoint was queried with the 1.5 km buffer geometry; responses are hashed in the GPU_WIDE log. |
| PL-06 | ADLFI (Archeologie de la France - Informations) notices through the OpenEdition search | ACCESS_FAILURE | The search URL returned a redirect to an empty results shell, as recorded in FR-DISC-1; one attempt only. |
| PL-07 | Inrap Dolia digital library (operation reports) | ACCESS_FAILURE | HTTP 403 with a JavaScript challenge page; one attempt only; no bot check was attempted. |
| HM-01 | Cassini map (BnF copy) via IGN WMS-R (BNF-IGNF_GEOGRAPHICALGRIDSYSTEMS.CASSINI) | SCOPED_NULL | Open sloping land at the lead; nothing at the lead. |
| HM-02 | Carte de l etat-major 1:40,000 (1820-1866) via IGN WMS-R (GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40) | SCOPED_NULL | The label "le Chaz[eaux]" runs across the spot and a road passes about 30 m west; open land; no building at the lead. |
| HM-03 | IGN 1:50,000 type-1922 map (SCAN50 1950 layer) via WMS-R | SCOPED_NULL | Woodland (wooded by 1949); a road about 20-25 m north; label "...eaux"; nothing at the lead. |
| HM-04 | Etalab/DGFiP cadastre lieux-dits (open data, 2026-06-01 edition) | SCOPED_NULL | Containing lieu-dit: LES TAILLES DU CORBIER. Nearby: LES CHAMPS DE LA METAIRIE 47 m, LES CHAZEAUX 87 m, LES TAILLES DU CORBIER 164 m, LES TERRES ROUGES 168 m, CHAMPS DE LA METAIRIE 274 m, CHAMP DU LAC 326 m. Les Chazeaux 87 m (neighbouring commune), Champ du Lac 326 m, Les Bois du Lac 399 m; no earthwork name. |
| HM-05 | IGN BD TOPO toponymie, lieux-dits, zones of interest, constructions and water (Geoplateforme WFS) | SCOPED_NULL | Ruins (construction lineaire) 138 m; Les Chazeaux hamlet 176 m; a "Tombeau" (zone of interest, unnamed) 395 m; no earthwork name. |
| AI-01 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R) with its WFS mosaic graph | SCOPED_NULL | Woodland; the mound cannot be seen: non-diagnostic. Registered to the current orthophoto at the 1 km scale: offset 4.0 m (phase correlation, peak/median 25.5); the 300 m correlation (3.6 m) is not used because land cover changed; BD TOPO roads overlaid on the 1 km view follow the visible roads at display scale (about 1 m/px). The graph gives a date range, not the exposure date of the mosaicked frame; mission scale 1:25,000 from the mission name; native ground resolution not read from metadata. |
| AI-02 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), 1 km context with BD TOPO roads and the parcel overlaid | SCOPED_NULL | Used for registration against the current orthophoto (1 km phase correlation offset 4.0 m) and land-use context. |
| AI-03 | IGN orthophotos ORTHOIMAGERY.ORTHOPHOTOS2000-2005 (WMS-R) | SCOPED_NULL | Closed canopy: non-diagnostic. |
| AI-04 | IGN current orthophoto ORTHOIMAGERY.ORTHOPHOTOS and colour-infrared ORTHOIMAGERY.ORTHOPHOTOS.IRC (WMS-R) | SCOPED_NULL | Closed canopy: non-diagnostic. |
| AI-05 | IGN historical orthomosaics ORTHOIMAGERY.ORTHOPHOTOS.1965-1980 and .1980-1995 (WMS-R) | ACCESS_FAILURE | HTTP 200 but blank near-white images (pixel standard deviation below 2) for both layers; the 1980-1995 graph returned no polygon. |
| AI-06 | IGN national aerial photograph frame index (Geoplateforme WFS pva:image) | SCOPED_NULL | 118 frames listed, 1949-2017; frames before 1966 dated 1949-06-22, 1957-04-22, 1961-05-30. Coverage metadata only: no individual frame was viewed. |
| LT-01 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), Garchy entry (commune 122), Gallica ContentSearch | HIT (CAG 58, Garchy 1*: rectangular enclosure (about 100 x 60 m) with, in its south-east corner, a pit or levelled tumulus (diam. about 50 m), Les Jarry (A. Bouthier, aerial 1995); 4890 m; distinct) | Also: two bronze bracelets found in the commune without a findspot. Excerpt-level read. |
| LT-02 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), full-text search through the Gallica ContentSearch service | SCOPED_NULL | Chazeaux and Corbier: only bibliography false matches; the commune entry (p. 179) holds Les Jarry and two bracelets without findspot. |
| LT-03 | Bouthier A., L occupation du Nord-Ouest du Nivernais aux epoques protohistoriques vue d avion (B@sic 1, UNA editions), HTML and PDF (FR-DISC-1 local copies) | SCOPED_NULL | Garchy: 1 enceinte in the commune inventory; no woodland tumulus for the commune. |
| LT-04 | Chevrier S. 2009, Les enceintes pre-medievales du Nivernais-Morvan, Revue archeologique de l Est 58 (OpenEdition) | SCOPED_NULL | No catalogue site in the commune of the lead. |
| LT-05 | Camosine, index of communes of the Nievre in the Annales des Pays Nivernais | SCOPED_NULL | No archaeology entry naming the locality of the lead. |
| LT-06 | terres-et-seigneurs-en-donziais.fr: fief notice Garchy (?p=5316) | SCOPED_NULL | Fiefs Montclavin, La Barre and Boisrond; none at this lead (La Barre 2.5 km from FR2-S10). |
| LT-07 | HAL open archive search API | SCOPED_NULL | No deposit on earthworks in these communes: 0 hits for Arquian, Alligny-Cosne, Saint-Loup-des-Bois and Argenoux; Garchy hits are papers of the geophysics research centre there; the Pouilly query hits are unrelated. |
| LT-08 | Persee full-text portal search | SCOPED_NULL | Relevant items only: the Gallia 1981 Bourgogne chronicle (ironworking traces in three of the communes, no earthworks or positions); Bouthier 1999 on fossil field systems of the Nohain valley; Gallia prehistoire 1974 index. None concerns an earthwork at this lead. |
| LT-09 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795): Gallica page view (texteBrut) of commune entry pages | ACCESS_FAILURE | Redirected to the Gallica security check; not attempted further. Full pages need an ordinary browser session. |
| LT-10 | CECAB, Chateaux forts de la Nievre (list of medieval castles and mottes) | SCOPED_NULL | None of the five communes is listed. |
| LT-12 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), entry of the neighbouring commune Pouilly-sur-Loire (215), Gallica ContentSearch | ACCESS_FAILURE | Item 1*: at La Colline a tumuliform stone heap yielded a broken bronze torc (information A. Bouthier). The item exists but cannot be positioned; it is assigned to the neighbouring commune, whose boundary is 94 m from the lead. |

## Q4

**Question:** Does the Carte archeologique nationale hold a tumulus, a ruin or a quarry at this woodland spot?

Changes: keep as a candidate for a qualified assessment versus drop.

- A CAN entity is here -> Q3 RECORDED: detection of a known site
- Nothing recorded here and no ordinary explanation found -> keep; candidate for the questions-only SRA letter after the challenge pass
- The pits and mound are shown to be quarry spoil -> Q2 ORDINARY_EXPLANATION_LIKELY: drop

Answerable by: SRA Bourgogne-Franche-Comte (CAN); public first: the 1830s cadastre of the commune.

Next action: 1. Independent challenge pass. 2. Check the 1830s cadastre for a building or quarry at the spot. 3. If unmatched, candidate for the questions-only SRA letter. No correspondence in this pass.

Outstanding public routes: 1830s cadastre of the commune (AD Nievre); Gallica page view of the CAG 58 entry (security check).

Contact gate: 1_public_routes_exhausted: fails: public routes remain; 2_specific_custodian_item: not yet identified; 3_answers_lead_to_different_actions: holds; 4_not_answered_duplicated_or_opinion: holds for a precise record question; 5_challenge_receipt: fails: the challenge pass has not run.

## Dated imagery (IGN 1950-1965)

Covered. Mosaic source mission 1957_F 2523-2623_P_25000 (1:25,000), graph dates 1957-04-05 to 1957-04-22 (a range, not an exposure date); viewed at 0.5 m/px (300 m) and 1 m/px (1 km); registered to the current orthophoto at the 1 km scale: offset 4.0 m (phase correlation, peak/median 25.5); the 300 m correlation (3.6 m) is not used because land cover changed; BD TOPO roads overlaid on the 1 km view follow the visible roads at display scale (about 1 m/px). Target: Woodland; the mound cannot be seen: non-diagnostic. Frame index: 3 dates before 1966 (1949-06-22, 1957-04-22, 1961-05-30), frames not viewed. Access limits: the 1965-1980 and 1980-1995 mosaics are blank; native ground resolution not read from metadata.

## Challenge priorities

- Test the quarry-spoil reading against the pit cluster in the DTM.
- Check the 1830s cadastre for buildings at Les Chazeaux.
- Identify the BD TOPO "Tombeau" 395 m away.

Correspondence: none. No contact in this pass.

## Challenge pass (2026-10-02, Claude Opus 5.5 challenge agent): SURVIVES

No prior record was found at the mound. Independent registration of the 2017 carte communale map puts every listed
site 1.0 km or more away; the CeCaB fortified-site inventory has nothing within 4.0 km (CH-RR-01); Atlas des
patrimoines ZPPA, MH, AC1 and SPR layers are empty within 3 km (CH-RR-03, CH-NI-01). The outstanding 1830s cadastre
route is closed: Garchy section A sheet 11 shows the Chazot farm and fields, nothing at the lead (CH-HM-01). The
CAG "La Colline" cairn (Pouilly-sur-Loire 1*) still cannot be positioned (CH-HM-02), so NEARBY_DISTINCT rests on its
commune attribution. Correction notes on LT-10 (wrong CeCaB page) and RR-03 (Atlas reachable over http). Validator
class after the challenge: **vetted**, 0 errors, contact_ready=false. The single CAN question for the SRA is in
[internal file] and `q4.sra_question_from_challenge`. A vetted lead is still an unconfirmed lead.
