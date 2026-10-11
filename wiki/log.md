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
