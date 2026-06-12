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

4. `PROGRESS_TRACKER_TEMPLATE.md`
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
3. Open `DAILY_OFFENSIVE_TEMPLATE.md`.
4. Execute the 6-hour routine.
5. If the day has a specific topic, open `TOPIC_LEARNING_TEMPLATE.md`.
6. End the day with one written output.
7. End the week with `PROGRESS_TRACKER_TEMPLATE.md`.

Copy-paste prompt:

```text
You are my offensive web security learning coach. I am following a 6-month web exploitation and bug bounty plan. I can study 6 hours today. My current level: beginner, comfortable with HTML and HTTP, brushing up JavaScript/cookies/sessions, new to backend logic and Burp Suite, currently around Natas level 2.

Today's topic is: [TOPIC].
Today's expected output is: [mini report / checklist / 5 labs / Burp workflow note].

Create a practical 6-hour routine for today in exact order. Do not give generic theory. For each block, tell me:
- what to learn
- what to practice
- what lab/source to use
- what to do inside Burp
- what notes to write
- what mistakes to avoid
- what final artifact to produce

Make the plan realistic for a beginner but aligned with job-ready web exploitation and bug bounty skills. Include a short end-of-day self-test.
```
