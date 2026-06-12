# 6-Month Web Exploitation Routine

Purpose: give you a fixed order to follow without wasting energy deciding what to do next.

Your target:

- become job-ready for a fresher web security role
- become capable of finding and reporting a meaningful real-world web bug

Your daily time:

- 6 hours per day
- 6 study days per week
- 1 weekly review/light day

Main platforms:

- PortSwigger Web Security Academy
- OverTheWire Natas
- OWASP Juice Shop
- Burp Suite Community
- browser dev tools
- curl
- disclosed bug bounty reports

## Weekly Rhythm

Use this rhythm every week.

### Day 1 - Learn And Map

Goal: understand the topic and where it appears in real apps.

Do:

1. Watch/read only enough theory to understand the root cause.
2. Draw the request flow in notes.
3. Identify attacker-controlled inputs.
4. List where the bug appears in URLs, forms, APIs, cookies, headers, or JavaScript.
5. Solve 1 easy lab.

Output:

- one-page topic map

### Day 2 - Lab Repetition

Goal: build hands-on recognition.

Do:

1. Solve 2-3 beginner labs.
2. Send every important request to Burp Repeater.
3. Change one parameter at a time.
4. Write why the exploit worked.

Output:

- solved lab notes with request, parameter, change, impact

### Day 3 - Tool Skill

Goal: connect the topic to Burp/dev tools/curl.

Do:

1. Reproduce one lab request manually in Burp Repeater.
2. Reproduce one request with curl.
3. Compare normal and modified responses.
4. Save useful payloads or test values.

Output:

- Burp workflow note

### Day 4 - Real-World Pattern

Goal: understand how the bug looks outside clean labs.

Do:

1. Read 2 disclosed reports or high-quality writeups.
2. Extract the affected feature, request, root cause, and impact.
3. Convert the reports into a reusable checklist.

Output:

- hunter checklist for that topic

### Day 5 - Harder Labs And Report

Goal: move from solving to explaining.

Do:

1. Solve 1-2 medium labs if possible.
2. If stuck for more than 40 minutes, read a hint, not the full solution.
3. Write a mini report for one solved lab.

Output:

- mini vulnerability report

### Day 6 - Mixed Practice

Goal: test recall without hand-holding.

Do:

1. Pick one older lab from the week and solve again without notes.
2. Continue Natas for 60-90 minutes.
3. Do one mixed PortSwigger lab from an older topic.
4. Update your weak-points list.

Output:

- weekly weak-points list

### Day 7 - Review Or Light Day

Goal: prevent forgetting.

Do:

1. Fill `PROGRESS_TRACKER_TEMPLATE.md`.
2. Score your skills honestly.
3. Revisit the hardest request from the week.
4. Choose next week's topic.

Output:

- weekly review

## Month-By-Month Topic Order

### Month 1 - Web App Foundations

Goal: understand how web apps work before attacking them deeply.

Weeks:

1. HTTP, Burp, browser dev tools, curl
2. cookies, sessions, authentication flow
3. JavaScript for hackers, frontend-to-backend API calls
4. backend logic basics: routes, controllers, databases, authorization checks

Expected outputs:

- 15+ labs or Natas levels
- 4 mini reports
- 4 Burp workflow notes
- 1 personal web app request-flow checklist

### Month 2 - Access Control And Authentication

Goal: become strong in bugs that are common and bounty-relevant.

Weeks:

1. access control basics
2. IDOR and object-level authorization
3. authentication flaws
4. session management and password reset logic

Expected outputs:

- 20+ PortSwigger labs
- 6 mini reports
- access control checklist
- authentication checklist

### Month 3 - Client-Side And Injection Basics

Goal: understand input, output, context, and server-side trust.

Weeks:

1. reflected XSS
2. stored XSS and DOM XSS basics
3. SQL injection basics
4. command injection and path traversal basics

Expected outputs:

- 25+ labs
- XSS context notes
- SQLi notes
- 6 mini reports

### Month 4 - File, API, And Server-Side Bugs

Goal: move into realistic app features.

Weeks:

1. file upload vulnerabilities
2. SSRF basics
3. API testing and JSON endpoints
4. CSRF and CORS basics

Expected outputs:

- API testing checklist
- SSRF checklist
- file upload checklist
- 6 mini reports

### Month 5 - Bug Bounty Methodology

Goal: learn how to test real authorized targets safely and methodically.

Weeks:

1. target selection and scope reading
2. recon for web apps
3. feature mapping and attack surface mapping
4. writing high-quality reports

Expected outputs:

- 2 realistic target maps on allowed programs
- 10 report rewrites from lab bugs
- personal testing methodology

### Month 6 - Job And Bounty Readiness

Goal: prove capability.

Weeks:

1. mixed labs under time limits
2. portfolio writeups
3. mock bug bounty testing on legal targets
4. interview prep and final weak-point repair

Expected outputs:

- 8-10 polished writeups
- one public or private portfolio folder
- one complete methodology document
- interview-ready explanations of major web bugs

## Exact Daily Execution Order

Use this when you sit down and do not want to think.

```text
00:00-00:10  Open yesterday's notes and today's topic.
00:10-00:30  Review yesterday's request, bug, and weak point.
00:30-01:30  Learn just enough theory for today's topic.
01:30-03:30  Solve labs with Burp open. Capture, modify, repeat.
03:30-04:30  Tool drill: Repeater, curl, dev tools, or session comparison.
04:30-05:15  Read real report/writeup and extract patterns.
05:15-05:50  Create output: report, checklist, lab notes, or workflow.
05:50-06:00  Score the day and plan tomorrow.
```

## No-Thinking Decision Rules

If you do not know what to do:

- If the topic is new, watch/read for 45-60 minutes, then stop and do labs.
- If you are stuck in a lab for 40 minutes, take one hint and continue.
- If you solved a lab too easily, write a report or solve a harder one.
- If you watched more than 90 minutes of video, stop and open Burp.
- If you feel confused, write the request flow: browser -> request -> server -> database/action -> response.
- If you are tired, do review, report rewriting, or Natas instead of skipping the day.

## Master Prompt For This Routine

Copy this prompt whenever you want a custom day plan.

```text
You are my offensive web security mentor and bug bounty training coach. Build me a practical study routine for today using my fixed 6-hour system.

My current level:
- I am a beginner in web exploitation and bug bounty.
- I know HTML and basic HTTP.
- I need brushing up on JavaScript, cookies, sessions, and backend logic.
- I have just started using Burp Suite.
- I am around Natas level 2.
- My goal is to become job-ready for a fresher web security role or capable of finding a meaningful bounty bug within 6 months.

Today's topic: [TOPIC]
Today's target output: [mini report / checklist / 5 labs / Burp workflow note / mixed practice]
Available time: 6 hours
Preferred style: practical first, video allowed only for initial understanding

Create a step-by-step routine in exact order with timestamps. For each stage include:
1. What exact subtopics to learn, in order.
2. What to ignore for now.
3. Which labs to practice, preferably PortSwigger/Natas/Juice Shop.
4. What exact actions to perform in Burp Suite.
5. What request/response details to observe.
6. What notes to write after each lab.
7. What real-world bug bounty patterns to extract.
8. What final artifact to produce.
9. A 10-question self-test at the end.

Make the plan beginner-friendly but not lazy. Keep it realistic, practical, and offensive-security oriented. Do not give a generic lecture. I want a routine I can follow like a gym workout.
```
