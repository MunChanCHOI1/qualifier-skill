# Submission Readiness

Use before the participant confirms the artifact. This check ends with a readiness judgment; it never clicks, submits, uploads, or confirms on the participant's behalf.

## Compare the final result with the task

- Match each mandatory requirement to the actual artifact and its relevant verification evidence. Reuse current evidence; do not rerun all checks solely to produce a new report.
- Confirm required filenames, paths, formats, and contents against the actual task. Do not require extra documents that the task does not request.
- Ensure the execution instructions match the final project, including necessary runtime, dependencies, inputs, and start or test commands. Do not claim an unexecuted clean-environment run occurred.
- Reconcile described behavior, design choices, verification results, and limitations with what was actually implemented. Do not invent participant decisions or prepare follow-up written answers.
- Inspect the final saved files. Ask the participant to confirm any editor-only unsaved changes or external-change conflicts that tools cannot observe. Preserve both versions until the conflict is understood; do not overwrite blindly.
- Check the final changes for unrelated edits, broken references, and unintended sensitive content. Do not delete supplied or existing files merely to make the submission look tidy.

## Account for the platform handoff

Reserve the time required by the current official instructions. Preview or preparation time may still count against a deadline. Do not treat a preview listing as the complete submitted file inventory unless the platform explicitly guarantees that.

The participant personally checks the preview, resolves any remaining save conflicts, and chooses whether to confirm. Confirmation freezes the artifact under the platform's rules. End AI task assistance before that action, including during any subsequent question-preparation wait.

## Return one judgment

| Judgment | When it applies |
| --- | --- |
| **Ready / 제출 준비됨** | Mandatory artifacts, required behavior, sufficient verification, and saved state are confirmed. Disclose any non-blocking limitation. |
| **Needs changes / 수정 필요** | A mandatory criterion is known to fail, a required artifact is missing, or a known save conflict remains. State the smallest required correction. |
| **Cannot determine / 확인 불가** | A mandatory criterion cannot be judged because necessary evidence or access is missing. State the missing observation. |

An optional unexecuted check does not automatically block readiness. Missing evidence for a mandatory criterion does. If both a known failure and uncertainty exist, report **Needs changes** and include the unresolved uncertainty.

Keep the handoff concise: judgment and reason, artifact locations and execution method, required-check results, remaining limitations, and the participant's next manual step. If a correction is still feasible and authorized, return to implementation and affected verification before handing off.

Do not claim final submission is complete. The participant verifies the platform's final receipt after completing all required personal stages. If asked for written-stage assistance, provide only a brief stop notice and no substantive answer help.
