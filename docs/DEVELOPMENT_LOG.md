# Focus Tracker — Development Log

## 1. The starting point: choose a problem worth investigating

I wanted to work on a data project that was personally useful, not simply download a public dataset, calculate a few averages, and make charts.

I explored several possible topics, including sports and fitness, finance, technology, business, deep work, and focus. After getting caught between too many interesting options, I chose to investigate my own focus.

That led to two different project directions:

- **Analysing human focus:** use an existing dataset and study focus patterns across other people.
- **Analysing my own focus:** build a small data-collection process, record my own sessions, store the observations, and investigate patterns in my everyday life.

The second idea excited me because it gave the project a real question, a real data source, and a problem I could examine from direct experience.

I also wanted to avoid relying on a one-time public dataset. Building my own collection process meant I would have to think about the entire pipeline: deciding what to measure, collecting the observations, storing them, and eventually analysing them.

## 2. Designing a way to measure something invisible

The first challenge was measurement. Focus is not directly visible, so I explored the idea of a **proxy metric**: a visible or recordable indicator used to represent something that cannot be measured directly.

My first thought was to count every time my mind wandered and I noticed it drifting. I called this *Drift Catching*. I eventually rejected it because constantly counting mind-wandering could interrupt the very focus I wanted to observe.

I chose a second approach: the **Density Rating Method**. Instead of interrupting an activity to count every drift, I would rate the quality of my focus after a natural work block.

The form used a 1–5 scale, from low presence / wandering to pure presence / flow state. The rating was subjective by design: it captured my own immediate assessment, rather than claiming to be an objective measurement of focus.

This was an important decision. I was not trying to measure every thought or create a perfectly precise psychological instrument. I wanted a practical way to record how present I felt during an activity without making the act of tracking itself a distraction.

