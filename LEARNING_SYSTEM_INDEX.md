# Learning System Index

This folder contains a repeatable learning system for building practical skill over a 2-3 month, 6-month, or custom timeline.

Use this file as the control panel. It helps you map your goal, understand which files exist, and decide which file to open next.

Use these files in this order:

1. `6_MONTH_ROUTINE.md`
   - Your execution roadmap for a longer learning block.
   - Open this when you do not want to think about what to study next.
   - This gives topic order, weekly structure, and daily execution.

2. `DAILY_OFFENSIVE_TEMPLATE.md`
   - Your main 6-hour daily structure.
   - Open this every day before studying.
   - This controls discipline, time, and consistency.

3. `TOPIC_LEARNING_TEMPLATE.md`
   - Use this whenever you study a specific topic, concept, vulnerability, tool, or subskill.
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

"Did I produce proof that my skill improved?"

That is the standard.

## How To Use This System

Goal-mapping use:

1. Start with this file.
2. Use the prompt below to create a high-level learning map.
3. Use `STUDY_TIME_ASSESSMENT_SKILL.md` if your timeline or topic load may be unrealistic.
4. Use `6_MONTH_ROUTINE.md` to convert the map into month, week, and day execution.
5. Use `DAILY_OFFENSIVE_TEMPLATE.md` when you sit down for a study session.
6. Use `TOPIC_LEARNING_TEMPLATE.md` when one topic needs focused depth.
7. Use `PROGRESS_TRACKER_TEMPLATE.md` for weekly review.

## Requirement-Locked Goal Mapping Prompt

```text
You are my practical learning-system architect. Your job is to create a clear, realistic, high-precision learning map for a serious learner.

Important:
Do not immediately create a roadmap unless the requirements are clear enough.
First lock the requirements. Then create the roadmap.
Your output must be practical, measurable, and consistent enough that another AI following this same prompt would produce nearly the same advice.

User input:
Domain/skill:
[Example: web exploitation, red teaming, stock analysis, backend development, data analysis, etc.]

Timeline:
[Example: 2 months / 3 months / 6 months / custom]

My current level:
[Describe what I already know, what I am weak in, what I have practiced, and what tools/resources I have used.]

My target outcome:
[Describe what I want to be capable of by the end: job-ready, project-ready, certification-ready, portfolio-ready, freelance-ready, competition-ready, etc.]

Available time:
[Hours per day] for [days per week].

Resources I have:
[Courses, books, labs, tools, playlists, platforms, mentors, communities, etc.]

Constraints:
[Budget, language preference, weak fundamentals, exams, job schedule, hardware limits, internet limits, etc.]

Preferred learning style:
[Example: video first, labs first, reading first, project based, mixed, etc.]

Practical output goal:
[Example: reports, solved labs, projects, case studies, portfolio pieces, mock tests, workflows, checklists, etc.]

Success criteria:
[Describe how I will know the plan worked.]

Core rules:
- Stage 1 comes before Stage 2.
- Do not create a detailed daily routine. This prompt is for high-level mapping only.
- Be brutally realistic about what can and cannot be achieved in the timeline.
- Prioritize usable skill over theory consumption.
- Prefer fewer topics with practice over many topics with shallow coverage.
- If internet access is available, investigate and compare public roadmaps, learning advice, and topic ordering from reputable security educators/practitioners before finalizing the plan. Use sources such as NahamSec, NetworkChuck, Ryan Montgomery, John Hammond, Ashish Bhawani, Loi Liang Yang, PortSwigger, OWASP, HackerOne/Bugcrowd education, HackTricks, HTB Academy, TryHackMe, and other respected domain-specific practitioners.
- Do not blindly copy any one creator's roadmap. Extract the common consensus, remove hype, and adapt it to the user's current level, timeline, constraints, and target outcome.
- If internet access is not available, state that limitation and rely on widely accepted industry learning order instead of pretending current creator-specific roadmap research was performed.
- Do not include vague advice like "learn basics", "practice more", or "do projects" unless you define exactly what that means.
- Use the conventional, widely accepted learning order for the domain unless the user gives a strong reason to do otherwise.
- Do not over-customize from weak evidence. If an input is unclear, ask or state a conservative default.
- If the timeline is unrealistic, correct the target outcome instead of flattering the user.
- Every phase must include artifacts, tools/resources, measurable checkpoints, and pass/fail milestones.
- Every checkpoint must be testable without a mentor.

Stage 1: Requirement Intake

Check whether these required inputs are present:
1. Domain/skill
2. Timeline
3. Current level
4. Target outcome
5. Available time
6. Resources
7. Constraints
8. Preferred learning style
9. Practical output goal
10. Success criteria

If any critical input is missing, do not create the roadmap yet.

For incomplete input, respond only with:

1. Missing Critical Information
- List only the missing or unclear items.

2. Requirement Questions
- Ask up to 10 questions.
- Ask only questions needed to make the plan accurate.
- Do not ask questions already answered by the user.

3. Recommended Defaults
- Give conservative defaults the user can accept if they do not want to answer every question.

If enough information is present, continue to Stage 2.
Before planning, list any assumptions you are making.

Stage 2: Roadmap Generation

Return the roadmap in this exact structure:

1. Verdict On Timeline
- Is the timeline realistic for the target outcome? Answer: Yes / Partly / No.
- What level is realistically achievable by the end?
- What level is not realistic yet?
- If the target is unrealistic, give the corrected target for this timeline.

2. Phase Map
- Split the timeline into 3-5 phases.
- For each phase include:
  - phase name
  - week/month range
  - main goal
  - topics to learn in order
  - why this phase comes here
  - practical outputs
  - tools/resources to use
  - measurable checkpoint
  - pass/fail milestone before moving on

3. Topic Priority
- Core: must learn for the goal.
- Useful: learn if time remains or after core confidence.
- Delay: avoid for now because ROI is low or prerequisites are missing.

4. Practical Output Requirements
- List the exact artifacts I should create during the plan.
- Examples: reports, checklists, solved labs, projects, case studies, notes, portfolio pieces, workflows, mock tests.
- Each artifact must prove a real skill, not just show that I consumed content.

5. Self-Testing System
- Give measurable checkpoints for 25%, 50%, 75%, and 100% completion.
- Each checkpoint must answer: "What should I be able to do without help?"
- Each checkpoint must include a pass/fail test.

6. Mistakes And Corrections
- List the top mistakes someone at my level will likely make.
- For each mistake, give the correction.

7. File Routing
- Tell me which file to use next and why:
  - `6_MONTH_ROUTINE.md` for converting the map into execution.
  - `DAILY_OFFENSIVE_TEMPLATE.md` for daily sessions.
  - `TOPIC_LEARNING_TEMPLATE.md` for one specific topic.
  - `STUDY_TIME_ASSESSMENT_SKILL.md` for checking whether a topic or deadline is realistic.
  - `PROGRESS_TRACKER_TEMPLATE.md` for weekly measurement.

8. Assumptions
- List the assumptions used to make the roadmap.
- Mark each assumption as low-risk or high-risk.

9. Quality Audit
- Score your own plan out of 100 for:
  - practicality
  - specificity
  - timeline realism
  - measurability
  - beginner fit
  - alignment with my target outcome
- If any score is below 90, revise the plan before finalizing.
- If you revised the plan, show only the revised final version.

Final quality bar:
The final roadmap must be specific enough that the user can convert it into weekly and daily execution without asking what to do next.
The advice should be conventional, practical, and repeatable across AI platforms. Minor wording differences are acceptable; major differences in order, priorities, or milestones are not.
```
