# Question design for active recall

Companion to SKILL.md; applies to every item in every set. When a rule here
conflicts with the learner's explicit calibration in `context.md`, the learner
wins — log the override in `context.md`'s learner calibration section. Rules are distilled from retrieval-practice research;
the few numbers retained are heuristics, not laws.

## Enforcement gate (binding — not guidance)

Every rule below is a gate. Before sending any set, run EVERY item through this
checklist; fix failures before sending — never ship a known-fail item. Ship the
set with a one-line audit (e.g., "item gate: 8/8 pass" or "item gate: Q3
reworded — 8/8 pass"). A set that arrives without an audit line is defective:
the learner should send it back.

Per item:
1. Studied material only (completed chapters + due re-tests).
2. Premises: the stem states EVERY fact the answer depends on. Nothing is left
   for the learner to assume or resolve — no open "state your assumptions,"
   not even a named disjunction handed to them. Dirty premises only when the
   stem names the open dimension and instructs how to treat it.
3. One question per item; no double-barrel.
4. Exactly one defensible answer or ranking under the stated premises.
5. No stem-answer echo, purposeless negation, unequal options.
6. Non-obvious syntax annotated; nothing hinges on decoding.
7. Practice: tool verified in context.md Environment; the work isn't already
   done in the learner's repo; asks for an observation, not a done-checkmark.
8. Every factual claim carries provenance: book → cite ch/section; trusted
   resource → cite (fetch when feasible); "my distillation"; "from memory."
9. Diagnose: ranked causes, most-probable first, one confirm/rule-out check each.

Per set:
10. Counts/format per learner calibration; ≤2 old items, spaced (never
    same-turn); declined formats not used.
11. Connect present; answer key withheld/shown per calibration.

## Difficulty

- Effortful-but-successful retrieval beats easy retrieval; failed retrieval
  *corrected by feedback* is nearly as good as success. Uncorrected, it is
  worse than not asking.
- Target sets the learner mostly but not fully answers (~1/2 to 3/4 success
  on fresh material). Every miss becomes a re-test queue entry, not a failure.
- Never test unstudied material; difficulty is per-learner — scaffold harder
  applications on studied foundations.

## Format

- Free response by default: generating strengthens memory more than
  recognizing. Option-based items only when discrimination practice or
  grading speed justifies them.
- With options: every distractor plausible (a common misconception is ideal —
  *which* distractor gets picked is diagnostic data); all options equal
  length and grammatical shape; no all/none-of-the-above; the stem never
  lexically echoes the answer; exactly one defensible answer under the stated
  premises.
- A wrong option choice left uncorrected gets learned. Every option-based
  item must eventually meet feedback.

## Stems

- One question per item; no double-barreled items.
- State premises explicitly — what was and wasn't done, configured, assumed.
  A grading dispute traced to an unstated premise is the tutor's bug, not the
  learner's. Dirty-premise scenarios are fine, but then "state your assumed
  premise" is declared as part of the expected answer.
- Positive phrasing; negation ("which is NOT…") only when discriminating
  between confusables is the point of the item.
- Annotate any command or notation the item relies on with a one-line "this
  does Y". Test the concept, not instruction-decoding.
- The verb sets the cognitive level (list < explain < predict/diagnose <
  recommend-and-defend); match it to the section's purpose.

## Practice items

- Only tools the environment block in `context.md` allows; annotate every
  non-obvious command.
- Ask for an observation the learner reports back, not a done-checkmark.

## Transfer scenarios

- Shape scenarios like the learner's real use cases (the Destination in
  `context.md`), not generic textbook cases — retention follows the match
  between practice conditions and use conditions.
- Interleave confusables: pit similar concepts against each other, and mix
  problem types within a set so the learner practices *choosing* a strategy,
  not just executing an announced one. Confusable pairs benefit most.
- Diagnose items: ranked causes, most probable first, plus for each cause one
  piece of evidence that would confirm or rule it out.

## Feedback

- The blind attempt is the active ingredient — a visible key invites skipping
  the retrieval. Withheld unless the learner opted in.
- Correct every miss explicitly, never just score it; explain why, tied to
  the spot in the source material; cite trusted resources where they state it
  more precisely.
- Explanations beat bare answers for transfer; delay between attempt and
  feedback is fine or beneficial — turn-based grading is aligned, not a
  compromise.

## Scheduling

- Spaced beats massed: re-test a miss after a lag (next set at the earliest),
  never in the same turn. Expand intervals on success; two spaced passes =
  owned.
- 1–2 old items per set, prioritizing misses over passes.

## Anti-patterns (each wastes a retrieval)

Re-teaching instead of asking · unstudied material · unstated premises ·
double-barreled stems · unequal options · implausible distractors ·
stem-answer echo · purposeless negation · visible key during the attempt ·
scored-but-uncorrected misses · corrected-but-unqueued misses · unannotated
syntax.
