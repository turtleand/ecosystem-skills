# Research provenance and limits

Checked: 2026-11-15. These are primary documentation and local workflow sources. This skill synthesizes their mechanisms; none establishes that a particular loop produces “AAA” design, and no numerical design-quality score is inferred.

## Verification and independent evidence

- [Anthropic, Harness design for long-running application development](https://www.anthropic.com/research/harness-design-long-running-apps), published 2026-03-24: describes a generator and a separate evaluator that navigates the live page, captures screenshots, and returns critique. Its author reports plateaus, non-monotonic quality, and sometimes preferring an intermediate candidate. Adopt independent observation and preservation of the best candidate. This skill uses five cycles as a practical default.
- [Vision-Guided Iterative Refinement for Frontend Code Generation](https://arxiv.org/abs/2604.05839), submitted 2026-04-07: evaluates a visual critic providing structured feedback on rendered pages over repeated refinement. The reported benchmark gains support testing this mechanism; they do not predict Turtleand results, establish universal design taste, or replace human direction selection.
- [OpenAI, Designing delightful frontends with GPT-5.4](https://developers.openai.com/blog/designing-delightful-frontends-with-gpt-5-4): recommends explicit design constraints, visual references, narrative/content strategy, and browser-based inspection of viewports and flows. Adopt those mechanisms. Model recommendations and example aesthetic prescriptions are contextual vendor advice, not permanent requirements or reasons to override a surface's design system.
- [Paul Bakaus, Impeccable](https://github.com/pbakaus/impeccable): provides distinct design critique, technical audit, targeted refinement, and persistent product/design context workflows. Adopt the separation and focused feedback vocabulary without installing its tooling, hooks, scoring system, or aesthetic blacklist. Repository demonstrations and author claims are not independent causal evidence.
- [Vercel Web Interface Guidelines](https://raw.githubusercontent.com/vercel-labs/web-interface-guidelines/main/command.md): offers concrete checks for semantics, focus, motion, content handling, images, and performance. Use these as relevant review lenses. Its framework examples and prescriptive style rules are not universal requirements; prefer semantic controls and the target project's actual contracts.
- [Claude Code best practices](https://code.claude.com/docs/en/best-practices): distinguishes instructions from enforced checks and recommends making otherwise invisible project knowledge and completion checks explicit. Adopt observable acceptance and bounded review rather than relying on a stronger adjective in a prompt. This is vendor workflow guidance, not a controlled study of visual quality; no Claude-specific commands are required here.
- [Playwright visual comparisons](https://playwright.dev/docs/test-snapshots): supports screenshot comparison and explains why browser/OS/rendering conditions affect results. Adopt matching capture conditions and deliberate inspection of differences. A pixel match confirms similarity to a baseline, not whether that baseline is a good design.
- [Playwright accessibility testing](https://playwright.dev/docs/accessibility-testing): shows state-aware automated accessibility checks and explicitly limits their coverage. Adopt real interaction and manual inspection alongside existing automation. Passing Axe or another scanner cannot establish full accessibility or usability.

## Turtleand's existing practice

Portal's avatar review pairs baseline and candidate captures under matching conditions, records the source revision, and distinguishes static browser checks from production verification. Its reports track visible changes, payload, and readiness separately.

Review the avatar's silhouette before its surface detail, and keep the camera fixed when assessing character motion. Follow the destination's asset and motion guidance.

Chronicle's reviews capture meaningful scene states across languages, motion preferences, and layout sizes. Verify the intended state change and its behavior under resizing using the destination's own design guidance.

These local artifacts demonstrate an existing process and reported measurements. Their screenshot inventory is not independent evidence of exceptional aesthetic quality. The independent critique and bounded retention loop in this skill is a design choice, not a claimed benchmark result.

## Maintenance

Recheck linked primary sources when changing the workflow or when tool behavior conflicts with the references. Read the actual destination repository instructions at invocation time rather than treating this source snapshot as current operational truth. Keep the entrypoint portable; tools and vendor integrations are replaceable implementation choices.
