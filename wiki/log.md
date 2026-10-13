# Activity Log
<!-- Format: ## [YYYY-MM-DD] action | description -->

## [2026-10-10] create | Wiki built from 5 source files, content re-sorted by CEFR level

Sources: Italian_A1/A2/B1/B2_Complete.md plus Italian_Master_A1-B2.md (the same content as the four level files merged, with newer section numbering). All five moved to raw/sources/. The master file was split into 85 topic pages (A1 24, A2 21, B1 21, B2 19). A line-count check confirmed nothing was lost or duplicated (4,212 content lines in and out).

Re-sort (content that was filed under the wrong level):

- A2 "A1 Foundations" (subject pronouns, essere/avere, articles, regular endings, numbers, adjectives) → A1 pages G01–G05, G10
- A2 full presente conjugation tables → A1-G01
- A2 articulated prepositions → A1-G08
- A2 CEFR roadmap split by level: A0 + A1 → A1-R03, A2 → A2-R03, B1 → B1-R03
- A2 film-opinion dialogue (uses congiuntivo, labelled B1) → B1-S02

Arabic coverage: 83 of 154 source sections had no Arabic. Added EN + AR quick-explanation callouts to all 39 grammar pages. Practice, sentence-bank and speaking pages are still English/Italian only.

Stale "Part N" cross-references were rewritten as `[[wikilinks]]`. No broken links remain.

## [2026-10-11] ingest | 33 Arabic-language grammar lessons

Source saved verbatim as raw/sources/Italian_Arabic_Lessons.md. Each lesson was appended to its topic page as a "🇸🇦 Arabic lesson" section: 🔊 audio markers removed, tab tables converted to markdown, `<!-- src: Arabic Lessons · Lnn -->` tags added. Related pages got cross-reference callouts. 29 pages now carry an Arabic lesson.

New pages: A1-G16 Demonstratives & Indefinites (questo/quello/qualche/ogni) and A2-G13 Impersonal Constructions (c'è, bisogna, si può, è vietato, weather verbs). Both have EN + AR boxes.

Placement follows the CEFR rules: A1 articles, prepositions, essere/avere, gender/plural, present tense, adjectives/possessives, pronouns, negation/questions, numbers/time, reflexives, demonstratives. A2 passato prossimo, imperfetto, futuro, politeness/condizionale, stare + gerundio, comparatives, object pronouns, ci/ne, adverbs, impersonals. B1 relatives, imperative, passive, if-clauses, congiuntivo presente/imperfetto, condizionale passato, trapassato, futuro anteriore, reported speech. B2 combined pronouns.

Corrections to the source, each flagged in a warning callout on its page: Lei takes a 3rd-person verb, not a "feminine" one; parlarei → parlerei (built on the future stem); the futuro stem rule (drop -e, -are → -er-); the French "Dr & Mrs Vandertramp" mnemonic replaced with the Italian essere rule; la gamba/le gambe is regular, so it was swapped for la mano/le mani; future of probability = «على الأرجح», not «أكيد»; sto male = «لست بخير»; nessuno = nobody, not nothing; "ce ne sono" ci = there; typo قابلها → قابلتها.

index.md, course_tracker.md and the README tables were rebuilt (87 pages).

## [2026-10-11] create | 17 bilingual EN + AR lessons + Lessons by Level page

Wrote 17 new lessons in the Arabic-lesson style, but bilingual: every explanation in English then Arabic, and tables with Italian | English | العربية. They cover every grammar topic that had no lesson: A1-G06 piacere, A1-G11 modals and everyday irregulars, A1-G15 pronunciation (with p/b, v/f, o/u traps and doubles = shadda), A2-G11 tense clue words, A2-G12 irregular verb survival kit, B1-G06 linking, B1-G07 tu/Lei register, B1-G10 gerund/implicit clauses, B2-G01 sequence of tenses, B2-G02 congiuntivo passato/trapassato, B2-G04 complete subjunctive triggers, B2-G05 time clauses/certainty/necessity, B2-G06 advanced passive (venire / andare + participle) and relatives, B2-G07 mixed conditionals and wishes, B2-G08 discourse markers, B2-G09 formal register and email template, B2-G11 passato remoto.

Six grammar pages already covered by an Arabic lesson on a sibling page got a cross-link callout instead (A1-G07, A1-G12, A1-G14, A2-G01, B1-G02, B2-G03). Every grammar page now has a lesson.

New page wiki/lessons.md lists all 50 lessons (33 🇸🇦 + 17 🇬🇧🇸🇦) by level, in a suggested study order. index.md and README link to it.

## [2026-10-11] privacy | Personal details removed from lessons and sources

Replaced the learner's name with "Ahmed" in example sentences, and swapped real cities and nationality for generic ones. Exam-specific references (date, "the paper you sent", "finishing tomorrow") now read as generic A2-exam material. Personal job and study details in model answers (degree, company, schedule) were rewritten as a neutral persona. raw/sources/ was edited for the same reason, and only for this. Git author metadata is unchanged, as the learner asked.

## [2026-10-13] translate | Full Arabic pass across the wiki

Arabic was added to every remaining content line: sentence banks (A1/B1/B2, ~800 sentences), all 83 speaking days, all dialogue pages, revision sheets, CEFR pages, answer-key rules, every grammar page's reference section, and the correction notes. Tables got an العربية column, and paragraphs, bullets and examples got a 🇸🇦 line underneath. Conjugation rows carry the Arabic conjugation (أعمل · تعمل · يعمل…). The only lines without Arabic are pure Italian conjugation tables inside the Arabic lessons and the English quick boxes, which each sit next to their Arabic twin.

Source errors flagged in Arabic along the way: B2 sentence bank English column shifted one row (rows 37–42); subjunctive misused after dopo che / non appena / finché; "gli begli amici" → "i begli amici"; mixed tu/Lei in the A1 directions dialogue. The English column of the B2 job-interview and job-application models still mentioned engineering/software and was fixed.
