# Evaluation Flow

## Merge PRs

**Human**: Clone the homework repo to working directory.

(Prompt)
```
Merge PRs to this repo, use gh.

Requirements: 
1. each user has his own folder, PR only modifies owner's folder
2. for multiple PRs with conflicts, merge the most suited one
3. use squash and merge
4. no files larger than 10M

For PRs hard to decide, list them in chat.
```

---

## Analyze Submissions

(Prompt)
```
Base on submissions, for student XXX, make a table:
- rows: assignments
- cols: execution output included? first submission date? AI generated? correctness (0-100)? completeness (0-100)?
```

**Human**: Check output, if good:

(Prompt)
```
Implement the same for other students, summarize into markdown.
```

---

## Score

(Prompt)
```
Based on the markdown file, rank students:
- A+: best 1-2
- A: <30%
- A-: 30-40%
- B+: 40%-70%
- B: 70%-93%
- B-: 93%-100%

First submission doubled. AI submission halved.
```
