---
name: loop-engineering-turtleand-frontend
description: Implement and refine Turtleand interfaces through bounded render, independent critique, and browser verification loops. Use for visual frontend work across Turtleand spaces, preserving each surface's selected direction; concept-only exploration belongs to the UX skill.
---

# Turtleand frontend loop

Turn a selected design into an excellent working interface, using observed results to guide revisions. Visual distinction and functional reliability require separate evidence; passing a build or screenshot diff does not establish design quality.

## Establish the target

- Read the destination's `AGENTS.md`, `CLAUDE.md`, relevant design guidance, actual source, package scripts, and existing checks. Reconcile stale documentation against current implementation and user decisions.
- Preserve existing work. Inspect the current route, design system, assets, content, and representative states before editing. Keep the requested scope: a spacing fix does not trigger a site redesign.
- Use the selected UX handoff when present: audience and purpose, chosen visual reference, content hierarchy and real copy, type/color/spacing tokens, responsive behavior, interaction states, accessibility requirements, and observable acceptance criteria.
- An existing interface is a valid direction for a focused improvement. If a consequential new direction remains undecided, use `loop-engineering-turtleand-ux` when available or present visual concepts, then obtain the user's choice before changing production source, unless the user explicitly delegated that choice. Do not require another choice when the session already establishes it.
- Reuse the task's artifact location, or choose one outside public routes and generated production assets. Keep `brief.md`, `loop.md`, candidate evidence, and `handoff.md` when a transfer is needed. Do not commit these artifacts or add site UI for the workflow unless requested.

## Respect the surface

Portal is the identity hub and router; Growth is reflective writing; Handbook supplies compact principles; Chronicle is symbolic narrative; Atlas provides tool discovery; Build, AI Lab, Hermes, Chain Lab, and Energy have distinct learning and practice roles. Verify local definitions instead of forcing a common page template.

Keep Turtleand's calm, precise voice, human responsibility, and evidence-based claims. Preserve pseudonymous public identity, relevant English/Spanish parity, destination links, and established routing. Keep private operational details out of public output.

When the Turtleand avatar appears, use canonical assets and the destination's avatar rules. Create a new version only when the task calls for it and follow the full local protocol. Do not reconstruct rest geometry from derivatives or add an avatar gallery simply to satisfy a global style. Chronicle's metaphors, Portal's palette, and any one surface's framework constraints are not universal defaults.

## Run the loop

Default to a maximum of **five critique/revise cycles for the invocation**, with an earlier stop after **two consecutive cycles without a defensible improvement**. User-specified effort bounds override this default. Resume the handoff's consumed/remaining cycles and plateau history across delegated work and phases of the same invocation; parallel reviewers do not create extra cycles. This is a ceiling, not a quota.

1. **Baseline and slice.** Capture the current experience when one exists. Implement the smallest complete slice that exposes the design's major risks: real content, a representative layout, one meaningful interaction, and narrow-screen behavior. For a small edit, the affected component is the slice. Favor composition, hierarchy, typography, and content fit before ornamental detail.
2. **Render and observe.** Use available native browser tools/connectors or the repository's established harness. Inspect the actual rendered candidate, not code imagined as a screen. Capture the desktop and narrow layouts plus states relevant to the change. Read [browser review](references/browser-review.md) before collecting evidence.
3. **Independent critique.** Give a fresh reviewer the authorized portions of the brief, selected reference, current captures, route/state metadata, and relevant constraints. Do not give the creator's rating, defense, or preferred fix. Ask for up to three consequential mismatches, their visible location, user impact, and supporting evidence; no material findings is a valid result. Keep aesthetic findings separate from behavioral failures. If an independent reviewer is unavailable, disclose that limit and use a fresh evidence-first review; do not call it independent validation.
4. **Focused revision.** Resolve one coherent cluster of the highest-impact findings. Preserve the selected direction and useful differences between surfaces. Confirm whether each proposed change addresses the brief rather than a reviewer's unrelated taste. Do not replace missing content or assets with extra decoration.
5. **Recapture and compare.** Capture matching states after the revision. Retain the better candidate based on visible improvement and functional checks, not recency. A regression in readability, accessibility, behavior, or a selected design invariant is not a net improvement. Revert only task-owned changes when restoring a candidate; never overwrite unrelated work.

Expand the slice across the requested scope once its core decisions survive review. Spend the remaining shared cycles on the completed experience rather than giving every component five separate loops. Record each cycle's observation, change, evidence paths, and keep/reject decision in a few lines.

## Verify completion

- Run the destination's required build and relevant existing checks. Do not invent a passing command or substitute a development server for production verification without reporting the difference.
- Exercise actual user paths: navigation, focus and keyboard activation, touch-relevant affordances, responsive layout, language switching, reduced motion, and the changed component's meaningful loading/empty/error states. Test only applicable states; extend tests for meaningful regressions rather than mirroring implementation.
- Check related performance risks when the change adds media, fonts, runtime code, animation, or loading dependencies. Reuse existing budgets and compare like conditions. Lab measurements do not prove physical-device or field performance.
- Preserve metadata, canonical URLs, schemas, sitemaps, and AI-readable artifacts where the change affects them. Do not silently refresh unrelated generated files.
- Freeze the final source state and recapture any view invalidated by later edits. Missing or stale screenshots mean visual verification remains incomplete. Automated accessibility checks and pixel similarity support review; neither certifies usability or excellence.

Stop when the acceptance criteria are evidenced and no consequential issues remain, when the declared cycle ceiling is reached, or on the two-cycle plateau. Keep the best non-regressing candidate and clearly list remaining issues. A budget stop is not a completion claim. Do not continue by resetting the counter, widening scope, or changing the art direction without the user.

## Report the outcome

Provide the working preview or artifact paths, a concise before/after explanation, final desktop/mobile evidence, actual checks and their limits, cycle count, and unresolved trade-offs. Separate observed visual improvements from functional results. Never award an invented “AAA” rating or treat the creator's self-score as validation.

This skill authorizes no deployment, messaging, publishing, dependency installation, or repository-wide configuration changes beyond the user's task. Discover tools at runtime; do not require a specific vendor, browser package, or model. For provenance and evidence limits, read [research](references/research.md). Behavioral evaluation scenarios live in [evals/cases.json](evals/cases.json).
