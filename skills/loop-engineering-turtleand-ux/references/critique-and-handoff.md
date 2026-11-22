# Critique and handoff

## Choose relevant standards

Use the brief and visually inspected references to describe what excellent means for this task. References calibrate judgment; they do not replace the product's purpose. Avoid a generic luxury, museum, SaaS, or cinematic target across unrelated spaces.

Review the dimensions that affect the visitor:

| Dimension | Evidence to inspect |
| --- | --- |
| Identity and specificity | Does content shape composition and interaction? Could a different product use this unchanged? |
| Hierarchy and orientation | Can a newcomer identify the subject, principal invitations, and useful next step? Inspect the initial viewport separately from the full page; assess whether visual emphasis delays the task's useful content. |
| Reading and content | Headings, copy length, measure, contrast, grouping, bilingual expansion where relevant; is a cut better than another section? |
| Composition and typography | Proportion, spacing rhythm, alignment, expressive type, image/text balance, desktop and mobile structure |
| Imagery and character | Asset quality, provenance, intentional crop, meaningful relationship to content; canonical Turtleand avatar references where used |
| Interaction and motion | Clear affordances, meaningful state changes, continuity, keyboard/touch alternatives, motion serving understanding; preserve the meaning of choices and sequences when explanatory labels disappear on mobile |
| Completeness and restraint | Essential visitor paths and states, sufficient detail, no gratuitous visual mechanisms or hidden information |

Do not average away a failure of an essential visitor path. Do not give numerical scores without a supplied calibrated rubric. Distinguish design preference from a reproduced defect. Heuristic walkthroughs do not establish that real visitors understand the design.

## Reviewer brief

Use a fresh agent with the minimum context required:

> Review these candidate artifacts against this brief, local design constraints, and reference evidence. Inspect the actual rendered images and, when possible, the preview at the specified states and sizes. Give strengths worth preserving and only material problems: location/state, visible evidence, visitor consequence, and a focused correction. Note unavailable evidence. Assess each concept on its own merits and compare them afterward. Do not assume a later iteration is better or invent required changes. Do not implement or choose on the user's behalf.

Provide full accessible artifact paths or URLs. Use separate tabs when browser work runs in parallel. If an independent agent is unavailable, conduct a separate self-review and identify that limitation in the report. Do not call it independent.

## Evidence and candidate preservation

- Save a baseline and each reviewed candidate with distinguishable identifiers. Record the file hash or revision that produced each capture; a git commit is unnecessary.
- Match viewport, content, language, state, theme, and browser conditions for before/after comparisons. Inspect an overview and important details at readable scale. For motion, inspect the actual transition or representative frames, not just the resting screen.
- Keep first-screen and full-page judgments separate. A full-page image does not show what fits in one viewport. Evaluate time-to-content and reading rhythm against the brief; do not impose a universal rule that every action must be above the fold.
- After code, copy, or assets change, recapture affected views before making claims about the final candidate. A screenshot of an earlier version is historical evidence only.
- Retain the best known candidate within the task's own artifacts. Do not reset a user's working tree or discard unrelated work to recover an older prototype.
- A candidate may be visually stronger but harder to navigate. Record that trade-off and keep it visible; neither aesthetic taste nor automated tests settle it alone.
- Stop after two consecutive cycles with no evidenced material gain, or the declared budget. Report remaining issues and the best retained version. Reopening the loop needs a new hypothesis, changed brief, or user instruction.

For substantial work, a useful row in `loop.md` is: cycle | candidate/revision | capture conditions | finding/evidence | proposed correction | outcome/regressions | retained candidate. Keep the record proportional for small work.

## Handoff

Record decisions that would otherwise be guessed during implementation:

- **Selection:** user-selected concept, version, and constraints; pending selections remain explicitly pending.
- **Content:** purpose, audience, page/section order, labels and representative copy, navigation destinations, items cut or relocated.
- **Visual target:** viewable desktop/mobile artifacts and inspected references, type roles/scale, spacing/grid, palette and contrast, image crops/assets. Reuse or map existing tokens when available.
- **Behavior:** layout changes at useful widths, what wraps/reflows, interaction states, focus/touch behavior, motion and reduced-motion equivalent.
- **Assets:** canonical source, generated/proposed/existing status, rights/provenance known to the task, missing assets and acceptable temporary treatment.
- **Acceptance:** concrete observations a reviewer can verify, scope boundaries, relevant repository checks, and unresolved trade-offs.
- **Loop state:** for a transfer within the same invocation, consumed and remaining cycles, the last two improvement decisions, best candidate identity, and stop status. The next agent resumes this state; a handoff does not replenish the budget.

Do not invent a full design system, exact breakpoint inventory, or interaction state that the task does not need. For a narrow refinement the current design plus an annotated change target can be the whole handoff. A selected concept does not itself authorize production work unless the user's task includes implementation.
