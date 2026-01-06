# Vibe Coding

---

## High level wisdom
Before introducing the coding flow, I want to share some high level wisdom about coding. Even though by talking to AI, we can code easily, surprisingly, the philosophical thinking, including **math**, **algorithm**, **computational theory**, **modern software engineering** etc. are even more important in the era of vibe coding.
- math is domain specific. I will not touch on it in this flow.
- for algorithms, you must be familiar with common design patterns, such as greedy, dynamic programming, branching, optimization, integer programming et al.
- for computational theory, you must be familiar with common concepts, such as time complexity, space complexity, big O notation, etc. You should also understand the classification of computational hardness, such as P, NP, NP-complete, NP-hard, etc. You should be familiar with computational concepts, such as expression tree, Turing machine et al.
- for modern software engineering, you must be familiar with common tools, such as version control, code review, continuous integration, continuous deployment, etc. You should also understand the principles of software development, such as agile, scrum, waterfall, etc. You should be familiar with some common HPC concepts, such as MPI, OpenMP, CUDA, OpenCL, etc.

---

## Step 1: Make a plan (for those start from scratch)
Planning can be done by interacting with claude code.
Suggestions for AI to improve the code:
- let AI use local environment tools such as `uv`.
- let AI create a Makefile for common tasks, like building documentation.
- let AI setup CI/CD.
- let AI use gh to protect your main branch and automate the pull request process.


## Step 2: Let AI prove their work to you

Should I check the work done by AI line by line? No nessessarily. But you should check the following:

- improve the test coverage, design some tests that you think are important.
- generate a profiling report and create a benchmark.
- document the algorithm design and implementation.

## Step 3: Release
- bump the version number properly
- register the package with proper tool, e.g. crate, pypi, JuliaRegistrator etc.
- tag a new version on GitHub.