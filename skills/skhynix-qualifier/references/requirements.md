# Requirements

Use when required behavior or deliverables are insufficiently clear to select an implementation. A new task with clear acceptance criteria can proceed directly to implementation. Stop analysis when the next implementation decision is supported.

## Extract what matters

From the actual task notice, README, supplied files, and confirmed clarifications, identify:

- The user or business need and the required observable outcome.
- Mandatory behavior, inputs and outputs, constraints, and any stated evaluation criteria.
- Required artifacts, filenames, paths, formats, and execution instructions.
- The smallest complete path that satisfies the requirements and what can remain optional.

Treat tutorial screenshots, sample ports, example apps, and example document names as examples unless the task makes them requirements. Do not infer a web app, a particular language, or hidden scoring weights from the environment guide.

## Distinguish evidence from assumptions

Reuse supplied acceptance criteria and add only missing checks, sources, or material assumptions. Use a compact checklist or table when it helps; a second specification is unnecessary:

| Requirement or decision | Source and certainty | Priority | Observable completion check |
| --- | --- | --- | --- |

Mark an item as explicitly required, confirmed by an authorized clarification, or an assumption. Prioritize mandatory behavior before optional improvements. A plausible assumption is not an official requirement or a participant decision.

Use current official rules for permitted actions and the task instructions for deliverables. Use stakeholder clarification to resolve business ambiguity, without treating it as authority to override competition rules. When sources materially conflict, identify the conflict and seek the appropriate clarification.

## Ask only decision-changing questions

First inspect available task evidence. Ask a concise question when the missing answer changes the approach, completion criteria, or permitted action. Proceed with a reversible, disclosed assumption for minor details when the task allows it.

Route business-context questions to the supplied stakeholder or business agent, platform-operation questions to the supplied helper, and technical platform faults to the official reporting route. Where these require UI interaction, ask the participant to perform it; do not automate that interaction.

### Questions for the supplied business agent

Use the authorized in-platform route under [Boundaries](../SKILL.md#boundaries). Select the unresolved question that changes implementation; do not send a fixed questionnaire or contact an external person. These Korean templates are examples, not assumed answers:

- Outcome: "이 결과를 보고 누가 어떤 결정을 내려야 하나요? 반드시 보여야 할 정보는 무엇인가요?"
- Ambiguous rule: "[문서의 규칙]을 [해석 A]로 이해했습니다. [경계 사례]도 같은 방식으로 처리하나요, 아니면 [해석 B]인가요?"
- Error handling: "[잘못된 입력]이 있으면 해당 항목만 제외하고 이유를 보여줄까요, 아니면 전체 처리를 중단해야 하나요?"
- Priority: "필수 [A]와 추가 요청 [B] 중 먼저 완성할 것은 무엇인가요? 현재 안내에서 [A]는 필수이므로 [B]는 추가 범위로 이해해도 될까요?"

Record the actual answer, its source, and the affected criterion in the existing checklist. Turn a confirmed business rule into a concrete input/expected-output check. If no answer arrives, continue independent work and label any reversible assumption; leave a decision that changes mandatory behavior unresolved rather than inventing stakeholder approval. Stakeholder preferences cannot waive explicit task requirements or competition rules.

## Leave a usable next step

Return the short completion criteria, mandatory-first implementation order, and any blocking question or material assumption. Continue authorized implementation once sufficiently clear. Do not create an extensive specification, choose a stack prematurely, or add optional features merely to make the plan look complete.
