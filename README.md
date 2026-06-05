# resume-per

`resume-per` is a Codex skill for practical resume rewriting.

It is built for cases where an existing resume needs to become more targeted, shorter, cleaner, and easier for recruiters or interviewers to screen quickly. The workflow is optimized for technical roles such as AI algorithms, computer vision, LLM applications, and related internships.

## What it does

- rebuilds an existing resume for a concrete target role
- compresses content into a strong one-page version when required
- rewrites project bullets around methods, actions, and measurable results
- supports Chinese, English, or bilingual resumes
- preserves factual details while removing weak or redundant content
- delivers a final PDF-oriented output standard

## Suitable scenarios

- technical internship resume revision
- algorithm / computer vision / AI resume targeting
- bilingual resume preparation for foreign companies
- converting a content-heavy academic resume into a recruiter-friendly version
- rebuilding a resume with platform-inspired layout logic without copying template filler

## Repository structure

```text
.
├── SKILL.md
└── agents/
    └── openai.yaml
```

## Install

Copy this repository into your Codex skills directory as:

```text
$CODEX_HOME/skills/resume-per
```

Typical Windows path:

```text
C:\Users\<your-user>\.codex\skills\resume-per
```

## Invoke

Example prompts:

```text
Use $resume-per to rewrite this resume into a one-page computer-vision internship version.
```

```text
使用 $resume-per，把这份简历改成一页内、面向算法岗的版本，并输出 PDF。
```

The skill also supports implicit invocation for clear resume-rewrite requests.

## Design standard

This skill is intentionally narrow and execution-oriented:

- no generic career coaching
- no decorative template explanation
- no unverifiable self-praise
- no literal but awkward bilingual translation

The target output is simple: concise, defensible, job-targeted, and ready for fast screening.
