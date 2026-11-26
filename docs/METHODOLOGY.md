# Methodology

## Purpose

I wanted to understand my own focus through everyday observations. I did not want to use a ready-made public dataset and stop at calculating averages. I wanted to decide what to record, collect the observations, and explore what they might mean in my own routine.

This is a personal self-tracking exercise. It is not a controlled experiment or a representative sample of other people.

## Measurement idea

Focus is not directly visible, so I needed a practical way to record how present I felt during an activity.

I first considered **Drift Catching**: counting each time my mind wandered and I noticed it. I rejected that approach because counting every drift could interrupt the focus I was trying to observe.

I chose the **Density Rating Method** instead. I completed a natural activity block and then gave it a subjective score from 1 to 5. The scale ran from wandering at the low end to Pure Presence / Flow state at the high end.

The score is my own judgement. It is not an instrument-validated or objective focus measure.

## Collection setup

- **Form:** Google Forms.
- **Storage and review:** Google Sheets.
- **Analysis used:** filters, pivot tables, manual interpretation, and charts.
- **Unit of observation:** one submitted activity session / macro-block.

The final form asked four required questions:

1. Activity (single choice).
2. Time block (single choice).
3. Focus Density (1–5).
4. Primary cause / drivers (multiple selections).

The final questionnaire and all answer choices are in [`QUESTIONNAIRE.md`](QUESTIONNAIRE.md).

## Logging rules

### Macro-blocks only

I did not want to record every small break or every few minutes. I submitted a new row when I completely switched my main activity.

The form description gave this example: **Study + 5min Calisthenics break = 1 Study Log**. A short active break did not automatically become a separate record.

### The 10-Second Gut Check Rule

I wanted the form to be quick to complete and to reduce overthinking during logging. I read the driver list and checked what immediately felt true. If I had to debate for a long time about whether I was in a flow state, I left it blank.

This was a practical anti-friction rule, not a formal measurement protocol.

### Granular activity choices

I preferred more specific activity options over broad categories because detailed entries can be grouped later, while broad entries cannot always be split into useful detail after collection.

### Multiple driver selections

I considered a single-choice driver question, but a session can have more than one factor. I chose checkboxes. This makes the counts overlap; they should not be read as parts of a 100% whole.

## Collection snapshot

The exported workbook contains:

- **79 self-recorded sessions**
- **12–22 May 2026**
- **9 distinct dates with entries**
- 13 activity options in the form
- 5 time blocks
- 14 possible driver selections

The initial plan mentioned around two weeks of collection and a practical target of 30 entries. The final export spans the dates above. The 30-entry idea was a working target, not a guarantee of statistical significance.

## Analysis process

I used filters and pivot tables to ask questions of the records, including:

- What did I do during sessions where I did not select Overthinking?
- What was present when Natural Flow was absent?
- What did the score-4 sessions have in common?
- Did any time block stand out?
- How did average focus scores vary by activity?

I then compared the spreadsheet results with what I remembered about the sessions. For example, an activity category could hide what I actually did inside that session. I used that context to question and refine my interpretation.

## Data included in this repository

The analysis workbook contains the 79 session rows, submission timestamps, activity, time block, focus score, and selected drivers. It also contains summary tabs for the score distribution, activities, time blocks, and drivers.

No respondent names or email addresses are included. These entries are my own self-tracking records.

## Limitations

- **One person:** these observations describe my experience only.
- **Subjective scores:** the 1–5 rating depends on my own judgement.
- **Self-reported drivers:** selecting a driver reflects what I noticed and chose to record.
- **Multiple selections:** driver counts overlap.
- **Uneven activity counts:** some activities have only one to four entries, so their averages are especially unstable.
- **No causal proof:** a pattern or association does not show that an activity or driver caused a score.
- **Short collection window:** 79 entries across nine dates are useful for reflection, but not enough to generalise broadly.
- **Context matters:** the activity label and score cannot capture every detail of what was happening in a session.

## Source Consistency Note

The downloaded Excel workbook and Google Forms response-chart PDF both contain 79 responses. However, two multiple-selection driver counts differ slightly between the exports:

| Driver | Google Forms PDF | Excel workbook |
|---|---:|---:|
| Good Environment | 53 | 52 |
| Mental Resistance | 43 | 42 |

The difference has not been conclusively explained. For consistency, the Excel workbook is used as the primary source for row-level calculations and the recreated charts in this project. The two exports are not mixed when calculating results.