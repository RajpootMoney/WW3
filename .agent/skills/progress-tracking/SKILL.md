---
name: progress-tracking
description: >-
  State management engine for the IELTS Band 8 coaching system. Maintains persistent records,
  tracks verified criteria scores, manages the weakness tracker, and schedules spaced-repetition revision queues.
---

# IELTS Progress Tracking Skill: Persistent Memory Protocol

## 1. Operating Rules
- **Evidence-Based Only**: Never increment a skill mastery rating or award a band estimate without citing concrete student text from a completed exercise or essay.
- **Continuous Synchronization**: At the end of every instructional interaction, synchronize all state files in `progress/`.
- **Pre-Session Initialization**: Always load `progress/STUDENT_PROFILE.md`, `progress/PROGRESS_DASHBOARD.md`, `progress/WEAKNESS_TRACKER.md`, and `progress/REVISION_QUEUE.md` before initiating or continuing a session.

## 2. File Responsibilities and Schema

### 1. `progress/STUDENT_PROFILE.md`
Maintains core identity and parameters:
- Student Name / Handle
- IELTS Module: Academic or General Training
- Examination Date & Target Timeline
- Target Band: Band 8.0
- Baseline Writing Band & Diagnostic Notes
- Preferred Learning Nuances (e.g., Hinglish explanations, mental models)

### 2. `progress/PROGRESS_DASHBOARD.md`
Top-level diagnostic cockpit:
- Current Estimated Band (TR, CC, LR, GRA, Overall)
- Baseline Comparison
- Number of Essays Completed
- Number of Coaching Sessions Completed
- High-Priority Recurring Weaknesses
- Recent Breakthroughs / Improvements
- Active Next Priorities

### 3. `progress/SKILL_MASTERY.md`
Granular mastery matrix across 4 criteria:
- Status indicators: `Not Started` | `In Progress` | `Demonstrated` | `Mastered (Consistent in Timed Writing)`
- Sub-categories:
  - Task Response: Question deconstruction, C-R-E-I depth, counter-argumentation.
  - Coherence & Cohesion: Paragraph progression, referential cohesion, topic sentences.
  - Lexical Resource: Academic precision, collocation sets, topic clusters, anti-repetition.
  - Grammatical Range & Accuracy: Subordinate clauses, conditionals, participles, passive voice, punctuation.

### 4. `progress/SESSION_HISTORY.md`
Session-by-session chronological ledger:
- Date & Timestamp
- Session Index
- Topics / Concepts Covered
- Mental Models Applied
- Drills Completed & Results
- Feedback & Assigned Next Actions

### 5. `progress/ESSAY_HISTORY.md`
Archive of complete essay evaluations:
- Submission Date
- Prompt & Task Type (Academic/GT, Task 1/Task 2)
- Word Count & Time Taken
- Criterion Bands: TR/TA, CC, LR, GRA, Overall
- Top 3 Actionable Priorities

### 6. `progress/WEAKNESS_TRACKER.md`
Quantitative error ledger:
- Error / Weakness Description
- Total Verified Occurrences
- Severity Level (`Low` | `Medium` | `High` | `Critical`)
- Status (`Identified` | `In Progress` | `Improving` | `Resolved`)
- Governing Rule / Mental Model Hook

### 7. `progress/REVISION_QUEUE.md`
Spaced-repetition scheduling queue:
- **Interval 1**: Next immediate session.
- **Interval 2**: 2–3 sessions later.
- **Interval 3**: Approximately 1 week later.
- **Interval 4**: Approximately 2 weeks later.
- Automatically promotes items upon successful active recall or demotes upon failure.
