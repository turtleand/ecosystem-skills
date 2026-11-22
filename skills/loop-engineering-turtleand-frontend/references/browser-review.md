# Browser evidence for frontend iteration

Use this reference when planning captures, reviewing a rendered candidate, or claiming frontend completion. Adapt the matrix to the changed behavior and local repository requirements; this is not a demand to run every possible browser and state for every edit.

## Establish what is actually running

Discover the current project's scripts, runtime, installed test tools, and available browser connectors. Prefer suitable native tools and existing harnesses. Do not install Playwright, a framework, or a new testing stack merely because this skill names them.

Record the route, source revision or task-owned diff identity, build mode, browser, viewport, locale, and relevant state for each evidence set. For a dirty checkout, a commit hash alone does not identify the rendered candidate. Use a diff fingerprint, relevant source hashes, or a clearly identified saved candidate.

Check the actual server and route. Wait for fonts, required images, and relevant UI readiness; avoid hiding a slow or broken loading state behind a long arbitrary delay. A screenshot of a placeholder or another worktree does not verify the candidate.

Use the project's production workflow for final integration checks. If it cannot run locally, say which alternative ran and which behavior remains untested. A static preview can verify client-side rendering and interactions, while dynamic routes and server behavior require the corresponding runtime.

Bind locally launched previews to loopback by default. Use the project's approved preview environment when access from another machine is needed. Exercise state-changing interactions with fixtures or test data in an authorized test environment.

## Capture states that matter

Capture the owner-specified viewport first when supplied. Otherwise use representative desktop and narrow-screen sizes supported by the project; 1440px desktop and 390px mobile are reasonable starting probes, not universal breakpoints. Add a narrower width, landscape, or intermediate breakpoint when layout behavior warrants it.

For the changed experience, select relevant evidence from:

- Initial view and complete reading order, with close crops where text or artwork needs inspection.
- Open navigation, dialog, selection, expansion, or other meaningful interaction result.
- Keyboard focus and activation; modal focus entry, containment, dismissal, and return when applicable.
- Loading, empty, error, retry, and success states when those states exist or change.
- English and Spanish where supported; use real text expansion rather than an empty translated shell.
- Reduced motion and other local accessibility modes; disabled motion must preserve meaning and control.
- Long text, zoom or enlarged text, overflow, and touch affordances where the layout is vulnerable.

Use full-page captures for structure and viewport/component captures for actual readability. Inspect the images, not only the screenshot filenames. A capture inventory proves acquisition, not design quality.

Freeze or synchronize animation only for deterministic comparisons. Separately inspect the real transition, interruption, replay, or pause behavior. Do not use camera movement as proof of character animation or a still image as proof of an interaction.

## Keep comparison conditions honest

Compare baseline and candidate in the same browser/rendering environment, viewport, content, locale, and interaction state. Keep fonts, hover, scroll position, and animation phase consistent. Record unavoidable differences before interpreting them.

For performance comparisons, also match build mode, cache, compression, network and CPU profiles. Run noisy timing measurements apart from other heavy browser work. Distinguish payload, response time, readiness, layout stability, frame cadence, and actual GPU measurements.

Pixel diffs can reveal accidental drift after a direction is selected. They cannot rank a new composition, and updating a snapshot must not erase an unexplained regression. Retain the baseline and inspect the difference before accepting a replacement.

## Brief a fresh reviewer

Provide the selected design target and constraints, actual candidate captures, and the state metadata. Keep implementation arguments and the creator's confidence score out of the initial review. The reviewer should inspect before reading proposed fixes.

Share only evidence needed for the review and authorized for the reviewer's environment. Crop or redact credentials, private routes and URLs, account data, and machine-specific paths from shared artifacts.

Ask for:

1. Up to three highest-impact visible mismatches, with screenshot/region and a concrete description.
2. The affected reader or user task and the relevant acceptance criterion.
3. A separate list of observed behavior failures, distinguishing observed facts from untested concerns.
4. Whether the candidate improves on the baseline while preserving the direction, with reasons and remaining uncertainty.

Useful aesthetic lenses are hierarchy, composition, typography, spacing rhythm, content fit, image relevance, character identity, and visual consistency. They are diagnostic lenses, not a numerical beauty rubric. A fix should address a visible problem instead of merely adding motion, gradients, or decoration.

Review attention should progress from large structural issues to refinements. Do not spend a cycle polishing a border while the primary message is obscured or the mobile navigation fails.

## Complete the behavioral checks

Use semantic roles and actual user input where possible. Confirm destinations and labels, visible focus, reasonable tab order, keyboard activation, touch-sized controls according to local requirements, and scrolling without traps. Automated accessibility scans supplement manual interaction checks; a clean scan is not comprehensive accessibility certification.

Run applicable project validation and record failures honestly. For a narrowly scoped cosmetic fix, reuse relevant existing tests and browser checks rather than constructing a large new suite. Add a regression test when it protects a meaningful behavior that has failed.

## Preserve usable evidence

Reuse the task's artifact location, keeping `brief.md`, `loop.md`, candidate capture folders, and `handoff.md` when another agent or phase needs the state. The report needs only the target, scope, acceptance observations, cycle count, ranked finding, focused change, keep/reject rationale, and links to supporting captures/check results. On a handoff within the same invocation, transfer consumed and remaining cycles, the last two improvement decisions, best candidate identity, and stop status; resume that budget instead of starting a fresh five cycles. Do not put private local paths or workflow logs into the public site.

After source changes, mark affected captures stale until refreshed. Keep the best candidate recoverable through task-owned patches or isolated workspace state without committing or disturbing unrelated edits. Missing browser access permits continued source work but not a claim that visual review passed.
