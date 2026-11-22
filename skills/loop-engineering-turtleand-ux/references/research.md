# Research basis

Checked 2026-11-15. These are sources for the workflow, not instructions to execute or packages to install. Recheck live sources when updating the method. The skill is an original synthesis of the mechanisms below.

- [Anthropic: Harness design for long-running application development](https://www.anthropic.com/research/harness-design-long-running-apps), 2026-03-24. A separate generator and evaluator, calibrated criteria, and live browser inspection improved examples over iterative runs. Later iterations were not always preferred; rubric wording could converge on one aesthetic and complexity grew. Firsthand engineering experiments, not a guarantee of exceptional design. Borrow independent critique, observable targets, and best-candidate retention.
- [Sansford et al.: Vision-Guided Iterative Refinement for Frontend Code Generation](https://arxiv.org/abs/2604.05839), submitted 2026-04-07. A visual critic provides structured feedback on rendered pages. Authors report improvements within their benchmark; that does not establish the same gains for Turtleand or prove real-user usability.
- [OpenAI: Designing delightful frontends with GPT-5.4](https://developers.openai.com/blog/designing-delightful-frontends-with-gpt-5-4). Establish references, content and visual direction, then inspect the rendered interface. Use the method without converting example fonts, heroes, palettes, or a named model into universal requirements.
- [Paul Bakaus: Impeccable](https://github.com/pbakaus/impeccable). Practitioner guidance separates design critique, implementation audits, and polish; different surface purposes deserve different ambitions. Borrow independent assessment and contextual design vocabulary. Do not inherit its executable downloads, hooks, permission conventions, arbitrary scores, or style restrictions.
- [Lulla et al.: Loop Engineering: Building Blocks, Adoption, and Impact](https://arxiv.org/abs/2608.21884), revised 2026-10-22. Describes persistent state, verification and termination controls, while identifying limited systematic evidence behind broad benefit claims. This skill implements bounded instruction-driven iteration, not unattended background automation.

## Local grounding

Portal's existing avatar QA demonstrates consistent captures, actual interaction checks, source identity, and honest measurement limits. Its captured `ready` status establishes render readiness, not aesthetic quality. Chronicle's visual tests cover meaningful scene states and multiple accessibility modes. Their domain-specific art rules stay local; inspect the current target repository instead of copying these contracts to all surfaces.

## Portability

[Codex skill discovery](https://learn.chatgpt.com/docs/build-skills) supports user skills in `~/.agents/skills` and symlinked folders. [Claude Code skills](https://code.claude.com/docs/en/skills) supports personal skills in `~/.claude/skills` and symlinked folders. Use one canonical local copy linked into Claude's personal directory. Local discovery does not imply synchronization into remote/cloud sessions. Invocation syntax belongs to the active host: Claude `/loop-engineering-turtleand-ux`; Codex skill selector or `$loop-engineering-turtleand-ux`.
