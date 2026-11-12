# L1 challenge pass receipt

- Brief: [internal file]. Web and in-app browser tools only; phase 1 on case inputs only,
  phase 2 (dossier summary + priority claims) sent afterwards in the same agent context.
- Transcript: `challenge_transcript.jsonl`, sha256 `488d1de6a087dd1ccbbaf9a6ccd05e0ed4472ce2059193683bc3b54de4fc85a5`. Counts below are mechanical ([internal file]); batched actions count as calls.
- Phase 1: 43 calls (budget 45); deviations: none.
- Phase 2: 30 calls (budget 30); deviations: none.

## Phase 1 report (verbatim)

P1_FINDINGS:

Method notes:
- I converted the CH-L1 position by hand using the inverse Lambert-93 conic formula (IGN constants n=0.7256077650, C=11754255.426, Xs=[coordinate removed], Ys=12655612.050, GRS80 ellipsoid). Result: about [coordinate removed]°N, [coordinate removed]°E, within roughly ±50 m.
- I converted Chevrier's coordinates by hand using the inverse Lambert II étendu formula (NTF datum, Clarke 1880 IGN ellipsoid, Paris meridian [coordinate removed]°E, n=0.7289686274, C=11745793.39, Ys=8199695.768). I then applied a three-parameter Molodensky shift from NTF to WGS84 (−168, −60, +320 m). This is also roughly ±50 m.
- Distances are straight-line Lambert-93 distances.
- Coordinates went only into IGN services. None went into web search.

1. **Cadastre.** IGN Parcellaire Express WFS and WMS on data.geopf.fr, bbox [coordinate removed],[coordinate removed],[coordinate removed],[coordinate removed] in EPSG:2154.
   - CH-L1 lies inside parcel `parcelle.31002657`: Sainte-Colombe-des-Bois (INSEE 58236), section C, n° 0202, 360,208 m² (about 36 ha).
   - To the south is Châteauneuf-Val-de-Bargis (58064) E 0717 (`parcelle.81198113`, about 22.3 ha).
   - I overlaid the cadastre on the LiDAR HD terrain hillshade (0.67 m per screen pixel). No parcel boundary coincides with any enclosure side.
   - The nearest cadastral line is a double line (a path strip between the two communes). It runs obliquely about 25–45 m south of the enclosure's south side.

2. **Commune boundary.** ADMIN EXPRESS COG CARTO WFS (`ADMINEXPRESS-COG-CARTO.LATEST:commune`).
   - The generalised boundary between Châteauneuf-Val-de-Bargis and Sainte-Colombe-des-Bois has vertices at ([coordinate removed], [coordinate removed]) and ([coordinate removed], [coordinate removed]). That is about 60 m south of the centre point, and it matches the cadastral path.
   - The enclosure is not on the commune boundary. The boundary explanation is not supported for the enclosure itself.

3. **Place names.** BD TOPO `BDTOPO_V3:lieu_dit_non_habite`.
   - "les Quatre-Vingts Arpents" (nature: Bois) at ([coordinate removed], [coordinate removed]), 62 m ENE of the centre. It names the wood block. 80 arpents is about 27–41 ha, which fits the 36 ha of parcel C 202.
   - "le Châtelet" (Bois) at ([coordinate removed], [coordinate removed]), 1.55 km SSW.
   - `BDTOPO_V3:zone_d_habitation` gives the inhabited place "le Châtelet" at about ([coordinate removed], [coordinate removed]), 1.30 km SW. The hamlet "Asvins" is at about ([coordinate removed], [coordinate removed]), 0.65 km S.

4. **Public forest.** IGN WMS layer `FORETS.PUBLIQUES`.
   - CH-L1 is inside a public-forest polygon, in forest parcel "23".
   - The straight dividing line between parcels 22 and 23 runs WNW–ESE about 40–60 m north of the enclosure's north side. It does not coincide with any side and is not parallel to the south side.
   - I could not get the forest's name or status: the GetFeatureInfo request returned HTTP 400.

5. **Historical maps.** WMS layers `GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40` and `ORTHOIMAGERY.ORTHOPHOTOS.1950-1965`, 1 km and 400 m windows.
   - État-major map (1820–1866): no woodland symbol and no enclosure symbol at CH-L1. The area is uncoloured with relief hachures. My reading of the colours is uncertain.
   - 1950–65 orthophoto: CH-L1 sits in an elongated smooth-textured zone matching parcel C 202, which looks like a clearing or young growth. Mature woodland lies south of the path, and that wood edge runs about 15–30 m south of the enclosure's south side. No enclosure outline is visible.
   - This leaves an agricultural or forestry-compound origin plausible, but it does not document one.

