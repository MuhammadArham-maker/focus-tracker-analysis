# Focus Tracker — Development Log

## 1. The starting point: choose a problem worth investigating

I wanted to work on a data project that was personally useful, not simply download a public dataset, calculate a few averages, and make charts.

I explored several possible topics, including sports and fitness, finance, technology, business, deep work, and focus. After getting caught between too many interesting options, I chose to investigate my own focus.

That led to two different project directions:

- **Analysing human focus:** use an existing dataset and study focus patterns across other people.
- **Analysing my own focus:** build a small data-collection process, record my own sessions, store the observations, and investigate patterns in my everyday life.

The second idea excited me because it gave the project a real question, a real data source, and a problem I could examine from direct experience.

## 2. Designing a way to measure something invisible

The first challenge was measurement. Focus is not directly visible, so I explored the idea of a **proxy metric**: a visible or recordable indicator used to represent something that cannot be measured directly.

My first thought was to count every time my mind wandered and I noticed it drifting. I called this *Drift Catching*. I eventually rejected it because constantly counting mind-wandering could interrupt the very focus I wanted to observe.

I chose a second approach: the **Density Rating Method**. Instead of interrupting an activity to count every drift, I would rate the quality of my focus after a natural work block.

The form used a 1–5 scale, from low presence / wandering to pure presence / flow state. The rating was subjective by design: it captured my own immediate assessment, rather than claiming to be an objective measurement of focus.

## 3. Designing the questionnaire and data structure

I created a Google Form connected to Google Sheets. The final questionnaire contained four required questions:

1. **What are you doing?** A single-choice activity category.
2. **Which time block?** A single-choice time-of-day category.
3. **Focus Density!** A 1–5 rating.
4. **What was the primary cause of this score? (Good or Bad)** A multiple-selection list of possible drivers.

The final activity list separated spiritual, physical, personal, university, and extra activities. The time blocks were Pre-Dawn / Early Morning, Late Morning, Afternoon, Evening, and Night. The driver list included factors such as Natural Flow, Overthinking, Self Talk (Bismillah...), Good Environment, Mental Resistance, Hyper-Clarity, and others.

I considered using broader activity categories, but chose more granular options because detailed categories can be grouped later, whereas broad categories cannot always be split into meaningful detail after collection. This was an early practical lesson in data structure design.

I also considered whether the driver question should use one answer or multiple checkboxes. I chose multiple selection because a focus session can have more than one contributing factor. That made the data richer, while also making interpretation and counting more involved.

The form evolved as I learned what I wanted to observe. The time-block question was added after I considered whether the time of day might matter. This was an example of **schema evolution**: changing the structure of a data-collection form as the investigation develops.

## 4. Reducing tracking friction

I did not want the collection process to become another distraction. I therefore adopted two practical rules.

**Macro-blocks only:** submit a new record when the main activity changes. A short active break within a study block does not automatically become a separate record.

**The 10-Second Gut Check Rule:** make the rating quickly and honestly. If I have to debate for a long time whether a session was truly in a flow state, I should leave that driver unchecked rather than manufacture certainty.

The form description captured the intended mindset:

> Log the Focus. The Stillness. The Presence. Ignore the outcome.

I initially considered a longer collection period and a target of at least 30 entries as a practical starting point. The notes from that stage referred to 30 as a useful rule of thumb, not a guarantee of statistical significance. I then continued collecting observations when I missed a day or two, rather than abandoning the experiment.

## 5. Data collection

The exported workbook contains **79 self-recorded sessions**, with timestamps spanning **12–22 May 2026** across nine distinct dates.

The data is a personal, self-reported record. It is not a representative sample of other people, and the 1–5 focus rating is my own subjective scale.

The final export includes the form responses, an activity-average pivot table, and an insights table. The response fields preserve the activity, time block, focus score, and selected drivers for each entry.

## 6. First look at the data

The 79 focus ratings were distributed as follows:

