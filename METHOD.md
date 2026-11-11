# Method

## Terrain

| Region | Terrain model | Licence |
|---|---|---|
| Lower Saxony, Germany | LGLN DGM1, 1 m | CC BY 4.0 |
| England | Environment Agency LiDAR composite DTM, 1 m | Open Government Licence |
| France | IGN LiDAR HD terrain model (MNT) | Etalab Open Licence 2.0 |
| Netherlands, Denmark | AHN; Danish national elevation model (DHM) | open public data |

## Detectors

All detectors start from ADAF, the public archaeological detector of the ADAF project
([EarthObservation/adaf](https://github.com/EarthObservation/adaf); code Apache-2.0, weights CC BY-SA 4.0).

| Name | What it is | Used for |
|---|---|---|
| **S_D + PROX** | Two-checkpoint ensemble fine-tuned for burial mounds in sand lowlands, with a proximity re-ranking rule (200 m radius) | Lower Saxony pools: D01, D03, D04, P01 |
| **D1** | Earlier burial-mound fine-tune of the ADAF barrow model | Lower Saxony pools: D01, D02 |
| **CONT e41** | Fine-tune for English earthworks | England and France |
| ADAF all-objects | The unmodified public ADAF model | England and France, as a comparator arm |

Checkpoints, with SHA-256 hashes, are in the Zenodo deposit
[10.5281/zenodo.23862470](https://doi.org/10.5281/zenodo.23862470) (CC BY-SA 4.0). Measured performance on registered
monuments, with protocols frozen before scoring, is in:

- *Adapting a public LiDAR barrow detector to a new region*, preprint,
  [10.5281/zenodo.23352619](https://doi.org/10.5281/zenodo.23352619);
- *Cross-border recovery of registered burial mounds by an adapted public LiDAR detector at fixed review workloads*,
  preprint, [10.5281/zenodo.23874293](https://doi.org/10.5281/zenodo.23874293).

Code and frozen protocols: [ndsbarrow-adapt](https://github.com/tee-20190/ndsbarrow-adapt).

Recovering registered monuments is not the same as finding new ones. On a later retrospective test of 270 mounds
that Danish museums had first noticed on LiDAR, mostly flattened by ploughing, S_D + PROX recovered only 3.3 %. The
detectors are much better at upstanding mounds than ploughed-out ones.

## Screening before submission

1. Detections within a set distance of a monument on the public register were removed.
2. Language-model readers reviewed terrain images (hillshades and relief visualisations) of the remaining detections
   and kept only plausible earthworks. In most batches the readers were not told which detector proposed a location.
   These are model judgments; no person reviewed every image.
3. The project owner sent small batches to the responsible authority, with LiDAR views, and asked for their
   assessment. Further batches were generally sent after asking the
   authority whether, and in what form, it wanted them.

## Who did what

- **Project owner (Thomas Shanahan):** direction, all correspondence with heritage authorities.
- **AI agents (Anthropic Claude models; OpenAI Codex):** detector training and evaluation, screening, package
  preparation, record keeping and independent re-checks of each other's numbers.
- **Heritage authorities:** every archaeological judgment in this repository.

## Not included

- Exact coordinates (site protection; salted SHA-256 commitments are on each site page) and per-location detector
  scores.
- Correspondence other than the assessing archaeologists' replies about the five Lower Saxony sites, which are quoted
  verbatim on their pages without contact details.
- Total compute and staff time per result: not yet tallied.
