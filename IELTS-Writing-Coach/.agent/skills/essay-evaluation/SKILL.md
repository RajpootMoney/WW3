---
name: essay-evaluation
description: >-
  Executes rigorous, uninflated IELTS Writing Task 1 and Task 2 evaluations based strictly on official
  examiner band descriptors across TR/TA, CC, LR, and GRA. Generates structured error tables, argument diagnostics, and Band 8 rewrites preserving candidate ideas.
---

# IELTS Essay Evaluation Skill: Official Examiner Protocol

## 1. Operating Principles
- **No Score Inflation**: Evaluate candidates against authentic IELTS Band 8 standards. Band 8 requires sustained fluency, natural lexical precision, sophisticated grammatical control, and fully developed logical argumentation.
- **Evidence-Based Scoring**: Every score must cite specific quotes from the candidate's essay.
- **Preserve Candidate Voice**: When providing improved Band 8 rewrites, upgrade the candidate's original arguments, examples, and line of thought rather than substituting an alien canned response.

## 2. Evaluation Output Template

Whenever an essay is submitted, output feedback in this exact sequence:

### A. Estimated IELTS Score
> **Notice**: *This is an educational assessment based on official public IELTS band descriptors, not an official test certificate.*

| Criterion | Estimated Band | Key Examiner Justification |
| :--- | :--- | :--- |
| **Task Response / Task Achievement** | `X.X` | *Brief summary of coverage, stance, and depth of arguments.* |
| **Coherence and Cohesion** | `X.X` | *Paragraph progression, topic sentences, referential cohesion.* |
| **Lexical Resource** | `X.X` | *Precision, collocations, absence of forced/inaccurate synonyms.* |
| **Grammatical Range & Accuracy** | `X.X` | *Complex structures, clause variety, error frequency.* |
| **OVERALL ESTIMATED BAND** | `X.X` | *(Calculated per official IELTS rounding rules)* |

---

### B. Detailed Criterion Assessment
1. **Task Response / Achievement**:
   - Did the candidate fully address all parts of the prompt?
   - Is there a clear, sustained position throughout?
   - Are main ideas adequately developed, or are they merely listed/unsupported?
2. **Coherence and Cohesion**:
   - Is there a logical progression of ideas across and within paragraphs?
   - Are topic sentences clear and followed by explanations?
   - Are linking devices natural, or are they mechanical, repetitive, or overused?
   - How effective is referential cohesion (pronouns, substitution)?
3. **Lexical Resource**:
   - Range and flexibility: Are collocations natural and topic-appropriate?
   - Precision: Were words chosen for accuracy rather than fake sophistication?
   - Minor slips vs frequent word-choice errors.
4. **Grammatical Range and Accuracy**:
   - Variety of complex sentences (relative clauses, conditionals, concessions, participle phrases).
   - Frequency of error-free sentences (Band 8 requires a majority of error-free sentences).
   - Punctuation accuracy (comma splices, run-ons, semicolons).

---

### C. Error Analysis Table
Extract specific sentences containing flaws and present them in this diagnostic table:

| # | Original Sentence | Problem Type | Improved Band 8 Version | Deep Explanation & Rule |
| :- | :--- | :--- | :--- | :--- |
| 1 | *"...sentence from essay..."* | Grammar / Lexis / Cohesion | *"Upgraded version..."* | *Why the error happened and how to avoid it.* |

---

### D. Argument Quality & Cognitive Depth
- **Relevance**: Did any points drift off-topic?
- **Depth (The C-R-E-I Test)**: Did the candidate progress through Claim → Reason → Explanation → Impact, or stop at general assertions?
- **Examples**: Were examples illustrative and logically integrated, or generic and artificial?

---

### E. Band 8 Rewrite (Preserving Student's Ideas)
Present a complete rewritten version of the candidate's essay that elevates vocabulary, coherence, and grammatical maturity while strictly preserving the student's authentic ideas and argumentative trajectory.

---

### F. Top Three Priorities for Next Essay
1. **Priority 1 (Highest Impact)**: e.g., Eliminating comma splices in compound-complex sentences.
2. **Priority 2**: e.g., Developing the second body paragraph with an explanatory mechanism.
3. **Priority 3**: e.g., Replacing mechanical transition words (*"Furthermore"*, *"Moreover"*) with referential transitions.

---

## 3. Persistent Logging
Following every evaluation:
- Append the essay metrics to `progress/ESSAY_HISTORY.md`.
- Update recurring mistakes in `progress/WEAKNESS_TRACKER.md`.
- Log the date and key priorities in `progress/SESSION_HISTORY.md`.
- Update overall band trends in `progress/PROGRESS_DASHBOARD.md`.
