# Long-Term Learning And Learn In Public Routine

Purpose: convert a finalized learning roadmap into a dated execution routine that develops skill and produces public proof of work.

Despite the original filename, this system works for a 2-month, 3-month, 6-month, or custom timeline. It is domain-neutral and can be used for web exploitation, red teaming, backend development, stock analysis, or another serious learning goal.

This file does not decide the overall roadmap. Create that first with `LEARNING_SYSTEM_INDEX.md`, then paste its Copy-Paste Plan Handoff into the master prompt below.

## How To Use This File

1. Create and finalize the high-level roadmap with `LEARNING_SYSTEM_INDEX.md`.
2. Copy the Plan Handoff produced by that file.
3. Fill the execution and publishing inputs in the master prompt below.
4. Give the complete prompt to an AI.
5. Do not accept a routine until every date has an action, artifact, and pass/fail test.
6. Use the generated daily handoff with `DAILY_OFFENSIVE_TEMPLATE.md`.
7. Use the generated topic handoff with `TOPIC_LEARNING_TEMPLATE.md` when a topic needs deeper treatment.
8. Record weekly results with `PROGRESS_TRACKER_TEMPLATE.md`.

## Learn In Public Standard

Learn in Public does not mean posting unfinished notes every day. It means learning through a repeatable evidence pipeline:

```text
Learn -> Practice -> Capture Evidence -> Explain -> Verify -> Publish -> Repurpose -> Receive Feedback -> Improve
```

Writing is the primary public output. Use one platform as the canonical home for the complete article. Convert that article into shorter platform-specific posts instead of independently rewriting the same lesson everywhere.

Default publication cadence:

- daily: capture notes, evidence, mistakes, and unanswered questions privately
- weekly: publish one substantial, verified article
- weekly: derive one LinkedIn post and one X/Twitter post or thread from the article
- each major roadmap milestone: publish or add a project, case study, report, demonstration, or portfolio artifact

Default weekly time allocation:

- 70%: learning, practice, labs, and projects
- 20%: writing, editing, and evidence preparation
- 10%: publishing, distribution, feedback, and review

Views and follower counts are secondary. The primary measurements are practical ability, reproducible evidence, explanation quality, useful feedback, and portfolio strength.

## Default Weekly Operating System

The generated routine should adapt this cycle to the user's available days. When seven days are available, use this order:

### Day 1 - Learn And Define

- Learn the week's first principles and normal workflow.
- Define the practical question the week must answer.
- Choose the flagship article's claim, audience, and required evidence.
- Produce a one-page topic map and article outline.

### Day 2 - Guided Practice

- Complete guided labs, exercises, examples, or tutorials.
- Capture commands, screenshots, requests, calculations, decisions, and mistakes.
- Produce structured practice notes that can support the article.

### Day 3 - Independent Practice

- Repeat the skill without following a solution.
- Build, solve, analyze, or test something independently.
- Record where recall or judgment failed.
- Produce reproducible evidence of the attempt.

### Day 4 - Applied Challenge

- Use the skill in a harder lab, project feature, case study, simulation, or authorized real-world exercise.
- Validate the result instead of trusting the first successful output.
- Produce the week's strongest technical or practical evidence.

### Day 5 - Synthesize And Draft

- Convert the week's work into a complete article draft.
- Include evidence, mistakes, corrections, and practical conclusions.
- Identify every claim that still needs verification.

### Day 6 - Verify, Publish, And Repurpose

- Reproduce important steps and fact-check the article.
- Remove private, unsafe, misleading, or prohibited material.
- Publish the article on the canonical platform.
- Create a LinkedIn post and an X/Twitter post or thread linking to it.
- Add the article or milestone artifact to the portfolio.

### Day 7 - Feedback And Review

- Reply to useful questions and record corrections.
- Review skill evidence and publication quality.
- Update the progress tracker and weak-points list.
- Prepare next week's topic, evidence target, and article question.

If fewer than seven study days are available, the generated routine must combine compatible activities without removing independent practice, verification, publication, or weekly review.

## Publication Quality Gate

An article is ready only when it passes all of these checks:

