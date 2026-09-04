# 🧿 Mindset Healer · 双系统命理导师

> **一个仓库，中英双语两个 Claude Code Agent。**
> 把"想不通的人生死循环"拆成可执行的修复方案 —— 中文版融合 **MBTI × 命理**；English edition is a pure-metaphysics **Mindset Healer**.

---

## 📦 一个仓库，两个 Agent

| Agent | 文件 | 语言 / 取向 | 特点 |
|-------|------|-------------|------|
| **双系统命理导师** | `.claude/agents/mindset-healer.md` | 中文 · MBTI × 八字/紫微/易经 | 从认知层（MBTI 功能）和能量层（命理病灶）交叉验证，给出"认知-能量"二元处方 |
| **Mindset Healer** | `.claude/agents/mindset-healer-en.md` | English · Bazi / Ziwei / Yijing | Translates metaphysics into engineering instructions; root-cause verdict + executable patches |

两个文件的 `name` 不同（`mindset-healer` / `mindset-healer-en`），**可以同时安装**，互不冲突。

---

## 🚀 安装 / Install

```bash
# 装到全局（推荐，任意项目可用） / Global (available in every project)
mkdir -p ~/.claude/agents
cp .claude/agents/mindset-healer.md    ~/.claude/agents/   # 中文版 Chinese
cp .claude/agents/mindset-healer-en.md ~/.claude/agents/   # English

# 或只装到某个项目 / Or install for one project only
mkdir -p <your-project>/.claude/agents
cp .claude/agents/mindset-healer-en.md <your-project>/.claude/agents/
```

装好后 **重启 Claude Code**。

> 💡 也可以直接把 `.md` 当系统提示词贴到任意 AI 对话框使用（如 claude.ai）。

---

## 💬 使用 / Usage

**中文**（对 Claude 说）：
> "让 mindset-healer 帮我诊断为什么我总想好了才做、却永远不开始"
> "用命理导师分析我最近的状态"

**English**（tell Claude）：
> "Use the mindset-healer-en agent to diagnose why I keep overthinking and never act."
> "Ask Mindset Healer for a root-cause analysis of my current block."

主代理会根据描述自动调度对应语言的 Agent。

---

## 🧠 诊断逻辑 / Diagnostic logic

```
你的症状描述 / Your symptom
        ↓
① 行为现象采集  /  Observation   —— 记录"死循环"，不跳步下结论
        ↓
② 认知层 / 命理层 拆解          —— MBTI 功能 or Bazi/Ziwei/Yijing 交叉验证病灶
        ↓
③ 联合处方 / Prescription      —— 反直觉、可执行的修复指令
        ↓
④ 落地与跟进 / Follow-up       —— "下一小时的物理动作" + 截止锚点
```

- 中文版补充说明：命理 = 能量底层硬限制，MBTI = 认知层行为模式，**单看哪个都是盲人摸象**。
- 提供出生时间（年月日时）可增强八字/紫微验证；不提供则按能量状态推断，不影响流程。
- Note: the chart is the **factory default setting**; your actions are the **system patches**.

---

## 🚫 设计红线 / Red lines

- ❌ **不恐吓** / No scare tactics —— never "you will face disaster"
- ❌ **不宿命** / No determinism —— never "you were born with XX destiny"
- ❌ **不空谈** / No empty talk —— 每条诊断必附一个"立刻可执行"的物理动作
