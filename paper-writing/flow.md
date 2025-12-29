# Paper Writing Flow

---

## Step 1: Prepare

**Human**: Create folder with note (method + results), plots, and a model paper for style.

---

## Step 2: Literature Review

(Prompt)
```
Based on <note-file>, generate literature review:
- use web search
- >30 citations
- markdown format
```

---

## Step 3: Plan the Story

**Human**: Make a plan. It contains a story telling, and the explanation of the method and result.

An example of `plan.md`:

```md
# Self correcting Rydberg atoms array (title: come up with a better one)

Use <model-paper> as template.

## TODO:
1. Review recent progress of Rydberg atoms array as a promising platform for quantum computing, based on <literature-review-report>.
2. Highlight the importance of quantum error correction.
3. Highlight the cost of moving and local addressing as a bottleneck.
4. Review the recent progress of having multiple species of atoms in the same device.
5. Main idea: with only global pulse and multiple species of atoms, without atoms moving and local addressing, can we realize error correction code?
6. Explain the method and result in this work based on <note-file>
```

---

## Step 4: Draft

(Prompt)
```
Implement plan.md, generate paper in <Physical Review X> style.
```

---

## Step 5: Human Review & Polish

**Human**: Review the paper draft, quote the specific part that needs improvement.

(Prompt)
```
@paper.tex:30-45 polish
```

```
Make sure all symbols and concepts are introduced before they are used.
```

```
please make sure the rest part consistent with the new notation.
```

---

## Powerful Prompts

```
Comment on how to improve to meet high standards of <journal>. Be critical.
```

```
Verify all facts in this paper.
```

### Diagrams
```
Draw a diagram about <topic> with tikz.
```