The rejection of Drift Catching and the decision to use post-session ratings are discussed in [Part 3, around 22:42](https://youtu.be/__dXH9GgBHc?t=1362).

## 3. Designing the questionnaire and data structure

I created a Google Form connected to Google Sheets. The final questionnaire contained four required questions:

1. **What are you doing?** A single-choice activity category.
2. **Which time block?** A single-choice time-of-day category.
3. **Focus Density!** A 1–5 rating.
4. **What was the primary cause of this score? (Good or Bad)** A multiple-selection list of possible drivers.

The final activity list separated spiritual, physical, personal, university, and extra activities. The time blocks were Pre-Dawn / Early Morning, Late Morning, Afternoon, Evening, and Night. The driver list included factors such as Natural Flow, Overthinking, Self Talk (Bismillah...), Good Environment, Mental Resistance, Hyper-Clarity, and others.

I considered using broader activity categories, but chose more granular options because detailed categories can be grouped later, whereas broad categories cannot always be split into meaningful detail after collection. This was an early practical lesson in data structure design:

> You can always group data later, but you cannot always split it apart.

I also considered whether the driver question should use one answer or multiple checkboxes. I chose multiple selection because a focus session can have more than one contributing factor. That made the data richer, while also making interpretation and counting more involved.

The form evolved as I learned what I wanted to observe. The time-block question was added after I considered whether the time of day might matter. This was an example of **schema evolution**: changing the structure of a data-collection form as the investigation develops.

I also decided not to include every possible explanation for a low score. For example, I considered past task failure but rejected it because I wanted to record factors affecting the session itself, rather than use a previous result as an explanation for the current one.

The driver list also included **Self Talk (Bismillah...)**. I wanted to observe whether beginning an activity with a deliberate internal reminder or affirmation was associated with how present I felt during the session.

## 4. Reducing tracking friction

I did not want the collection process to become another distraction. I therefore adopted several practical rules.

**Macro-blocks only:** submit a new record when the main activity changes. A short active break within a study block does not automatically become a separate record.

**Context-Switch Rule:** distinguish between a genuine change of activity and a brief interruption. For example, a short two-to-five-minute movement break during a study session could remain part of the surrounding study block if it did not represent a meaningful change in the main activity.

**The 10-Second Gut Check Rule:** make the rating quickly and honestly. If I have to debate for a long time whether a session was truly in a flow state, I should leave that driver unchecked rather than manufacture certainty.

**The No-Averaging Rule:** avoid combining substantially different activities or focus states into one rating simply because they happened within the same long period. A long study session followed by calisthenics, for example, could contain different levels of attention and recovery. Averaging the entire period into one score could hide those differences. The purpose of macro-blocks was to preserve meaningful activity boundaries, not to force unrelated experiences into a single number.

These rules were intended to protect both the quality of the observations and the experience of collecting them. I wanted the form to remain quick enough that I would actually use it.

The form description captured the intended mindset:

> Log the Focus. The Stillness. The Presence. Ignore the outcome.

I initially considered a longer collection period and a target of at least 30 entries as a practical starting point. The notes from that stage referred to 30 as a useful rule of thumb, not a guarantee of statistical significance.

I also set some working rules for the broader capstone process: use manageable work blocks, avoid spending more than two hours searching for data, and spend around 30 minutes attempting to resolve a technical error before asking AI for help. I wanted to keep the project moving rather than become stuck in endless preparation or debugging.

The tracking safeguards, including the No-Averaging Rule and the 10-Second Gut Check, are discussed in [Part 3, around 40:51](https://youtu.be/__dXH9GgBHc?t=2451).

## 5. Data collection

I launched the Google Form on **12 May 2026** and connected it to Google Sheets. This created a simple collection pipeline:

**Google Forms → Google Sheets → Exploratory Analysis**

The form allowed me to record an activity, its time block, a focus score, and the drivers I associated with that score. Google Sheets stored the submitted responses and became the working space for later analysis.

I initially planned to collect data over approximately two weeks, with at least 30 entries as a practical minimum target. However, the first two days produced more responses than I expected.

### Collection timeline and checkpoints

The four recordings document how the experiment progressed:

| Date | Milestone |
|---|---|
| 12 May 2026 | Launched the Google Form and began collecting personal focus observations. |
| 14 May 2026 | Reached 34 responses after roughly 48 hours of active collection. |
| Around 16–18 May 2026 | Experienced a collection gap after becoming tired of the tracking process and missing entries for roughly one or two days. |
| 21 May 2026 | Reached 72 responses and resumed the collection process despite the earlier interruption. |
| 26 May 2026 | Recorded the completed analysis walkthrough, showing the 79-response project and its pivot tables, charts, and insights. |

The early response rate made me reconsider whether I needed the full two-week collection window. At the 34-response checkpoint, I was already thinking about whether I could finish collection earlier. I continued the experiment, though, rather than treating the first milestone as the end of the process.

At the 34-response checkpoint, the early focus-score distribution shown in Google Forms was:

- Score 2: 6 sessions.
- Score 3: 15 sessions.
- Score 4: 13 sessions.
- Scores 1 and 5: no recorded sessions yet.

This was only an early snapshot, not the final distribution. It was interesting to see that the first entries were concentrated around the middle of the scale.

The early progress and the first Google Forms summary are shown in [the 14 May update, around 04:30](https://youtu.be/d1ASyFmt0nA?t=270).

### The collection gap and restarting

The collection process was not perfectly consistent. Around 16–18 May, I became tired of maintaining the tracking routine and missed entries for roughly one or two days. In the later recording, I revisited the gap visible between the entries around 15 May and 19 May.

At first, missing days felt discouraging because I had wanted to maintain consistency. I had to decide whether a break in the process meant I should abandon the experiment. Instead, I resumed logging.

By 21 May, the form showed 72 responses. The checkpoint was a useful reminder that a personal data-collection process has to work around real routines, interruptions, and motivation—not just an ideal timetable.

The missed entries and decision to restart are discussed in [Part 4, around 02:24](https://youtu.be/m1_zzu41ga0?t=144), with the Google Sheets timeline shown again [around 15:31](https://youtu.be/m1_zzu41ga0?t=931).

### Final collection record

The exported workbook contains **79 self-recorded sessions**, with timestamps spanning **12–22 May 2026** across nine distinct dates.

The data is a personal, self-reported record. It is not a representative sample of other people, and the 1–5 focus rating is my own subjective scale.

The final export includes the form responses, an activity-average pivot table, and an insights table. The response fields preserve the activity, time block, focus score, and selected drivers for each entry.

An important detail about the collection process is that event-based logging naturally produced more records for activities that occurred frequently. For example, Namaz appeared often because it is part of my daily routine. A larger number of records for an activity does not automatically mean that it took more total time or had greater importance. It reflects the way I divided and recorded my activities.

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

The final walkthrough also showed a pivot-table view described as displaying 78 of the 79 records. I have not established why that view appeared to contain one fewer record. The exported response workbook contains 79 sessions, and the row-level calculations in this project use those 79 records.

## 7. Exploratory analysis: look for the absence of Overthinking

Overthinking appeared in 71 of 79 sessions. Because it was so common, I tried a different filter: instead of examining every session where Overthinking appeared, I looked at the eight sessions where it did not.

Those eight records consisted of:

- Calisthenics: 3 sessions.
- Talk / Social Connection: 2 sessions.
- Unstructured Screen Time: 2 sessions.
- YouTube Content Creation: 1 session.

The two screen-time entries both scored 3. Among the other six records, two scored 3, two scored 4, and two scored 5. This led me to explore whether physical movement, social interaction, and creative activity were associated with sessions where I did not report Overthinking.

I called this early interpretation **Movement & Creation**. It was a useful pattern to investigate, but the small number of observations does not establish that these activities cause Overthinking to disappear.

In the final walkthrough, I also demonstrated why I changed the direction of the filtering. Since Overthinking appeared in so many records, filtering for its presence returned most of the dataset. Looking at the smaller group without it made the exceptions easier to inspect.

There is a numerical difference worth preserving here: the video walkthrough describes an on-screen filter result of roughly 75–76 records containing Overthinking, while the exported workbook's row-level count is **71**. I have not established why these counts differ. The quantitative findings in this log use the 71 selections calculated from the exported workbook rather than replacing them with the approximate figure mentioned during the recording.

## 8. The Flow Assassin: when Natural Flow was absent

I next filtered the five sessions in which Natural Flow was not selected. All five had focus scores of 1 or 2, and all five included Overthinking. Three also included Mental Resistance, three included Extreme Emotions, and three included Good Environment.

This challenged a simple assumption that a quiet or suitable environment would necessarily produce focus. In three low-scoring sessions, I had still selected Good Environment.

My reflection became:

> A quiet room cannot fix a loud mind.

The data did not prove a universal psychological rule, but it prompted me to pay more attention to what I brought into a session: emotional carryover, mental resistance, and Overthinking.

The important distinction was that a suitable environment and a focused mind were not necessarily the same thing. An external condition could be favourable while the internal experience remained difficult.

This discovery is discussed in [Part 5, around 12:17](https://youtu.be/gwVauXLdDHU?t=737).

## 9. The Anatomy of a 4 and the rarity of a 5

I initially wanted to understand what a perfect score of 5 looked like. The workbook contains only **two** score-5 sessions, so any pattern among them is highly tentative. Both included Natural Flow and Self Talk (Bismillah...). One was YouTube Content Creation; the other was Talk / Social Connection.

I then examined score-4 sessions. There were 23. All 23 included Natural Flow, and 21 also included Overthinking (91.3%). Eighteen included Self Talk (Bismillah...) and 15 included Hyper-Clarity.

This changed the question. Overthinking could be present in a high-scoring session without necessarily preventing a strong focus rating.

I began thinking of Overthinking as background radio: it could still be playing, but it did not always have to take control of the activity. A score of 4 could represent a session in which I experienced distractions or thoughts but managed to remain engaged with what I was doing.

My interpretation shifted from trying to eliminate every thought to practising a return to the present action.

The phrase that became central to this reflection was **Focus in me & my moment**. My faith also shaped how I understood this: I cannot know or control every step of the day; I can ask Allah for help, begin with Bismillah, and attend to the action in front of me.

This distinction between having thoughts and allowing them to take over is discussed in [Part 5, beginning around 16:01](https://youtu.be/gwVauXLdDHU?t=961).

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

My earlier idea of a *Golden Hour* therefore became less convincing. The pivot-table comparison showed that the averages across the five time blocks stayed within a narrow range of approximately 3.0–3.3.

When I looked back at what I was doing during some more engaging sessions, I noticed that the activity itself might matter more than the clock. Reading Quran or listening to Hadees / Muzakra could require active attention and novelty for me, rather than simply happening at a particular time.

For example, I am not a Hafiz, so reading Quran requires me to pay attention to the words rather than recite entirely from memory. Listening to unfamiliar Hadith stories can also hold my attention because I am actively following something new.

This helped me move from a time-based explanation toward a question about engagement. The pivot table did not prove that an activity caused a higher score, but it challenged my initial assumption that the clock itself was responsible.

The time-block pivot table is discussed in [Part 5, around 30:24](https://youtu.be/gwVauXLdDHU?t=1824).

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

This was also a form of **goal-action mismatch**. I could spend a long time exploring a topic through detailed YouTube explanations when my immediate goal was to prepare for a particular university examination. The activity might be intellectually interesting, but it did not necessarily match the task I needed to complete at that moment.

This is where my own context became important. I had to bring in the person who filled out the form — me. I jokingly thought of myself as the “field expert” because I could look back at what I had actually done and felt, even when the activity label did not tell the whole story.

I revisited a session that had been labelled as passive learning, but my actual experience had gone beyond watching a course: I explored an idea, researched shadow techniques, used AI to brainstorm, and drew a cracked coffee mug with a chain handle to represent struggle. The activity label did not fully capture the creative work I had done.

That made me question a simple *active versus passive* or *university versus personal* explanation. The more useful distinction for my reflection became **pure theory versus real-world application and creation**. This was a contextual interpretation of the records, not something the spreadsheet could establish on its own.

The same issue appeared when I considered charts. A bar chart can make a category look straightforward, but a category average may combine sessions that were quite different in practice. A label alone cannot always explain the activity behind a record. The cracked-mug drawing session was one example of why I needed to revisit the original experience rather than trust a chart without context.

The final walkthrough includes this discussion of how charts can mislead without historical and personal context [around 38:20](https://youtu.be/gwVauXLdDHU?t=2300).

## 12. From Engagement Threshold to the Autopilot Trap

For a while, I thought the answer was to make activities more interesting. But not every task can be novel, and even interesting tasks can become routine through repetition.

I therefore changed the question. Instead of always trying to change the task, could I change the way I attended to it?

This led to the **Autopilot Trap** insight: when an activity becomes deeply familiar, I may perform it with less conscious attention. My interpretation was that I should not depend only on external novelty; I should practise bringing attention to the ordinary action in front of me.

This reflection became especially meaningful when I looked at the activity averages. Namaz had the lowest average focus score among the listed activities, at 2.94. I did not interpret this as meaning that Namaz had less value or importance. My interpretation was that a familiar routine, performed five times daily over many years, can become so familiar that my attention may wander unless I consciously renew my presence.

By contrast, activities such as Quran reading and listening to Hadees / Muzakra could demand more active attention from me because of the way I engaged with them.

The activity averages raised the question; my own experience and faith informed how I interpreted it. The spreadsheet could not measure the spiritual value of an activity or establish why my attention varied. It only recorded the focus ratings I assigned to those sessions.

I also began applying this idea to ordinary actions outside the main activity categories. For example, saying Bismillah and deliberately paying attention to the experience of drinking a glass of water could become a small practice in being present. The point was not to make every activity more exciting, but to change how consciously I experienced it.

This became part of my broader conclusion: attention should not depend entirely on novelty, a perfect environment, or a special time of day.

## 13. Data work completed and future scope

The project developed through three practical levels:

1. **Data collection:** built a Google Form and connected it to Google Sheets.
2. **Exploratory analysis:** used filters, comparisons, pivot tables, and a structured insights sheet to investigate patterns and exceptions.
3. **Data visualisation / business intelligence:** reviewed the Forms response charts and created pivot-table summaries and charts to compare categories.

A more automated, continuously updating business-intelligence dashboard was an intended next step, not something completed in this version.

I also considered a fourth level:

4. **Predictive AI / automation:** applying predictive modelling or AI-based analysis to forecast focus patterns or automate further analysis.

I deliberately did not add predictive modelling to this version. With 79 self-recorded sessions, a small and highly personal dataset, forcing a machine-learning model into the project would have added complexity without necessarily producing a meaningful result. The goal was to understand and interpret the observations I had collected, not to use machine learning simply because it was available.

The completed project therefore focused on collection, exploratory analysis, pivot tables, and visualisation. Predictive modelling and more advanced automation remained possible future directions rather than claimed achievements.

## 14. Challenging assumptions and AI-generated advice

During the final analysis, I also revisited advice I had received about improving focus. Some early suggestions emphasised external conditions, such as improving the environment, creating more structured schedules, or seeking greater clarity before beginning.

Those ideas were not necessarily useless, but I realised they did not fully explain what I was observing. Some of my low-scoring sessions occurred even when I had selected Good Environment. The time-block averages were also close together.

I therefore challenged the idea that a better external setup or a perfectly planned day would automatically solve the problem. I had to use my own experience and the collected observations to question advice that sounded reasonable but did not fully match the evidence.

My faith shaped this conclusion too. I cannot know or control every step in advance. I can make an effort, begin with Bismillah, ask Allah for help, and practise Tawakkul rather than expecting myself to create a flawless plan for every outcome.

This was also a useful lesson in using AI: its suggestions can help generate possibilities, but they still need to be examined against the actual problem, the data, and the experience of the person doing the work. I did not want to accept a generic recommendation simply because it sounded convincing.

## 15. Final reflection

I began with a question about why my environment, schedule, or activity seemed to affect my focus. The process made me look more carefully at the measurement itself, the limits of averages, the context behind a record, and the difference between a pattern and a cause.

The project was not a perfectly continuous experiment. I had to make practical decisions about what to measure, change parts of the form, avoid overcomplicating the tracking process, and restart after missing entries. I also had to look beyond the final charts to understand what the records actually represented.

The spreadsheet could show counts and averages. It could not fully explain what was happening in a session. I had to return to the experience behind the entry and question whether the category I selected captured what I had actually done.

The most important personal conclusion I took from the experiment was:

> **Focus in me & my moment.**

This is my reflection from a small self-tracking experiment, not a universal conclusion about human focus. The value of the project was learning to collect observations, question my assumptions, interpret the numbers carefully, and use the results to ask better questions.

The final analysis and reflections are documented in [Part 5, the completed project walkthrough](https://youtu.be/gwVauXLdDHU).
