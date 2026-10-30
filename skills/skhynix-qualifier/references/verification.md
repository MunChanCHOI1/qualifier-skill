# Verification and Error Resolution

Use after a meaningful implementation change, when a failure appears, and before a claim of readiness. Verify the actual mandatory behavior with available permitted means.

## Select checks that establish the claim

- Exercise a representative path from required input to observable output.
- Include relevant invalid input, failure conditions, and boundary cases based on the actual requirements. Do not generate an exhaustive suite unrelated to the change.
- Use appropriate project tests, build or lint checks, CLI runs, local data checks, or permitted local endpoint requests under [Boundaries](../SKILL.md#boundaries), including its guidance for inspected commands.
- A running server, successful build, or passing linter alone does not prove the required workflow works. Mock or synthetic results do not establish integration with a real system.
- When a visual or interactive check is necessary, have the participant use the supplied preview. Do not automate it or capture the exam screen. If manual confirmation is unavailable, record the affected check as not run.

## Map requirements to runnable smoke checks

Map each mandatory behavior to a reproducible check with a representative input and an expected observable result derived from the task. Reuse existing tests first; add a case when coverage is missing or a concrete failure risk needs checking. One existing check may cover several criteria; no separate script, case, or document is required for every row. Use a small local script only when it makes repeated checks easier than manual commands.

For example, a CSV aggregation task might map valid rows to exact totals, malformed input to the required error/exit behavior, and repeated runs to unchanged supplied files. Include the task's actual boundary rules rather than assuming these examples are requirements. Assert outputs and errors, not just exit code zero or server startup. Keep expected results independent of the implementation being tested.

Run the first path's smoke check early, add cases for remaining mandatory behavior, and rerun affected checks after corrections. For behavior that only the participant can observe, record reproducible manual steps and leave it not run until that observation arrives.

Keep test scope tied to requirements and observed risks. Platform-specific optional cases need a concrete reason; they are not a prerequisite for handoff. If an optional check is blocked, record it as not run and continue without expanding permissions. A blocked mandatory check still prevents readiness. Use a permitted workspace location for disposable test fixtures when supported, preserving supplied files and existing data.

## Record observable evidence

For each necessary check, record enough to understand and, where allowed, repeat it. Existing test output plus a concise summary is sufficient if it contains these fields; the table is optional:

| Criterion | Command, input, or manual steps | Expected and observed result | Status | Evidence source and limit |
| --- | --- | --- | --- | --- |

Use **pass / fail / not run** (`통과 / 실패 / 미실행`). Use pass only when the relevant result was observed, and identify who observed it. Participant-reported manual success is not an agent-executed test. File review and another AI's opinion are reviews, not execution evidence or independent validation of behavior.

Read actual outputs and exit status. Preserve useful logs inside the permitted workspace when needed without exposing secrets. Limit a claim to what its evidence establishes. Relevant code or configuration changes invalidate affected earlier results; rerun those checks on the final version.

## Investigate failures

1. **Observe:** Reproduce the smallest failing case when possible. Inspect the error, relevant logs, and recent changes. Preserve unrelated work.
2. **Hypothesize:** State a specific cause and the observation that would distinguish it from alternatives. Do not declare a platform outage without evidence.
3. **Change minimally:** Make the smallest justified correction to participant-owned work. Avoid unrelated refactoring or weakening tests to obtain a pass.
4. **Recheck:** Reproduce the original case, then run affected regression checks. Update the evidence and remaining limitations.

Do not repeat an unchanged failed approach without new evidence. If cause or verification remains uncertain, report it and choose the next useful observation within the remaining time.

For a web preview connection problem, check the application's actual running process, errors, port, permitted bind address, and route. Follow the current environment guide; do not invent a tunnel or change platform networking to bypass a restriction.

For platform, supervision, or blocked-permission failures, retain the time, affected stage, last action, and non-sensitive error text for the provided reporting route. Do not modify management processes or security settings. Continue unrelated permitted work where possible.

## Finish with a bounded conclusion

Report passed, failed, and unexecuted required checks and the remaining limitations. A known failure needs correction; a missing observation remains unverified. Stop retesting unchanged successful behavior unless a concrete concern remains. Move to submission checking when implementation and required evidence are ready, or when time requires an honest final status.
