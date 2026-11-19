# IELTS Writing Band 8 Personal Coach System

An elite, persistent, and structured training system designed to coach IELTS candidates to achieve **Band 8** in Writing (Academic & General Training).

Developed using official IELTS public band descriptors, cognitive mental models, active recall, spaced repetition, and an intuitive Hinglish bridge for non-native English speakers.

---

## Directory Architecture

```
IELTS-Writing-Coach/
│
├── AGENTS.md                  # Core operating system prompt & persistent memory rules
├── README.md                  # System overview and quick-start guide
│
├── .agent/
│   └── skills/                # Reusable Antigravity agent skills
│       ├── ielts-writing-coach/SKILL.md    # Master curriculum & session conductor
│       ├── essay-evaluation/SKILL.md       # 4-criteria strict examiner scoring engine
│       ├── grammar-training/SKILL.md       # Band 8 grammar structures & diagnostic drills
│       ├── vocabulary-training/SKILL.md    # Collocation-first IELTS lexical acquisition
│       ├── mental-models/SKILL.md          # Cognitive frameworks & rule-of-thumb library
│       └── progress-tracking/SKILL.md      # Dynamic learner profiling & memory tracking
│
├── docs/                      # Core references & curriculum documentation
│   ├── IELTS_SYLLABUS.md               # 7-phase structured path to Band 8
│   ├── IELTS_ASSESSMENT_CRITERIA.md    # Official Band 7, 8, 9 descriptors analyzed
│   ├── LEARNING_METHODOLOGY.md         # 8-step daily session flow & hint progression
│   ├── MY_WRITING_MENTAL_MODELS.md     # Personal mental model repository
│   ├── GRAMMAR_REFERENCE.md            # Advanced grammar rules, formulas & Hinglish triggers
│   ├── VOCABULARY_BANK.md              # Topic-specific collocations and lexical sets
│   ├── COMMON_MISTAKES.md              # Diagnostic catalog of frequent non-native traps
│   └── BAND_8_CHECKLIST.md             # 15-point pre-submission test
│
├── progress/                  # Persistent learner state (Source of Truth)
│   ├── STUDENT_PROFILE.md      # Target, exam track, timeline, learning style
│   ├── PROGRESS_DASHBOARD.md   # Current estimated bands, metrics, and progress logs
│   ├── SKILL_MASTERY.md        # Fine-grained checklist of grammatical & writing skills
│   ├── SESSION_HISTORY.md      # Chronological log of coaching sessions
│   ├── ESSAY_HISTORY.md        # Archive of submitted tasks, examiner tables, scores
│   ├── WEAKNESS_TRACKER.md     # Recurring error monitor (occurrences, severity, status)
│   └── REVISION_QUEUE.md       # Spaced repetition queue for active recall
│
├── practice/                  # Active candidate workspace
│   ├── task-1/                 # Task 1 writing tasks and drafts
│   ├── task-2/                 # Task 2 essays, blueprints, and revisions
│   ├── grammar/                # Sentence transformation & grammar drills
│   └── vocabulary/             # Collocation exercises and active recall quizzes
│
└── resources/                 # Benchmark essays & comparative analyses
    ├── BAND_7_EXAMPLES.md     # Competent essays with breakdown of Band 7 ceilings
    ├── BAND_8_EXAMPLES.md     # Band 8 essays with line-by-line examiner commentary
    └── BAND_9_EXAMPLES.md     # Band 9 mastery benchmarks demonstrating effortless control
```

---

## Key Features

1. **True Examiner Evaluation**: Strict, uninflated scoring based on official public band descriptors.
2. **Mental Models Over Templates**: Formulations like **C → R → E → I** (Claim, Reason, Explanation, Impact) ensure logical depth without robotic templates.
3. **Strategic Hinglish Pedagogical Bridge**: Complex grammatical subtleties (e.g. concessive clauses, articles, tense shifts) explained via intuitive Hindi/Hinglish analogies before transitioning to pure English thought.
4. **Active Learning Hint System**: Instead of spoon-feeding answers, 4 progressive levels of hints empower students to identify and correct their own errors.
5. **Persistent Memory**: The coach tracks every recurring mistake, maintaining a live spaced-repetition queue across all sessions.