| Focus score | Sessions | Share |
|---:|---:|---:|
| 1 | 2 | 2.5% |
| 2 | 8 | 10.1% |
| 3 | 44 | 55.7% |
| 4 | 23 | 29.1% |
| 5 | 2 | 2.5% |

The overall mean was **3.19 out of 5**. Scores of 3 and 4 accounted for 67 of the 79 records (84.8%).

In the response-level workbook, the most frequently selected drivers were:

- Natural Flow: 74 selections (93.7% of sessions).
- Overthinking: 71 selections (89.9%).
- Self Talk (Bismillah...): 63 selections (79.7%).

These are multiple-selection counts. They are not mutually exclusive categories, so their percentages do not add up to 100%.

The exported response-chart PDF differs from the workbook by one selection for two drivers: it shows Good Environment as 53 and Mental Resistance as 43, while counting the exported workbook's response rows gives 52 and 42 respectively. Both exports show 79 responses. I have retained this discrepancy as a data-version note rather than silently choosing one figure.

## 7. Exploratory analysis: look for the absence of Overthinking

Overthinking appeared in 71 of 79 sessions. Because it was so common, I tried a different filter: instead of examining every session where Overthinking appeared, I looked at the eight sessions where it did not.

Those eight records consisted of:

- Calisthenics: 3 sessions.
- Talk / Social Connection: 2 sessions.
- Unstructured Screen Time: 2 sessions.
- YouTube Content Creation: 1 session.

The two screen-time entries both scored 3. Among the other six records, two scored 3, two scored 4, and two scored 5. This led me to explore whether physical movement, social interaction, and creative activity were associated with sessions where I did not report Overthinking.

I called this early interpretation **Movement & Creation**. It was a useful pattern to investigate, but the small number of observations does not establish that these activities cause Overthinking to disappear.

## 8. The Flow Assassin: when Natural Flow was absent

I next filtered the five sessions in which Natural Flow was not selected. All five had focus scores of 1 or 2, and all five included Overthinking. Three also included Mental Resistance, three included Extreme Emotions, and three included Good Environment.

This challenged a simple assumption that a quiet or suitable environment would necessarily produce focus. In three low-scoring sessions, I had still selected Good Environment.

My reflection became:

> A quiet room cannot fix a loud mind.

The data did not prove a universal psychological rule, but it prompted me to pay more attention to what I brought into a session: emotional carryover, mental resistance, and Overthinking.

## 9. The Anatomy of a 4 and the rarity of a 5

I initially wanted to understand what a perfect score of 5 looked like. The workbook contains only **two** score-5 sessions, so any pattern among them is highly tentative. Both included Natural Flow and Self Talk (Bismillah...). One was YouTube Content Creation; the other was Talk / Social Connection.

I then examined score-4 sessions. There were 23. All 23 included Natural Flow, and 21 also included Overthinking (91.3%). Eighteen included Self Talk (Bismillah...) and 15 included Hyper-Clarity.

This changed the question. Overthinking could be present in a high-scoring session without necessarily preventing a strong focus rating. My interpretation shifted from trying to eliminate every thought to practising a return to the present action.

The phrase that became central to this reflection was **Focus in me & my moment**. My faith also shaped how I understood this: I cannot know or control every step of the day; I can ask Allah for help, begin with Bismillah, and attend to the action in front of me.

## 10. Questioning the Golden Hour

I investigated whether a particular time block held the strongest focus scores. The workbook's averages were:

| Time block | Sessions | Average focus score |
|---|---:|---:|
| Pre-Dawn / Early Morning | 14 | 3.07 |
| Late Morning | 20 | 3.10 |
| Afternoon | 20 | 3.30 |
| Evening | 23 | 3.26 |
| Night | 2 | 3.00 |

The observed averages were close, and the Night group had only two records. The data did not show a strong time-of-day pattern in this sample.

My earlier idea of a *Golden Hour* therefore became less convincing. When I looked back at what I was doing during some more engaging sessions, I noticed that the activity itself might matter more than the clock. Reading Quran or listening to Hadees / Muzakra could require active attention and novelty for me, rather than simply happening at a particular time.

