# D03: Barrow field, Gemeinde Groß Berßen, Landkreis Emsland

![150 m LiDAR hillshade centred on D03](lidar_hillshade_150m.png)

| | |
|---|---|
| Status | **Confirmed: previously unknown archaeological site** |
| Location | Gemeinde Groß Berßen, Landkreis Emsland, Lower Saxony (municipality level; exact coordinates withheld, see below) |
| Feature | Barrow field (several mounds; number not stated by the assessor) |
| Assessed by | **Thomas Kassens, Kreisarchäologe (district archaeologist)**, Kreisarchäologie Landkreis Emsland (district archaeology service) |
| Written assessment | 2026-10-29 |
| Label in the submission | `EL-11` |
| Official record | none reported |
| Detector | S_D + PROX |
| Terrain | LGLN DGM1, 1 m (CC BY 4.0) |
| Coordinate commitment (SHA-256) | `3b40323d000630d0d164068147d4124eb5315da180181824c1a18e2de42e8c58` |

## How it was found

Proposed by S_D + PROX. The assessor confirmed the field as previously unknown without stating how many mounds it contains, so it is counted once. The location was screened against the public Denkmalatlas Niedersachsen and reviewed by language-model readers
before it was submitted. The project owner then sent it to the responsible archaeologist with coordinates and LiDAR
views.

## The assessment, verbatim

The archaeologist's reply, as received. Contact details and the quoted earlier message are removed; `[…]` marks other
omissions and `[Fundstelle entfernt]` marks the names and numbers of already known sites, which are not ours to publish.

> Sehr geehrter Herr Shanahan,
>
> vielen Dank für die Daten. In einigen Fällen waren es tatsächlich bisher unbekannte Grabhügel.
>
> EL-01 Bekannt
> EL-02 Bekannt
> EL-03 kein Grabhügel
> EL-04 Bekannt
> EL-05 bekannt aber bisher Falsch Markiert
> EL-06 Bisher Unbekannt
> EL-07 Unsicher
> EL-08 Kein Grabhügel
> EL-09 Kein Grabhügel
> EL-10 Bisher Unbekannt
> EL-11 Bisher Unbekannt (Grabhügelfeld)
> EL-12 unsicherer Grabhügel
> EL-13 kein Grabhügel
> EL-14 bekannt aber bisher Falsch Markiert
> EL-15 Bekannt
>
> Mit freundlichem Gruß
> Im Auftrag
>
> Thomas Kassens
> (Kreisarchäologe)

**English translation (ours):**

> Dear Mr Shanahan,
>
> Thank you for the data. In some cases these were indeed previously unknown burial mounds.
>
> EL-01 known · EL-02 known · EL-03 not a burial mound · EL-04 known · EL-05 known but previously marked wrongly ·
> **EL-06 previously unknown** · EL-07 uncertain · EL-08 not a burial mound · EL-09 not a burial mound ·
> **EL-10 previously unknown** · **EL-11 previously unknown (barrow field)** · EL-12 uncertain burial mound ·
> EL-13 not a burial mound · EL-14 known but previously marked wrongly · EL-15 known
>
> Kind regards, Thomas Kassens (district archaeologist)

## Everything we looked at

The full internal evidence card is in [`evidence/`](evidence/) ([file list](evidence/README.md)): every image and
record the project used to decide whether to submit this location, plus what was sent to the authority.
Coordinates are removed; nothing else is edited.

**LiDAR terrain (LGLN DGM1, 1 m).** Hillshade at 150 m and 500 m, and a local relief model:

![DGM1 hillshade 150 m and 500 m](evidence/lidar_dgm1_hillshade_150m_and_500m.png)

<img src="evidence/lidar_dgm1_local_relief_150m.png" width="360" alt="Local relief model, 150 m">

**Orthophotos (LGLN DOP20), every year available**, used to rule out modern heaps, buildings and earthworks:

| 2014-05-18 | 2017-05-28 | 2020-04-05 | 2023-06-03 | 2025-03-08 | 2025-03-08 |
|---|---|---|---|---|---|
| <img src="evidence/dop20_2014-05-18.jpg" width="150"> | <img src="evidence/dop20_2017-05-28.jpg" width="150"> | <img src="evidence/dop20_2020-04-05.jpg" width="150"> | <img src="evidence/dop20_2023-06-03.jpg" width="150"> | <img src="evidence/dop20_2025-03-08.jpg" width="150"> | <img src="evidence/dop20cir_2025-03-08.jpg" width="150"> |

**The model reader's review before submission** (verbatim extracts from [`reader_review.json`](evidence/reader_review.json)):

> A small discrete round mound about 8 m across and about 0.9 m high in a conifer plantation on flat ground crossed by fine parallel furrows. Several similar small round highs lie within about 100 m, including a ring-shaped mound with a central hollow about 35 m to the south. No modern object is visible at the point in five aerial flights from 2014 to 2025. No registered burial mound lies within 300 m.

Open alternative it asked the archaeologist to weigh: *Could this small mound and its neighbours be natural sand hummocks, like the uneven ground to the south-west, or heaps left from clearing or planting, rather than a group of burial mounds?*

Most likely non-archaeological explanation it considered: `NAT` (OPEN-WEAK); verdict `SENDABLE`.

**Detector output** ([`detection.json`](evidence/detection.json)): model `D_101`; mean probability 0.951; area 399 m², roundness 0.95; nearest registered burial mound 1770 m away in the public register snapshot.

**What the authority received.** The location list (coordinates removed: [`submitted_row.json`](evidence/submitted_row.json)) and, on 2 November,
detail maps of the barrow field (coordinate labels removed):

![Barrow field detail 600 m](evidence/submitted_detail_600m.png)

## What the assessment does and does not establish

Written confirmation by the district archaeologist that it is a previously unknown barrow field. Counted as one site. No field visit, excavation, date or record number reported.

## The batch it came from

Emsland batch of 15 locations: 3 previously unknown (D01, D02, D03), 6 already known (2 of them previously marked in the wrong place), 4 not burial mounds, 2 uncertain.

## How to check this yourself

1. Ask the assessing authority, named above, about the label in the submission (`EL-11`)
   and the date of its assessment. Its contact details are on its public website.
2. Look at the terrain yourself: the hillshade above is made from public LGLN DGM1 data, which anyone can download.
3. The coordinate commitment is the SHA-256 of a string containing this ID, the exact submitted ETRS89/UTM32N
   coordinates and a random salt. The exact coordinates are withheld to protect the site (see the
   [README](../../README.md#why-exact-coordinates-are-not-published)). When they are released, to a researcher or
   publicly, the string can be published and checked against this hash, proving which point was submitted on which
   date.
