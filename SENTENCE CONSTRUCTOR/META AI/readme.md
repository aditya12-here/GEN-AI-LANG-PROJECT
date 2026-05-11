Sanskrit Teacher Prompt — README
What This Prompt Does
A Socratic Sanskrit teaching assistant. Given an English sentence, it guides the student to translate it into Sanskrit without revealing the answer. It provides:

Sentence split into logical parts
Grammatical clues per part: which vibhakti (case), which lakāra (tense/mood), which dhātu (verb root)
A single combined vocabulary table: Sanskrit | Transliteration | English | Case/Verb hint
Student assembles the final sentence themselves


Shortcomings
No post-answer feedback instructions — the prompt has no guidance on what to do after the student submits a translation. Should it correct morphology, explain meaning, or both? This is entirely unspecified.
Mother tongue assumed to be Hindi — never explicitly asked or detected, therefore the prompt breaks for any non-Hindi speaker.
Clue depth unspecified — no rule for how many clues to give per sentence part. Complex sentences risk either giving too much away or leaving the student stuck.
No scaffolding for beginners — terms like prathamā vibhakti, laṭ lakāra, and tumuṇ are used without explanation, with no fallback for someone unfamiliar with Sanskrit grammar terminology.
Romanisation standard unstated — IAST is implied but never mandated, risking inconsistent transliteration.
No handling for multi-clause sentences — splitting guidance works for two parts but gives no direction for three or more clauses.
Persian-origin word restriction has no examples — the instruction to avoid Hindi words of Persian origin is stated but never clarified, leaving the model to judge case by case without a clear boundary.