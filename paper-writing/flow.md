# Paper Writing Flow

A structured workflow for AI-assisted scientific paper writing.

---

## Step 1: Prepare Raw Materials

**Human**: Create a folder for the paper, and put the note and data to it.

```
paper/
├── note.md          # Brief description of method and main results
├── plots/           # Generated figures
├── model-paper.pdf  # Template paper to follow style
└── paper.bib        # Bibliography
```

> The note should contain method overview and main results (e.g. plots). The plots generation can also be automated.

---

## Step 2: Literature Review

(Prompt)
```
Based on the <note-file>, generate a literature review report
- use web search.
- contains >30 literature citations.
- in markdown format
```

---

## Step 3: Plan the Story

**Human**: Make a plan. It contains a story telling, and the explanation of the method and result.

An example of `plan.md`:

```md
# Self correcting Rydberg atoms array (title: come up with a better one)

Use <model-paper> as a template.

## TODO:
1. Review recent progress of Rydberg atoms array as a promising platform for quantum computing, based on <literature-review-report>.
2. Highlight the importance of quantum error correction.
3. Highlight the cost of moving and local addressing as a bottleneck.
4. Review the recent progress of having multiple species of atoms in the same device.
5. Main idea: with only global pulse and multiple species of atoms, without atoms moving and local addressing, can we realize error correction code?
6. Explain the method and result in this work based on <note-file>
```

---

## Step 4: Write the Draft

(Prompt)
```
Implement the plan in plan.md, generate a paper, in <Physical Review X> style.
```

---

## Step 5: Human Review & Polish

**Human**: Review the paper draft, quote the specific part that needs improvement.

### Line-specific editing
```
@paper.tex:30-45 polish
```

```
please polish the updated part of this paper (those changes not yet committed)
```

### Notation consistency
```
Please use the more standard DNF notation to represent D(R).
```

```
please also change the following tuple representation.
```

```
please make sure the rest part consistent with the new notation.
```

```
The energy notation now is H
```

---

## Step 6: Bibliography Management

(Prompt)
```
update @paper.bib:
- 10.22331/q-2020-06-04-279 may be a valid DOI for title: Graph-Theoretic Simplification of Quantum Circuits...
```

---

## Powerful Prompts

### Quality Control
```
Comment on how to improve the paper to meet the high standards of <Physical Review X>. Be critical and constructive.
```

```
Verify all facts in this paper.
```

```
Make sure all symbols and concepts are introduced before they are used.
```

### Diagrams
```
Draw a diagram about <topic> with tikz.
```

### Polish Chinese Text
```
优化这段中文：<text>
```

```
润色如下中文：<text>
```

### Simplify
```
简化这段话，保持核心要点
```

```
too much, simplify
```

---

## Tips

1. **Use line references**: `@file.tex:30-45` for precise edits
2. **Notation consistency**: Establish notation early, then enforce across paper
3. **Incremental polish**: Fix sections one at a time
4. **Verify citations**: AI may hallucinate; always check DOIs
5. **Keep uncommitted changes small**: Polish before committing