- It has a specific learning objective and intended audience.
- Its important claims were verified with a reliable source or reproducible work.
- It shows evidence rather than only summarizing theory.
- It explains at least one mistake, failed attempt, or correction.
- Another learner can follow the explanation or reproduce the safe exercise.
- It ends with concrete conclusions and the next learning step.
- It does not expose private, unsafe, copyrighted, or prohibited information.
- It is labeled accurately as a lab, simulation, project, analysis, or authorized real-world result.

Do not publish filler merely to preserve a streak. Keep an unverified draft private until it passes the quality gate.

## Cybersecurity Publication Safety

For cybersecurity plans, these rules are mandatory:

- Practice only on labs, systems you own, or targets where you have explicit authorization.
- Follow the target's scope, disclosure policy, and the lab platform's writeup rules.
- Never publish an unresolved vulnerability from a live target.
- Redact credentials, tokens, cookies, personal data, private URLs, customer information, flags, and identifying program details.
- Do not publish exploit steps that violate a platform rule or create unnecessary risk.
- Clearly distinguish deliberately vulnerable labs from real applications.
- Coordinate disclosure before discussing an accepted real-world finding publicly.
- When public disclosure is not permitted, publish a generalized lesson that contains no target-identifying details.

## Web Exploitation Example Week

This is an example of applying the operating system, not a fixed curriculum.

```text
Weekly topic: IDOR and object-level authorization
Day 1: Map the normal object-access flow and outline an article around ownership checks.
Day 2: Solve guided access-control labs and capture sanitized Burp request comparisons.
Day 3: Repeat two-account testing without a solution and record failed hypotheses.
Day 4: Complete a harder authorized lab and write a mini vulnerability report.
Day 5: Draft the article using the flow map, lab evidence, mistakes, and checklist.
Day 6: Reproduce the steps, sanitize evidence, publish, and create LinkedIn/X versions.
Day 7: Review feedback, retest the weak point, update the tracker, and plan the next topic.
```

Suitable public artifacts for this domain include sanitized lab writeups, Burp workflow notes, testing checklists, deliberately vulnerable demo applications, responsible-disclosure retrospectives, and defensive explanations of root causes.

## Master Roadmap-To-Routine Prompt

Copy this prompt after creating the Plan Handoff in `LEARNING_SYSTEM_INDEX.md`.

````text
You are my learning-execution architect and Learn in Public editor. Convert my finalized roadmap into a realistic, dated routine that I can follow without deciding what to do next.

Do not redesign my roadmap unless it contains a direct contradiction, unsafe instruction, or workload that cannot fit the available time. Preserve its phase order, priorities, outcomes, and checkpoints.

FINALIZED PLAN HANDOFF
[PASTE THE COMPLETE COPY-PASTE PLAN HANDOFF FROM LEARNING_SYSTEM_INDEX.md]

EXECUTION INPUTS

Start date:
[YYYY-MM-DD]

End date or exact duration:
[YYYY-MM-DD or number of weeks/months]

Study schedule:
[Hours per study day, study days per week, unavailable days, and preferred rest/light day]

Target audience:
[Examples: beginners, peers, recruiters, clients, hiring managers, practitioners, or a specific community]

Canonical publishing platform:
[Choose one primary home, such as Hashnode, Medium, a personal website, or another platform]

Social distribution platforms:
[Examples: LinkedIn and X/Twitter. Add others only when they serve the target audience.]

Portfolio location:
[Examples: GitHub, personal website, Notion portfolio, or another public collection]

Privacy, disclosure, and platform restrictions:
[State confidentiality, employer, lab, competition, client, program, copyright, safety, or responsible-disclosure limits. Write "none known" only after checking.]

Preferred content language and format:
[Language, article length preference, text/video preference, screenshot availability, and accessibility needs]

CORE RULES

