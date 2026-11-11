# LiDAR archaeology: independently assessed outcomes

This repository is the public record of what an AI-assisted LiDAR survey has found so far, as judged by the
archaeologists responsible for each area. Each location was submitted to the heritage authority for that area, and
this page reports what they said, including the cases where they said no.

**As of 11 November 2026:**

| | Count |
|---|---|
| Locations submitted to heritage authorities | **178**, to 22 authorities in 5 countries |
| Locations with a written assessment so far | **90** (80 have had no reply yet; 8 acknowledged or pending) |
| **Previously unknown archaeological sites, confirmed by the responsible archaeologist** | **4** (three burial mounds and one barrow field, Lower Saxony, Germany) |
| Previously unknown probable site, inspected on the ground, not yet confirmed | 1 |
| Completed additions to official heritage records | 16 (one of them is a confirmed site above) |
| All documented positive outcomes | 28 |

![Outcomes of all 178 submitted locations](figures/funnel.svg)

The four confirmed sites are the headline result. They are listed in [`discoveries/`](discoveries/). Everything else,
including record additions that turned out to be modern, is in the [catalogue](CONTENTS.md). Machine-readable versions
are in [`status.json`](status.json) and [`data/outcomes.csv`](data/outcomes.csv).

## What "confirmed" means here

A site counts as a confirmed discovery only when the archaeologist responsible for that area states in writing that it
is (a) archaeological and (b) previously unknown to their records. Their judgment is the test. Our own model reviews,
an absence from a public map, or a record addition do not count. The full rules are in
[VERIFICATION.md](VERIFICATION.md).

None of the four has been excavated or dated, and no field visit has been reported for them. They were assessed from
the desk, using the LiDAR views we supplied together with the authority's own records. One has been given an official
site number. These are assessments by qualified people, not excavation results, and we describe them that way.

## How the results were produced

1. **Terrain.** Public LiDAR terrain models (in Lower Saxony, LGLN DGM1, CC BY 4.0; in England, the Environment
   Agency composite DTM; in France, the IGN LiDAR HD terrain model).
2. **Detection.** Neural detectors adapted from the public ADAF archaeological detector, trained and tested on
   registered monuments. The weights of the detectors that found the four confirmed sites are public (Zenodo
   [10.5281/zenodo.23862470](https://doi.org/10.5281/zenodo.23862470)). The measured performance of these detectors,
   with frozen protocols, is in two preprints ([10.5281/zenodo.23352619](https://doi.org/10.5281/zenodo.23352619),
   [10.5281/zenodo.23874293](https://doi.org/10.5281/zenodo.23874293)) and the code repository
   [ndsbarrow-adapt](https://github.com/tee-20190/ndsbarrow-adapt).
3. **Screening.** Detections that matched a public monument register were set aside. Language-model readers then
   reviewed terrain images of the remainder, in most batches without being told which detector proposed them, and
   only the locations they kept were considered for submission.
4. **Assessment.** Small batches were sent to the responsible heritage authority by the project owner. Each
   authority compared the locations with its own records, which are more complete than any public map. Some also
   looked at historical imagery or visited the site.

The engineering and analysis were carried out by AI agents (Anthropic Claude models and OpenAI Codex) working in one
project repository under the owner's direction. People made the archaeological judgments. [METHOD.md](METHOD.md) has
the details and what each step does and does not show.

## What this does not show

- **It is not a precision estimate.** The submitted locations were selected, batches differ by region and detector,
  and 80 locations still have no reply. Unanswered is not negative. Of the 90 assessed, 14 were already recorded, 30
  were judged modern, natural, landscaping or otherwise not archaeological, and 18 remain undetermined
  ([FUNNEL.md](FUNNEL.md)).
- **"Not on the public map" does not mean "unknown".** Several authorities hold far more than they publish. One
  Lower Saxony authority found that of 11 places that were blank on the public atlas, 6 were already known to them.
  This is why every claim in this repository rests on the authority's own check.
- **No dates or functions are claimed.** "Burial mound" is the assessing archaeologist's interpretation of the form.

## Why exact locations are not published

Coordinates, maps and images precise enough to find a site are withheld. Unprotected burial mounds can be damaged by
illegal metal detecting and digging, and decisions about publishing sites belong to the heritage authorities. Anyone
with a legitimate research need can ask the relevant authority. Personal names of the assessing archaeologists are also
omitted; the authorities are named.

## Contents

| Path | Content |
|---|---|
| [`CONTENTS.md`](CONTENTS.md) | Catalogue of all 28 positive outcomes, by tier |
| [`discoveries/`](discoveries/) | One page for each confirmed site, plus the field-inspected probable site |
| [`FUNNEL.md`](FUNNEL.md) | Every outcome of the 178 submissions, negatives included |
| [`VERIFICATION.md`](VERIFICATION.md) | Tier definitions and counting rules |
| [`METHOD.md`](METHOD.md) | Data, detectors, screening and assessment |
| [`status.json`](status.json), [`data/outcomes.csv`](data/outcomes.csv) | Machine-readable records |
| [`history.md`](history.md) | Versions and corrections |

## Versions and corrections

This is a live record. When an authority revises an assessment, the change is recorded in [history.md](history.md) and
earlier versions stay in the Git history. One correction is already recorded: a Hertfordshire mound added to the
record turned out, on our own later check of dated surveys, to have formed between 2003 and 2009.

## Credit

The archaeological assessments belong to the heritage authorities listed in [CONTENTS.md](CONTENTS.md). Terrain data:
LGLN (CC BY 4.0), Environment Agency (Open Government Licence), IGN. The detectors build on ADAF (Apache-2.0 code,
CC BY-SA 4.0 weights). Register data: Denkmalatlas Niedersachsen (CC BY-SA 4.0), Historic Environment Records.

Contact: open an issue in this repository.

## Licence

Text and data in this repository: [CC BY 4.0](LICENSE). Cite with [CITATION.cff](CITATION.cff).
