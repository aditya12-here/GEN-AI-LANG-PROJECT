A Socratic Sanskrit teaching assistant. Given an English sentence, it guides the student to translate it into Sanskrit without revealing the answer. It operates in the following two distinct phases:
Phase 1 — Input: Splits the sentence into parts, provides a combined vocabulary table with case/verb hints, and gives a brief structural clue per part. Student assembles the sentence themselves.
Phase 2 — Response: Receives the student's attempt, names one correct element first, interprets exactly what the student wrote, identifies gaps, and gives feedback bilingually (Sanskrit + student's mother tongue). Tracks attempt number and adjusts hint depth accordingly across up to three attempts.

Structural Features

Multi-clause sentences split into numbered भागः
Single combined शब्दसूची table — no separate tables per part
Attempt policy: clues only → one direct hint per error → reveal only the wrong word (never full sentence)
Hint count reduces as student accuracy improves across sentences


Shortcomings
Mother tongue still assumed — the prompt says "mother tongue of student" but never asks or detects it. Defaults silently to Hindi, breaking for any non-Hindi speaker.
Negative example still embedded in live prompt — adds token overhead every call and risks partial imitation despite the warning label.
"Too much into his own head" problem unresolved — the attempt policy handles gibberish and partial errors but gives no guidance when the student's sentence is grammatically valid Sanskrit yet semantically drifts far from the original meaning.
Persian-origin word rule has no examples — the instruction to avoid Hindi words of Persian origin is stated but never illustrated, leaving the model to judge case by case without a clear boundary.
Attempt counter has no memory mechanism — the prompt instructs tracking attempt number but provides no actual state-tracking. In a stateless model, attempt count resets every session unless the conversation history is intact.
Romanisation standard unstated — IAST is used in examples but never mandated, risking inconsistent transliteration.
No scaffolding for beginners — terms like prathamā vibhakti, lṛṭ lakāra, saptamī are used without explanation, with no fallback for a student unfamiliar with Sanskrit grammar terminology.