- Validate the requirements before creating the routine.
- The roadmap handoff, date range, study schedule, audience, canonical platform, distribution platforms, portfolio location, and publication restrictions are critical inputs.
- If a critical input is missing or contradictory, stop and ask only for that missing or conflicting information. Do not generate a partial routine.
- Use exact calendar dates. Include every date from the start date through the end date, including rest, recovery, and review days.
- Preserve the roadmap's phase order and prerequisite relationships.
- Use a conventional learning order and do not invent unnecessary topics.
- Writing is the primary public output: schedule one substantial, verified article per week unless the available schedule makes that objectively unrealistic.
- Use one canonical platform for the full article. Repurpose it into platform-specific LinkedIn and X/Twitter content rather than duplicating the complete article everywhere.
- Use approximately 70% of available time for learning/practice/projects, 20% for writing/editing, and 10% for publishing/distribution/feedback. Show the actual hours.
- Every major roadmap milestone must create a project, case study, report, demonstration, or portfolio artifact appropriate to the goal.
- Never use vague instructions such as "study X", "practice more", "work on the project", "write a post", or "review the topic" by themselves.
- Convert every action into a specific task with a time allowance, named output, and observable completion condition.
- Every study day must contain active practice. Content production must not replace skill development.
- Every public claim must be supported by reproducible work or a reliable source.
- Do not schedule publication before the required practical evidence exists.
- Do not optimize for impressions, followers, or daily posting streaks at the expense of skill or accuracy.
- If the requested workload is unrealistic, reduce scope or publication frequency explicitly. Do not compress impossible work into the calendar.
- If the complete calendar exceeds one response's output limit, divide it into consecutive labeled parts without changing the plan. State the exact final date covered and provide a continuation prompt containing all state needed to resume from the next date. Never silently omit or summarize the remaining dates.

WEEKLY LEARN IN PUBLIC CYCLE

Use this sequence unless the number of available study days requires carefully combining adjacent activities:

1. Learn and define the week's public outcome.
2. Perform guided practice and capture evidence.
3. Perform independent practice or build work.
4. Complete an applied challenge and validate the result.
5. Synthesize the learning and draft the flagship article.
6. Fact-check, edit, publish, add it to the portfolio, and repurpose it for social platforms.
7. Process feedback, update the progress tracker, and prepare the next week.

Required weekly article structure:

1. Specific title and learning question
2. Intended audience and prerequisites
3. Normal concept, system, or workflow
4. What I practiced, built, tested, or analyzed
5. Evidence and reproducible method
6. Mistakes, failed attempts, and corrections
7. Practical conclusions or reusable checklist
8. Limitations, safety, disclosure, or scope note when relevant
9. Next learning step

CYBERSECURITY SAFETY OVERRIDE

If the roadmap includes cybersecurity:

- Use only legal labs, owned systems, or explicitly authorized targets.
- Enforce scope, responsible-disclosure rules, and each platform's writeup policy.
- Never schedule publication of unresolved live-target vulnerabilities.
- Require redaction of credentials, tokens, cookies, personal data, flags, private URLs, customer information, and identifying private-program details.
- Clearly label labs and simulations.
- If disclosure is prohibited, replace the target-specific writeup with a generalized, non-identifying educational article.
- Treat these as hard constraints, not optional suggestions.

RETURN THE ROUTINE IN THIS EXACT STRUCTURE

1. Requirement Validation
- Reproduce the locked execution inputs in a compact table.
- Identify contradictions or unresolved critical information.
- If anything critical is unresolved, ask only the necessary questions and stop.

2. Timeline And Workload Verdict
- Answer whether the roadmap fits the dates and available hours: Yes / Partly / No.
- Calculate total available study hours.
- Convert the 70/20/10 allocation into actual weekly hours.
- State any scope or cadence correction required before scheduling.

3. Weekly Operating System
- Define each available day's role.
- Give a reusable timestamped schedule for every day type.
- Show where learning, practice, evidence capture, drafting, publication, distribution, feedback, rest, and review occur.
- Preserve at least one independent-practice block and one verification block every week.

4. Full Dated Execution Calendar
- Cover every calendar date from Day 1 through the final date.
- Organize the calendar by phase, month, and week.
- Use one concise row per date with these columns:

| Date | Day Number | Phase/Week | Day Type | Exact Actions And Time | Required Artifact | Pass/Fail Test |

- For an active day, name the exact topic or roadmap objective, practical activity, evidence to capture, and public-output contribution.
- For a rest or recovery day, label it explicitly and state whether any optional light action is allowed.
- Do not write "continue yesterday's work" without naming what remains and what completion means.
- Do not skip later months or replace them with a repeated generic week.

5. Weekly Article And Artifact Requirements
- For every week, specify:
  - article question or working title
  - intended audience
  - practical evidence required before drafting
  - article outline
  - milestone artifact, when applicable
  - drafting deadline
  - publication deadline
  - publication quality-gate checklist
  - pass/fail definition
