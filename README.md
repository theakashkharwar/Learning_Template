# Plan Mapper

Plan Mapper is a personal learning system for offensive web security, web exploitation, and bug bounty preparation.

It is designed for a beginner who wants a practical, disciplined, repeatable routine instead of randomly watching videos or jumping between resources.

The main goal is simple:

```text
Study every day with structure, practice in labs, use Burp actively, write reports, and track real skill growth.
```

## Who This Is For

This repo is useful for:

- beginners starting web exploitation from scratch
- students learning bug bounty methodology
- people studying platforms like OverTheWire Natas and PortSwigger Web Security Academy
- learners who know some HTML/HTTP but need structure for JavaScript, cookies, sessions, backend logic, and vulnerabilities
- anyone who wants a daily cybersecurity study routine they can follow without overthinking

It is especially focused on offensive web security topics such as:

- HTTP and web app fundamentals
- Burp Suite usage
- cookies and sessions
- authentication and access control
- IDOR
- XSS
- SQL injection
- SSRF
- CSRF
- file upload bugs
- API security
- bug bounty report writing

## What This Repo Contains

### `LEARNING_SYSTEM_INDEX.md`

Start here.

This file explains the order in which to use the system. Open it when you are unsure which file to use.

### `6_MONTH_ROUTINE.md`

This is the main roadmap.

Use it when you want to know:

- what to study this month
- what to study this week
- what to do today
- how to follow a fixed 6-hour routine
- how to avoid wasting time deciding what comes next

This file works like a gym workout plan.

### `DAILY_OFFENSIVE_TEMPLATE.md`

Use this every study day.

It gives you a 6-hour daily structure:

- review
- learn just enough theory
- solve labs
- practice tools
- read real-world reports
- create output
- plan tomorrow

### `TOPIC_LEARNING_TEMPLATE.md`

Use this whenever you choose a specific topic.

Examples:

- "Today I am learning XSS."
- "Today I am learning IDOR."
- "Today I am learning SQL injection."
- "Today I am learning authentication bugs."

It helps you learn a topic practically by focusing on:

- root cause
- normal feature flow
- attacker-controlled input
- server-side trust mistake
- labs
- Burp workflow
- real-world reports
- reusable checklist
- mini report

### `STUDY_TIME_ASSESSMENT_SKILL.md`

Use this before starting a topic block when you are unsure whether your planned timeline is realistic.

Examples:

- "Can I learn XSS and SQLi in 4 days?"
- "Can I finish IDOR, auth bugs, and sessions in one week?"
- "Is 2 days enough for SSRF basics?"

It helps you check:

- whether your deadline is realistic
- which topics are too broad
- what can be learned in one day
- what should be moved into follow-up one-day slices
- what prerequisites are missing
- how much time each topic may actually need
- which repo files to use after the assessment
- what corrected plan to follow if your estimate is wrong

### `PROGRESS_TRACKER_TEMPLATE.md`

Use this once per week.

It helps you measure actual progress instead of only counting hours or videos watched.

Track:

- study hours
- labs solved
- reports written
- Burp skills practiced
- weak points
- next week's focus

## How To Use This Repo

Recommended daily flow:

1. Open `LEARNING_SYSTEM_INDEX.md`.
2. Open `6_MONTH_ROUTINE.md`.
3. Find your current month, week, and day.
4. Open `DAILY_OFFENSIVE_TEMPLATE.md`.
5. Follow the 6-hour study routine.
6. If studying a specific vulnerability, open `TOPIC_LEARNING_TEMPLATE.md`.
7. If your topic list or deadline feels uncertain, use `STUDY_TIME_ASSESSMENT_SKILL.md`.
8. At the end of the week, fill `PROGRESS_TRACKER_TEMPLATE.md`.

## When To Use Each File

Use `6_MONTH_ROUTINE.md` when:

- you do not know what to study next
- you want the long-term plan
- you want weekly structure
- you want a fixed daily order

Use `DAILY_OFFENSIVE_TEMPLATE.md` when:

- you are starting today's study session
- you need a practical 6-hour routine
- you want to make sure the day produces output

Use `TOPIC_LEARNING_TEMPLATE.md` when:

- you picked a vulnerability or concept
- you want a practical learning method
- you want to turn theory into labs, checklists, and reports

Use `STUDY_TIME_ASSESSMENT_SKILL.md` when:

- you picked multiple topics
- you set a deadline
- you are unsure if your estimate is realistic
- you want to know the best one-day version of a topic
- you want a corrected plan before starting
- you need to know which files to use for that plan

Use `PROGRESS_TRACKER_TEMPLATE.md` when:

- it is the end of the week
- you want to review progress
- you want to find weak points
- you want to plan the next week

## How To Make Changes

This repo should grow with your skill level.

You can edit the files when:

- a routine is too easy or too hard
- you discover better labs or resources
- you finish a month and want to adjust the next one
- you notice a repeated weak point
- you want to add a new vulnerability category
- your daily available time changes

Suggested way to update:

1. Do not rewrite everything at once.
2. Change only the part that failed in practice.
3. Keep the system practical.
4. Prefer specific actions over vague advice.
5. Add examples from your own labs and reports.

Good change:

```text
For IDOR week, add two-account testing and API object ID comparison.
```

Weak change:

```text
Study IDOR deeply.
```

## Rules For Using This System

- Do not only watch videos.
- Do not study without Burp open.
- Do not count a day as successful unless you produced an output.
- Do not chase advanced topics before web fundamentals are comfortable.
- Do not copy reports blindly; extract patterns.
- Do not test real targets unless they are authorized and in scope.
- Do not confuse solving labs with being ready for real bug bounty; use labs to build pattern recognition.

## Main Success Standard

After studying a topic, ask:

```text
Can I recognize it, test it in a lab, explain why it works, describe impact, and write a mini report?
```

If yes, you are building usable skill.

If no, repeat the topic with more practical work.

## Current Best Starting Point

If you are new, start here:

1. `LEARNING_SYSTEM_INDEX.md`
2. `6_MONTH_ROUTINE.md`
3. Month 1, Week 1: HTTP, Burp, browser dev tools, curl
4. Use `DAILY_OFFENSIVE_TEMPLATE.md` for your first 6-hour session
5. Track the week in `PROGRESS_TRACKER_TEMPLATE.md`

## Important Note

This repo is for ethical learning and authorized security testing only.

Use it for:

- legal labs
- CTFs
- training platforms
- intentionally vulnerable apps
- authorized bug bounty programs

Do not use it for attacking systems without permission.
