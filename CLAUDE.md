# Italian A1 → B2 Wiki — Schema

## Purpose
This wiki supports structured self-study of **Italian from A1 to B2 (CEFR)**. The LLM acts as a tutor. The learner provides source files and directs sessions. Explanations are always given in **English + Arabic**.

## Directory Structure
```
linuga_it/
├── CLAUDE.md                     ← this schema file
├── raw/                          ← immutable sources (never edit)
│   ├── course_tracker.md         ← per-page status / review tracking
│   └── sources/                  ← original study-guide files (.md)
│       ├── Italian_A1_Complete.md … Italian_B2_Complete.md
│       └── Italian_Master_A1-B2.md   ← same content as the 4 level files merged (newer numbering); used as the split source
└── wiki/                         ← LLM-maintained knowledge base
    ├── index.md                  ← full catalog of all wiki pages
    ├── log.md                    ← append-only activity log
    ├── overview.md               ← learner status, roadmap, weak areas
    ├── a1/  a2/  b1/  b2/        ← topic pages, one folder per CEFR level — never mix levels
    └── quizzes/{a1,a2,b1,b2}/    ← one subfolder per level — never mix
```

## Page IDs and file names
File name = `<ID> - <Title>.md` (ID first so files sort; `:` and `/` in titles become ` -`). Link with the full file name: `[[A2-G02 - Passato Prossimo]]`.

| Code | Type | Contains |
|------|------|----------|
| `Lv-Gnn` | grammar | one grammar topic: rules, tables, examples |
| `Lv-Vnn` | vocabulary | vocabulary lists (IT / EN / AR), sentence banks |
| `Lv-Snn` | speaking | daily speaking models, dialogues, slang, role-plays, oral-exam prep |
| `Lv-Pnn` | practice | exercises with answer keys, checkpoints |
| `Lv-Rnn` | revision | one-page revision sheet, common mistakes, CEFR can-do lists |
| `Lv-Qnn` | quiz | generated quizzes (in `wiki/quizzes/<level>/`) |

`Lv` = A1, A2, B1, B2.

### Page frontmatter
```yaml
---
id: A2-G02
aliases: [A2-G02]
title: "Passato Prossimo"
level: A2
type: grammar | vocabulary | speaking | practice | revision | quiz
sources: ["A2 Part 4 · 4.2", …]   # sections of Italian_Master_A1-B2.md this page came from
status: Not Reviewed | In Progress | Solid | Needs Review
last_reviewed: YYYY-MM-DD
weak_areas: []
tags: [a2, grammar, passato-prossimo]
---
```
Grammar pages open with two callouts, `> [!tip] Quick explanation (English)` and `> [!note] شرح سريع (عربي)`, followed by the source sections. Every section carries a `<!-- src: … -->` comment. Sections that came from a different level's file are tagged `*(moved here from Xn file)*`.

## Level placement rules (used for the re-sort)
Place content at the CEFR level where it is **first taught**, not the file it arrived in:
- **A1:** present tense (regular + core irregulars), essere/avere, articles, gender/plural, adjectives, possessives, prepositions, piacere, negation, numbers/time, reflexives, basic imperative, pronunciation.
- **A2:** passato prossimo, imperfetto, futuro semplice, condizionale presente, stare + gerundio, object pronouns, ne/ci, -mente adverbs, comparatives.
- **B1:** congiuntivo presente/imperfetto/trapassato, periodo ipotetico, compound tenses, relatives, passive / si passivante, implicit clauses, full imperative, reported speech.
- **B2:** sequence of tenses, advanced subjunctive use, combined pronouns, register, discourse markers, passato remoto (recognition).
- Mixed-level material (e.g. a CEFR roadmap covering A0 → B1) is split so each part sits on its own level's page.

## Workflows

### Ingest a new source
1. Drop the file into `raw/sources/`.
2. Say: `ingest <file>`.
3. The LLM reads it, sorts each section by the placement rules above, merges it into an existing topic page or creates a new one, adds the bilingual box if missing, then updates `index.md` and `raw/course_tracker.md` and appends to `log.md`.

### Review (the learner is A2 and forgets A1 basics)
Say: `review <topic or ID>`. The LLM gives a short refresher (EN + AR), then 5–8 quick questions. It updates `status`, `last_reviewed` and `weak_areas` on the page.

### Quiz me
Say: `quiz me on <topic/level>`. The LLM writes scenario-style questions (fill-in, transformation, translation EN/AR → IT) and saves the quiz to `wiki/quizzes/<level>/<Lv>-Qnn - <Title>.md` with an answer key. It grades the answers and records weak areas on the topic pages.

### Query
Ask anything. The LLM reads `index.md` first, then the relevant pages. A good synthesis gets filed as a new page.

### Lint
Say: `lint the wiki`. The LLM checks for misplaced-level content, broken `[[links]]`, grammar pages missing the EN/AR boxes, stale weak areas and duplicate topics across levels, then suggests what to review next.

## Learner Profile
**Name:** Taha
- **Current level:** A2. Sat the A2 exam on 12 June 2026 (L'Aquila). Now moving toward B1.
- **Native language:** Arabic. Strong English.
- **Lives and works in Italy.** Real-world, workplace and bureaucracy examples are relevant.
- **Known gap:** forgets A1 basics at times (articles, prepositions, irregular presents). Mix quick A1 recall into A2/B1 work.

**Calibration:**
- Every explanation is in **English + Arabic**: English first, then an Arabic version (`بالعربية:` or the `شرح سريع` callout).
- Keep Italian examples in Italian with an EN translation and, where helpful, an AR one.
- Flag the "Mistakes Arabic speakers make" patterns: dropped essere, gender/article agreement, prepositions, false friends.

## Teaching Structure (per session)
1. Quick explanation (EN)
2. شرح سريع (AR)
3. Forms / table
4. Examples (IT → EN / AR)
5. Common mistakes
6. Practice (5–8 items)
7. Answer key + recap

## Log Format
Each entry: `## [YYYY-MM-DD] action | description`