This helped me move from a time-based explanation toward a question about engagement.

## 11. Activity averages and the importance of context

The workbook's activity pivot table showed these averages:

| Activity | Sessions | Average focus score |
|---|---:|---:|
| Namaz | 32 | 2.94 |
| Quran | 11 | 3.64 |
| Hadees / Muzakra | 4 | 3.50 |
| University passive learning (exam lectures) | 8 | 3.25 |
| Talk / Social Connection | 8 | 3.25 |
| Football | 4 | 3.00 |
| Calisthenics | 3 | 3.33 |
| YouTube Content Creation | 3 | 3.67 |
| Unstructured Screen Time | 3 | 3.00 |
| Personal Active Building (Projects) | 2 | 3.00 |
| Personal Passive Learning (Coursera / Tutorials) | 1 | 4.00 |

The small counts matter. For example, the 4.00 average for Personal Passive Learning comes from a single session; it cannot support a broad comparison by itself. The Talk / Social Connection average of 3.25 also hides variation: its eight scores ranged from 2 to 5 (three 2s, one 3, three 4s, and one 5). An average can flatten very different session experiences into one number.

I also questioned the apparent difference between university lectures (3.25 across eight sessions) and personal passive learning (4.00 in one session). At the time, I had been switching between the goal of preparing for university exams and the desire to understand topics more deeply. The records mainly captured the confused phase; I did not record enough of the later, more exam-aligned study phase to compare the two fairly. This was a reminder that the data only describes the period it actually captures.

This is where my own context became important. I had to bring in the person who filled out the form — me. I jokingly thought of myself as the “field expert” because I could look back at what I had actually done and felt, even when the activity label did not tell the whole story. I revisited a session that had been labelled as passive learning, but my actual experience had gone beyond watching a course: I explored an idea, researched shadow techniques, used AI to brainstorm, and drew a cracked coffee mug with a chain handle to represent struggle. The activity label did not fully capture the creative work I had done.

That made me question a simple *active versus passive* or *university versus personal* explanation. The more useful distinction for my reflection became **pure theory versus real-world application and creation**. This was a contextual interpretation of the records, not something the spreadsheet could establish on its own.

## 12. From Engagement Threshold to the Autopilot Trap

For a while, I thought the answer was to make activities more interesting. But not every task can be novel, and even interesting tasks can become routine through repetition.

I therefore changed the question. Instead of always trying to change the task, could I change the way I attended to it?

This led to the **Autopilot Trap** insight: when an activity becomes deeply familiar, I may perform it with less conscious attention. My interpretation was that I should not depend only on external novelty; I should practise bringing attention to the ordinary action in front of me.

This reflection connected the data back to everyday routines, including Namaz and other repeated activities. The activity averages raised the question; my own experience and faith informed how I interpreted it.

## 13. Data work completed and future scope

The project developed through three practical levels:

1. **Data collection:** built a Google Form and connected it to Google Sheets.
2. **Exploratory analysis:** used filters, comparisons, pivot tables, and a structured insights sheet to investigate patterns and exceptions.
3. **Data visualisation:** reviewed the Forms response charts and created an activity-average pivot table to compare categories.

A more automated, continuously updating business-intelligence dashboard was an intended next step, not something completed in this version. Predictive modelling or AI-based forecasting was also a future possibility, not part of the delivered analysis.

## 14. Final reflection

I began with a question about why my environment, schedule, or activity seemed to affect my focus. The process made me look more carefully at the measurement itself, the limits of averages, the context behind a record, and the difference between a pattern and a cause.

The spreadsheet could show counts and averages. It could not fully explain what was happening in a session. I had to return to the experience behind the entry and question whether the category I selected captured what I had actually done.

The most important personal conclusion I took from the experiment was:

> **Focus in me & my moment.**

This is my reflection from a small self-tracking experiment, not a universal conclusion about human focus. The value of the project was learning to collect observations, question my assumptions, interpret the numbers carefully, and use the results to ask better questions.
