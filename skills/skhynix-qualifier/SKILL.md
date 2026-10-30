---
name: skhynix-qualifier
description: Guide authorized SK hynix AI Hackathon qualifier practice and task work (SK하이닉스 예선, 과제풀이, 해커톤 과제) through requirements, implementation, verification, and submission readiness. Use only in permitted task stages; exclude follow-up written answers and submission execution.
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

Within those boundaries, reading and editing project files, running local tests and servers, and installing project dependencies (for example, `pip install` or `npm install`) are ordinary task work when the environment guidance permits them. Use existing authorization without asking again; it does not extend to global tools, settings, or unapproved network access. Inspect unfamiliar scripts and install hooks for external effects once, and reassess when the command, configuration, dependency, or destination changes. Routine reuse of an inspected local command needs no new approval ritual.

## Establish the current state

Read the task notice, README, applicable project instructions, and only the relevant existing artifacts. Reuse current evidence instead of restarting discovery. Identify:

- Current phase, requested outcome, mandatory deliverables, and unresolved decisions.
- Existing work and changes that must be preserved; repository and revision if available. Do not require Git or create a worktree just to use this skill.
- Actual permitted tools, runtime, and available ways to verify the result.
- Any stated deadline and official timing requirements for later stages and submission. Ask about missing timing only when it changes the next decision; otherwise continue without inventing a countdown or time allocation.

If the current phase is unclear and determines whether AI use is permitted, resolve that before processing task content. Stop only the affected action when another uncertainty or permission blocks it.

## Continue from the current result

Move directly to the next needed action once its prerequisites are met. There are no fixed-duration stages or percentage reserves. Reuse the task's acceptance criteria and current evidence instead of making a second checklist or repeating discovery. Run a relevant baseline command when it will resolve uncertainty about existing behavior; an explicitly unimplemented starter needs no ceremonial failure run. This does not replace verification of the implemented result or any task-required check.

| Current need | Read or do |
| --- | --- |
| Required behavior or deliverables are unclear | [Requirements](references/requirements.md); stop discovery once the next implementation decision is supported. |
| Requirements are sufficiently clear | Implement the smallest usable path through the required behavior, using the supplied project and conventions. |
| A core path is implemented, a relevant change needs checking, or something fails | [Verification](references/verification.md) |
| Mandatory behavior and its evidence are ready, handoff is requested, or an actual deadline requires a final status | [Submission check](references/submission-check.md) |

Read only the relevant reference. Previously read guidance does not need to be reloaded when unchanged. Implementation and verification may repeat; a resumed bug fix need not repeat requirements discovery.

## Keep work proportional

- Give a short next-step plan, then perform authorized work. Ask only questions that materially affect correctness, deliverables, or permission. Do not add a separate approval ritual for routine reversible choices.
- Preserve mandatory criteria while minimizing optional scope. Do not replace supplied work wholesale with a downloaded solution or choose a stack before reading the task.
- Honor actual deadlines and official handoff requirements. Prioritize missing mandatory behavior, observed failures, verification, and saving; use the remaining work to decide what is feasible. Report unmet requirements rather than silently weakening them.
- When a core path changes, verify the affected behavior. Once required checks pass, repeat only for relevant changes, failures, or a specific unresolved concern.
- Keep real decisions, evidence, and limitations in the task's required or existing documents when needed. Avoid a parallel tracking system or invented work history; apply Boundaries to later-stage requests.

## Communicate and hand off

At meaningful milestones, briefly report the result, its evidence or limitation, and the next action, then continue authorized work without a separate stage-completion approval. Separate implementation, actual execution, participant-reported checks, and self-review. Reuse this evidence at handoff; create a separate report file only when the task requires one or an existing project record needs updating.

Example format only; replace every value with actual observations:

```text
구현: CSV 입력부터 집계 출력까지 연결했고, 필수 요건 5개 중 3개를 확인했습니다.
검증: 통과 3 / 실패 1 / 미실행 1 — 에이전트가 로컬 테스트를 실행했고, 빈 입력 처리가 실패했습니다.
다음: 빈 입력 처리를 수정하고 재검증합니다. 화면 확인은 참가자 관찰이 필요합니다.
```

Use the submission reference to report readiness. The participant performs submission and confirms the final platform receipt personally. A readiness report is not a submission receipt or proof of competition acceptance.
