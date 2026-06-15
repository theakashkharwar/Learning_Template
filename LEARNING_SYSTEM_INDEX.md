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

## Goal Mapping Prompt

```text
You are my practical learning-system architect. Create a clear, realistic, high-precision learning map for [DOMAIN/SKILL] over [TIME PERIOD: 2 months / 3 months / 6 months / custom].

Your job is not to motivate me or give a broad syllabus. Your job is to design a practical roadmap that a serious learner can follow and measure.

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

Create a high-level learning map only. Do not create a detailed daily routine yet.

Rules:
- Be brutally realistic about what can and cannot be achieved in the timeline.
- Prioritize usable skill over theory consumption.
- Prefer fewer topics with practice over many topics with shallow coverage.
- Every phase must include practical outputs, not just topics to study.
- Every milestone must be testable.
- Do not include vague advice like "learn basics", "practice more", or "do projects" unless you define exactly what that means.
- If the timeline is unrealistic, correct it and explain what can still be achieved.
- Separate core topics, useful-but-secondary topics, and delayed topics.
- Include self-assessment checkpoints so I can prove progress without a mentor.

Return the answer in this exact structure:

1. Verdict On Timeline
- Is the timeline realistic for the target outcome? Answer: Yes / Partly / No.
- What level is realistically achievable by the end?
- What level is not realistic yet?

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
  - milestone to pass before moving on

3. Topic Priority
- Core: must learn for the goal.
- Useful: learn if time remains or after core confidence.
- Delay: avoid for now because ROI is low or prerequisites are missing.

4. Practical Output Requirements
- List the exact artifacts I should create during the plan.
- Examples: reports, checklists, solved labs, projects, case studies, notes, portfolio pieces, workflows, mock tests.

5. Self-Testing System
- Give measurable checkpoints for 25%, 50%, 75%, and 100% completion.
- Each checkpoint must answer: "What should I be able to do without help?"

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

8. Quality Score
- Score your own plan out of 100 for:
  - practicality
  - specificity
  - timeline realism
  - beginner suitability
  - measurability
  - alignment with my target outcome
- If any score is below 90, revise the plan before finalizing.

Keep the final answer practical, comparable, and decision-ready. It should produce a plan that two different AIs would make similarly because the structure, criteria, and output format are tightly defined.
```