6. **Nearest recorded enclosure: Le Châtelet.** This is NEARBY_DISTINCT.
   - Chevrier 2009 (https://journals.openedition.org/rae/5544?lang=fr), site 4, "Châteauneuf-Val-de-Bargis, Le Châtelet":
     - Quadrangular, oriented SE/NW, long sides 80 m, short sides 60 m, about 1 ha.
     - Bank about 2 m high, flat-bottomed ditch about 1 m deep, a single entrance on the NW flank. No dating evidence.
     - Recorded position: Lambert II étendu x 663.148 km, y 2255.108 km, 270 m altitude.
   - Wiki58 (https://www.gennievre.net/wiki/index.php/Chateauneuf_Val_De_Bargis_Arch%C3%A9ologie), citing B. Colas: protohistoric quadrangular enclosure, 70–100 m per side, inner bank 1–2 m, ditch 0.5–1 m.
   - LiDAR HD hillshade shows a sharp quadrangular banked enclosure about 90–97 m per side (outer crest, read at 1 m per screen pixel). Its centre is about ([coordinate removed], [coordinate removed]), 283 m from the BD TOPO "le Châtelet" wood label.
   - Chevrier's position converts to about ([coordinate removed], [coordinate removed]), about 315 m west of that enclosure. At the converted point there are only field banks and forest-ride lines, no second enclosure.
   - Distance to CH-L1: 1.49 km to the visible enclosure, about 1.55 km to the converted Chevrier point.
   - Form comparison: same plan type and similar size (CH-L1 is 88 × 71 m). Le Châtelet has much stronger relief: a 1–2 m bank plus a ditch. CH-L1's west bank is 0.3 m above the inner foot and 1.1 m above the outer foot, no ditch is reported, and its north side is discontinuous.

7. **Other Wiki58 entries for Châteauneuf-Val-de-Bargis (A. Magdelaine).**
   - "La Forêt": a ditch outlining a motte-like quadrangular platform, undated.
   - "La Rolande": a small quadrangular platform, two ditches near the farm, and an old path to the west.
   - Neither place name appears in BD TOPO `zone_d_habitation` within ±3 km of CH-L1, so I could not place them.

8. **Searches that found nothing** (scoped).
   - Wiki58 archaeology index (https://www.gennievre.net/wiki/index.php/Arch%C3%A9ologie_et_vestiges): the "Sainte Colombe" page does not exist.
   - Chevrier 2009: no entry for Sainte-Colombe-des-Bois, Suilly-la-Tour or Bellary. This is weak evidence: an earlier summary of the same page also missed site 4.
   - WebSearch `"Sainte-Colombe-des-Bois" Nièvre archéologie enceinte OR camp OR Châtelet OR retranchement`: no enclosure record. Mousterian tools are the only archaeology mentioned.
   - WebSearch for "Quatre-Vingts Arpents" with Sainte-Colombe, Suilly or Bargis: nothing relevant.
   - WebSearch for a ZPPA (archaeological presumption zone) order covering either commune: none found.
   - WebSearch for the commune's entry in the Carte archéologique de la Gaule 58 (Bigeard 1996): the text is not online, so unchecked.

9. **Access failures and routes not reached.**
   - Access failures:
     - www.wiki58.fr did not resolve (DNS).
     - Two gennievre URL guesses returned 404 before I found the correct page.
     - The WMS refused a three-layer request (limit is two).
     - The browser zoom action is not supported.
     - The Nièvre archives search hit (https://archives.nievre.fr/ark:/60877/a011513328229WVeqW7) is only a 1907 postcard (2 Fi Communes 236/6).
   - Not reached within budget: the Napoleonic cadastre plans for Sainte-Colombe, the Atlas des patrimoines, and the Géoportail de l'urbanisme / API Carto.

P1_BEST_READING: NEARBY_DISTINCT. I found no record, publication or map of CH-L1 itself in the sources above. The nearest recorded enclosure of the same kind is Le Châtelet (Chevrier 2009 site 4; Wiki58/B. Colas). It is about 1.49 km SSW and matches a sharp LiDAR enclosure at its own place, so it is not a mislocated record of CH-L1. No ordinary explanation is documented. Current cadastral parcel, commune and ONF forest-parcel boundaries do not coincide with any side. CH-L1 lies inside the named wood block "les Quatre-Vingts Arpents", inside a public forest. That block was mapped without woodland in 1820–66 and looked cleared or young around 1950–65. A post-medieval agricultural or forestry-compound origin therefore stays plausible but undocumented.

CALLS: 43. This includes two calls I mistakenly sent to tabId "3" before `tabs_create` returned my tab: a navigate that reported "denied or failed" and a screenshot that reported "tab 3 no longer open". No action is known to have taken effect in another tab. ToolSearch is not counted.

## Phase 2 report (verbatim)

P2_CLAIMS:
1. **Lead at or within metres of the commune boundary, possibly partly in Châteauneuf-Val-de-Bargis: CONTRADICTED.**
   - Test: an exact intersection query on IGN Parcellaire Express (`[query URL with coordinates removed] [coordinate removed],[coordinate removed] [coordinate removed],[coordinate removed] [coordinate removed],[coordinate removed] [coordinate removed],[coordinate removed] [coordinate removed])))`).
   - Result: "1 feature … parcelle.31002657 … Sainte-Colombe-des-Bois … 0C … 0202".
   - Control: a strip at Y [coordinate removed]–[coordinate removed] returns both C0202 and Châteauneuf E0717, so the boundary lies south of Y [coordinate removed] across X [coordinate removed]–[coordinate removed].
   - Why the dossier saw both communes: a plain bounding-box query on [coordinate removed],[coordinate removed],[coordinate removed],[coordinate removed] also returns "2/2", but that filter matches parcel envelopes, not shapes. E0717's envelope peaks at Y [coordinate removed] at its west end, about X [coordinate removed] (the ADMIN EXPRESS vertex there is [coordinate removed], [coordinate removed]), roughly 200 m west of the enclosure. The dossier's two-commune hit is this envelope artefact.
   - Position: the boundary is the path strip about 25–45 m south of the enclosure's south side (hillshade and cadastre overlay; generalised ADMIN EXPRESS vertex [coordinate removed], [coordinate removed]). That path is also where two public-forest ownerships meet.
   - Precision: my footprint corners are read from 0.67 m/pixel screenshots, about ±5 m. The cadastral dataset itself is accurate to within metres to tens of metres in rural areas.
   - The enclosure lies wholly in Sainte-Colombe-des-Bois at cadastral precision.
2. **Boundary or parcel-bank explanation (≥2 sides followed): current and mapped limits CONTRADICTED; 1827 cadastre UNVERIFIABLE.**
   - Current cadastre: the exact test above puts the whole footprint inside one 36.0 ha parcel (C0202). The overlay shows no parcel limit on any side.
   - Public-forest parcels (IGN `FORETS.PUBLIQUES` layer over the LiDAR hillshade, 400 m window): the line between forest parcels 22 and 23 is oblique and runs 35–80 m north of the enclosure. The southern ownership limit is the commune path, 25–45 m south.
   - État-major map (1820–66, 400 m window, `GEOGRAPHICALGRIDSYSTEMS.ETATMAJOR40`): no line runs through or along the enclosure, only relief hachures. The dotted, colour-washed commune-limit band lies at least 70 m SW (map registration about ±50 m). A straight N–S line at X ≈ [coordinate removed] lies about 120 m east of the east side. The dossier's "boundary-style line near the centre" does not reproduce. It may have been the cadastral overlay drawn on top.
   - 1827 cadastre, section C "dite de Couthion": I located the sheets but could not view them. Sheet 1 is 3PPLANS/236/5 (https://archives.nievre.fr/ark:/60877/tp2x1g9jrkmf). Sheet 2 is 3PPLANS/236/6 (https://archives.nievre.fr/ark:/60877/f4mvzn1hpq8t). Sheet 3 is 3PPLANS/236/7 (https://archives.nievre.fr/ark:/60877/xhf5j4k8vn2c). The assembly sheet is 3PPLANS/236/1. The viewer stayed covered by a menu overlay and the cookie notice. Plot name not checked. Châteauneuf's old plans not searched.
3. **"La Forêt" and "La Rolande" can be located (SUPPORTED); either being the lead is CONTRADICTED.**
   - Source: BD TOPO `zone_d_habitation` place-name search.
   - "la Rolande" is at ([coordinate removed], [coordinate removed]), in Châteauneuf section A parcel 0213, **7.99 km ESE** of CH-L1.
   - "la Forêt" is at ([coordinate removed], [coordinate removed]), in Châteauneuf section A parcels 0083/0085, **6.18 km ESE**.
   - A third "Forêt" at ([coordinate removed], [coordinate removed]) is in Chasnay (58061), 7.1 km SSW.
   - The Wiki58 entries are placed by these hamlets: "A La Forêt a été photographié un fossé…" and "A l'est de La Rolande…".
   - The forms also differ from CH-L1: a ditch round a platform, and a small platform, against CH-L1's banks round a sloping interior.
4. **Chevrier 2009 has no other entry for either commune: SUPPORTED.**
   - Method: browser text search of the full French article (https://journals.openedition.org/rae/5544?lang=fr).
   - "Bargis" gives 5 matches, all for site 4: "4- Châteauneuf-Val-de-Bargis, Le Châtelet (x : 663,148 ; y : 2255,108 ; 270 m)" and "Fig. 6. A. Plan du camp carré du Châtelet".
   - "Colombe" gives 0 matches.
5. **A CAG 58 or other published entry describing the lead: UNVERIFIABLE.**
   - The CAG 58 text (Bigeard 1996) is not online.
   - Cahiers du Val de Bargis lieux-dits page (http://cahiersduvaldebargis.free.fr/chat_lieux-dits.html): "enceinte" gives 0 matches.
   - A search snippet from the same site repeats Colas's Le Châtelet text and says Le Châtelet belonged to the Chartreuse de Bellary before the Revolution.
   - B. Colas's description (via Wiki58) refers to Le Châtelet.
   - None of these routes found an entry describing CH-L1.

P2_MISSED:
- The bounding-box envelope artefact behind the Q2 commune claim.
- Le Châtelet is visible as a sharp banked quadrangle on LiDAR HD at about ([coordinate removed], [coordinate removed]), 1.49 km away, and Chevrier publishes its plan as Fig. 6. It is the recorded analogue, and it is distinct from CH-L1.
- CH-L1 sits in a public forest, forest parcel 23. The southern path also divides two public forests.
- Land-use history: non-wooded on the État-major map, and a clearing or low growth on the 1950–65 photography. The current woodland is probably later than the 1860s. That leaves a post-medieval field or pasture enclosure possible, but undocumented.
- Le Châtelet belonged to the Bellary estate, which is relevant if old estate limits are tested.

P2_OVERSTATED:
- "At or near the boundary": the boundary is 25–45 m south and the enclosure is wholly in Sainte-Colombe.
- The État-major "line near the centre" does not reproduce.
- Q3 reason 1: La Forêt and La Rolande can be positioned, and they are 6–8 km away.
- Q3 reason 2: the Sainte-Colombe SRA extract covers the lead's commune. A Châteauneuf extract is a minor residual check only.
- "91 Arpens" / "Quatre-Vingts Arpents" measures a 27–41 ha wood lot. It is not evidence for a 0.6 ha bank.

P2_STATUS_SURVIVES: No. UNRESOLVED's stated grounds 1 and 2 fail. The best reading is NEARBY_DISTINCT: the nearest positioned record of this form is Le Châtelet, 1.49–1.55 km away and matched to a separate visible enclosure. If the protocol's radius excludes 1.5 km, the reading is SCOPED_NULL. The scope must name what stays unread: CAG 58, the 1827 cadastre sheets C1–C3, and the SRA extract for Châteauneuf. Only those could move it to RECORDED.

P2_Q4_SURVIVES: Partly. The present-day half is answered: no current limit follows ≥2 sides, and the commune limit passes 25–45 m south. Under the rule as written that is a keep. The 1827 half is open. Proposed rewording: "Using exact geometry (not bounding boxes), does any present-day cadastral limit, public-forest parcel or ownership limit, or 1827 plot limit follow ≥2 sides? Does the 1827 plan show the enclosure as a separate plot, a building, or a named feature, and with what land use? Follows ≥2 sides or a matching separate plot → drop as a probable post-medieval plot. Earthwork name → keep as possibly known. Neither → keep. Sheet not registered → no change." Register sheet C2 on the commune path and a parcel corner.

LIMITS:
- The 1827 cadastre was not viewed (viewer overlay).
- CAG 58 and the SRA archaeological map were not accessible.
- My Lambert II étendu and WGS84 conversions were done by hand, about ±50 m.
- Corner positions come from screenshots, about ±5 m.
- État-major registration is about ±50 m.
- WFS results were summarised by a helper model. Counts and parcel IDs are reliable; vertex lists are not.
- The forest's name and status are unknown (the feature-info request returned HTTP 400).
- One query hit a 20-feature cap and was redone.

CALLS: 30. The first call was `tabs_create` (tab-18), and every browser call used that tab. One click landed on a site menu link ("Salle de lecture"): navigation only, no form submitted, cookie notice not clicked. tab-18 closed at the end.
