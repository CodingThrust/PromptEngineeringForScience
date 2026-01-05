# Prompt Engineering For Science

Human-AI collaboration workflows for scientific tasks.

[Warning: under construction.]

## Philosophy
- **Be open**: Describe what you need, not how to do it. Instead of "use Quantum ESPRESSO for DFT", ask "I want to simulate a hydrogen molecule—what are the approaches? Compare methods and suggest the best tool." Expect solutions beyond your assumptions.
- **Manage context**: Keep relevant files in your workspace—source code, examples, templates. Reference them with `@file` to ground AI responses.
- **Make a demo**: For batch tasks, polish one example first. Then ask AI to process the rest following that standard.

## Flows

| Category | Flows |
|----------|-------|
| [Paper Writing](paper-writing/flow.md) | Literature → Plan → Draft → Polish |
| [Coding](coding/coding-flow.md) | Build · Debug · Explain |
| [Research](research/flow.md) | Literature review · Gap identification |
| [Teaching](teaching/) | [Slides](teaching/slides-flow.md) · [Quiz](teaching/quiz-flow.md) · [Homework](teaching/homework-flow.md) · [Exam](teaching/exam-flow.md) · [Evaluation](teaching/evaluation-flow.md) |
| [MCP](workflow-automation/mcp-flow.md) | Build AI tool servers |

### Universal Workflow
1. **Human prepares** → materials, context
2. **AI generates** → drafts, suggestions
3. **Human reviews** → quality control
4. **Iterate** → "fix", "simplify", "continue"
