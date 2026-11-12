# FR1-S5 lead dossier (lead_vetting_v1.1), 2026-10-02, before the challenge pass

Private summary without coordinates; the location is only in `dossier.json` ([internal file]).

**Validator:** `python [internal file] [internal file] gives class **unvetted**, 0 errors, `contact_ready=false`.

Commune: Ciez (58077). Review codes: N026.

| Question | Status | One-line basis |
|---|---|---|
| Q1: is the terrain feature real? | LIKELY_REAL | A discrete mound about 29 m across at half height and about 1 m high stands clear of the broad rise in one DTM. |
| Q2: is it plausibly archaeological? | PLAUSIBLE | A round mound about 29 m across and 1 m high with a slight central dish fits a disturbed tumulus, and a group of Hallstatt dry-stone tumuli in woodland is recorded about 240 m away (les Usages de Jussy; one excavated in 2005 ahead of quarrying). |
| Q3: does it match existing records? | UNRESOLVED | Partial match: a recorded group of Hallstatt dry-stone tumuli in woodland at les Usages de Jussy, 237 m away (lieu-dit polygon), one excavated in 2005; the individual tumulus positions and sizes are not public (Dolia blocked). |

## Q1: LIKELY_REAL

A discrete mound about 29 m across at half height and about 1 m high stands clear of the broad rise in one DTM. Orthophotos cannot test it, so REAL is not earned. Untested: the hummocks along the strip may partly be vegetation or tree-throw relief; point cloud not inspected.

- **Q1-E1** (records-screen render: hillshade 315/45, 8-direction hillshade, local relief (10 m Gaussian) and residual from an annulus plane): A rounded mound on top of a broad low rise (about 90 m), with a hummocky NW-SE wooded strip running through it and two small pits 12-20 m to the east; the residual shows a slight central dish.
- **Q1-E2** (four detrended profiles (0, 45, 90, 135 deg) and a 1 m radial profile about the lead): Radial mean +1.03 m at the centre relative to the 45-60 m annulus plane, a slight dip to +0.93 m at 3-5 m and a rim at +1.02 m at 7-8 m; half height at about 14.5 m radius (diameter about 29 m). Detrended profiles peak 1.0-1.9 m.
- **Q1-E3** (canopy height within 5 m and 30 m of the lead): MNH within about 5 m: mean 2.28 m, max 10.6 m; within 30 m: mean 6.09 m, 73 % above 2 m.
- **Q1-E4** (300 m and 100 m windows centred on the lead): Scrub with scattered bushes in 1957, dense young wood in 2002, wood in 2023: the mound is not visible in any year; non-diagnostic.

Dimensions: {"half_height_diameter_m": 29.0, "height_above_annulus_plane_m": 1.03, "central_dip_m": 0.1}

## Q2: PLAUSIBLE

A round mound about 29 m across and 1 m high with a slight central dish fits a disturbed tumulus, and a group of Hallstatt dry-stone tumuli in woodland is recorded about 240 m away (les Usages de Jussy; one excavated in 2005 ahead of quarrying). The windmill reading is not supported by any map after Cassini. Quarry spoil and clearance remain open but undocumented.

| Ordinary explanation | For | Against | Status |
|---|---|---|---|
| quarry spoil or quarry test pits | A large quarry lies about 100 m away; two small pits lie 12-20 m E of the mound. | The 2002 orthophoto shows dense wood at the spot and no quarry within 150 m; dumping into the wood after 2002 would have cleared it. | OPEN |
| windmill mound | Hilltop; slight central dish; Cassini plots a windmill about 250 m away (approximate positions). | No mill on the etat-major map (1820-1866), the 1828 cadastre (Les Montpaurous is one undivided parcel with no structure) or the 1949 map; no mill lieu-dit within 400 m (the Entrains lieu-dit LE MOULIN A VENT is about 5 km away). | DISFAVOURED |
| field-clearance cairn or natural knoll with tree-throw hummocks | Stony hilltop near a limestone quarry; scrub in 1957; hummocks along the wooded strip. | A discrete round mound about 29 m across and about 1 m high with a slight central dish stands clear of the broad rise. | OPEN |

## Q3: UNRESOLVED

Partial match: a recorded group of Hallstatt dry-stone tumuli in woodland at les Usages de Jussy, 237 m away (lieu-dit polygon), one excavated in 2005; the individual tumulus positions and sizes are not public (Dolia blocked). Other records are distinct (les Dessertis enclosure 434 m; Bois Bouleau enclosure and building 438 m; Le Pontot 745 m).

| Family | Rows |
|---|---|
| national_inventory | NI-01 SCOPED_NULL; NI-02 ACCESS_FAILURE |
| regional_record | RR-01 SCOPED_NULL; RR-02 ACCESS_FAILURE; RR-03 ACCESS_FAILURE |
| planning_grey_literature | PL-01 SCOPED_NULL; PL-02 SCOPED_NULL; PL-03 SCOPED_NULL; PL-06 ACCESS_FAILURE; PL-04 HIT; PL-05 HIT; PL-07 ACCESS_FAILURE |
| historic_maps | HM-01 SCOPED_NULL; HM-02 SCOPED_NULL; HM-03 SCOPED_NULL; HM-04 SCOPED_NULL; HM-05 SCOPED_NULL; HM-06 SCOPED_NULL |
| aerial_index | AI-01 SCOPED_NULL; AI-02 SCOPED_NULL; AI-03 SCOPED_NULL; AI-04 SCOPED_NULL; AI-05 ACCESS_FAILURE; AI-06 SCOPED_NULL |
| literature | LT-01 SCOPED_NULL; LT-02 SCOPED_NULL; LT-03 HIT; LT-04 HIT; LT-05 SCOPED_NULL |

| Row | Source | Outcome | Note |
|---|---|---|---|
| NI-01 | Ministry of Culture Merimee open dataset (merimee.csv, local copy downloaded 2026-09-23, sha256 65c493db...) | SCOPED_NULL | No record within 2 km; nearest protected record: PA00112847 church of Ciez at 3,958 m. Merimee holds protected monuments and inventory files, not the Carte archeologique nationale. |
| NI-02 | Carte archeologique nationale (Patriarche), Ministry of Culture / SRA Bourgogne-Franche-Comte | ACCESS_FAILURE | The CAN is restricted; the project holds no SRA extract for this commune. A blank public query never establishes absence from the CAN; the SRA can answer this. |
| RR-01 | DRAC Bourgogne-Franche-Comte archaeology page (ZPPA procedure) and web searches for a ZPPA order naming the commune (lead-researcher pass B) | SCOPED_NULL | The DRAC page says ZPPA are set by prefectoral order and gives no list; no order naming the commune was found. Engine-level null, weaker than a record check. |
| RR-02 | data.gouv.fr dataset "Zone de presomption de prescriptions archeologiques" | ACCESS_FAILURE | Read by lead-researcher pass B: the dataset covers the Eure department only, so it cannot answer for Nievre. |
| RR-03 | SRA Bourgogne-Franche-Comte commune extract of the CAN | ACCESS_FAILURE | The project holds an SRA extract for Sainte-Colombe-des-Bois only (2026-09-10); none for this commune. Not requested here (no correspondence in this pass). |
| PL-01 | Geoportail de l urbanisme document catalogue (GPU API) | SCOPED_NULL | No planning document is published for the commune (empty list; the 2026-10-01 department catalogue of 95 current documents also lists none for it), so no PLU heritage annex exists to read. |
| PL-02 | IGN API Carto GPU module: document, zone and sector at the lead | SCOPED_NULL | No document at the point; municipality endpoint for 58077 returns is_rnu=false (https://apicarto.ign.fr/api/gpu/municipality?insee=58077). |
| PL-03 | IGN API Carto GPU module: servitudes, information and prescription layers | SCOPED_NULL | No servitude, information or prescription feature within 200 m. |
| PL-06 | ADLFI (Archeologie de la France - Informations) operation notices via OpenEdition search | ACCESS_FAILURE | The search returned a 973-byte redirect shell without results; engine searches found only a 2009 ADLFI notice for the Bois des Huets at Entrains (late 19th-century charcoal platforms, quarry extension; snippet only, notice unread). |
| PL-04 | Inrap Dolia digital library, list of operation reports (page 101) | HIT [Ducreux F. et al. 2006, Ciez, Usages-de-Jussy: fouille du tumulus n.1 du premier age du Fer (Inrap GES, Dijon); 237 m; partial] | Excavation report of tumulus 1 of the Usages de Jussy group (read by pass B; title confirmed by a records-screen web search). Distance is to the cadastral lieu-dit LES USAGES DE JUSSY polygon (237 m); the positions and sizes of the individual tumuli are not public. Form class matches (round mound); position not comparable. |
| PL-05 | Inrap activity report 2005, p.74 (yumpu copy) | HIT [Inrap 2005 operation at Ciez, Usage de Jussy: excavation of a large dry-stone tumulus 1 with several burials; 237 m; partial] | Read by pass B: a preventive excavation in 2005 funded by the quarry developer; no size or position given. Same record family as PL-04. |
| PL-07 | Inrap Dolia record ark:/64298/016954 (Ducreux et al. 2006) | ACCESS_FAILURE | HTTP 403 behind an automated browser check (Cloudflare challenge); not attempted further. The report plan would place the tumuli. |
| HM-01 | Cassini map (BnF copy) via IGN WMS-R (BNF-IGNF_GEOGRAPHICALGRIDSYSTEMS.CASSINI) | SCOPED_NULL | Open land; a windmill symbol plotted about 250 m from the lead near "le Chalumeau" (Cassini positions are approximate to hundreds of metres). |
| HM-02 | Carte de l etat-major 1:40,000 (1820-1866) via IGN WMS-R (GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40) | SCOPED_NULL | Open land with relief hachures; no windmill or other symbol at or near the lead (2 km window also read, HM-06). |
| HM-03 | IGN 1:50,000 type-1922 map (SCAN50 1950 layer; sheet graph gives 1949) via WMS-R | SCOPED_NULL | Wood edge with tree symbols; the symbol at the lead is a tree symbol, not a mill (checked at 900 m and 2 km spans, HM-06). |
| HM-04 | Etalab/DGFiP cadastre lieux-dits (open data), four communes | SCOPED_NULL | inside LES MONTPAUROUS (Ciez); LE CHALVARI 33 m; USAGES DU CHALUMEAU (Entrains) 113 m; LES BERGOTS 191 m; LES USAGES DE JUSSY 237 m. No lieu-dit with motte, butte, tertre, tumulus, chatel or moulin within 400 m of the lead. |
| HM-05 | IGN BD TOPO toponymie, lieux-dits, zones of interest and orographic details (Geoplateforme WFS) | SCOPED_NULL | quarry zone 99 m; Foret sectionale de Chalumeau 122 m; les Bergots 211 m; les Usages de Jussy label 918 m; no earthwork or mill name. |
| HM-06 | Cadastre napoleonien of Ciez (1828), section D de Jussy sheet 6 (AD Nievre 3PPLANS/077/16) with the tableau d assemblage (3PPLANS/077/1); plus etat-major and 1949 map at 2 km | SCOPED_NULL | In 1828 Les Montpaurous (the lieu-dit containing the lead today) is one large undivided parcel with no building or mill drawn; the Usages de Jussy are subdivided woodland lots along the Entrains boundary. No mill symbol on the 2 km etat-major or 1949 windows. Registration by name only: the parcel extent is approximate. |
| AI-01 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), with its WFS mosaic graph | SCOPED_NULL | Scrub with scattered bushes and trees on open ground; no mound discernible. Registration: phase correlation under canopy/scrub was unreliable (inconsistent offsets, weak peaks); BD TOPO road lines overlaid on the 1 km view follow the visible rides/roads at display scale (about 1 m/px), not measured. Exact exposure of the mosaicked frame not established beyond the graph range; native ground resolution not read from metadata. |
| AI-02 | IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), 1 km context with BD TOPO roads and the parcel overlaid | SCOPED_NULL | Open fields and scrub; road and field boundaries as today; quarry not present in the window. |
| AI-03 | IGN orthophotos ORTHOIMAGERY.ORTHOPHOTOS2000-2005 (WMS-R) | SCOPED_NULL | Dense young wood at the spot; no quarry within 150 m. |
| AI-04 | IGN current orthophoto ORTHOIMAGERY.ORTHOPHOTOS (WMS-R) and colour-infrared ORTHOIMAGERY.ORTHOPHOTOS.IRC | SCOPED_NULL | Wood; quarry works to the north-east of the strip. |
| AI-05 | IGN historical orthomosaics ORTHOIMAGERY.ORTHOPHOTOS.1965-1980 and .1980-1995 (WMS-R) | ACCESS_FAILURE | HTTP 200 but blank near-white images (pixel standard deviation below 2) for both layers; the 1980-1995 graph returned no polygon. |
| AI-06 | IGN national aerial photograph frame index (Geoplateforme WFS pva:image) | SCOPED_NULL | 93 frames listed, 1949-2017, including 1949-06-14 (dataset 2622-0081), 1957-04-04 (2622-0071, the mission behind the 1950-1965 mosaic) and 1957-06-20 (2622-0061). Coverage metadata only: no individual frame was viewed, and a frame index records no features. |
| LT-01 | Chevrier S. 2009, Les enceintes pre-medievales du Nivernais-Morvan, Revue archeologique de l Est 58 (OpenEdition), read by lead-researcher passes A and B | SCOPED_NULL | No catalogue site in the four communes. Read through a fetch summariser; truncation of a long page is possible. |
| LT-02 | Bouthier A., L occupation du Nord-Ouest du Nivernais ... aux epoques protohistoriques, vue d avion (B@sic 1, UNA editions), HTML and PDF | SCOPED_NULL | Ciez: 5 enceintes (aerial). Woodland Hallstatt dry-stone tumuli at les Usages de Jussy, one excavated by F. Ducreux (see PL-04/PL-05 for the record). |
| LT-03 | CAG 58 (Bigeard 1996), Gallica ContentSearch for the Ciez entry (commune 077, view PAG_113) and names | HIT [CAG 58 commune 077 item 1* (005): large rectangular enclosure about 100 x 120 m at les Dessertis; 434 m; distinct] | Distance to the cadastral lieu-dit LES DESSERTIS (Ciez) polygon. Other Ciez items: 2* enclosure at la Vallee Savard; 5* (003) Roman substructions found in the woods near Jussy in the early 19th century (unlocated; buildings, not a mound); 6* small Roman building near Picarnon. No tumulus, mill, Bergots, Chalvari or Montpaurous item: the CAG (1996) predates the 2005 tumulus excavation. Excerpt-level read. |
| LT-04 | CAG 58 (Bigeard 1996), Gallica ContentSearch: Entrains items near the commune boundary | HIT [CAG 58 commune 109 item 76* (016): quadrangular enclosure and small square building photographed at Bois Bouleau; 438 m; distinct] | Distance to the Entrains lieu-dit PIECE DU BOULEAU (identification with "Bois Bouleau" by name only). Item 70* Le Pontot ditched enclosure is 745 m away. Enclosures and a building are different forms from a round mound. |
| LT-05 | Wiki58 archaeology index and French Wikipedia, Ciez (lead-researcher pass B) | SCOPED_NULL | No Wiki58 page exists for Ciez; Wikipedia gives no archaeology, mill or quarry. |

## Q4 (draft; contact not justified before the challenge pass)

**Question:** Is this mound one of the recorded Hallstatt tumuli of the Usages de Jussy group, and is it distinct from tumulus 1 excavated in 2005?

- The CAN or the Ducreux et al. 2006 plan places a tumulus at this spot -> Q3 RECORDED: detection of a known site; drop from the discovery count and keep as a known positive
- The group plan places all tumuli elsewhere and no entity is here -> Q3 NEARBY_DISTINCT: keep; after the challenge pass, include in the questions-only SRA letter
- The mound is quarry spoil or a clearance heap -> Q2 ORDINARY_EXPLANATION_LIKELY: drop

**Answerable by:** SRA Bourgogne-Franche-Comte (CAN entities and the 2006 Inrap report and plan); Inrap Dolia (report; blocked to automated access). The owner could try Dolia in an ordinary browser first.

**Next action:** 1. Independent challenge pass. 2. Owner tries the Dolia record in an ordinary browser. 3. If the plan is not reachable, this site is a candidate for the questions-only SRA letter (specific item: the 2006 report plan and CAN entities for the group). No correspondence in this pass.

## Challenge priorities

- Locate the Usages de Jussy tumuli (Ducreux et al. 2006 plan, BSR Bourgogne 2005) and compare with this mound.
- Check whether quarry works (Deromedi or OMYA) dumped spoil or dug test pits at this strip after 2002.
