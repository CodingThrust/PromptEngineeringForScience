# Recommended prompt flow

## Step 1: Prepare raw materials
(Human)
> Create a folder for the paper, and put the note and data to it. The note should contain a brief description of method and main results (e.g. plots). Copy a `<model-paper>` to the working directory, so your paper can follow its style.


The plots generation can also be automated, use your imagination.

## Step 2: Literature review
(Prompt)
```
Base on the <note-file>, generate a literature review report
- use web search.
- contains >30 literature citations.
- in markdown format
```

## Step 3: Plan a story
(Human)
> Make a plan. It contains a story telling, and the explanation of the method and result.

An example of `plan.md` look like:

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


## Step 4: Write a paper draft
(Prompt)
```
Implement the plan in plan.md, generate a paper, in <physical review X> style.
```

## Step 5: Human review
(Human)
> Review the paper draft, quote the specific part of the paper that needs improvement. Use clear prompts to fine tune the paper.

## Other very powerful prompts

(Prompt)
```
Comment on how to improve the paper to meet the high standards of <physical review X>. Be critical and constructive.
```

```
Verify all facts in this paper.
```

```
Make sure all symbols and concepts are introduced before they are used.
```

```
Draw a diagram about <topic> with tikz.
```