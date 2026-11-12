# FR2-S26 lead dossier (lead_vetting_v1.1), 2026-10-02, before the challenge pass

Private summary without coordinates; the location is only in `dossier.json` ([internal file]).

**Validator:** `python [internal file] [internal file] gives class **unvetted**, 0 errors, `contact_ready=false`.

Commune: Pouilly-sur-Loire (58215). Review codes: N183. Feature: Compact round mound about 20-25 m across and 1.0-1.3 m high in mixed woodland.

| Question | Status | Basis (first sentence) |
|---|---|---|
| Q1: is the terrain feature real? | LIKELY_REAL | A compact convex mound stands clear of the surrounding gentle slope in renders and four profiles of one IGN LiDAR HD DTM (leaf-off flight). |
| Q2: is it plausibly archaeological? | PLAUSIBLE | A compact round mound fits a tumulus. |
| Q3: does it match existing records? | UNRESOLVED | The tumuliform stone heap of La Colline (CAG 58, commune entry 1*) cannot be positioned: the name is absent from the current cadastre of the commune and from BD TOPO within 1.5 km. |

## Q1: LIKELY_REAL

A compact convex mound stands clear of the surrounding gentle slope in renders and four profiles of one IGN LiDAR HD DTM (leaf-off flight). Orthophotos are non-diagnostic under canopy (canopy height about 6-8 m), so REAL is not earned.

- **Q1-E1** (records-screen render: multi-direction hillshade, hillshade 315/25, local relief and residual from an annulus plane): Isolated compact mound with a smooth convex crown and a low skirt.
- **Q1-E2** (four detrended profiles (0, 45, 90, 135 deg), refined-centre profiles and a 1 m radial profile): Detrended DTM values within 22 m: radial mean about the review mark +0.93 m at the centre, half height at 8.5 m radius, lowest +0.00 m at 26.5 m; S-N (refined centre): centre +1.18 m, highest +1.29 m at +2 m, lowest +0.16 m at -19 m; W-E (refined centre): centre +1.04 m, highest +1.11 m at -1 m, lowest +0.03 m at -20 m; SW-NE: centre +0.94 m, highest +0.95 m at +1 m, lowest +0.01 m at -18 m; NW-SE: centre +1.34 m, highest +1.44 m at -3 m, lowest +0.24 m at -22 m.
- **Q1-E3** (canopy height within 5 m and 30 m of the lead): MNH within 5 m: mean 6.04 m, max 11.19 m; within 30 m: mean 8.04 m, 97 % above 2 m.
- **Q1-E4** (300 m and 100 m windows centred on the lead): 1957: young plantation or open woodland in regular rows; 2002 and 2023: canopy; the mound cannot be seen; non-diagnostic.

Dimensions: {"base_diameter_m": 25.0, "height_above_trend_m": 1.2}

## Q2: PLAUSIBLE

A compact round mound fits a tumulus. CAG 58 records for this commune, at an unpositioned place called La Colline, a tumuliform stone heap ("pierrier tumuliforme") that yielded a broken bronze torc; Bouthier reports Hallstatt dry-stone tumuli in woods of the Nohain valley. The spot was open land on Cassini and the etat-major map and wooded by 1949, so field clearance and estate features (La Faisanderie 94 m, Le Colombier 133 m) remain open.

| Ordinary explanation | For | Against | Status |
|---|---|---|---|
| field-clearance cairn from former cultivation | Open land on Cassini and the etat-major map; plantation rows in 1957. | A single compact mound 1.2 m high. | OPEN |
| estate or hunting feature (ice-house, pheasantry mound, belvedere) | Lieux-dits La Faisanderie (94 m) and Le Colombier (133 m). | No structure or name at the spot on any map. | OPEN |
| spoil or dump heap | Possible near a track. | No quarry or pit mapped within 400 m (BD TOPO, historic maps). | DISFAVOURED |
| vegetation residue in the DTM | Canopy over the spot. | Smooth convex form in four profiles from a leaf-off flight. | DISFAVOURED |

## Q3: UNRESOLVED

The tumuliform stone heap of La Colline (CAG 58, commune entry 1*) cannot be positioned: the name is absent from the current cadastre of the commune and from BD TOPO within 1.5 km. Positioned records are distinct (SRA list in the neighbouring carte communale: Vallee du Bois Mollet anomalies and irregular enclosure, 0.69 km). The CAN is restricted.

| Family | Rows |
|---|---|
| national_inventory | NI-01 SCOPED_NULL; NI-02 ACCESS_FAILURE |
| regional_record | RR-01 HIT; RR-02 ACCESS_FAILURE; RR-03 ACCESS_FAILURE |
| planning_grey_literature | PL-01 SCOPED_NULL; PL-02 SCOPED_NULL; PL-03 SCOPED_NULL; PL-04 SCOPED_NULL; PL-06 ACCESS_FAILURE; PL-07 ACCESS_FAILURE |
| historic_maps | HM-01 SCOPED_NULL; HM-02 SCOPED_NULL; HM-03 SCOPED_NULL; HM-04 SCOPED_NULL; HM-05 SCOPED_NULL; HM-06 SCOPED_NULL |
| aerial_index | AI-01 SCOPED_NULL; AI-02 SCOPED_NULL; AI-03 SCOPED_NULL; AI-04 SCOPED_NULL; AI-05 ACCESS_FAILURE; AI-06 SCOPED_NULL |
| literature | LT-01 ACCESS_FAILURE; LT-02 SCOPED_NULL; LT-03 SCOPED_NULL; LT-04 SCOPED_NULL; LT-05 SCOPED_NULL; LT-07 SCOPED_NULL; LT-08 SCOPED_NULL; LT-09 ACCESS_FAILURE; LT-10 SCOPED_NULL |

| Row | Source | Outcome | Note |
|---|---|---|---|
| NI-01 | Ministry of Culture Merimee dataset (local copy [internal file], sha256 65c493db...) | SCOPED_NULL | No record within 2 km; nearest record in the five communes: PA00112894 (église, commune 58122) at 4,187 m. Merimee holds protected monuments and inventory files, not the Carte archeologique nationale. |
| NI-02 | Carte archeologique nationale (Patriarche), Ministry of Culture / SRA Bourgogne-Franche-Comte | ACCESS_FAILURE | The CAN is restricted; the project holds no SRA extract for this commune. A blank public query never establishes absence from the CAN. |
| RR-01 | SRA site list and map in the neighbouring Garchy carte communale (2017), rapport pp. 30-31 | HIT (Garchy SRA list site 7, La Vallee du Bois Mollet: numerous anomalies including an irregular enclosure; 692 m; distinct) | Aerial anomalies in fields of the neighbouring commune; distinct from a woodland mound. Les Saules (site 1) 1.35 km. |
| RR-02 | SRA Bourgogne-Franche-Comte commune extract of the CAN | ACCESS_FAILURE | The project holds an SRA extract for another commune only (2026-09-10); none for this commune. Not requested here (no correspondence in this pass). |
| RR-03 | Archaeological presumption zones (ZPPA): IGN Geoplateforme WFS catalogue and Atlas des patrimoines | ACCESS_FAILURE | The only ZPPA layer in the national WFS catalogue is zppa_cvl_executoire_2025 (Centre-Val de Loire), which does not cover the Nievre. |
| PL-01 | PLU of Pouilly-sur-Loire (DU_58215): rapports 2025-11-06 (text) and 2002-09-17 (scan; Windows OCR); 2006 and 2012 rapports and the PADD (scans, no text layer) | SCOPED_NULL | No archaeology section in either report; La Faisanderie appears only as a farm in the landscape chapter (2002). The 2006 and 2012 rapports and the PADD were not OCRed. |
| PL-02 | IGN API Carto GPU module: document, zone and sector at the lead | SCOPED_NULL | PLU 58215_PLU_20251106 applies; zone or sector A; no archaeological zone or prescription at the point. |
| PL-03 | IGN API Carto GPU module: servitudes, information and prescription layers | SCOPED_NULL | Features within 200 m: Batiment susceptible de changer de destination; espace boisé classé. No heritage servitude (AC1/AC4), archaeological information zone or heritage prescription. |
| PL-04 | IGN API Carto GPU module: zones, information and prescriptions within 1.5 km | SCOPED_NULL | No archaeology-flagged zone or information layer within 1.5 km. Prescriptions and information features: Batiment susceptible de changer de destination (129 m); espace boisé classé (0 m). Each endpoint was queried with the 1.5 km buffer geometry; responses are hashed in the GPU_WIDE log. |
| PL-06 | ADLFI (Archeologie de la France - Informations) notices through the OpenEdition search | ACCESS_FAILURE | The search URL returned a redirect to an empty results shell, as recorded in FR-DISC-1; one attempt only. |
| PL-07 | Inrap Dolia digital library (operation reports) | ACCESS_FAILURE | HTTP 403 with a JavaScript challenge page; one attempt only; no bot check was attempted. |
| HM-01 | Cassini map (BnF copy) via IGN WMS-R (BNF-IGNF_GEOGRAPHICALGRIDSYSTEMS.CASSINI) | SCOPED_NULL | Blank open land at the lead; "le Colom[bier]" with a building symbol about 250-300 m south-east. |
| HM-02 | Carte de l etat-major 1:40,000 (1820-1866) via IGN WMS-R (GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40) | SCOPED_NULL | Open sloping land (no woodland symbol) at the lead; nothing at the lead. |
| HM-03 | IGN 1:50,000 type-1922 map (SCAN50 1950 layer) via WMS-R | SCOPED_NULL | Woodland (wooded by 1949) with a path nearby; nothing at the lead. |
| HM-04 | Etalab/DGFiP cadastre lieux-dits (open data, 2026-06-01 edition) | SCOPED_NULL | Containing lieu-dit: LE BOIS MIGNON. Nearby: LA FAISANDERIE 94 m, LE COLOMBIER 133 m, LA PETITE CHAUME 332 m, CHAUMES AUX DEMOISELLES 370 m, LA CHARNAIE 395 m, LA CHAUME DES GALLETAS 510 m. La Faisanderie 94 m, Le Colombier 133 m; no motte, butte, tertre or tumulus name; La Colline (CAG) is absent from the current cadastre of the commune. |
| HM-05 | IGN BD TOPO toponymie, lieux-dits, zones of interest, constructions and water (Geoplateforme WFS) | SCOPED_NULL | Bois Mignon 93 m; La Faisanderie hamlet 142 m; Le Colombier wood 543 m; no earthwork name. |
| HM-06 | Cadastre napoleonien of Pouilly-sur-Loire (1849): tableau d assemblage (AD Nievre 3PPLANS/215/1) | SCOPED_NULL | The overview names sections (A des Loges, B du Nozet, C du Bouchot, D de la Metairie Buchot, E de Charenton, F de Pouilly) and hamlets; Le Colombier and La Metairie Buchot lie in section D near the lead. La Colline is not named at this scale; the section sheets (3PPLANS/215/2-42) carry field names and were not read. |
| AI-01 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R) with its WFS mosaic graph | SCOPED_NULL | Young plantation or open woodland in rows; the mound cannot be seen: non-diagnostic. Registration not established: 1 km phase correlation gave 34.0 m (peak/median 12.3); the 300 m correlation (49.7 m) is not used because land cover changed; BD TOPO roads overlaid on the 1 km view follow the visible roads at display scale (about 1 m/px). The graph gives a date range, not the exposure date of the mosaicked frame; mission scale 1:25,000 from the mission name; native ground resolution not read from metadata. |
| AI-02 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), 1 km context with BD TOPO roads and the parcel overlaid | SCOPED_NULL | Used for registration against the current orthophoto (1 km phase correlation offset 34.0 m) and land-use context. |
| AI-03 | IGN orthophotos ORTHOIMAGERY.ORTHOPHOTOS2000-2005 (WMS-R) | SCOPED_NULL | Canopy: non-diagnostic. |
| AI-04 | IGN current orthophoto ORTHOIMAGERY.ORTHOPHOTOS and colour-infrared ORTHOIMAGERY.ORTHOPHOTOS.IRC (WMS-R) | SCOPED_NULL | Canopy: non-diagnostic. |
| AI-05 | IGN historical orthomosaics ORTHOIMAGERY.ORTHOPHOTOS.1965-1980 and .1980-1995 (WMS-R) | ACCESS_FAILURE | HTTP 200 but blank near-white images (pixel standard deviation below 2) for both layers; the 1980-1995 graph returned no polygon. |
| AI-06 | IGN national aerial photograph frame index (Geoplateforme WFS pva:image) | SCOPED_NULL | 96 frames listed, 1949-2017; frames before 1966 dated 1949-06-22, 1957-04-22, 1961-05-30. Coverage metadata only: no individual frame was viewed. |
| LT-01 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), Pouilly-sur-Loire entry (commune 215), Gallica ContentSearch | ACCESS_FAILURE | Item 1*: at La Colline a tumuliform stone heap yielded a broken bronze torc (information A. Bouthier). The record exists but cannot be positioned; a tumuliform heap is the same form class as this lead. Other items: the ancient road beside the Loire and the question of an ancient settlement at the bourg (4*). |
| LT-02 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), full-text search through the Gallica ContentSearch service | SCOPED_NULL | Mignon and Faisanderie: 0 items; Colombier matches only other communes; Colline and pierrier return the commune item 1* (LT-01) and items of other communes. |
| LT-03 | Bouthier A., L occupation du Nord-Ouest du Nivernais aux epoques protohistoriques vue d avion (B@sic 1, UNA editions), HTML and PDF (FR-DISC-1 local copies) | SCOPED_NULL | Pouilly-sur-Loire: 2 enceintes on one site and 1 circular enclosure (aerial, unpositioned); no woodland tumulus for the commune. |
| LT-04 | Chevrier S. 2009, Les enceintes pre-medievales du Nivernais-Morvan, Revue archeologique de l Est 58 (OpenEdition) | SCOPED_NULL | No catalogue site in the commune of the lead. |
| LT-05 | Camosine, index of communes of the Nievre in the Annales des Pays Nivernais | SCOPED_NULL | Pouilly-sur-Loire: "Archeologie gallo-romaine" (48, p. 7; not read, no locality given); nothing for this woodland. |
| LT-07 | HAL open archive search API | SCOPED_NULL | No deposit on earthworks in these communes: 0 hits for Arquian, Alligny-Cosne, Saint-Loup-des-Bois and Argenoux; Garchy hits are papers of the geophysics research centre there; the Pouilly query hits are unrelated. |
| LT-08 | Persee full-text portal search | SCOPED_NULL | Relevant items only: the Gallia 1981 Bourgogne chronicle (ironworking traces in three of the communes, no earthworks or positions); Bouthier 1999 on fossil field systems of the Nohain valley; Gallia prehistoire 1974 index. None concerns an earthwork at this lead. |
| LT-09 | Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795): Gallica page view (texteBrut) of commune entry pages | ACCESS_FAILURE | Redirected to the Gallica security check; not attempted further. Full pages need an ordinary browser session. |
| LT-10 | CECAB, Chateaux forts de la Nievre (list of medieval castles and mottes) | SCOPED_NULL | None of the five communes is listed. |

## Q4

**Question:** Is this mound the tumuliform stone heap of La Colline (CAG 58) or another tumulus recorded in the CAN?

Changes: drop as a discovery lead (known site) versus keep for a qualified assessment.

- La Colline or a CAN entity lies here -> Q3 RECORDED: detection of a known site
- La Colline lies elsewhere and the CAN holds nothing here -> Q3 NEARBY_DISTINCT: keep; candidate for the questions-only SRA letter after the challenge pass
- An estate feature or clearance cairn is documented -> Q2 ORDINARY_EXPLANATION_LIKELY: drop

Answerable by: Public first: the 1849 section sheets of the commune (field name La Colline) and a full page view of the CAG entry. Then SRA Bourgogne-Franche-Comte.

Next action: 1. Independent challenge pass. 2. Locate La Colline on the 1849 section sheets. 3. If unmatched, candidate for the questions-only SRA letter. No correspondence in this pass.

Outstanding public routes: 1849 section sheets of the commune (AD Nievre 3PPLANS/215/2-42): position of La Colline; Gallica page view of the CAG 58 entry (security check); estate history of La Faisanderie and Le Colombier.

Contact gate: 1_public_routes_exhausted: fails: public routes remain; 2_specific_custodian_item: not yet identified; 3_answers_lead_to_different_actions: holds; 4_not_answered_duplicated_or_opinion: holds for a precise record question; 5_challenge_receipt: fails: the challenge pass has not run.

## Dated imagery (IGN 1950-1965)

Covered. Mosaic source mission 1957_F 2523-2623_P_25000 (1:25,000), graph dates 1957-04-05 to 1957-04-22 (a range, not an exposure date); viewed at 0.5 m/px (300 m) and 1 m/px (1 km); registration not established: 1 km phase correlation gave 34.0 m (peak/median 12.3); the 300 m correlation (49.7 m) is not used because land cover changed; BD TOPO roads overlaid on the 1 km view follow the visible roads at display scale (about 1 m/px). Target: Young plantation or open woodland in rows; the mound cannot be seen: non-diagnostic. Frame index: 3 dates before 1966 (1949-06-22, 1957-04-22, 1961-05-30), frames not viewed. Access limits: the 1965-1980 and 1980-1995 mosaics are blank; native ground resolution not read from metadata.

## Challenge priorities

- Position La Colline on the old cadastre.
- Test the estate-feature reading with estate history.
- Look for other mounds in the same plantation in the DTM.

Correspondence: none. No contact in this pass.

## Challenge pass (2026-10-02, Claude Opus 5.5 challenge agent): SURVIVES

No prior record was found at the mound. The CeCaB fortified-site inventory has nothing within 4.6 km (CH-RR-01);
Atlas des patrimoines ZPPA, MH, AC1 and SPR layers are empty within 3 km (CH-RR-03, CH-NI-01); CAG 58 has no entry at
Bois Mignon, La Faisanderie, Le Colombier or Le Puisac. The outstanding Napoleonic route was advanced: section D
sheet 2 names the lead's parcel "Bois Mignon n°5", with nothing drawn in it and no parcel named La Colline
(CH-HM-01). The CAG "La Colline" cairn (Pouilly-sur-Loire 1*) stays unpositioned (CH-HM-02), so Q3 stays
UNRESOLVED. A local DTM census found two other compact mounds of similar height 95 m SE and 399 m SSW in the same
wood (q2.challenge_note); a barrow group, clearance heaps and estate features all remain possible. Correction notes
on LT-10 (wrong CeCaB page) and RR-03 (Atlas reachable over http); HM-06 annotated. Validator class after the
challenge: **unvetted** (Q3 UNRESOLVED), 0 errors, contact_ready=false. The single CAN question for the SRA, which
also covers the two neighbouring mounds, is in [internal file] and `q4.sra_question_from_challenge`.
