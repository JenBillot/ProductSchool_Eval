# First LLM-as-a-Judge Eval, Module 1

## Version A, Concise, system prompt used

You are an executive briefing assistant.
Summarize in exactly 3 bullet points under 60 words. No preamble, no extra text.

## Version B, Narrative, system prompt used

You are a PR communications assistant.
Write a 100-word narrative summary highlighting wins first, then risks and next steps. Keep a positive tone. No bullets.

## Eval setup, dataset name + judge model/family

Used dataset Module1Output; choose a consiseness LLM as a Judge (choosing a different LLM model; I choose one of the 5.0 family of models) compared to the 4.0 family used for the original LLM set up

## Cold-start, the prompt you used to seed a starter dataset

Generate 20 example rows for evaluating email-summary quality. Each row: input email + candidate summary + a first-pass label (good/bad) + one-line reason. Make ~half concise/faithful (good) and half verbose or inaccurate (bad). Return as a markdown table

## Your definition of good vs bad (golden-set criteria) — the graded part, write your own

Groundedness
Good: every claim traces back to something actually in Ascend's verified data.
Bad: sounds plausible but isn't actually sourced from the data.
Completeness
Good: comparative queries get proportionate coverage of every side asked about.
Bad: only answers the easier half of the question and presents it as complete.
No unlabeled inference
Good: synthesis or opinion is clearly flagged as IQ's own read, separate from observed fact.
Bad: inference is blended in and stated as if it were fact.
Calibrated uncertainty
Good: thin, old, or conflicting data is flagged as such.
Bad: a confident answer is given despite thin, old, or conflicting data.
Sourcing
Good: claims are traceable to a specific source doc/date so users can verify them.
Bad: claims are correct but unsourced, so users can't check them.
Decision-usable structure
Good: length and structure preserve the real distinctions the user needs to act on.
Bad: brevity flattens the answer and erases meaningful differences.
Gut check (overall)
Good: a VP could act on it and it would hold up if they checked the source data themselves.
Bad: it looks trustworthy but falls apart the moment someone checks it against the source.

## Screenshots, links or repo paths (optional if you followed the demo)

_…_

