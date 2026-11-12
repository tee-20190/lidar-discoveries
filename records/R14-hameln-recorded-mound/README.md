# R14: Mound reported before, now formally recorded, Stadt Hameln, Lower Saxony

| | |
|---|---|
| Status | Added to an official heritage record (not a confirmed new archaeological site) |
| Assessed by | Dr Daniel Lau, Kommunalarchäologe (municipal archaeologist), Kommunalarchäologie Schaumburger Landschaft (municipal archaeology service) |
| Assessment date | 2026-11-02 |
| Official record | Hameln FStNr. 254 |
| Label in the submission | `SL-05` |
| Detector | S_D + PROX |
| Limitations | Known before our submission; our evidence enabled formal recording. Not a discovery. |

The assessing archaeologist's reply is quoted on the [D04 page](../../discoveries/D04-schaumburg-burial-mound/README.md#the-assessment-verbatim), which covers the same batch.

## Everything we looked at

The full internal evidence card is in [`evidence/`](evidence/) ([file list](evidence/README.md)): every image and
record the project used to decide whether to submit this location, plus what was sent to the authority.
Coordinates are removed; nothing else is edited.

**LiDAR terrain (LGLN DGM1, 1 m).** Hillshade at 150 m and 500 m, and a local relief model:

![DGM1 hillshade 150 m and 500 m](evidence/lidar_dgm1_hillshade_150m_and_500m.png)

<img src="evidence/lidar_dgm1_local_relief_150m.png" width="360" alt="Local relief model, 150 m">

**Orthophotos (LGLN DOP20), every year available**, used to rule out modern heaps, buildings and earthworks:

| 2013-07-08 | 2016-07-20 | 2019-04-07 | 2022-05-03 | 2025-03-09 | 2025-03-09 |
|---|---|---|---|---|---|
| <img src="evidence/dop20_2013-07-08.jpg" width="150"> | <img src="evidence/dop20_2016-07-20.jpg" width="150"> | <img src="evidence/dop20_2019-04-07.jpg" width="150"> | <img src="evidence/dop20_2022-05-03.jpg" width="150"> | <img src="evidence/dop20_2025-03-09.jpg" width="150"> | <img src="evidence/dop20cir_2025-03-09.jpg" width="150"> |

**Historic map.** First-edition Messtischblatt (1897), checked for a mapped structure, pit or building at the point:

<img src="evidence/messtischblatt_1897.png" width="300" alt="Messtischblatt">

**The model reader's review before submission** (verbatim extracts from [`reader_review.json`](evidence/reader_review.json)):

> Isolated round domed mound about 12 m across and 0.9 m high on a gentle wooded slope; no adjacent pit; a registered Grabhügel of similar size lies 271 m away.

Open alternative it asked the archaeologist to weigh: *Is this a natural knoll or a charcoal-burning platform on the slope rather than a barrow?*

Most likely non-archaeological explanation it considered: `NAT` (OPEN-WEAK); verdict `SENDABLE`.

**Detector output** ([`detection.json`](evidence/detection.json)): model `D_101`; mean probability 0.952; area 364 m², roundness 0.95; nearest registered burial mound 271 m away in the public register snapshot.

**What the authority received** (one sheet per location, coordinate line removed):

<img src="evidence/submitted_sheet.png" width="600" alt="Submitted sheet">
