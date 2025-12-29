# Recommended prompt flow

## Step 1: Prepare raw materials
[Human]: Create a folder for the paper, and put the note and data to it. The note should contain a brief description of method and main results (e.g. plots).

The plots generation can also be automated, use your imagination.

Also, please copy a `<model-paper>` in this field to the working directory, so your paper can follow its style.

## Step 2: Literature review
[Prompt]:
```
Base on the <note-file>, generate a literature review report (in markdown format) on the background of the problem and related work, use web.
```

## Step 3: Plan a story
[Human]: Make a plan. An example of `plan.md` look like:
```md
# Self correcting Rydberg atoms array (title: come up with a better one)

Use <model-paper> as a template.

## TODO:
1. Review recently progress of Rydberg atoms array as a promising platform for quantum computing, based on <literature-review-report>.
2. Highlight the important of quantum error correction.
3. Highlight the cost moving and local addressing as a bottleneck.
4. Review the recent progress of having multiple species of atoms in the same device.
5. Main idea: with only global pulse and multiple species of atoms, without atoms moving and local addressing, can we realize error correction code?
6. Explain the method and result in this work based on <note-file>
```

It contains a story telling, and the explanation of the method and result is based on the `<note-file>`.

## Step 4: Write a paper draft
[Prompt]:
```
Implement the plan in plan.md, generate a paper, in <physical review X> style.

Comment on how to improve the paper to meet the high standards of <physical review X>. Be critical and constructive.
```