- If the week cannot responsibly support a full article, schedule a smaller verified learning note and explain why. Do not publish filler.

6. Publication And Social Distribution Workflow
- Define the canonical-platform workflow from outline to publication.
- Create a reusable LinkedIn format containing a clear lesson, evidence, practical takeaway, and canonical link.
- Create a reusable X/Twitter post or thread format containing the strongest concise lessons and canonical link.
- Recommend no more than three distribution platforms unless I explicitly request more.
- Include fact-checking, proofreading, accessibility, link testing, evidence redaction, and disclosure review.
- Do not copy the full article into every platform.

7. Phase And Portfolio Milestones
- At the end of each roadmap phase, define one portfolio-quality artifact.
- Give its purpose, required components, due date, storage/publication location, and pass/fail standard.
- Show how the artifacts collectively demonstrate progress toward the final target outcome.

8. Public-Learning Metrics And Checkpoints
- Define weekly metrics for:
  - independent practical ability
  - completed exercises, labs, or project work
  - reproducible evidence
  - article accuracy and clarity
  - useful feedback received and applied
  - portfolio quality
- Treat views, likes, and follower growth as optional context, not proof of learning.
- Give pass/fail checkpoints at 25%, 50%, 75%, and 100% of the timeline.

9. Recovery And Adjustment Rules
- Give exact rules for a missed learning day, missed publication day, failed checkpoint, unfinished artifact, illness/low-energy day, and one-week backlog.
- Protect prerequisite learning and independent practice first.
- Never solve a missed week by deleting verification or publishing unverified work.
- State which low-priority tasks should be postponed first.
- Provide a minimum viable recovery week that preserves practice, one verified artifact, and review.

10. Daily And Topic Handoff Prompts
- Produce a ready-to-copy Daily Handoff for `DAILY_OFFENSIVE_TEMPLATE.md` containing the selected date, topic, current phase, available hours, exact practical task, evidence requirement, article contribution, dependencies, safety constraints, artifact, and pass/fail test.
- Produce a ready-to-copy Topic Handoff for `TOPIC_LEARNING_TEMPLATE.md` containing the topic, prerequisite knowledge, operational target, practice source, required exercises, evidence, public artifact contribution, time budget, and completion test.
- These handoffs must preserve this routine and must not ask the next prompt to redesign the roadmap.

Use this format for the Daily Handoff:

```text
I am executing a finalized learning and Learn in Public routine.

Date and day number:
Phase and week:
Today's topic/objective:
Available time:
Prerequisites already completed:
Exact practical task:
Evidence to capture:
Contribution to this week's article:
Required artifact:
Safety/privacy constraints:
Pass/fail test:

Use this context to generate the detailed daily session. Preserve the roadmap and do not add unrelated topics.
```

Use this format for the Topic Handoff:

```text
I am executing a finalized learning and Learn in Public routine.

Topic:
Current phase and week:
Why this topic is required now:
Prerequisite knowledge:
Operational skill target:
Available time:
Practice source and exercises:
Evidence to capture:
Contribution to the public artifact:
Safety/privacy constraints:
Completion test:

Use this context to generate the topic-learning session. Preserve the roadmap, time budget, and required artifact.
```

11. Assumptions
- List every assumption used to schedule the routine.
- Mark each as low-risk or high-risk.
- Do not hide missing critical information as an assumption.

12. Quality Audit
- Score the routine out of 100 for:
  - complete date coverage
  - action specificity
  - workload realism
  - practical exposure
  - Learn in Public integration
  - artifact measurability
  - publication quality and safety
  - alignment with the finalized roadmap
- Every score must be at least 90.
- Verify that every active date has a specific action, artifact, time allowance, and pass/fail test.
- Verify that every week contains practical work, evidence collection, writing, verification, publication or a justified private draft, distribution, and review.
- If any score is below 90 or any date/week fails validation, revise the routine before showing it.
- Show only the corrected final routine.

FINAL STANDARD

The output must function like a workout program: on any date, I can open the calendar and immediately know what to do, for how long, what evidence to preserve, what I am producing publicly, and how to decide whether the day passed or failed.
````

## Recovery Principle

The calendar is a control system, not a punishment system. When reality interrupts the schedule, preserve prerequisite learning, independent practice, verification, and honest review. Reduce optional distribution and low-priority breadth before reducing the work that creates genuine skill.
