# Prompt Engineering For Science

Human-AI collaboration workflows for scientific tasks.

## Philosophy
- _Be open_: Be open to potential solutions. Do not preassume the solution, just describe what you need! e.g. instead of "use DFT to simulate a hydrogen molecule, use quantum espresso", you can ask "I want to simulate hydrogen molecule, what are the possible approaches? Compare pros and cons of different methods, make suggestions for the best software for this task". You should always expect LLM to come up with a solution beyond your expectation.
- _Manage context_: Keep all relevant information in your workspace. Refer to the most helpful information when needed, e.g. package source code, previous examples, etc. It will make your prompts much easier.
- _Make a demo_: Imagine you want to use AI for processing multiple similar tasks. You should pick one task and make a polished demo. Then ask AI to process the rest of the tasks.

## Flows

| Category | Flows |
|----------|-------|
| [Paper Writing](paper-writing/flow.md) | Literature → Plan → Draft → Polish |
| [Coding](coding/coding-flow.md) | Build · Debug · Explain |
| [Research](research/flow.md) | Literature review · Gap identification |
| [Teaching](teaching/) | [Slides](teaching/slides-flow.md) · [Quiz](teaching/quiz-flow.md) · [Homework](teaching/homework-flow.md) · [Exam](teaching/exam-flow.md) · [Evaluation](teaching/evaluation-flow.md) |
| [MCP](workflow-automation/mcp-flow.md) | Build AI tool servers |

### Univeral workflow
1. **Human prepares** → materials, context
2. **AI generates** → drafts, suggestions
3. **Human reviews** → quality control
4. **Iterate** → "fix", "simplify", "continue"
