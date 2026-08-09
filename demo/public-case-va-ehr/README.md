# VA EHR Public Verification Case

This folder contains the source, construction record, runtime evidence, and validation materials for one public case.

## Test design

1. Start with the real 77-page VA OIG audit.
2. Reconstruct six evidence artifacts from factual chronology, documented responsibilities, attributed accounts, survey results, and operating data.
3. Package those artifacts into one seven-page blind-test PDF while withholding the OIG's findings, conclusions, causal labels, and recommendations.
4. Run the diagnostician on the evidence-only PDF.
5. Compare the unedited result with the full audit only after the run.

The six artifacts are page-sourced reconstructions from one public report. They are not represented as independently obtained raw memoranda, survey exports, training files, or system records.

## Evidence-only blind-test packet

- File: `VA-EHR-evidence-only-packet.pdf`
- Source edition: `VA-EHR-evidence-only-packet.md`
- Purpose: a harder causal test that withholds the OIG's findings, conclusions, causal labels, and recommendations

The packet retains the report's factual chronology, attributed accounts, quantitative results, documented responsibilities, and explicit evidence limitations. It is a reconstruction from material reproduced or described in the official report, not a claim that the underlying memoranda and survey files were independently obtained.

Use the evidence-only PDF as the case input. Keep the full report out of the project until after the diagnosis; it serves as the held-out validation source.

## Audit trail

- `source-map.md`: maps every packet artifact to the report's printed pages and records what was withheld
- `held-out-validation.md`: compares the unedited result with the audit after the run
- `../transcripts/2026-08-09-va-ehr-evidence-only-blind-test.md`: preserves the model output without repair

## Original raw-report test

- File: `VA-EHR-training-deficiencies-case.pdf`
- Title: *Training Deficiencies with VA's New Electronic Health Record System at the Mann-Grandstaff VA Medical Center in Spokane, Washington*
- Publisher: U.S. Department of Veterans Affairs, Office of Inspector General
- Publication date: July 8, 2021
- Report number: 20-01930-183

## Official sources

- Report record: https://www.oversight.gov/reports/training-deficiencies-vas-new-electronic-health-record-system-mann-grandstaff-va-medical
- Official PDF: https://www.oversight.gov/sites/default/files/documents/reports/2021-07/VAOIG-20-01930-183.pdf

The original PDF is retained in its raw published form. It was uploaded without a prompt for the recorded 2026-08-09 run. Because the report contains the auditors' own findings, that run demonstrates ingestion and causal prioritization but is not the strongest independent-discovery test.
