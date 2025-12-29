# Grant Proposal Flow

AI-assisted workflow for writing grant proposals and project reports.

---

## Step 1: Prepare Materials

**Human**: Gather project guidelines and reference materials.

```
proposal/
├── material.txt     # Project guidelines (整体指南)
├── hunan.typ        # Your responsible section
├── personal.md      # Team member profiles
└── report.typ       # Output proposal
```

---

## Step 2: Draft Based on Guidelines

(Prompt)
```
根据 @hunan.typ （负责的部份） 和 @material.txt （项目整体指南）完成 @report.typ 。
负责的部份是 materials.txt 中核心指标3-5，所以仅仅需要完成约1/2的内容，约2000字内容。
```

---

## Step 3: Add References

(Prompt)
```
请列举出具体参考文献。
```

```
在正文中引用，谢谢
```

---

## Step 4: Fact Check and Correct

(Prompt)
```
纠正文中的事实性错误，让引文和事实描述相符，添加引文链接，确保事实可查证。
```

```
纠错码方面，量子LDPC码不是解码器，请修正。
```

---

## Step 5: Align with Project Goals

(Prompt)
```
选中部份，请按照修改后的技术路线调整核心技术，创新点和先进性。
```

```
把GPU的研究内容合并到Clifford模拟中。作为同一个研究内容的不同阶段，适当简化。
```

---

## Step 6: Simplify and Focus

(Prompt)
```
简化核心技术到3个
```

```
不要明确标注阶段。
```

```
保留基金申请最重要的部份
```

---

## Step 7: Team Introductions

(Prompt)
```
模仿劳玲玲的介绍，参考 @personal.md 里面的资料，介绍刘金国。
```

```
参考下面的资料，以及上面上海交通大学的介绍格式，介绍香港科技大学（广州）
```

---

## Step 8: Final Adjustments

(Prompt)
```
我修改了预期成果及水平，现在我只需要负责一个研究内容：大规模高性能量子模拟器实现技术。
技术路线还是一个内容两个点这么写。
```

```
让研究内容部份行文更加适合阅读
```

---

## Powerful Prompts

### Length Control
```
稍微把香港科技大学（广州）的介绍拓展下
```

```
简化算力介绍，保持长度差不多
```

```
还是太长了
```

### Structure Adjustment
```
整合内容2-4为一点
```

```
1和4为一点，2和3为一点
```

```
针对研究内容，对第6部份作修改。技术路线每个内容写两个点。
```

### Keep Headers Stable
```
不要改标题
```

---

## Tips

1. **Follow guidelines strictly**: Always reference the project指南
2. **Match style**: Use existing team member intros as templates
3. **Fact-check citations**: Ensure all claims are verifiable
4. **Control length**: Grant proposals have strict word limits
5. **Iterate on structure**: Combine/split sections as needed
