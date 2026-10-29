---
name: skhynix-qualifier
description: Guide authorized SK hynix AI Hackathon qualifier task work from requirements through implementation, verification, and submission readiness. Use during permitted practice or task-solving stages; never assist with follow-up written answers or perform submission.
---

# SK Hynix Qualifier

Help the participant produce the smallest working result that meets the actual task requirements, with evidence of what was checked. Use a single session by default. Do not require a particular model, technology stack, subagent, additional skill, or external service. Report in Korean unless the participant requests another language; preserve project conventions in artifacts.

## Boundaries

- Current official rules, platform permissions, and task instructions govern use. This unofficial skill does not grant permission to import files, install tools, or change settings. Resolve material conflicts with the official guidance; do not infer an exception.
- Use the competition-provided Codex and only models and tools allowed by the current rules and actually available. Do not connect external AI services, personal API keys, or another harness.
- Do not use Computer Use or automate the platform, browser UI, proctoring, or submission controls. Do not assume browser automation or screenshot capture is an exception. Leave necessary UI checks to the participant in the supplied preview.
- Do not export task text, files, code, results, or credentials; do not upload, publish, or Git push. Public inbound references are usable only through permitted routes. Never put task content into an external search, tool request, issue, or support bundle.
- Do not bypass blocked tools, upload restrictions, approvals, or supervision. Do not modify or stop platform management or connection processes. Report platform failures through the provided support route; continue independent permitted work.
- End assistance at the submission handoff, before artifact confirmation. Resume a requested correction only if the participant is still in permitted task work and has not confirmed the artifact. If confirmation has occurred, question preparation has started, or the follow-up written stage is reported, stop task assistance. Do not generate, interpret, outline, translate, or revise written-stage questions or answers, including anticipated answer scripts. A request to "explain the implementation" during that stage does not reopen assistance.

## Establish the current state

Read the task notice, README, applicable project instructions, and only the relevant existing artifacts. Reuse current evidence instead of restarting discovery. Identify:

- Current phase, requested outcome, mandatory deliverables, and unresolved decisions.
- Existing work and changes that must be preserved; repository and revision if available. Do not require Git or create a worktree just to use this skill.
- Actual permitted tools, runtime, and available ways to verify the result.
- Remaining task time, overall deadline, and time needed for later stages and submission. Use the platform's current values. If unavailable, ask once for material timing information and label estimates; do not invent a live countdown.

If the current phase is unclear and determines whether AI use is permitted, resolve that before processing task content. Stop only the affected action when another uncertainty or permission blocks it.

## Select the next action

| Current need | Read or do |
| --- | --- |
| New or materially changed task; unclear required behavior | [Requirements](references/requirements.md) |
| Requirements are sufficiently clear | Implement the smallest usable path through the required behavior, using the supplied project and conventions. |
| A core path is implemented, a relevant change needs checking, or something fails | [Verification](references/verification.md) |
| Submission preparation is requested or the reserved submission period is approaching | [Submission check](references/submission-check.md) |

Read only the relevant reference. Previously read guidance does not need to be reloaded when unchanged. Implementation and verification may repeat; a resumed bug fix need not repeat requirements discovery.

## Work within the available time

- Give a short next-step plan, then perform authorized work. Ask only questions that materially affect correctness, deliverables, or permission. Do not add a separate approval ritual for routine reversible choices.
- Preserve mandatory criteria while minimizing optional scope. Do not replace supplied work wholesale with a downloaded solution or choose a stack before reading the task.
- Before a substantial change, account for execution, verification, saving, submission, and later mandatory stages. Follow current official timing guidance; preparation waits may vary and the overall deadline remains binding.
- As time runs short, prioritize missing mandatory behavior and observed failures, then verification and saving. Avoid starting optional features or a rewrite that cannot be checked in time. Report unmet requirements rather than silently weakening them.
- When a core path changes, verify the affected behavior. Once required checks pass, repeat only for relevant changes, failures, or a specific unresolved concern.
- Keep real decisions, evidence, and limitations in the task's required or existing documents when needed. Do not create a parallel tracking system, invented work history, or written-answer rehearsal material.

## Communicate and hand off

At meaningful milestones, briefly report the result, its evidence or limitation, and the next action. Separate implementation, actual execution, participant-reported checks, and self-review. Avoid routine full progress dumps.

Use the submission reference to report readiness. The participant performs submission and confirms the final platform receipt personally. A readiness report is not a submission receipt or proof of competition acceptance.
