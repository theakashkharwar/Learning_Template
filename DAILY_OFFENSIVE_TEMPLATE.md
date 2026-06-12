# Daily Offensive Learning Template

Purpose: build discipline and practical web exploitation skill every day.

Time available: 6 hours per day.

Daily goal:

By the end of the day, you should produce one clear output:

- a solved lab
- a mini report
- a checklist
- a Burp workflow note
- a short explanation of a concept in your own words

If there is no output, the day was probably too passive.

## Before You Start

Pick today's mode:

- Foundation day: HTTP, JavaScript, cookies, sessions, backend logic, Burp basics.
- Vulnerability day: IDOR, XSS, SQLi, SSRF, CSRF, auth bug, file upload, etc.
- Mixed practice day: old labs, Natas, report writing, weak-point repair.

Then write:

```text
Today's topic:
Today's mode:
Today's lab source:
Today's Burp skill:
Today's output:
```

## The 6-Hour Structure

### 1. Review And Warm Up - 30 Minutes

Do this before learning anything new.

- Review yesterday's notes.
- Reopen one request or lab you solved.
- Explain yesterday's topic in 5-7 lines.
- Write one thing you still do not understand.

Prompt:

```text
Yesterday I learned:
The bug happened because:
The attacker controlled:
The server trusted:
The impact was:
Today I need to improve:
```

Practical task:

- reopen one old request in Burp history or your notes
- explain what each important parameter did
- write one test you could have tried but did not

### 2. Learn Just Enough Theory - 60 Minutes

Use video first if that helps you start, but do not watch passively.

Write only these five points:

- What is the concept or vulnerability?
- What condition makes it possible?
- What does the attacker control?
- What does the server trust incorrectly?
- What is the real-world impact?

Rule:

Stop theory when you can attempt a lab. Do not wait until you feel fully ready.

Theory order:

1. definition
2. root cause
3. where it appears in real web apps
4. simple exploit example
5. impact
6. common developer mistake

Ignore for now:

- rare bypasses
- advanced payload chains
- deep internals that do not help today's lab
- long tool installation rabbit holes

### 3. Attack Labs - 120 Minutes

Primary platforms:

- PortSwigger Web Security Academy
- OverTheWire Natas
- OWASP Juice Shop
- DVWA, only for basic practice

Lab workflow:

1. Open the app normally.
2. Use browser dev tools.
3. Intercept requests in Burp.
4. Identify all inputs you control.
5. Modify one thing at a time.
6. Observe the response carefully.
7. Repeat until you understand the behavior.
8. Write the exact steps that solved it.

Minimum lab target:

- beginner day: 1-2 labs
- normal day: 2-3 labs
- strong day: 4-5 labs

While solving, keep asking:

```text
What request caused this action?
Which parameter matters?
What is client-side only?
What is checked on the server?
What happens if I change this value?
What would the business impact be?
```

After each lab, write:

```text
Lab:
Feature tested:
Original request:
Parameter changed:
Security check bypassed:
Proof:
Impact:
```

### 4. Tool Practice - 60 Minutes

Rotate tools depending on the topic.

For now, prioritize:

- Burp Suite Proxy
- Repeater
- Intruder basics
- Browser dev tools
- curl
- basic JavaScript console usage

Tool practice is not random clicking. Pick one skill for the day.

Examples:

- Send 10 requests from Proxy to Repeater.
- Change cookies manually and observe behavior.
- Replay login and logout requests.
- Compare two user sessions.
- Use curl to reproduce one browser request.
- Find where frontend JavaScript calls backend APIs.

Tool drill menu:

- If studying cookies/sessions: compare two users' cookies and session behavior.
- If studying IDOR/access control: use two accounts and compare authorization.
- If studying XSS: test input/output reflection and context.
- If studying SQLi: send suspicious parameters to Repeater and test safely in labs.
- If studying API bugs: inspect JSON requests and change IDs, roles, or states.

### 5. Real-World Pattern Reading - 45 Minutes

Read 1-2 real disclosed reports or writeups related to today's topic.

Good sources:

- HackerOne Hacktivity
- Bugcrowd reports
- PortSwigger research
- Assetnote blog
- Writeups from trusted researchers

Extract only:

- Where was the bug found?
- What request or parameter was changed?
- What was the impact?
- What made the report convincing?
- What pattern can I reuse?

Avoid endless writeup reading. Your goal is pattern extraction.

Report reading rule:

Convert every report into this sentence:

```text
The attacker changed _____ in _____, because the server failed to check _____, causing _____.
```

### 6. Output - 45 Minutes

Create one artifact before ending the day.

Choose one:

- mini vulnerability report
- topic checklist
- solved lab notes
- Burp request/response notes
- "how I would test this on a real target" plan

Mini report format:

```text
Title:
Target/Feature:
Vulnerability:
Steps To Reproduce:
Observed Result:
Expected Result:
Impact:
Fix Recommendation:
What I Learned:
```

Output quality check:

- Can another beginner reproduce the issue from your steps?
- Did you include the vulnerable request or parameter?
- Did you explain impact, not only the trick?
- Did you write what the server should have checked?

### 7. Tomorrow Plan - 15 Minutes

Decide tomorrow before you stop today.

Write:

```text
Tomorrow's topic:
Main lab:
Tool skill:
One weak point to improve:
Expected output:
```

## Daily Success Score

Score yourself out of 5:

- 1 point: I reviewed yesterday.
- 1 point: I learned only useful theory.
- 1 point: I practiced in a lab.
- 1 point: I used Burp/dev tools/curl actively.
- 1 point: I produced a written output.

Minimum acceptable score: 4/5.

## Current Priority For You

Since you are at Natas level 2 and just starting Burp, your first focus should be:

1. HTTP request/response confidence
2. cookies and sessions
3. basic JavaScript for web hackers
4. backend logic basics
5. authentication and access control
6. PortSwigger beginner labs
7. report writing from lab findings

Do not rush into advanced payloads before this base is comfortable.

## Copy-Paste Prompt For A Custom Daily Plan

Use this when you want me or another GPT to generate your exact day.

```text
You are my practical offensive web security coach. I study 6 hours per day and I want a no-confusion daily routine that I can follow step by step.

My current level:
- beginner in web exploitation and bug bounty
- comfortable with HTML and basic HTTP
- need brushing up on JavaScript, cookies, sessions, and backend logic
- just started using Burp Suite
- around Natas level 2

Today's topic: [TOPIC]
Today's mode: [foundation / vulnerability / mixed practice]
Today's desired output: [mini report / checklist / 5 labs / Burp workflow note / notes]

Create my exact 6-hour plan with timestamps. Include:
- the subtopics to learn in order
- what I should ignore today
- specific practical tasks
- recommended labs or practice sources
- exact Burp actions to perform
- what to observe in requests and responses
- what notes to write after each stage
- one final artifact I must create
- a short self-test to prove I learned it

Make it practical, beginner-friendly, and offensive-security focused. Avoid generic motivation or theory-only advice.
```
