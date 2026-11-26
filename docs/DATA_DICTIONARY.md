# Data Dictionary

The analysis workbook contains one row per submitted session.

| Field | Meaning |
|---|---|
| Record | Sequential row number added for reference; not a respondent ID. |
| Recorded at | Google Forms submission timestamp. |
| Activity | Single activity category selected in the form. |
| Time block | Single time block selected in the form. |
| Focus score | Self-reported score from 1 to 5. |
| Selected drivers | Comma-separated list of checked driver options. Multiple drivers may be selected in one session. |

## Workbook summary sheets

- **Overview:** headline counts, average and median focus score, score distribution, and frequently selected drivers.
- **Session Data:** the 79 exported self-tracking rows.
- **Activity Summary:** session counts and average focus score by activity, plus score counts.
- **Time Summary:** session counts and average score by time block, plus score counts.
- **Driver Summary:** number and share of sessions in which each driver was selected.
- **Driver Flags:** one 0/1 column per driver to support transparent multi-select counts.
- **Notes & Limits:** interpretation notes and source-version discrepancy.

The timestamp field is the exact form-submission time, not an independently measured start or end time for the activity.
