# Claude Code Skills — 使用 SOP

## 一句话总结

在对话中出现特定信号词/场景时，系统自动匹配对应 skill，agent 按方法论框架输出结构化的分析/决策辅助。

## 使用方式

直接说触发场景的话即可，无需特殊格式：

```
"用 XXX 帮我分析 YYY"
"我觉得 ZZZ，帮我检查一下"
直接描述问题，系统自动匹配
```

---

## 一、投资决策场景

### 你刚发现一个投资机会

```
先走: know-thy-time          → "我有足够的时间研究吗？"
再走: circle-of-competence   → "这个行业我懂吗？"
再走: business-picker        → "这是一个好企业吗？"
再走: economic-moat          → "它的护城河在哪？"
再走: aesop-three-questions  → "它值多少钱？"
再走: margin-of-safety       → "现在的价格够低吗？"
```

### 你在纠结要不要卖

```
先走: loss-aversion          → "我是因为怕亏损才不卖吗？"
再走: mr-market              → "我是在听市场先生的报价吗？"
再走: hold-forever           → "如果永远不能卖我还买这个吗？"
```

### 你看到市场狂热/恐慌

```
fear-and-greed               → "现在是该逆着市场走的时候吗？"
availability-heuristic       → "我是被最近新闻影响了吗？"
```

### 你在选合作伙伴/管理层

```
partner-with-admired         → "我愿意和这些人长期合作吗？"
ceo-as-risk-officer          → "CEO把风控放在第一位吗？"
real-conservatism            → "随大流≠保守，我独立思考了吗？"
```

### 你在评估财务报表

```
look-through-earnings        → "穿透会计数字看真实盈利"
first-law-of-capital-allocation → "留存收益能创造价值吗？"
float-thinking               → "有低成本资金来源吗？"
```

### 你在做资产配置

```
three-asset-categories       → "货币/黄金/股票/房产，选哪个？"
compounding-thinking         → "时间维度上复利怎么起效？"
```

### 你准备用杠杆/融资

```
no-leverage                  → "永远不要用杠杆"
never-issue-shares           → "用现金不用股票做收购"
cigar-butt-vs-great-business → "便宜差公司 vs 合理价好公司"
institutional-imperative     → "组织为什么总做蠢事？"
```

---

## 二、问题解决场景

### 你有一个"模糊的问题"

```
先走: check-your-lights           → "我的灯亮着吗？我先理解对了吗？"
再走: problem-definition-formula  → "期望是什么？体验是什么？差距在哪？"
再走: problem-analysis-3steps     → "谁有问题？各自的问题是什么？从哪来？"
再走: dont-mistake-solution-for-problem → "你说的这个'问题'是不是其实是个方案？"
```

### 你卡住了，只想得到常规答案

```
problem-restatement          → "换个说法重新描述这个问题"
foreign-perspective          → "用盲人/外国人/孩子的视角看"
```

### 方案刚上线，又出新问题

```
solution-chain-awareness     → "每种方案都会生新问题，预判3个"
regression-to-mean           → "这次变好/变坏是真的效果还是回归均值？"
```

---

## 三、管理与执行场景

### 你感觉"太忙了，时间不够"

```
know-thy-time                → "记录2周时间日志，砍25%"
first-things-first           → "一次只做一件事，做最重要的"
```

### 你在思考"我该做什么"

```
contribution-focus           → "我能贡献什么？（成果/价值观/人才）"
effectiveness-learnable      → "卓有成效是可以学会的，不是天赋"
```

### 你在招人/组队/评绩效

```
strengths-based              → "这个人擅长什么？怎么让长处发挥？"
```

### 你要做重要决策

```
effective-decisions          → "先判断是偶发还是经常性问题"
two-systems                  → "系统1直觉还是系统2分析？"
overconfidence               → "用区间预测校准自信"
```

---

## 四、认知偏见自检场景

| 你说的话 | 可能的问题 | 检查用 |
|---------|-----------|--------|
| "肯定涨" | 过度自信 | `overconfidence` |
| "最近老看到" | 可得性偏误 | `availability-heuristic` |
| "亏了不想卖" | 损失厌恶 | `loss-aversion` |
| "市场价是X" | 锚定效应 | `anchoring-effect` |
| "90%存活率很好" | 框架效应 | `framing-effect` |
| "两周能做完" | 规划谬误 | `planning-fallacy` |
| "上次骂了他就改了" | 回归均值误判 | `regression-to-mean` |
| "这体验糟透了" | 记忆≠体验 | `remembering-vs-experiencing` |

---

## 五、技能触发速查表

```
需要决策框架
  └─ effective-decisions / two-systems

需要估值分析
  └─ aesop-three-questions → margin-of-safety → business-picker

需要问题分析
  └─ check-your-lights → problem-definition-formula → problem-analysis-3steps

需要创意突破
  └─ problem-restatement → foreign-perspective

需要人员管理
  └─ strengths-based → contribution-focus

需要时间管理
  └─ know-thy-time → first-things-first

需要认知检查
  └─ overconfidence → loss-aversion → framing-effect → availability-heuristic

需要投资决策
  └─ circle-of-competence → economic-moat → mr-market → compounding-thinking
```

## 六、注意事项

1. **不要一次调用太多 skill**— 一次聚焦 1-2 个，效果最好
2. **skill 是辅助不是替代**— 它提供框架，你提供具体数据和判断
3. **按场景选 skill**— 不相关的 skill 强行用会适得其反
4. **可以组合**— 复杂问题可以串联多个 skill，如"先 two-systems 再 effective-decisions"
