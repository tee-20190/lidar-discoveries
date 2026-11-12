# FR2-S2 lead dossier (lead_vetting_v1.1, research pass, pre-challenge)

Private: contains coordinates, parcel ids and lieux-dits. Never copy into a committed, public or sent file. Updated 2026-10-02.

Validator: `python [internal file] [internal file] -> pass=True, class=unvetted, contact_ready=False.

| Question | Status |
|---|---|
| Q1 terrain reality | LIKELY_REAL |
| Q2 ordinary explanation | PLAUSIBLE |
| Q3 existing documentation | UNRESOLVED |

Location: [coordinate removed], [coordinate removed] (EPSG:2154); Donzy (58102) by exact point-in-polygon WFS query (ADMINEXPRESS-COG.2026; geometry, not envelope); parcel 58102000YC0111 (section YC, contenance 9622 m2) by exact point-in-polygon WFS query; nearest parcel limit 0.9 m.

Origin: FR-DISC-2 locked source-blind review (review codes N003): outcome archaeological_discrete; reviewer_kind=model, reviewer_role=primary, human_confirmed=false. Detector identities, arms and selection files were not read in this records screen (arm-blind).

## Q1 terrain reality

A smooth closed dome is clear in the own hillshade, local-relief and residual renders and in four profiles of one IGN LiDAR HD DTM; it is broad and smooth, unlike vegetation residue, and lies 300 m inside the tile. Orthophotos are non-diagnostic under canopy, so REAL is not earned.

- **Q1-E1** (IGN LiDAR HD MNT 0.5 m, mission 23LHDLH (Optech ALTM Galaxy T2000), acquisition 2024-03-08, edition 2025-01-21; prepared tile LHD_FXX_0707_6703_MNT_O_0M50_LAMB93_IGN69.tif; records-screen renders: hillshade 315/45, multi-direction hillshade, local relief (Gaussian) and residual from an annulus plane (dtm/dtm_views.png)): Smooth isolated dome about 40 m across at its base and 0.7-1.3 m high under broadleaf woodland, crossed by a later boundary groove.
- **Q1-E2** (IGN LiDAR HD MNT 0.5 m, mission 23LHDLH (Optech ALTM Galaxy T2000), acquisition 2024-03-08, edition 2025-01-21; prepared tile LHD_FXX_0707_6703_MNT_O_0M50_LAMB93_IGN69.tif; detrended profiles through the mark (dtm/profiles.png) and radial residual profile ([internal file])): Radial residual from a plane fitted on the 15-30 m annulus reaches zero at about 21 m; profile heights are detrended on their outer 25 m.
- **Q1-E3** (IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R); mosaic graph mission 1957_F 2422-2622_P_25000; 300 m window at 0.5 m/px and 1 km window at 1 m/px (imagery/o1950_300.png, o1950_1000.png)): Young woodland or scrub at the spot; a pale strip (track or ride) runs from the north-west to the spot; the mound cannot be seen: non-diagnostic. Context: Woodland west of a road, small fields to the east and south-east; parcel strips as today.
  - coverage: mosaic graph polygon at the lead: mission 1957_F 2422-2622_P_25000; frame index lists 1949-06-14 (2622-0081), 1957-04-04 (2622-0071), 1959-04-21 (2522-0081)
  - date_range: 1957-04-04 to 1957-04-05 (graph range; the exposure of the mosaicked frame is not established)
  - scale_resolution: mission scale 1:25,000 (from the mission name); viewed at 0.5 m/px (300 m) and 1 m/px (1 km); native ground resolution not read from metadata
  - target_registration: moderate: 1 km window offset (+5, -7) m, peak/median 17; 300 m window (+3.5, -4) m
  - access_limits: processed WMS mosaic only; no individual frame viewed; 1965-1980 and 1980-1995 layers returned blank tiles (AI-06)
- **Q1-E4** (IGN BD ORTHO 2000-2005 (WMS-R ORTHOIMAGERY.ORTHOPHOTOS2000-2005); 300 m window at 0.5 m/px (imagery/o2000_300.jpg)): 2000-2005 view: Closed broadleaf canopy: non-diagnostic.
- **Q1-E5** (IGN current orthophoto and infrared colour orthophoto (WMS-R); 300 m and 1 km windows (imagery/ocur_300.jpg, ocur_1000.jpg, irc_300.jpg)): Current view: Closed broadleaf canopy (IRC: broadleaf): non-diagnostic.
- **Q1-E6** (IGN LiDAR HD MNH (canopy height), same survey 23LHDLH; canopy height at the centre and around (imagery/mnh_300.tif)): Canopy height mean 8.26 m (max 19.03 m) within 5 m of the centre and 12.3 m within 30 m: no tall clump on the dome.

Dimensions: base_diameter_m 42.0, core_diameter_resid_gt_0_3m_m 20.0, height_resid_centre_m 0.72, height_profile_max_m 1.29

Measured on the prepared 0.5 m DTM (p3_dtm_imagery.py). Heights are residuals from an annulus plane or detrended profiles, not construction heights. Radial residual from a plane fitted on the 15-30 m annulus reaches zero at about 21 m; profile heights are detrended on their outer 25 m.

## Q2 ordinary explanations

An isolated smooth dome about 40 m across and up to 1.3 m high in woodland shown as wood on the Cassini, Etat-major and 1949 maps fits a round barrow; a parcel-boundary groove crosses it, so the mound is older than that boundary. An iron-smelting slag heap remains open (a wood named "les Fourneaux" lies about 1 km away). No ordinary explanation is supported by the maps or setting. Morphology spans periods; no date.

Reading: Round barrow or slag heap; period unknown.

| Explanation | For | Against | Status |
|---|---|---|---|
| field-clearance cairn or dumped spoil | A rounded heap. | Woodland since at least the 18th-19th century maps, so no field to clear; no pit, quarry or track end large enough nearby; smooth symmetric dome. | DISFAVOURED |
| iron-smelting slag heap (ferrier) or post-medieval forge waste | Iron working is widespread in the area; a wood named "les Fourneaux" lies about 1 km north. | No slag or furnace name at or next to the spot; a smooth dome without extraction pits; would itself be an archaeological iron-working site if ancient. | OPEN |
| charcoal-burning platform | Woodland industry. | A dome, not a level platform; 40 m across is far larger than charcoal hearths. | DISFAVOURED |
| natural knoll or erosion remnant | Gentle slope (5 %). | Isolated symmetric dome on a planar slope, unrelated to slope features. | DISFAVOURED |
| vegetation residue (unfiltered tree clump) | Under canopy. | Broad smooth dome; canopy height at the centre (mean 8 m) is lower than around it (12 m), so no tall clump explains it. | DISFAVOURED |
| track or boundary earthwork | A narrow groove (path or boundary ditch) crosses it. | The groove cuts across the dome, so the mound predates it. | DISFAVOURED |

Name trap: 'les Fourneaux' (a wood about 1 km away) and 'Chatelaine' (0.4-0.5 km) are furnace and castle names, not at the spot; no earthwork name at the lead.

## Q3 existing documentation

No public record places a site at the mound: Merimee has nothing within 5 km, the planning documents and GPU layers carry no archaeological item, no ZPPA order names the commune, the placeable CAG Donzy items lie 3.1 km or more away and no name at the spot refers to an earthwork. It stays UNRESOLVED because the CAG lists one Donzy circular enclosure without location (1*) and a regional synthesis mentions tumuli around Donzy without locations (LT-04); the woodland setting argues against an aerial record here but does not place them. The restricted CAN was not consulted.

| Family | Rows |
|---|---|
| national_inventory | NI-01 SCOPED_NULL; NI-02 ACCESS_FAILURE |
| regional_record | RR-01 SCOPED_NULL; RR-02 ACCESS_FAILURE; RR-03 ACCESS_FAILURE; RR-04 ACCESS_FAILURE |
| planning_grey_literature | PL-01 SCOPED_NULL; PL-02 SCOPED_NULL; PL-03 SCOPED_NULL; LR-18 ACCESS_FAILURE; LR-20 ACCESS_FAILURE |
| historic_maps | HM-01 SCOPED_NULL; HM-02 SCOPED_NULL; HM-03 SCOPED_NULL; HM-04 SCOPED_NULL; HM-05 SCOPED_NULL |
| aerial_index | AI-01 SCOPED_NULL; AI-02 SCOPED_NULL; AI-03 SCOPED_NULL; AI-04 SCOPED_NULL; AI-05 SCOPED_NULL; AI-06 ACCESS_FAILURE |
| literature | LT-01 SCOPED_NULL; LT-02 SCOPED_NULL; LT-03 SCOPED_NULL; LT-04 ACCESS_FAILURE; LR-02 ACCESS_FAILURE; LR-03 ACCESS_FAILURE; LR-04 SCOPED_NULL; LR-07 SCOPED_NULL; LR-12 ACCESS_FAILURE; LR-17 SCOPED_NULL; LR-21 ACCESS_FAILURE; LR-22 SCOPED_NULL; LR-25 SCOPED_NULL |

| Id | Family | Source | Query | Outcome | Record / distance / form | Notes |
|---|---|---|---|---|---|---|
| NI-01 | national_inventory | [Ministry of Culture Merimee open dataset (local copy of 2026-09-22, sha256 65c493db...)](https://ministere-culture.s3.sbg.io.cloud.ovh.net/POP/merimee.csv) | records whose protection INSEE code or commune fields name 58102, 58094, 58281, 58077 or 58189; distances from the WGS84 record coordinates | SCOPED_NULL |  | No record within 1 km. Nearest records: PA00112847 Église at 5,288 m; PA00113063 Moulin de Maupertuis at 5,905 m; PA00112882 Maison à pans de bois at 6,041 m. Merimee holds protected monuments and inventory files, not the Carte archeologique nationale.  |
| NI-02 | national_inventory | [Carte archeologique nationale (Patriarche), held by the SRA Bourgogne-Franche-Comte](https://www.culture.gouv.fr/regions/drac-bourgogne-franche-comte/votre-drac/patrimoines-et-architecture/archeologie) | entities at or near the lead in commune 58102 | ACCESS_FAILURE |  | Not publicly accessible; answerable by the SRA. Public nulls below do not clear it. Alternatives: ZPPA orders and DRAC pages (RR-01); Atlas des patrimoines catalogue (RR-04); CAG 58 (1996), the published extract of the regional record (LT-01) |
| RR-01 | regional_record | [DRAC Bourgogne-Franche-Comte archaeology page (ZPPA procedure) and engine searches for a ZPPA order naming the commune](https://www.culture.gouv.fr/regions/drac-bourgogne-franche-comte/votre-drac/patrimoines-et-architecture/archeologie) | ZPPA order or list for Donzy | SCOPED_NULL |  | The DRAC page (fetched 2026-10-02, HTTP 200) says ZPPA are set by prefectoral order and gives no list; four engine searches by the lead-researcher (ZPPA Nievre with the commune names; recueil des actes administratifs) found no order naming the commune. Engine-level null, weaker than a record check.  |
| RR-02 | regional_record | [data.gouv.fr dataset "Zone de presomption de prescriptions archeologiques"](https://www.data.gouv.fr/datasets/zone-de-presomption-de-prescriptions-archeologiques) | dataset coverage | ACCESS_FAILURE |  | Published by the DDTM of the Eure and covering the Eure only (read by the lead-researcher); no Nievre ZPPA dataset was found. Alternatives: DRAC page and engine searches (RR-01); Atlas des patrimoines (RR-04) |
| RR-03 | regional_record | [SRA Bourgogne-Franche-Comte commune extract of the CAN](https://www.culture.gouv.fr/regions/drac-bourgogne-franche-comte/votre-drac/patrimoines-et-architecture/archeologie) | extract for commune 58102 | ACCESS_FAILURE |  | Released on request only; no request made in this pass (no correspondence). Alternatives: ZPPA search (RR-01); CAG 58 (LT-01); Atlas des patrimoines (RR-04) |
| RR-04 | regional_record | [Atlas des patrimoines (Ministry of Culture), metadata catalogue for archaeological presumption zones](http://atlas.patrimoines.culture.fr/) | records for zones de presomption de prescription archeologique in the Nievre | ACCESS_FAILURE |  | The catalogue request returned the Geosource HTML interface (5,639 bytes, saved as web/atlas_csw_presomption.xml), not records. Interactive map not attempted. Alternatives: GPU information and prescription layers (PL-02); DRAC page (RR-01) |
| PL-01 | planning_grey_literature | [Geoportail de l urbanisme via API Carto GPU]([query URL with coordinates removed]) | planning document and zone at the lead (point query) | SCOPED_NULL |  | PLU 'DONZY' (58102_PLU_20231109); zone N (N : Zone naturelle). No archaeological zone or sector at the point.  |
| PL-02 | planning_grey_literature | [Geoportail de l urbanisme via API Carto GPU]([query URL with coordinates removed]) | servitudes (SUP), information and prescription layers within 200 m of the lead | SCOPED_NULL |  | SUP: none; prescriptions: none; information: none. No archaeological prescription, information zone or servitude (AC1 = historic-monument perimeter, AC4 = SPR heritage area, PM1 = flood-risk plan).  |
| PL-03 | planning_grey_literature | [PLU of Donzy (2008): presentation report and SUP list (GPU document files)](https://data.geopf.fr/annexes/gpu/documents/DU_58102/ba2b7570ad0aa802cfb4d972226bea60/58102_rapport_1_20231109.pdf) | archaeolog*, vestige, motte, butte, tumulus, enclos, enceinte, ZPPA, minier and the lieux-dits near the lead | SCOPED_NULL |  | No archaeological site list or zone. The 'ZPPA' hits are ZPPAUP entries (architectural heritage area, now SPR) in the SUP list; the report mentions archaeological information only in general (p.9). SUP list: https://data.geopf.fr/annexes/gpu/documents/DU_58102/ba2b7570ad0aa802cfb4d972226bea60/18102_liste_sup_20231109.pdf  |
| LR-18 | planning_grey_literature | [ADLFI (Archeologie de la France - Informations), OpenEdition, places index and ADLFI-restricted search](https://journals.openedition.org/adlfi/22423) | 'Lieux' index to Bourgogne-Franche-Comte > Nievre > the five communes; OpenEdition search q=Donzy Nievre, s=adlfi | ACCESS_FAILURE |  | Places index: socket hang up (twice, with and without ?lang=en). The ADLFI-restricted OpenEdition search returned only a JavaScript shell, so it was not repeated. Tried once in this pass, as the brief requires for routes recorded as blocked. Alternatives: OpenEdition search restricted to ADLFI (JavaScript shell); engine site:journals.openedition.org/adlfi searches for the five communes (no notice surfaced); Inrap Dolia catalogue (HTTP 403; PL-04) |
| LR-20 | planning_grey_literature | [Inrap Dolia catalogue (operation reports)](https://dolia.inrap.fr/flora/jsp/index.jsp) | catalogue entry page, for commune searches on the five communes | ACCESS_FAILURE |  | HTTP 403 Forbidden; no search possible. Not retried (one attempt per route recorded as blocked). Alternatives: FR1 records screen (FR1-S5 PL-07): an Inrap Dolia record page returned HTTP 403 behind an automated browser check; ADLFI places index (socket hang up; LR-18) |
| HM-01 | historic_maps | [Cassini map, 18th century (BnF-IGN, WMS-R layer BNF-IGNF_GEOGRAPHICALGRIDSYSTEMS.CASSINI)]([query URL with coordinates removed]) | 2 km window centred on the lead | SCOPED_NULL |  | Wood patches around the spot and the label "Chateleine" with a building symbol about 400 m south-east; no symbol at the lead. Registration: IGN web service; display-scale reading only.  |
| HM-02 | historic_maps | [Carte d etat-major 1820-1866 (IGN, WMS-R layer GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40)]([query URL with coordinates removed]) | 1 km and 2 km windows centred on the lead | SCOPED_NULL |  | Woodland (ochre tint with slope hachures) west of a road; no symbol at the lead.  |
| HM-03 | historic_maps | [IGN 1:50,000 map of about 1950 (WMS-R layer GEOGRAPHICALGRIDSYSTEMS.MAPS.SCAN[coordinate removed])]([query URL with coordinates removed]) | 1 km window centred on the lead | SCOPED_NULL |  | Woodland (tree symbols); nothing at the lead.  |
| HM-04 | historic_maps | [Etalab cadastre, lieux-dits layer (latest)](https://cadastre.data.gouv.fr/data/etalab-cadastre/latest/geojson/communes/58/58102/cadastre-58102-lieux_dits.json.gz) | lieux-dits containing and near the lead (commune 58102) | SCOPED_NULL |  | inside LES MAUFENAUDS (Donzy); CHAMP DE FEE 67 m; BOIS BRULE 109 m; CHAMP DE CHATELAINE 118 m; LES TAILLES BUISSONS 198 m; BOIS MARET 222 m; CHAMP DU PUITS 342 m. Names of interest: CHAMP DE CHATELAINE 118 m, CHAMP DU PUITS 342 m, CHATELAINE 481 m; no motte, butte, tertre, tumulus or slag name.  |
| HM-05 | historic_maps | [IGN BD TOPO V3 toponymy and named objects (WFS)]([query URL with coordinates removed]) | names and objects within 400 m and named places within about 1.5 km | SCOPED_NULL |  | Bois les Maufrenauds 206 m; Bois Maret 468 m; hamlet Chatelaine 436-526 m; Bois de la Billotte 554 m; le Champ du Puits 865 m; wood "les Fourneaux" 961 m; no earthwork name.  |
| AI-01 | aerial_index | [IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), with its WFS mosaic graph]([query URL with coordinates removed]) | 300 m window at 0.5 m/px; graph polygon at the lead | SCOPED_NULL |  | Young woodland or scrub at the spot; a pale strip (track or ride) runs from the north-west to the spot; the mound cannot be seen: non-diagnostic. Registration: moderate: 1 km window offset (+5, -7) m, peak/median 17; 300 m window (+3.5, -4) m. Exact exposure of the mosaicked frame not established beyond the graph range; native ground resolution not read from metadata. The catalogue records frames, not sites.  |
| AI-02 | aerial_index | [IGN historical orthomosaic ORTHOIMAGERY.ORTHOPHOTOS.1950-1965 (WMS-R), 1 km context]([query URL with coordinates removed]) | 1 km window at 1 m/px | SCOPED_NULL |  | Woodland west of a road, small fields to the east and south-east; parcel strips as today.  |
| AI-03 | aerial_index | [IGN aerial frame index (WFS pva:image)]([query URL with coordinates removed]) | frames whose footprint contains the lead | SCOPED_NULL |  | Frames 1949-1965 listed for the point: 1949-06-14 (2622-0081), 1957-04-04 (2622-0071), 1959-04-21 (2522-0081). Coverage only; no individual frame was viewed in this pass.  |
| AI-04 | aerial_index | [IGN BD ORTHO 2000-2005 (WMS-R ORTHOIMAGERY.ORTHOPHOTOS2000-2005)]([query URL with coordinates removed]) | 300 m window at 0.5 m/px | SCOPED_NULL |  | Closed broadleaf canopy: non-diagnostic.  |
| AI-05 | aerial_index | [IGN current orthophoto and infrared colour orthophoto (WMS-R)]([query URL with coordinates removed]) | 300 m and 1 km windows | SCOPED_NULL |  | Closed broadleaf canopy (IRC: broadleaf): non-diagnostic.  |
| AI-06 | aerial_index | [IGN historical orthomosaics ORTHOIMAGERY.ORTHOPHOTOS.1965-1980 and 1980-1995 (WMS-R)]([query URL with coordinates removed]) | 300 m window at 0.5 m/px | ACCESS_FAILURE |  | Both layers returned blank tiles for this window (tried once). Alternatives: FR1 records screen: the IGN 1965-1980 and 1980-1995 orthomosaic layers returned blank tiles there as well; IGN frame index (AI-03) lists later frames; individual frames not viewed (interactive viewer); BD ORTHO 2000-2005 (AI-04) |
| LT-01 | literature | [Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), commune entry](https://gallica.bnf.fr/services/ContentSearch?ark=bd6t542083795&query=%22102%20-%20Donzy%22) | "102 - Donzy" and thematic queries (enclos, enceinte, tumulus, motte, ferrier, scories, etang, circulaire) | SCOPED_NULL |  | Donzy entry (pp. about 141-142): placeable items lie 3.1 km or more away (14* Terres de la Motte, rectangular enceinte about 85 x 58 m, 3,115 m; 2* Les Chandeliers, circular enclosure about 35 m, 4,259 m; 16* La Chaume Martin and 3* Champ de Gehenne enceintes, not nearer). Item 1* has no location (LT-04). No tumulus, slag heap or motte item names a lieu-dit near the lead. Read at excerpt level (Gallica ContentSearch); full pages show a security check to automated access.  |
| LT-02 | literature | [Bigeard H. 1996, Carte archeologique de la Gaule 58: La Nievre (Gallica ark:/12148/bd6t542083795), lieu-dit search](https://gallica.bnf.fr/services/ContentSearch?ark=bd6t542083795&query=Maufenauds) | names of the lieux-dits and places within about 1 km of the lead | SCOPED_NULL |  | Maufenauds 0 hits; Maufrenauds 0 hits; Châtelaine 0 hits; Fourneaux 18 hits; "Champ de Fée" 0 hits; "Bois Brûlé" 0 hits; "Bois Maret" 0 hits; "Chétifs Bois" 0 hits; "Champ du Puits" 3 hits. No hit places an item at or next to the lead, other than the items rowed in LT-01/LT-05; hits elsewhere concern other communes or generic words.  |
| LT-03 | literature | [Bouthier A., 'L'occupation du Nord-Ouest du Nivernais et les zones voisines aux epoques protohistoriques, vue d'avion', B@sic 1 (Ausonius, 2013; online 2024)](https://una-editions.fr/occupation-nord-ouest-nivernais-epoques-protohistoriques/) | commune inventory and the tumulus passage | SCOPED_NULL |  | Donzy: 13 enceintes; 5 square enclosures on 2 sites without enceintes; 1 circular enclosure (aerial cropmarks, no positions). Circular enclosures in the study area measure 8-30 m (28 on 17 sites). Counts read from the local text copy and independently from the HTML edition by the lead-researcher.  |
| LT-04 | literature | [Unlocated items of compatible class in the commune: CAG 58 Donzy 1* (004) and tumuli near Donzy (Vielmanay monograph)](https://gallica.bnf.fr/services/ContentSearch?ark=bd6t542083795&query=%22102%20-%20Donzy%22) | location of the item | ACCESS_FAILURE |  | CAG 1* '(Localisation ?) Sur un cliche de J. Meissonnier, on devine des traces peu nettes qui evoquent un enclos circulaire' (aerial report 1983); the Vielmanay monograph (LR-07) mentions Hallstatt tumuli observed 'aux environs de Donzy'. Neither is placed. The lead has been woodland since the Cassini map, which argues against an aerial cropmark record here, but the positions must be read before the mound can be called distinct. Alternatives: CAG thematic index (enclos circulaire: 102 1*, 2*); Persee phrase search for Donzy (LR-17); Bouthier 2013 counts (LT-03); Gallica ContentSearch of nearby lieux-dits (LT-02) |
| LR-02 | literature | [Google Books full-text API (all books)](https://www.googleapis.com/books/v1/volumes?q=Maufenauds&maxResults=20) | q=Maufenauds, maxResults=20 | ACCESS_FAILURE |  | HTTP 429 Too Many Requests on the second request to this service. Alternatives: HathiTrust full-text search for the same term (HTTP 403; LR-03); engine search for Maufenauds (address directories only); Gallica ContentSearch of the CAG 58 for Maufenauds and Maufrenauds (0 hits; LT-02) |
| LR-03 | literature | [HathiTrust full-text search](https://babel.hathitrust.org/cgi/ls?q1=Maufenauds&anyall1=phrase&lmt=all) | q1=Maufenauds, phrase, all volumes | ACCESS_FAILURE |  | HTTP 403 Forbidden. Alternatives: Google Books API (HTTP 429; LR-02); engine search (directories only) |
| LR-04 | literature | [Chevrier S. 2009, 'Les enceintes pre-medievales du Nivernais-Morvan', Revue archeologique de l'Est 58 (OpenEdition)](https://journals.openedition.org/rae/5544) | full text, figures and inventory checked for Donzy, Narcy, Ciez, Dampierre-sous-Bouhy, Suilly-la-Tour | SCOPED_NULL |  | None of the five communes appears in the text, figures or inventory (1, Asnan to 24, Varzy).  |
| LR-07 | literature | ['Le tumulus-necropole de la Bonneterie a Vielmanay (Nievre)', ARTEHIS Editions (OpenEdition Books), section 1 'Situation' (authorship given by the fetch as Adam et al. 2002, not checked)](https://books.openedition.org/artehis/17380) | sentences naming Donzy, Ciez, Narcy, Suilly, Dampierre, Bouhy, Jussy | SCOPED_NULL |  | Donzy occurs only in general statements: Hallstatt tumuli observed 'aux environs de Donzy' with central inhumations, and bracelets and torques from Bouhy and Donzy in an old collection. Neither is located. The tumuli are a compatible class (round mound), so this row is carried as unlocated in LT-04.  |
| LR-12 | literature | [Bouthier A. 1999, 'Parcellaires fossiles dans la vallee du Nohain', Revue archeologique de Picardie, numero special (Persee)](https://www.persee.fr/doc/pica_1272-6117_1999_hos_17_1_2132) | article text checked for the five communes and the lieux-dits near the leads | ACCESS_FAILURE |  | Metadata and page thumbnails only; no text layer readable by the fetch tool. Snippets say Ciez is among 17 Nohain-valley communes studied. Alternatives: https://www.persee.fr/docAsPDF/pica_1272-6117_1999_hos_17_1_2132.pdf (HTTP 403) |
| LR-17 | literature | [Persee full-text search](https://www.persee.fr/search?q=%22Donzy%20(Ni%C3%A8vre)%22) | "Donzy (Nievre)" | SCOPED_NULL |  | Town, castle and priory notices (Bouthier 1986, 1999, 2000; Meissonnier 2000; Notre-Dame-du-Pre). No tumulus, motte, enclosure, slag heap, forge or the lieux-dits near the leads. Results 11-90 not viewed.  |
| LR-21 | literature | [Gallica (BnF) SRU API](https://gallica.bnf.fr/SRU?operation=searchRetrieve&version=1.2&query=gallica%20all%20%22Chailloy%22&maximumRecords=20) | gallica all "Chailloy", maximumRecords=20 | ACCESS_FAILURE |  | HTTP 403. No security check was attempted or bypassed. Alternatives: FR1 records screen (2026-10-02): Gallica page views of the CAG 58 show a security check to automated access; Gallica ContentSearch inside the CAG 58 (worked; LT-01, LT-02); HathiTrust full-text search (HTTP 403); camosine.fr general index (LR-22) |
| LR-22 | literature | [camosine.fr general index (Nievre local-history publication index)](https://camosine.fr/pages/pages-index/page-table-index-general.html) | index entries for Donzy, Suilly-la-Tour, Chailloy, Narcy, Ciez, Dampierre-sous-Bouhy, forges, fourneaux, ferriers, laitiers, tumulus, motte, Usages, tuilerie | SCOPED_NULL |  | No entry names the five communes or Chailloy. A thematic heading on metallurgy covers the Nohain valley (issue not identified; not read).  |
| LR-25 | literature | [HAL search API, archaeology domain filter](https://api.archives-ouvertes.fr/search/?q=(Donzy%20OR%20%22Suilly-la-Tour%22%20OR%20Ciez%20OR%20Narcy%20OR%20%22Dampierre-sous-Bouhy%22)%20AND%20Ni%C3%A8vre&fq=domainAllCode_s:shs.archeo&rows=50&wt=json) | (Donzy OR "Suilly-la-Tour" OR Ciez OR Narcy OR "Dampierre-sous-Bouhy") AND Nievre; fq=domainAllCode_s:shs.archeo | SCOPED_NULL |  | numFound 0. The filter was not validated against a known positive, so this null is provisional.  |

Searches without a URL:

- LRP3 engine (regional_record, ZPPA): "zones de presomption de prescription archeologique Nievre arrete Donzy Narcy Suilly-la-Tour"; the same with site:culture.gouv.fr; "Bourgogne-Franche-Comte ... arretes communes Nievre Yonne liste"; "recueil des actes administratifs" Nievre "presomption de prescription archeologique": no DRAC BFC ZPPA page, order or commune list for the five communes; the Nievre RAA index was listed but not opened.
- LRP3 engine (ADLFI): site:journals.openedition.org/adlfi with Donzy Nievre, and with Suilly-la-Tour OR Narcy OR Ciez OR "Dampierre-sous-Bouhy": no notice for the five communes.
- LRP3 engine (literature): CAG 58 open copy (publisher and bookseller pages only); "Usages de Jussy" Ciez tumulus and Ducreux tumulus Ciez (only via Bouthier and the Vielmanay monograph); Narcy Usages / Gros Laitiers / ferrier / tuilerie Bertranges; "Marteauneuf" Narcy forge (led to IA58000639); local society tumulus articles with the communes: none found.
- LRP3 engine (planning): PLUi "Coeur de Loire" archeologie "entites archeologiques" Donzy Suilly-la-Tour Ciez; PLUi Puisaye-Forterre annexe archeologie "zones de presomption" OR "sites archeologiques" Dampierre-sous-Bouhy: no archaeology annex found.
- LRP3 engine (lieux-dits): "Maufenauds" OR "Maufrenauds" OR "Champ de Chatelaine" Donzy: street and address directories only.

## Q4 decision-changing question (draft; contact not justified in this pass)

Question: Does the restricted Carte archeologique nationale hold an entity at this mound in the Donzy woods (for example a tumulus or a slag heap), and where is the unlocated Donzy circular-enclosure item of the CAG 58 (commune 102, item 1*, Meissonnier 1983)?

Changes: drop as a discovery lead (known site) versus keep for a qualified assessment

- A CAN entity or the CAG item lies here -> Q3 RECORDED: detection of a known site; drop from the discovery count
- No entity here and the CAG item lies elsewhere -> Q3 SCOPED_NULL or NEARBY_DISTINCT: after the challenge pass, candidate for the questions-only SRA letter asking for a record check and assessment
- A challenger or the SRA identifies post-medieval slag or spoil -> Q2 ORDINARY_EXPLANATION_LIKELY: drop

Answerable by: Public first: full CAG 58 page for Donzy (printed p. about 134) read by the owner in an ordinary browser (Gallica shows a security check to automated page access); then SRA Bourgogne-Franche-Comte for the CAN.

Next action: 1. Independent challenge pass. 2. Owner or challenger reads the full CAG Donzy entry. 3. If still unmatched, candidate for the questions-only SRA letter. No correspondence in this pass.

Outstanding public routes: full CAG 58 Donzy page in an ordinary browser; forest-management or local-history sources for the wood; Atlas des patrimoines (catalogue route failed here); IGN frames 1949-1959 viewed individually (woodland: low value)

## Challenge priorities

- Read the full CAG 58 Donzy entry (printed p. about 134) and place item 1* (unlocated circular enclosure, Meissonnier 1983).
- Search for slag-heap (ferrier) and furnace records for the woods around "les Fourneaux" and "Chatelaine".
- Check whether the mound is a known barrow in Donziais woodland literature (local societies, Bouthier).

## Evidence caveats

- All terrain views come from one IGN LiDAR HD DTM; the MNH is a product of the same survey. Orthophotos are the only independent source.
- Heights are residuals from an annulus plane or detrended profiles, not construction heights.
- The 1950-1965 imagery is IGN's processed orthomosaic served by WMS: the mosaic graph gives a date range, not the exposure of the frame used, and no individual frame was viewed.
- The CAG 58 (1996) was read at excerpt level through Gallica ContentSearch; full pages show a security check to automated access. Distances to CAG items are to cadastral lieu-dit polygons, not to the items.
- Public nulls do not clear the restricted Carte archeologique nationale (Patriarche).

Correspondence: none (No draft exists for this lead. The challenge pass and contact gate come first.)

## Challenge pass (2026-10-02)

Reviewer: Claude Opus 5.5 challenge agent; independent of the research pass; receipt [internal file]. **Outcome: SURVIVES.** Validator re-run after the challenge block was added: pass, class unvetted.

- Independent search (POP Merimee form, PLU 2023 rapport and SUP list, GPU point layers, Cassini, Etat-major, SCAN50 1950, IGN 1950-65 orthophoto, Camosine index, Bouthier 2013/2024 counts, web) found no record at the mound; the PLU carries no SRA list and the CAN is restricted.
- Factual error corrected: q3.basis said Merimee has nothing within 5 km; the same open dataset (merimee_current.csv, sha256 65c493db...) holds PA00112985 chateau de la Motte-Josserand (Perroy) at 3.9 km and PA00112788 church of Alligny-Cosne at 4.6 km. NI-01 was restricted to five communes. Both distinct; status unaffected.
- Added historic map: cadastre ancien Donzy section B feuille 1 (AD Nievre ark:/60877/tnmq6fljhsgk) shows lieu-dit Les Maufenauds in narrow NW-SE strips, the orientation of the groove crossing the mound, and no symbol at the mound; supports the parcel-boundary reading of the groove.
- Method caveat: the 0.72 m centre residual uses a 15-30 m annulus that overlaps the mound flank (zero at r about 21 m); a 35-50 m annulus gives 1.15 m, consistent with the 1.29 m profile maximum.
- Two pit clusters lie 0.3-0.6 km N and W in the same DTM tile (unassessed ore or quarry pits): relevant to the slag-heap reading, not adjacent to the mound.
- Q4 survives. SRA question: is there a recorded entity at this mound (parcel YC 111), and is it the unlocated CAG 58 Donzy item 1*?

Correction applied in `dossier.json` (`q3.correction`): the Q3 basis above that reads "Merimee has nothing within 5 km" is superseded by "Merimee has nothing within 3.9 km (nearest: PA00112985 chateau de la Motte-Josserand, Perroy, 3.9 km; distinct)".
