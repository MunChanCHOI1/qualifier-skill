# Requirements

Use when an implementation decision lacks evidence or a new implementation unit needs a participant-facing briefing. Reuse an existing briefing while its scope and mechanism remain unchanged.

- Combine the participant's stated goal with relevant supplied materials to identify the business outcome, mandatory behavior, inputs/outputs, constraints, deliverable paths/formats, and execution instructions. Summarize the decision-relevant requirements with their source location so the participant can inspect them naturally; do not dump files or turn reading into a compulsory exercise.
- Reuse acceptance criteria; add only missing checks, sources, or material assumptions. Distinguish explicit requirements, authorized clarifications, and assumptions. Examples do not mandate a stack, app type, or hidden scoring rule.
- Ask only questions that change correctness, scope, or permission. For minor reversible details, disclose an assumption and continue. Resolve material source conflicts; stakeholder preferences cannot waive task requirements or official rules.

## Principle briefing before implementation

Help the participant see what will happen and why before asking them to request the work. Keep it proportional: a small change may need only a few sentences; an API with persistent state may need a flow and a concrete example. Use ordinary Korean, explain technical terms, and relate each concept to this feature rather than giving a generic development lecture.

Cover the relevant parts, without forcing every item into every reply:

- **Outcome and source:** what the user can do, the requirement it satisfies, and any assumption requiring a choice. Distinguish required behavior from a suggested implementation.
- **Mechanism:** trace input → validation → business logic → storage or external interaction → response. Omit nonexistent stages. For an API, explain its request method/path, input fields, success/error response, and where state lives. Distinguish the interface clients call from the server logic that handles it.
- **Concrete example:** follow one small illustrative input to its expected output and one meaningful failure or boundary. Mark invented examples as illustrative; they are neither observed tests nor actual task data.
- **Reason and limit:** why this approach fits, and a consequential tradeoff when one exists. For example, in-memory state disappears on restart; persistent storage has different behavior. Do not invent authentication, transactions, concurrency handling, or persistence the plan does not include.
- **Work to request:** state the coherent scope, the checks it needs, and any real choice. Make a recommendation rather than asking the participant to design every detail.

Show the briefing in the conversation, not only in a generated file. A compact shape to adapt:

```text
만들 동작: [목표와 확인할 요구사항 위치]
처리 흐름: [입력] → [검증] → [핵심 처리] → [결과]
예시: [입력]이면 [결과], [실패 조건]이면 [처리]
이유·한계: [선택 이유와 중요한 한계]
작업 범위: [구현할 기능과 확인할 동작]
```

Then leave the work request to the participant under the entrypoint's participant-directed loop. If they ask "why?" or "what is an API?", explain with this flow and keep implementation pending. An optional understanding check is conversational support, never a mandatory quiz or an inferred approval. Once work is requested, proceed within that scope without requiring another confirmation.

After implementation, replace predictions with actual code locations and test observations. Explain changes to the proposed mechanism and unresolved limitations. Do not turn the explanation into a memorized answer for anticipated follow-up questions; the written-stage cutoff still applies.

## Stakeholder questions

Under [Boundaries](../SKILL.md#boundaries), route business questions to the supplied stakeholder/agent, platform questions to the helper, and faults to official support. The participant performs any required UI interaction; do not contact external people.

Choose only the unresolved question, for example:

- "누가 어떤 결정을 위해 이 결과를 사용하나요?"
- "[규칙]을 [A]로 이해했습니다. [경계 사례]도 같나요, 아니면 [B]인가요?"
- "[오류 입력]은 항목만 제외하나요, 전체를 중단하나요?"

Record the actual answer/source and affected criterion in the existing record; turn the rule into an input/expected-result check. Without an answer, continue independent work, label assumptions, and leave mandatory decisions unresolved. Do not invent stakeholder approval or a second specification.
