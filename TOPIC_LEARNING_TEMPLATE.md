# Topic Learning Template

Purpose: learn one offensive security topic quickly without becoming shallow.

Use this for topics like:

- IDOR
- XSS
- SQL injection
- CSRF
- SSRF
- authentication flaws
- access control bugs
- file upload bugs
- command injection
- business logic bugs
- API security issues

One-day goal:

Become operational with the topic.

Operational means:

- I can explain it simply.
- I can recognize where it may appear.
- I can test it in a lab.
- I can exploit a simple case.
- I can explain business impact.
- I can write a mini report.

It does not mean total mastery.

## Topic Execution Order

Follow this exact order for any topic.

```text
Step 1: Define the bug in one sentence.
Step 2: Learn the normal feature flow.
Step 3: Identify what the attacker controls.
Step 4: Identify what the server should check.
Step 5: Solve one simple lab.
Step 6: Repeat with 2-4 more labs.
Step 7: Use Burp to replay and modify the important requests.
Step 8: Read 1-2 real reports.
Step 9: Create a checklist.
Step 10: Write a mini report.
```

Do not skip the normal feature flow. You cannot break what you cannot describe.

## 1. Simple Definition

Write the concept in one sentence.

Template:

```text
[Topic] happens when the server/app _____, and the attacker can _____, causing _____.
```

Example:

```text
IDOR happens when the server trusts a user-supplied object ID, and the attacker can change that ID, causing access to another user's data.
```

## 2. Cause And Condition

Answer:

```text
This bug becomes possible when:
The missing security check is:
The attacker-controlled input is:
The protected asset/action is:
```

This step matters because real hacking is not memorizing payloads. It is understanding broken trust.

## 2.5 Normal Feature Flow

Before attacking, describe how the feature should work.

Template:

```text
User action:
Browser request:
Server receives:
Server checks:
Server reads/writes:
Server response:
What should be protected:
```

Example:

```text
User action: user opens invoice page.
Browser request: GET /invoice?id=123.
Server receives: invoice ID and session cookie.
Server checks: user is logged in and owns invoice 123.
Server reads/writes: reads invoice 123 from database.
Server response: returns invoice details.
What should be protected: invoice data of other users.
```

## 3. Where To Look

List common places this topic appears.

Template:

```text
URLs:
Query parameters:
POST body:
JSON APIs:
Cookies:
Headers:
Hidden form fields:
JavaScript files:
File upload points:
Admin/user settings:
Billing/subscription flows:
Team/org/workspace features:
```

Delete what does not apply to the topic.

## 4. Detection Checklist

Create a checklist you can use on labs and real authorized targets.

Template:

```text
When I see _____, I should test _____.
When the app returns _____, it may mean _____.
If I change _____ and still get success, that suggests _____.
If the check happens only in JavaScript, I should _____.
```

Example for IDOR:

```text
When I see user_id, account_id, file_id, invoice_id, org_id, or order_id, I should test access control.
If I change an ID and still get data, that suggests missing object-level authorization.
If the UI hides a button but the request still works, the check may be client-side only.
```

## 5. Lab Plan

Use at least one lab source.

Preferred order:

1. PortSwigger Web Security Academy
2. Natas, if relevant
3. OWASP Juice Shop
4. DVWA for basic concepts only

For each lab, record:

```text
Lab name:
Goal:
Important request:
Important parameter:
What I changed:
Why it worked:
Final exploit steps:
```

## 6. Burp Workflow

Record exactly how Burp helped.

Template:

```text
Proxy:
Repeater:
Intruder:
Comparer:
Decoder:
Logger/history:
```

Example:

```text
Proxy: captured the request.
Repeater: modified account_id and replayed the request.
Comparer: compared responses from two users.
Decoder: decoded a base64 value in a cookie.
```

## 7. Real-World Reports

Read 1-2 real reports on the topic.

Extract:

```text
Report title/link:
Affected feature:
Root cause:
Attack steps:
Impact:
Why the report was accepted:
Pattern I can reuse:
```

Do not copy reports blindly. Extract patterns.

## 7.5 Real-App Simulation

After labs, imagine testing the same topic on a legal target.

Write:

```text
Features I would inspect first:
Requests I would capture:
Parameters I would modify:
Two-account test needed? yes/no
Impact I would try to prove safely:
What I must avoid because it is out of scope or unsafe:
```

This builds bug bounty judgment, not only lab-solving skill.

## 8. Mini Report

Write a report even if the bug is from a lab.

Template:

```text
Title:
Severity:
Affected Feature:
Summary:
Steps To Reproduce:
Evidence:
Impact:
Recommended Fix:
Learning Notes:
```

Impact examples:

- account takeover
- unauthorized data access
- privilege escalation
- payment or subscription abuse
- sensitive file disclosure
- admin action execution
- internal service access

## 9. Final Compression

End the topic with this summary:

```text
The shortest explanation:
The main root cause:
Top 5 places to test:
Top 5 mistakes developers make:
Top 5 Burp actions:
Real-world impact:
My current weakness:
Next revisit date:
```

## The One-Day Rule

Do not try to finish a topic forever in one day.

In one day, create version 1.

Then revisit it later:

- after 3 days
- after 1 week
- after 1 month
- when you see it in a real app

This is how topics compound.

## Copy-Paste Prompt For A Topic Plan

Use this when you choose a topic like XSS, IDOR, SQLi, SSRF, CSRF, authentication flaws, or API bugs.

```text
You are my offensive web exploitation mentor. I want to learn this topic in a practical, bug-bounty-oriented way in one day.

Topic: [TOPIC]
My current level:
- beginner in web exploitation
- comfortable with HTML and basic HTTP
- brushing up JavaScript, cookies, sessions
- weak in backend logic
- new to Burp Suite

My target for today:
- learn the topic enough to recognize it
- solve [NUMBER] labs
- create [mini report/checklist/Burp workflow note]

Create a practical topic-learning plan in exact order. Include:
1. The minimum theory I need, explained simply.
2. The normal web feature flow I must understand before attacking.
3. The root cause of the bug.
4. Where this bug appears in real apps.
5. The exact order of subtopics to learn.
6. Which PortSwigger/Natas/Juice Shop labs or lab categories to practice.
7. What exact actions to perform in Burp Suite.
8. What parameters, headers, cookies, or responses to observe.
9. What mistakes beginners make with this topic.
10. What real-world bug bounty reports/patterns to search for.
11. A checklist I can reuse on authorized targets.
12. A mini report template filled with placeholders for this topic.
13. A final self-test with practical questions.

Do not give a broad theoretical syllabus. Give me a realistic execution plan that turns the topic into hands-on skill today.
```
