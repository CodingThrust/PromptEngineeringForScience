# Data Analysis Flow

AI-assisted workflows for scientific data analysis.

---

## Flow 1: Exploratory Data Analysis

### Step 1: Load and Inspect

**Human**: Put your data file in the working directory.

(Prompt)
```
Load <data-file> and provide:
- Summary statistics
- Data types and missing values
- Distribution of key variables
- Initial observations
```

### Step 2: Visualize

(Prompt)
```
Create exploratory visualizations for <data-file>:
- Distribution plots for numerical variables
- Correlation heatmap
- Time series plots (if applicable)
- Highlight any anomalies
```

### Step 3: Document Findings

(Prompt)
```
Summarize the key findings from this exploratory analysis:
- Main patterns observed
- Potential issues (outliers, missing data, etc.)
- Hypotheses to investigate further
```

---

## Flow 2: Statistical Analysis

### Step 1: Plan Analysis

(Prompt)
```
What statistical tests are appropriate for:
- Research question: <question>
- Data: <description of variables>
- Sample size: <n>

Explain assumptions and alternatives.
```

### Step 2: Run Analysis

(Prompt)
```
Perform <statistical test> on <data>:
- Check assumptions first
- Report effect sizes and confidence intervals
- Interpret results in context
```

### Step 3: Visualize Results

(Prompt)
```
Create publication-quality figures showing:
- <main results>
- Use <journal style> formatting
- Include appropriate error bars/confidence intervals
```

---

## Flow 3: Machine Learning Pipeline

### Step 1: Problem Setup

(Prompt)
```
Set up a ML pipeline for:
- Task: <classification/regression/clustering>
- Target: <variable to predict>
- Features: <available variables>

Recommend preprocessing steps.
```

### Step 2: Model Selection

(Prompt)
```
Compare different models for <task>:
- Train-test split appropriately
- Use cross-validation
- Report relevant metrics
- Visualize performance
```

### Step 3: Interpretation

(Prompt)
```
Interpret this ML model:
- Feature importance
- SHAP values or similar
- Explain predictions for specific examples
```

---

## Flow 4: Reproducible Analysis

### Step 1: Environment Setup

(Prompt)
```
Create a reproducible analysis environment:
- requirements.txt with pinned versions
- Makefile or script for full pipeline
- README with instructions
```

### Step 2: Document Analysis

(Prompt)
```
Convert this analysis into a Jupyter notebook:
- Include markdown explanations
- Show intermediate results
- Add comments for key decisions
```

---

## Powerful Prompts for Data Analysis

```
What's wrong with this analysis? Be critical.
```

```
What alternative interpretations exist for these results?
```

```
How would a skeptical reviewer critique this analysis?
```

```
Suggest robustness checks for <finding>.
```

```
What would happen if we removed <subset of data>?
```

```
Generate synthetic data with known properties to validate this method.
```

---

## Tips

1. **Check AI-generated code**: Always run and verify before trusting
2. **Understand the method**: Don't just run what AI suggests; understand why
3. **Version control**: Track your analysis in git
4. **Reproducibility**: Document random seeds, package versions, data versions
5. **Sanity checks**: Always verify results make sense in context
