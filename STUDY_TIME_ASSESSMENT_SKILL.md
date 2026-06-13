# Study Time Assessment Skill

Purpose: check whether your planned study time is realistic, then convert it into a practical one-day learning slice.

Use this when you have chosen topics and a deadline, but you are not sure if your estimate is correct.

Main question:

```text
Can I learn this topic enough in one day to become operational?
```

Operational means:

- I can explain the concept simply.
- I can recognize where it appears in a web app.
- I can solve at least one beginner lab.
- I can use Burp on the important request.
- I can explain the root cause and impact.
- I can create a mini report, checklist, or Burp workflow note.

Operational does not mean mastery.

## The One-Day Upper Cap Rule

For this system, one day is the maximum size of a first learning block.

If a topic is too large, do not ask:

```text
How many days do I need to learn all of this?
```

Ask:

```text
What useful version of this can I learn in one day?
What should I ignore today?
What should become Day 2, Day 3, or later?
```

The answer should never only say:

```text
This topic needs one week.
```

It should say:

```text
You cannot learn the full topic properly in one day.
But in one day, you can learn this slice:
- ...

Then continue with:
- Day 2:
- Day 3:
- Later revisit:
```

## When To Use This

Use this before:

- starting a new topic
- planning a week
- combining multiple topics
- setting a deadline
- asking an AI assistant to create a custom plan
- deciding whether your goal is too broad for one day

Examples:

```text
I want to learn XSS, SQLi, IDOR, and CSRF in 7 days.
Is that realistic?
What can I learn today?
```

```text
I want to learn SQL injection in 6 hours and solve 5 labs.
Is that correct for my level?
```

```text
I want to study cookies, sessions, authentication, and IDOR this week.
How should I split the one-day blocks?
```

## Your Current Baseline

Use this baseline unless your level changes:

```text
Current level:
- beginner in web exploitation and bug bounty
- comfortable with HTML and basic HTTP
- brushing up JavaScript, cookies, sessions
- weak in backend logic
- new to Burp Suite
- around Natas level 2
- available time: 6 hours per day
- goal: job-ready fresher web security skill or meaningful bug bounty capability in 6 months
```

## Verdict Labels

Every assessment should return one of these.

### Green - One-Day Plan Is Realistic

Your topic is narrow enough for one operational day.

Examples:

- HTTP request/response refresh
- Burp Proxy basics
- cookies basics
- simple IDOR intro
- reflected XSS intro
- one small PortSwigger lab category
- one Natas level cluster

Expected one-day output:

- 1-3 labs
- one mini report or checklist
- one Burp workflow note

### Yellow - One-Day Plan Is Possible Only If Narrowed

The topic is useful, but the full version is too broad.

Examples:

- XSS as a whole
- SQL injection as a whole
- authentication flaws
- session management
- SSRF basics
- API security basics
- file upload vulnerabilities

Expected correction:

- choose one subtopic
- solve 1-2 beginner labs
- create one checklist or mini report
- schedule follow-up slices

### Red - Plan Is Not Realistic In One Day

The plan mixes too many topics or expects mastery too fast.

Examples:

- complete XSS mastery in one day
- complete SQL injection mastery in one day
- full bug bounty methodology in one day
- all authentication vulnerabilities in one day
- JavaScript, backend logic, and exploitation together in one day
- recon, exploitation, and reporting for real targets in one day

Expected correction:

- reduce to one topic slice
- define a realistic one-day output
- schedule the remaining slices later

## Assessment Rules

### Rule 1: One Day Can Build Version 1

Bad goal:

```text
Learn XSS completely in one day.
```

Corrected goal:

```text
Learn reflected XSS basics in one day:
- input reflection
- output context
- 2 beginner labs
- Burp Repeater testing
- one mini report
```

### Rule 2: Broad Topics Must Be Split

Bad topic:

```text
Authentication bugs
```

One-day slices:

```text
Day 1: login flow and session creation
Day 2: password reset logic
Day 3: brute force protections in labs
Day 4: MFA bypass basics
Day 5: session/logout behavior and report writing
```

### Rule 3: Labs Decide Reality

If the plan has no lab time, the estimate is wrong.

Minimum one-day split:

- 20 percent theory
- 40 percent labs
- 20 percent Burp/tool practice
- 20 percent notes, reports, and review

### Rule 4: Your Weak Fundamentals Slow The Topic

Add prerequisite time when needed.

Examples:

- DOM XSS needs JavaScript and browser behavior.
- SQLi needs basic database/backend query understanding.
- auth bugs need cookies, sessions, and backend checks.
- SSRF needs URL parsing, internal services, and request behavior.

### Rule 5: Completion Requires An Artifact

A topic is not complete because you watched a video.

Completion means you produced at least one:

- mini report
- reusable checklist
- solved lab notes
- Burp workflow note
- real-world pattern summary

## How To Split Big Topics Into One-Day Slices

### XSS

One-day slices:

- reflected XSS basics
- stored XSS basics
- DOM XSS basics
- XSS contexts: HTML body, attribute, JavaScript string
- filter bypass basics
- impact and report writing

### SQL Injection

One-day slices:

- SQLi mental model and login bypass labs
- UNION-based SQLi basics
- blind SQLi basics
- error-based SQLi basics
- SQLi impact and data extraction in labs
- SQLi reporting and remediation

### Authentication

One-day slices:

- login flow and session creation
- weak password reset logic
- brute force protections in labs
- MFA bypass basics
- session fixation and logout behavior
- account takeover report writing

### Access Control

One-day slices:

- access control mental model
- IDOR with numeric IDs
- IDOR with UUIDs and APIs
- vertical privilege escalation
- horizontal privilege escalation
- two-account testing workflow

### Backend Logic

One-day slices:

- request -> route -> controller -> database -> response
- authentication middleware
- authorization checks
- database query basics
- state-changing actions
- business logic mistakes

### SSRF

One-day slices:

- SSRF mental model and URL-controlled requests
- basic SSRF labs
- internal service targeting in labs
- blind SSRF basics
- SSRF impact and safe reporting

### API Security

One-day slices:

- API request/response mapping
- JSON body manipulation
- object ID testing
- role and permission testing
- mass assignment basics
- API report writing

## Which Repo File To Use After Assessment

If verdict is Green:

1. Use `DAILY_OFFENSIVE_TEMPLATE.md`.
2. Use `TOPIC_LEARNING_TEMPLATE.md` if it is a vulnerability topic.
3. End with a mini report, checklist, or Burp workflow note.

If verdict is Yellow:

1. Use this file to narrow the topic.
2. Pick only one one-day slice.
3. Use `TOPIC_LEARNING_TEMPLATE.md`.
4. Put the follow-up slices into `6_MONTH_ROUTINE.md` style.

If verdict is Red:

1. Remove extra topics.
2. Pick the highest-value beginner slice.
3. Use `DAILY_OFFENSIVE_TEMPLATE.md` for today's 6-hour execution.
4. Schedule the rest as future one-day blocks.

If planning a full week:

1. Use this skill first to split the topic list into day-sized blocks.
2. Use `6_MONTH_ROUTINE.md` to place those blocks into the week.
3. Use `PROGRESS_TRACKER_TEMPLATE.md` on Day 7.

## Required Input Format

When asking an AI assistant to assess your plan, provide:

```text
My current level:
Topics I want to study:
Time I want to complete them in:
Hours per day:
Current tools/platforms:
Expected output:
Reason I chose this timeline:
```

Example:

```text
My current level:
Beginner, know HTML and HTTP, new to Burp, weak in JS/cookies/sessions/backend logic.

Topics I want to study:
XSS, IDOR, SQL injection.

Time I want to complete them in:
3 days.

Hours per day:
6 hours.

Current tools/platforms:
PortSwigger, Natas, Burp Community.

Expected output:
5 labs per topic and one mini report each.

Reason I chose this timeline:
I want to move fast toward bug bounty.
```

## Assessment Output Format

The answer should use this structure:

```text
Verdict: Green / Yellow / Red

Is my time estimate correct?

Why:

What I can learn in one day:

What I should not try today:

Corrected one-day slice:

Exact 6-hour routine:

Labs/practice:

Burp actions:

Final artifact:

Which repo files to use:

Follow-up slices:

End-of-day self-test:
```

## Master Prompt

Copy this prompt when you want a realistic time assessment.

```text
You are my offensive web security learning planner and time-estimation coach.

My current baseline:
- beginner in web exploitation and bug bounty
- comfortable with HTML and basic HTTP
- brushing up JavaScript, cookies, sessions
- weak in backend logic
- new to Burp Suite
- around Natas level 2
- available study time: [HOURS PER DAY]
- goal: become job-ready for a fresher web security role or capable of finding a meaningful bug bounty issue within 6 months

Topics I want to study:
[LIST TOPICS]

My desired deadline:
[TIME PERIOD]

My expected output:
[labs, reports, checklist, notes, Burp practice, etc.]

Assess this plan honestly.

Important rule:
The upper cap for a first pass is one day. If the full topic cannot be learned properly in one day, do not simply say "it takes longer." Tell me exactly what useful slice I can learn in one day, what I should ignore for now, and what follow-up slices I should schedule after that.

Return the answer in this format:
1. Verdict: Green, Yellow, or Red.
2. Is my time estimate correct? Answer directly.
3. Why is it correct or wrong for my current level?
4. What can I realistically learn in one day?
5. What should I not try to learn today?
6. Corrected topic breakdown into one-day slices.
7. Exact 6-hour routine for the first day.
8. Recommended labs or practice sources.
9. Exact Burp Suite actions to perform.
10. What notes or artifact I must produce.
11. Which repo files I should use: `6_MONTH_ROUTINE.md`, `DAILY_OFFENSIVE_TEMPLATE.md`, `TOPIC_LEARNING_TEMPLATE.md`, `PROGRESS_TRACKER_TEMPLATE.md`.
12. Follow-up plan after day one.
13. End-of-day self-test to check if I became operational.

Be practical and strict. Do not motivate me with generic advice. Protect me from overestimating myself, but keep momentum by giving me a useful one-day version.
```

## Example Assessment

Plan:

```text
Topics: reflected XSS, stored XSS, DOM XSS, filter bypasses
Deadline: 1 day
Hours: 6 hours
Expected output: 5 labs and one mini report
```

Assessment:

```text
Verdict: Red

Your time estimate is not realistic because this is all of beginner XSS, not one day of XSS.

What you can learn in one day:
- reflected XSS basics
- input reflection
- output context
- 2-3 beginner labs
- Burp Repeater testing
- one mini report

What to ignore today:
- stored XSS
- DOM XSS
- advanced bypasses
- WAF/filter bypass tricks

Follow-up slices:
- Day 2: stored XSS
- Day 3: DOM XSS basics
- Day 4: XSS contexts
- Day 5: filter bypass basics
```

## Final Decision Rule

If the plan has too many topics and not enough labs, it is not a learning plan.

It is only a wish list.

Convert it into:

```text
fewer topics + one-day slices + labs + Burp practice + written output
```

