# Generate Slides Flow

_Remark_: It is important to make a template slides for chapter 1, so the AI can follow the style. I recommend using text-based typst.

---

## Step 1: Prepare Materials

**Human**: Prepare a lecture PDF or a chapter from a textbook `<chapter.pdf>`, and a template file `<slides.typ>`.

> The chapter PDF can be split from a textbook. AI cannot read large PDF files.

---

## Step 2: Generate Initial Slides

(Prompt)
```
Generate slides for lecture <chapter.pdf>, in typst format.
- based on <slides.typ>
```

---

## Step 3: Polish for Audience

(Prompt)
```
@slides.typ:30-80 make this slides friendly to non-experts.
Keep all highlighted text.
```

or

```
keep it simple, and please go to the key parameters (highlighted texts) more directly.
```

---

## Step 4: Draw Diagrams

(Prompt)
```
visualize this automaton at line 87
```

```
draw a <diagram description> with cetz.
```

```
Draw a <cellular automaton> about <topic> with cetz.
```

> For library-specific drawing, reference an existing example:
```
please draw automaton with the automaton lib, check @legacy/week1.typ .
```

---

## Powerful Prompts for Slide Design

### Examples and Stories
```
Come up with example about <concept>.
```

```
Cite the comments about <topic> from a famous person.
```

```
Present a story to highlight the importance of <concept>.
```

### Research Connections
```
List recent studies that connects <concept> to research frontier of AI.
```

### Format Conversion
```
@homeworks/hw1.txt to typst
```

### Consistency
```
The course name is "Theories in Computing", find all "Theory of Computation" and replace it with the correct name.
```

---

## Tips

1. **Use line references**: `@file.typ:30-40` for precise edits
2. **Keep template consistent**: AI learns from your template style
3. **Split large PDFs**: AI handles smaller chunks better
4. **Iterative polish**: Use "fix", "simplify", "continue" for refinement
