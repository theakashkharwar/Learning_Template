# Offensive Cyber Learning System

This folder contains your repeatable learning system for web exploitation and bug bounty.

Use these files in this order:

1. `6_MONTH_ROUTINE.md`
   - Your fixed routine for the first 6 months.
   - Open this when you do not want to think about what to study next.
   - This gives topic order, weekly structure, and daily execution.

2. `DAILY_OFFENSIVE_TEMPLATE.md`
   - Your main 6-hour daily structure.
   - Open this every day before studying.
   - This controls discipline, time, and consistency.

3. `TOPIC_LEARNING_TEMPLATE.md`
   - Use this whenever you study a specific topic such as IDOR, XSS, SQLi, CSRF, SSRF, authentication bugs, or business logic bugs.
   - This controls depth and prevents shallow learning.

4. `STUDY_TIME_ASSESSMENT_SKILL.md`
   - Use this before starting a new topic block when you are unsure if your timeline is realistic.
   - This helps you check what can be learned in one day, what should be ignored today, and how to split larger topics into follow-up one-day slices.

5. `PROGRESS_TRACKER_TEMPLATE.md`
   - Copy or reuse this for weekly tracking.
   - This helps you measure actual skill growth instead of only counting videos watched.

Core rule:

Do not ask, "Did I study today?"

Ask:

"Can I recognize, test, exploit in a lab, explain impact, and write a mini report for what I studied today?"

That is the standard.

## How To Use This System

Daily use:

1. Open `6_MONTH_ROUTINE.md`.
2. Find the current week and current day.
3. If you are unsure about your time estimate, open `STUDY_TIME_ASSESSMENT_SKILL.md`.
4. Open `DAILY_OFFENSIVE_TEMPLATE.md`.
5. Execute the 6-hour routine.
6. If the day has a specific topic, open `TOPIC_LEARNING_TEMPLATE.md`.
7. End the day with one written output.
8. End the week with `PROGRESS_TRACKER_TEMPLATE.md`.

General copy-paste prompt:

```text
You are my practical learning coach for [DOMAIN/SKILL]. I want to build real usable ability in this domain over the next 6 months, not just consume theory.

My current level:
[Describe what I already know, what I am weak in, what tools/resources I have used, and any relevant background.]

My goal:
[Describe the outcome I want in 6 months: job-ready, project-ready, certification-ready, freelance-ready, competition-ready, portfolio-ready, etc.]

Available time:
[Hours per day] for [number of days per week].

Today's topic:
[Specific topic I want to study today.]

Today's expected output:
[Example: solved labs, mini report, checklist, project artifact, case study, notes, practice problems, analysis report, tool workflow, portfolio piece.]

Create a practical routine for today in exact order. Do not give a generic syllabus or motivation. For each block, tell me:
- what to learn first
- what to ignore for now
- what to practice
- which resources/labs/projects/exercises to use
- what tool actions to perform
- what observations or notes to capture
- what mistakes to avoid
- what final artifact to produce
- how to verify that I actually learned it

Make the plan realistic for my current level and aligned with my 6-month goal. If my topic is too broad for one day, narrow it to the most valuable one-day version and give follow-up steps.
```
