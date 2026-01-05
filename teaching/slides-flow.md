# Generate Slides Flow

_Remark_: It is important to make a template slides for chapter 1, so the AI can follow the style. I recommend using text-based typst.

---

## Step 1: Prepare

**Human**: Prepare `<chapter.pdf>` and template `<slides.typ>`.

> Split large PDFs. AI cannot read large files.

---

## Step 2: Generate

(Prompt)
```
Generate slides for lecture <chapter.pdf>, in typst format.
- based on <slides.typ>
```

---

## Step 3: Polish

(Prompt)
```
@slides.typ:30-80 make this friendly to non-experts.
Keep all highlighted text.
```

---

## Step 4: Diagrams

(Prompt)
```
visualize this automaton at line 87
```

> Reference existing examples:
```
draw automaton with the automaton lib, check @legacy/week1.typ
```

---

## Powerful Prompts

```
Come up with example about <concept>.
```

```
Cite comments about <topic> from a famous person.
```

```
Present a story to highlight the importance of <concept>.
```

```
List recent studies connecting <concept> to AI research frontier.
```

---

## Tips

1. **Line references**: `@file.typ:30-40` for precise edits
2. **Iterative**: Use "fix", "simplify", "continue"
