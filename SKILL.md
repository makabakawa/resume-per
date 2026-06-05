---
name: resume-per
description: Create or revise resumes for job applications with a disciplined one-page workflow, job-targeted content pruning, bilingual handling, project rewriting, and final PDF delivery. Use when Codex needs to turn an existing resume into a cleaner, stronger, more targeted version for a specific role, format, or hiring context.
---

# Resume Per

## Overview

Build resumes with a fixed process: extract the source content, identify the target job direction, cut weak or redundant material, rewrite high-value sections, lock the layout to one page where required, and deliver a final PDF.

Prioritize hiring value over literal preservation. Keep evidence, metrics, technical actions, and role fit. Remove weak filler, duplicated information, and ornamental explanations.

## Workflow

### 1. Read the source resume

- Extract the current content from the provided resume source.
- Check whether the source is Chinese-only, English-only, or bilingual.
- Identify the actual sections present: header, target role, summary, education, skills, projects, internships, awards, certificates, links.
- Record hard facts that must not drift:
  - name
  - phone
  - email
  - school
  - degree
  - dates
  - cities
  - scores or metrics

Never rewrite factual details speculatively. If a detail looks corrupted by parsing, verify it from the clearest source before reusing it.

### 2. Determine the job target

- Infer or ask for the target direction only when necessary.
- Rewrite the resume for one concrete target, not for all possible jobs.
- If the user is targeting AI, algorithm, computer vision, LLM application, or similar roles:
  - surface model, data, deployment, and measurable results early
  - reduce generic school-style wording
  - prefer evidence of implementation over course-like descriptions

### 3. Prune content aggressively

Apply these deletion rules by default:

- Delete duplicated English/Chinese information unless the user explicitly wants both.
- Delete weak statements such as "familiar with only at a surface level", "light exposure only", "open to any opportunity", or generic self-praise unless they are converted into concrete capability statements.
- Delete low-information sections that consume layout space without helping screening.
- Delete decorative notes explaining the template, workflow, or formatting logic.
- Delete metrics that weaken the project unless they are necessary for honesty or context.

Keep only what improves screening probability for the target role.

### 4. Rewrite the high-value sections

#### Header

- Use a compact, role-oriented header.
- Prefer:
  - name
  - school and degree status
  - target role
  - graduation year when relevant
  - phone, email, city, English score if useful

Do not waste top space on age, gender, or vague labels unless the user explicitly wants them.

#### Summary / Profile

- Keep to 1-2 short sentences.
- State:
  - current status
  - technical focus
  - strongest practical value

Bad summary style:
- broad claims
- personality claims
- empty ambition

Good summary style:
- domain + workflow ownership + project depth

#### Skills

Group skills into 2-4 buckets only. Typical buckets:

- programming / engineering
- deep learning / vision
- LLM / AI applications
- tools / deployment

Rules:

- List tools the candidate can plausibly defend in interview.
- Rephrase weak API-only claims into workflow capability when justified by project evidence.
- Keep wording tight and concrete.

#### Projects

Projects are the core evidence section. Rewrite each project to show:

1. what problem or task was handled
2. what technical method was used
3. what the candidate actually implemented
4. what result or metric was achieved

Preferred project pattern:

- project title
- context / role label
- 2-3 bullets only

Each bullet should trend toward:

- technical action + method + result

Avoid:

- long narrative paragraphs
- method dumping without outcome
- outcome dumping without implementation detail

If bilingual output is required:

- write the Chinese first
- translate for hiring clarity, not word-for-word symmetry
- keep English concise, natural, and readable by recruiters
- preserve technical meaning exactly

### 5. Handle bilingual resumes correctly

If the user wants Chinese and English paired:

- put the Chinese statement first
- place the English directly below the corresponding Chinese statement
- make the English shorter than the Chinese when possible
- remove Chinese-specific rhetorical structure from the English

Translation rules for project bullets:

- keep technical nouns accurate
- keep metrics exact
- use natural resume verbs:
  - built
  - developed
  - implemented
  - designed
  - collected
  - deployed
  - achieved
- avoid inflated or academic-sounding English if a simpler version is clearer

Do not translate literally if literal phrasing sounds machine-generated.

### 6. Enforce one-page layout

If the user requires one page:

- enforce one page as a hard constraint
- reduce section count before shrinking fonts excessively
- shorten summaries before cutting project evidence
- merge low-value sections into nearby sections
- keep projects as the priority content block

Recommended compression order:

1. delete notes / decorative text
2. compress summary
3. compress skills
4. remove low-value sections
5. tighten project bullets
6. adjust spacing and font sizes

Do not produce a crowded page that looks unreadable just to satisfy one-page formatting.

### 7. Use template style pragmatically

When asked to follow a platform style such as Liepin:

- replicate the layout logic, visual hierarchy, and section rhythm
- do not copy branded marketing text into the resume
- keep the resume content independent from the template source

Use template inspiration for:

- left/right layout structure
- title hierarchy
- spacing rhythm
- visual emphasis

Not for:

- explanatory footer text
- template notes
- platform copy

### 8. Deliverable rules

- Output the final resume as PDF when the user asks for PDF.
- If an editable source is created, keep it as a working artifact but treat the PDF as the deliverable.
- Save the final artifact to the exact path the user requested.
- If overwriting an existing file, preserve the filename exactly unless the user asks for a new one.

### 9. Final validation

Before delivery, verify:

- page count matches the requirement
- phone and email are correct
- job target is visible near the top
- major projects contain concrete methods and metrics
- no stray template notes remain
- Chinese and English, if present, correspond correctly
- no obvious machine-translation phrasing remains

## Output standard

The finished resume should be:

- targeted
- concise
- technically defensible
- visually orderly
- easy to screen in under 30 seconds

If tradeoffs are required, prefer screening strength over completeness.
