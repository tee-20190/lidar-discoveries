# FR1-S3 lead dossier (lead_vetting_v1.1), 2026-10-02, before the challenge pass

Private summary without coordinates; the location is only in `dossier.json` ([internal file]).

**Validator:** `python [internal file] [internal file] gives class **unvetted**, 0 errors, `contact_ready=false`.

Commune: Entrains-sur-Nohain (58109). Review codes: N011, N016.

| Question | Status | One-line basis |
|---|---|---|
| Q1: is the terrain feature real? | LIKELY_REAL | A regular square of ditch, external bank and raised platform is clear in several renders and in axis profiles of one IGN LiDAR HD DTM, and was proposed twice (two review codes 3.5 m apart). |
| Q2: is it plausibly archaeological? | PLAUSIBLE | A regular square ditch with an external bank around a raised platform is anthropogenic, and no ordinary explanation is supported by the historic maps (Cassini, 18th century, to the 1949 map), land use (forest throughout) or context. |
| Q3: does it match existing records? | UNRESOLVED | No positioned record matches: the Roman road crossing the wood is linear, the Miniers castle ditches are in another wood 4.4 km away, and the located CAG enclosure items are 1.8-5.3 km away. |

## Q1: LIKELY_REAL

A regular square of ditch, external bank and raised platform is clear in several renders and in axis profiles of one IGN LiDAR HD DTM, and was proposed twice (two review codes 3.5 m apart). Orthophotos are non-diagnostic under canopy, so REAL is not earned. A tile seam is excluded (210 m inside the tile). Untested: point-cloud classification under canopy.

- **Q1-E1** (records-screen render: hillshade 315/45, 8-direction hillshade, local relief (10 m Gaussian) and residual from an annulus plane): Square ditch, nearly cardinal (rotation 3.0 deg): ditch outer rectangle 23.0 x 23.8 m, enclosing a slightly raised platform about 10-12 m across, with an external bank on all sides; total extent about 35-40 m. Its centre lies about 8 m E and 3 m N of the review mark.
- **Q1-E2** (four detrended profiles (0, 45, 90, 135 deg) and a 1 m radial profile about the lead): Axis profiles through the square centre (mean of 3 lines): ditch minima at -8.5/8.0 m and -10.0/8.0 m (ditch centrelines 16.5-18 m apart); bank crests at about +/-14 m, 0.35-0.53 m above the plane; platform +0.23-0.25 m; ditch floor -0.03 to -0.15 m.
- **Q1-E3** (canopy height within 5 m and 30 m of the lead): MNH within about 5 m: mean 19.76 m, max 25.81 m; within 30 m: mean 19.75 m, 92 % above 2 m.
- **Q1-E4** (300 m and 100 m windows centred on the lead): Closed broadleaf canopy in 1957, 2002 and 2023: the earthwork is not visible; non-diagnostic.

Dimensions: {"ditch_outer_side_m": 23.4, "ditch_centreline_spacing_m": 17.0, "bank_crest_spacing_m": 28.0, "bank_height_above_plane_m": 0.5, "platform_height_above_plane_m": 0.25, "overall_extent_m": 37.0}

## Q2: PLAUSIBLE

A regular square ditch with an external bank around a raised platform is anthropogenic, and no ordinary explanation is supported by the historic maps (Cassini, 18th century, to the 1949 map), land use (forest throughout) or context. The external bank and small size fit a small moated platform or a protohistoric or Roman square enclosure; the same wood is crossed by the Roman road Autun-Orleans (CAG 58), and a Roman sanctuary lies about 0.9 km away (lieu-dit polygon). Morphology spans periods; post-medieval forestry use remains open.

| Ordinary explanation | For | Against | Status |
|---|---|---|---|
| post-medieval forestry or hunting structure (lodge, enclosure, feeding place, nursery) | The forest was managed for hunting: a star of rides is drawn on the etat-major map and on the 1830 cadastre (registered locally, median ray misfit 1.1 deg). | No building, enclosure or name at the spot on Cassini, the etat-major map, the 1830 cadastre (undivided wood plot 94, "Foret d Entrains") or the 1949 map. Post-1949 works cannot be tested under canopy. | OPEN |
| pond or reservoir with a central island | Square planform. | The ditch floor is only 0.03-0.15 m below the local plane and the platform is raised; no water symbol on any map. | DISFAVOURED |
| charcoal-burning platform | Woodland industry in the area. | A square ditch with external bank around a raised platform is not a circular level charcoal floor. | DISFAVOURED |
| iron-ore extraction pit with spoil | Ore-named wood; small pits nearby. | A regular square ditch around a raised platform is not a pit with spoil rings. | DISFAVOURED |
| 20th-century military emplacement or depot | A compact square earthwork in woodland. | No access track to it (nearest ride 90 m), nothing on maps to 1949; no WWII source read for this wood. | OPEN, unsupported |

Name trap: The medieval seat of the lordship of Miniers (large deep ditches in the woods) lies in a different wood, Bois de Minier, about 4.4 km away (LT-05); Minerai and Minier are distinct places.

## Q3: UNRESOLVED

No positioned record matches: the Roman road crossing the wood is linear, the Miniers castle ditches are in another wood 4.4 km away, and the located CAG enclosure items are 1.8-5.3 km away. It stays UNRESOLVED because several aerial enclosure items in the CAG Entrains entry could not be positioned (LT-07), Bouthier counts one unpositioned square enclosure at Entrains, and the CAN is restricted.

| Family | Rows |
|---|---|
| national_inventory | NI-01 SCOPED_NULL; NI-02 ACCESS_FAILURE |
| regional_record | RR-01 SCOPED_NULL; RR-02 ACCESS_FAILURE; RR-03 ACCESS_FAILURE |
| planning_grey_literature | PL-01 SCOPED_NULL; PL-02 SCOPED_NULL; PL-03 SCOPED_NULL; PL-06 ACCESS_FAILURE |
| historic_maps | HM-01 SCOPED_NULL; HM-02 SCOPED_NULL; HM-03 SCOPED_NULL; HM-04 SCOPED_NULL; HM-05 SCOPED_NULL; HM-06 SCOPED_NULL |
| aerial_index | AI-01 SCOPED_NULL; AI-02 SCOPED_NULL; AI-03 SCOPED_NULL; AI-04 SCOPED_NULL; AI-05 ACCESS_FAILURE; AI-06 SCOPED_NULL |
| literature | LT-01 SCOPED_NULL; LT-02 SCOPED_NULL; LT-03 HIT; LT-04 SCOPED_NULL; LT-05 HIT; LT-06 SCOPED_NULL; LT-07 ACCESS_FAILURE |

| Row | Source | Outcome | Note |
|---|---|---|---|
| NI-01 | Ministry of Culture Merimee open dataset (merimee.csv, local copy downloaded 2026-09-23, sha256 65c493db...) | SCOPED_NULL | No record within 2 km; nearest protected record: PA58000004 church of Entrains at 3,466 m. Merimee holds protected monuments and inventory files, not the Carte archeologique nationale. |
| NI-02 | Carte archeologique nationale (Patriarche), Ministry of Culture / SRA Bourgogne-Franche-Comte | ACCESS_FAILURE | The CAN is restricted; the project holds no SRA extract for this commune. A blank public query never establishes absence from the CAN; the SRA can answer this. |
| RR-01 | Prefectoral archaeological zoning order (ZPPA) n. 2004/257 of 30 November 2004, as reproduced in the carte communale report (PL-01, report page 13) | SCOPED_NULL | The order zones the whole commune as the territory of the Roman town Intaranum and lowers the referral threshold; it lists no individual site, so it is not a record of this feature. |
| RR-02 | data.gouv.fr dataset "Zone de presomption de prescriptions archeologiques" | ACCESS_FAILURE | Read by lead-researcher pass B: the dataset covers the Eure department only, so it cannot answer for Nievre. |
| RR-03 | SRA Bourgogne-Franche-Comte commune extract of the CAN | ACCESS_FAILURE | The project holds an SRA extract for Sainte-Colombe-des-Bois only (2026-09-10); none for this commune. Not requested here (no correspondence in this pass). |
| PL-01 | Carte communale of Entrains-sur-Nohain (DU_58109, approved 2011-06-22): rapport de presentation, 72 pp. (GPU) | SCOPED_NULL | Archaeology section (p.13) reproduces the commune-wide zoning order 2004/257 (RR-01); history section names Intaranum, the Apollo statue and the theatre. No site list and no mention of the wood. File sha256 c66b6083... |
| PL-02 | IGN API Carto GPU module: document, zone and sector at the lead | SCOPED_NULL | Carte communale DU_58109 applies (non-constructible sector); no zone or prescription. |
| PL-03 | IGN API Carto GPU module: servitudes, information and prescription layers | SCOPED_NULL | No servitude, information or prescription feature within 200 m. |
| PL-06 | ADLFI (Archeologie de la France - Informations) operation notices via OpenEdition search | ACCESS_FAILURE | The search returned a 973-byte redirect shell without results; engine searches found only a 2009 ADLFI notice for the Bois des Huets at Entrains (late 19th-century charcoal platforms, quarry extension; snippet only, notice unread). |
| HM-01 | Cassini map (BnF copy) via IGN WMS-R (BNF-IGNF_GEOGRAPHICALGRIDSYSTEMS.CASSINI) | SCOPED_NULL | Forest at the lead; wood label read as "...ineray"; no symbol at the lead. |
| HM-02 | Carte de l etat-major 1:40,000 (1820-1866) via IGN WMS-R (GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40) | SCOPED_NULL | Forest edge country; nothing at the lead. |
| HM-03 | IGN 1:50,000 type-1922 map (SCAN50 1950 layer; sheet graph gives 1949) via WMS-R | SCOPED_NULL | Forest; nothing at the lead. |
| HM-04 | Etalab/DGFiP cadastre lieux-dits (open data), four communes | SCOPED_NULL | inside BOIS DU MINERAY; FORET D'ENTRAINS (Menestreau) 382 m. No lieu-dit with motte, butte, tertre, tumulus, chatel or moulin within 400 m of the lead. |
| HM-05 | IGN BD TOPO toponymie, lieux-dits, zones of interest and orographic details (Geoplateforme WFS) | SCOPED_NULL | Bois du Minerai label 413 m; hamlet le Minerai 886 m; Bois du Sauveur 1.24 km; no earthwork name. |
| HM-06 | Cadastre napoleonien of Entrains (1830), section C du Minerai, sheet 2 (AD Nievre 3PPLANS/109/14), with the tableau d assemblage (3PPLANS/109/1) | SCOPED_NULL | The lead lies inside wood plot 94 of the "Foret d Entrains", about 100-150 m from a ride; no building, pond, symbol or name within 160 m; only faint pencil construction lines. |
| AI-01 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), with its WFS mosaic graph | SCOPED_NULL | Continuous broadleaf canopy; the earthwork cannot be seen: non-diagnostic. Registration: phase correlation under canopy/scrub was unreliable (inconsistent offsets, weak peaks); BD TOPO road lines overlaid on the 1 km view follow the visible rides/roads at display scale (about 1 m/px), not measured. Exact exposure of the mosaicked frame not established beyond the graph range; native ground resolution not read from metadata. |
| AI-02 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), 1 km context with BD TOPO roads and the parcel overlaid | SCOPED_NULL | Forest throughout; a straight ride/parcel line SE of the lead matches BD TOPO at display scale. |
| AI-03 | IGN orthophotos ORTHOIMAGERY.ORTHOPHOTOS2000-2005 (WMS-R) | SCOPED_NULL | Closed canopy: non-diagnostic. |
| AI-04 | IGN current orthophoto ORTHOIMAGERY.ORTHOPHOTOS (WMS-R) and colour-infrared ORTHOIMAGERY.ORTHOPHOTOS.IRC | SCOPED_NULL | Closed canopy: non-diagnostic. |
| AI-05 | IGN historical orthomosaics ORTHOIMAGERY.ORTHOPHOTOS.1965-1980 and .1980-1995 (WMS-R) | ACCESS_FAILURE | HTTP 200 but blank near-white images (pixel standard deviation below 2) for both layers; the 1980-1995 graph returned no polygon. |
| AI-06 | IGN national aerial photograph frame index (Geoplateforme WFS pva:image) | SCOPED_NULL | 117 frames listed, 1949-2017, including 1949-06-14 (dataset 2622-0081), 1957-04-04 (2622-0071, the mission behind the 1950-1965 mosaic) and 1957-06-20 (2622-0061). Coverage metadata only: no individual frame was viewed, and a frame index records no features. |
| LT-01 | Chevrier S. 2009, Les enceintes pre-medievales du Nivernais-Morvan, Revue archeologique de l Est 58 (OpenEdition), read by lead-researcher passes A and B | SCOPED_NULL | No catalogue site in the four communes. Read through a fetch summariser; truncation of a long page is possible. |
| LT-02 | Bouthier A., L occupation du Nord-Ouest du Nivernais ... aux epoques protohistoriques, vue d avion (B@sic 1, UNA editions), HTML and PDF | SCOPED_NULL | Entrains: 6 enceintes, 1 enclos carre, 1 enclos circulaire (aerial cropmarks, no positions). The single Entrains square enclosure is an aerial cropmark record; the lead lies under forest recorded since the 18th century. Square enclosures in the inventory measure 5-20 m a side. Not positionable: see LT-07. |
| LT-03 | CAG 58 (Bigeard 1996), full-text search through the Gallica ContentSearch service | HIT [CAG 58, commune 109 (Entrains), item 2* (043-045), view PAG_147; lieu-dit index view PAG_297 "Minerai (bois du): 2*"; 0 m; distinct] | The Roman road Autun-Orleans arrives from the south by les Affouages de Menestreau and crosses the bois du Minerai (Goguey 1978). A linear road is a different form from this feature. The Entrains lieu-dit index gives no other item for the wood. Excerpt-level read: the full page view is behind a Gallica security check (CAPTCHA, not attempted). |
| LT-04 | CAG 58 (Bigeard 1996), Gallica ContentSearch, filtered to the Entrains entry pages (views PAG_143-178) | SCOPED_NULL | No tumulus, tertre or motte item in the Entrains pages and no hit for the woodland lieux-dits around the lead. Located enclosure items lie at Le Pontot (70*), Les Criots de Mirebeau / Marais du Nohain (71*, palisaded enclosure 50 x 25 m), Bois Bouleau (76*) and Piece du Bois Blin (66*): 1.8-5.3 km from the lead (cadastral lieu-dit polygons). Unlocated aerial enclosure items remain (LT-07). |
| LT-05 | terres-et-seigneurs-en-donziais.fr: "Miniers, aux sources du Nohain" (2015) and its notice PDF Miniers.pdf | HIT [Seat of the lordship of Miniers: large deep ditches in the wood of the same name, 1,500 m east of Entrains; 4359 m; distinct] | The ditches lie in the Bois de Minier (cadastral lieu-dit BOIS DE MINIER, 2 km ENE of the church; LES MINIERS nearby), not in the Bois du Minerai; distance is to the BOIS DE MINIER polygon. Page fetched with curl (TLS certificate mismatch on https); PDF sha256 4a2b387e... |
| LT-06 | Wiki58 (gennievre.net), Entrains-sur-Nohain and Entrains archaeology pages (lead-researcher pass A) | SCOPED_NULL | Gallo-Roman town only; the commune page names the fiefs of Miniere and Fondelin without positions or earthworks. |
| LT-07 | CAG 58 Entrains entry: aerial enclosure items without a lieu-dit in the search excerpts (views PAG_176-177) | ACCESS_FAILURE | These items could not be positioned: their lieux-dits are outside the returned excerpts and the full pages are behind a CAPTCHA. They are aerial cropmark records, while the lead lies under forest recorded since the 18th century, but their positions must be read before this feature can be called distinct. |

## Q4 (draft; contact not justified before the challenge pass)

**Question:** Does the restricted Carte archeologique nationale hold an entity at this spot in the Bois du Minerai, and do the unlocated aerial enclosure items of the CAG 58 Entrains entry (Goguey 1982, Magdelaine 1989, Bouthier 1991, Delor 1988) lie here or elsewhere?

- A CAN entity or CAG item is at this spot with a matching ditched square -> Q3 RECORDED: count as detection of a known site; drop from the discovery count
- No entity here, and the unlocated CAG items lie in open fields elsewhere -> Q3 NEARBY_DISTINCT: keep; after the challenge pass, include in the questions-only SRA letter asking for a record check and assessment
- The SRA or a challenger identifies a post-medieval forestry or military structure -> Q2 ORDINARY_EXPLANATION_LIKELY: drop

**Answerable by:** Public first: the full CAG 58 Entrains pages (printed pp. about 168-169) read in an ordinary browser by the owner (Gallica shows a security check to automated access). Then SRA Bourgogne-Franche-Comte for the CAN.

**Next action:** 1. Independent challenge pass (priorities below). 2. Owner or challenger reads CAG 58 pp. about 168-169. 3. If still unmatched, this site is a candidate for the questions-only SRA letter. No correspondence in this pass.

## Challenge priorities

- Read the full CAG 58 Entrains pages around printed pp. 168-169 and place the unlocated aerial enclosure items (LT-07).
- Search for post-medieval forestry, hunting or WWII structures in the Bois du Minerai / Foret d Entrains (forest management plans of the foret sectionale, local history).
- Test whether the square could be a forestry nursery or game enclosure recorded in ONF or communal forest documents.
- Look for the Roman road line through the wood in the LiDAR and its distance to the square.
