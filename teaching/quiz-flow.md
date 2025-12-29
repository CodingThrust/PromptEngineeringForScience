# Generate Quiz Flow

Generate quizzes based on lecture notes and textbooks.

---

## Step 1: Prepare Materials

**Human**: Organize lecture PDFs and textbook in a folder structure.

```
course/
├── textbook/
│   └── textbook.pdf
├── lectures/
│   ├── lec1.pdf
│   └── lec2.pdf
└── quizzes/
    └── week1/
```

---

## Step 2: Generate Quiz

(Prompt)
```
Prepare quiz for week1, covering the contents in lectures/lec1.pdf and lectures/lec2.pdf.
Please refer to the textbook in @textbook.
```

---

## Step 3: Scale to Full Course

(Prompt)
```
Good job! Continue to generate the quiz for week 3 to 13.
```

---

## Step 4: Polish and Format

(Prompt)
```
@week1/week1.typ:30-40 polish
```

```
make it suited for slides
```

```
@week1/week1.typ:33-46 organize better
```

---

## Tips

1. **Reference textbook**: Always point AI to the authoritative source
2. **Batch generation**: After verifying week 1, generate remaining weeks
3. **Use line references**: For precise polishing of specific sections
4. **Follow template**: Reference previous quizzes for consistency
