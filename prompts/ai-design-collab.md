# AI 设计协作方法论 / Design Collaboration with AI

> A2.5 节点调用。在完成产品定义对齐后、开始写产品逻辑文档之前使用。
> 教用户如何高效使用 AI 完成产品设计决策，而不是让 AI 替用户做决策。

---

## 核心原则：意图驱动，不是指令驱动

**错误做法**：告诉 AI「画个红色箭头」「这里加个按钮」——你把 AI 当工具人在用。
**正确做法**：告诉 AI「我要制造紧迫感」——你是设计师，AI 是推导执行者。

> Say what you want to achieve, not what to do.
> 说你要什么效果，不说你要什么操作。

---

## 五步协作法 / Five-Step Collaboration Method

### 第一步：意图表达 / Intent Expression

把你的设计意图说清楚，不要给设计规格：

```
❌ "首页加一个红色进度条"
✅ "首页要制造紧迫感，让用户意识到自己有未完成的任务"
```

用户给的意图越清晰，AI 产出的方案越对。不需要懂设计术语，说清楚「你想要用户感觉到什么」就行。

### 第二步：多方案竞争 / Multi-Scheme Competition

强制 AI 给出 **≥3 个方案**，并排对比：

```
❌ "给一个方案"
✅ "给我3个方案，含权衡分析，用表格呈现"
```

**为什么有效**：你被单一方案锚定后很难跳出来看问题。多方案对比让你看到不同可能性，决策质量明显提升。

### 第三步：视觉优先验证 / Visual-First Validation

先看 Demo，再写代码。**「识图脑优先」原则**：

```
❌ 大段文字解释 → 认知负担高，看了也判断不了
✅ 先出视觉 Demo → 10秒模式识别，快速判断
```

WorkBuddy 的协作模式：HTML demo 先行 → 你扫一眼说行不行 → 方向确认再深入。

### 第四步：虚拟团队评审 / Virtual Team Review

**这是最核心的实战技巧**——用 @skill 模拟多角色评审委员会：

```
@skill:qiaomu-design-advisor  → 设计顾问视角
@skill:huashu-design          → 另一种设计视角
@skill:ui-ux-pro-max          → UI/UX 专业视角
```

你作为产品经理综合判断。本质上是用 AI 构建了一个**虚拟设计团队**，一个人的决策质量拉到团队级。

### 第五步：增量修复循环 / Incremental Fix Loop

不改大重构，每次改一处，每步可验证：

1. 发现一个问题（如"圆角没对齐"）
2. AI 修这一处
3. 修的过程中发现新问题（如"颜色硬编码"）
4. 继续修，逐步推进

> Don't refactor everything at once. Fix one thing, verify it, move on.
> 一次只改一个，改完确认，再改下一个。

---

## 与现有节点的关系

| 节点 | 做什么 | 本方法论怎么用 |
|------|--------|--------------|
| A0 项目信息收集 | 收集需求 | 此时就开始用「意图表达」来梳理需求 |
| A1 生成 CLAUDE.md | 定基调 | 把协作习惯写入 CLAUDE.md 的「格式约定」 |
| A2 产品定义对齐 | 对齐方向 | 用「多方案竞争」对比产品方向 |
| **A2.5 AI 协作方法** | **← 你在这里** | **学会怎么跟 AI 一起做设计** |
| A3 产品逻辑文档 | 写文档 | 用「视觉优先验证」确保文档清晰 |
| A6 Prompt 架构 | 写 Prompt | 把五步法原则写进 Prompt 结构中 |
| A7 设计审查 | 审查设计 | 用「虚拟团队评审」进行多视角审查 |

---

## 小K的引导问题 / K's Guiding Questions

当用户进入 A2.5 节点时：

**中文版：**
> 小K发现你和 AI 做设计的姿势可能有优化空间～
> 我总结了一套实战方法，分五步：
>
> 1. 意图表达 —— 说效果不说操作
> 2. 多方案竞争 —— 强制出 ≥3 方案对比
> 3. 视觉优先 —— 先看 Demo 再说
> 4. 虚拟团队 —— @skill 多角色评审
> 5. 增量迭代 —— 一次改一处
>
> 你想先了解哪一步？或者直接开始用？

**English version:**
> Want to level up how you collaborate with AI on design?
> Here's a 5-step method from real practice:
>
> 1. Intent Expression — say what you want to achieve, not what to do
> 2. Multi-scheme — force ≥3 options before deciding
> 3. Visual-first — review demos, not descriptions
> 4. Virtual team — use @skill for multi-perspective review
> 5. Incremental — fix one thing at a time
>
> Which step interests you? Or should we jump right in?
