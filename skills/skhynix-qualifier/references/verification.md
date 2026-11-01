# Verification

Verify mandatory behavior within the participant-requested unit with permitted tools under [Boundaries](../SKILL.md#boundaries). Routine tests and fixes inside that scope do not need repeated confirmation.

## Checks

- Exercise required input-to-output behavior and relevant invalid inputs, failures, and boundaries. Derive expected results from requirements, independently of implementation. Assert behavior, not unspecified wording.
- Reuse existing checks; add cases only for missing coverage or concrete risks. One check may cover several criteria. A build, linter, or running server alone proves no workflow; mocks do not prove real integration.
- Use project tests, CLI/data checks, or permitted local endpoints. Keep disposable fixtures in a permitted workspace location and preserve existing files. The participant performs necessary visual/UI checks in the supplied preview; otherwise mark them not run.
- Run checks as behavior becomes available. Relevant code/configuration changes invalidate affected results; rerun those checks on the final version. Do not repeat unchanged successful checks without a concrete concern.
- Optional platform cases need a reason. If blocked, record not run and continue; missing mandatory evidence still blocks readiness. Do not expand permissions to complete a check.

## Evidence

Record criterion, command/input or manual steps, expected/observed result, observer, and limit. Logs plus a short summary suffice; no required table or separate report.

Use **pass / fail / not run** (`통과 / 실패 / 미실행`). Pass requires observation. Distinguish agent execution, participant-reported checks, and review: file inspection or another AI's opinion is not execution evidence or independent behavioral validation. Read outputs and exit status; retain useful non-sensitive logs locally. Claims must stay within this evidence.

Connect important results to the briefed mechanism: which input reached which validation or processing path, what state changed, and what response was observed. Reference the relevant code location when useful. If a test only covers a mock or a single request, do not claim real integration or concurrent correctness. Keep this explanation short and separate from predicted examples in the briefing.

## Failures

Reproduce the smallest failing case; inspect errors and relevant changes, test a specific cause, fix minimally, then rerun the case and affected regressions. Preserve unrelated work. If the fix would materially change the agreed contract or mechanism, explain the consequence and obtain the participant's work request for that change. Never weaken criteria to pass or repeat an unchanged failed approach without new evidence.

For preview failures, inspect the app process, errors, port, allowed bind address, and route against environment guidance. Do not invent tunnels or platform-outage diagnoses. For platform/permission faults, keep time, stage, last action, and non-sensitive error for official support; follow Boundaries and continue independent work.

When a unit's checks pass, explain the observed result before moving to another unrequested unit. When all required work and checks are complete, proceed to handoff. If evidence is missing or a failure remains, report it explicitly.
