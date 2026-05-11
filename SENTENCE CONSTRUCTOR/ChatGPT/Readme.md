Sanskrit Teacher Prompt — README

What This Prompt Does
A Socratic Sanskrit teaching assistant. Given an English sentence, it guides students to translate it into Sanskrit without giving the answer directly. It provides:

Sentence split into logical parts (वाक्यविभाजनम्)
Grammatical clues per part: which vibhakti (case), which lakāra (tense/mood), which dhātu (verb root)
A vocabulary table: Sanskrit | Transliteration | English | Case/Verb hint
After the student submits an attempt, it explains the meaning of what they wrote — in Sanskrit and their mother tongue (Hindi)


Formatting Rules-

Word order follows classical Sanskrit (S-O-V suggested, student figures out exact order)
Vocabulary in a single combined table (no separate tables for grammar and words)
No explicit adverb labels in the table; no pre-declined/conjugated forms given away
Post-attempt feedback is bilingual (Sanskrit + student's mother tongue)

Shortcomings-
**Mother tongue assumption** — the prompt assumes Hindi without ever asking, so it breaks for any non-Hindi speaker.

**No error correction guidance** — after a student submits an answer, the prompt only says to explain the meaning, leaving no instruction on whether or how to flag wrong vibhakti endings or incorrect lakāra usage.

**Clue depth is unspecified** — there's no rule for how many clues to give per sentence part, so complex sentences risk either giving too much away or leaving the student completely stuck.

**Romanisation standard unstated** — IAST is implied but never mandated, which opens the door to inconsistent transliteration across sessions.

**No scaffolding for beginners** — the prompt assumes the student already knows terms like prathamā vibhakti, laṭ lakāra, and tumuṇ, with no fallback explanation for a novice.

**Bad example is still in the live prompt** — embedding it adds token overhead and risks the model partially following it despite the warning label; it should be removed entirely.

**Step 4 is redundant** — the desired example includes a "build it yourself" section that just restates the table, which is exactly what the bad example was penalised for; the good example should model the omission, not repeat the mistake.

**No handling for multi-clause sentences** — the guidance only covers splitting a sentence into two parts, with nothing for three or more clauses.

