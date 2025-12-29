# Vibe Coding

AI-assisted programming workflows for scientific computing.

---

## Case 1: Build a Project from Scratch

**Human**: Describe what you want to build in natural language.

(Prompt)
```
Build a <project-description>.
- use <language/framework>
- <key requirements>
- <constraints>
```

**Pro tips:**
- Start with a minimal working version, then iterate
- Specify the tech stack if you have preferences
- Include example input/output if possible

---

## Case 2: Add Features to Existing Code

**Human**: Put your codebase in the working directory or open it in Cursor.

(Prompt)
```
Add <feature> to this project.
- <requirements>
- follow the existing code style
```

---

## Case 3: Debug

**Human**: Copy the error message.

(Prompt)
```
I got this error:
<error-message>

Fix it.
```

**Pro tips:**
- Include the full traceback
- Describe what you were trying to do
- Mention what you've already tried

---

## Case 4: Refactor

(Prompt)
```
Refactor <file/function> to:
- <improvement goal>
- keep the same functionality
- add tests if not present
```

---

## Case 5: Code Review

(Prompt)
```
Review this code for:
- bugs
- performance issues
- readability
- best practices

Be critical and constructive.
```

---

## Case 6: Explain Code

(Prompt)
```
Explain what this code does:
<code-snippet>

Include:
- high-level purpose
- step-by-step breakdown
- any potential issues
```

---

## Case 7: Write Tests

(Prompt)
```
Write unit tests for <file/function>.
- use <testing framework>
- cover edge cases
- aim for high coverage
```

---

## Case 8: Optimize Performance

(Prompt)
```
Optimize this code for <speed/memory>:
<code-snippet>

Explain the trade-offs.
```

---

## Powerful Prompts

```
Make it work, then make it right, then make it fast.
```

```
Simplify this code without changing its behavior.
```

```
What's the idiomatic way to do <task> in <language>?
```

```
Convert this <algorithm/pseudocode> to <language>.
```

```
Generate documentation for this codebase in <format>.
```

---

## Tips for Vibe Coding

1. **Trust but verify**: Run the code, don't just read it
2. **Iterate quickly**: Get something working, then refine
3. **Be specific**: Vague prompts produce vague code
4. **Show examples**: Input/output examples beat long descriptions
5. **Use context**: Keep related files open so AI has full context
