# OPC Starter Skills — 一人公司起步技能集（中文本地化版）

一套为「AI 时代的独立开发者 / 一人公司」准备的 Claude Code 技能集，**分两部分**：

- **Part 1 · Mindset（极简创业者 · 哲学）** — 10 个技能，源自 Sahil Lavingia《The Minimalist Entrepreneur》，回答「该不该做、怎么开始」。
- **Part 2 · Playbook（AI 一人公司 · 打法）** — 7 个技能，源自实操拆解，回答「用 AI 具体怎么做」。

两部分**互补不重叠**：Mindset 讲心态与哲学，Playbook 讲可复制的 vibe coding 打法。可以独立使用，也可以串成完整链路。

> 📖 **English README: [/README.en.md](./README.en.md)**

---

## 它是什么

把两份高质量内容（《极简创业者》原书 + AI 一人公司实操拆解）蒸馏成 **17 个可调用的 Claude Code 技能**。每个技能都是一个会提问、会给结论的「顾问 / 教练」，对应创业旅程的一个阶段。

它不是「读完书自己理解」，而是「装上就能让 AI 按框架逼你回答」。

## 安装

### 方式 A：作为 Claude Code 插件（推荐）

在 Claude Code 会话里：

```
/plugin marketplace add kalias/OPC_starter_skills
/plugin install minimalist-entrepreneur
```

### 方式 B：本地克隆

```bash
git clone git@github.com:kalias/OPC_starter_skills.git ~/.claude/plugins/opc-starter-skills
```

然后在 Claude Code 里：

```
/plugin marketplace add ~/.claude/plugins/opc-starter-skills
/plugin install minimalist-entrepreneur
```

### 方式 C：直接当提示词用（不装插件）

每个技能本质就是 `skills/<名字>/SKILL.md` 一个 Markdown 文件。直接把它丢给任意 LLM，让它扮演那个「顾问」，效果一样。

> **结构说明**：所有技能物理上平铺在 `skills/` 下（这是 Claude Code 插件加载器的约定，只扫一层 `skills/<name>/SKILL.md`）。分区通过 frontmatter 的 `part: mindset|playbook` 字段实现，README 按此分区展示。

---

## Part 1 · Mindset（极简创业者 · 哲学）

源自 Sahil Lavingia《The Minimalist Entrepreneur》。回答「要不要做、怎么开始」。顺序本身就是反直觉的方法论——**从社区开始，而不是从产品想法开始**。

| 技能 | 命令 | 什么时候用 |
|-------|---------|-------------|
| **找社区** | `/find-community` | 在找创业方向、找你的社区 |
| **验证想法** | `/validate-idea` | 测试一个想法值不值得做 |
| **MVP** | `/mvp` | 准备做第一个产品、或在范围上挣扎 |
| **流程化** | `/processize` | 想在写代码前先手动交付价值 |
| **前 100 个客户** | `/first-customers` | 有产品了，要找头 100 个客户 |
| **定价** | `/pricing` | 在定价、或考虑调价 |
| **营销方案** | `/marketing-plan` | 已有 PMF（约 100 客户），用内容放大 |
| **可持续增长** | `/grow-sustainably` | 在做花费/招聘/融资/扩张决策 |
| **公司价值观** | `/company-values` | 定义文化、准备招聘 |
| **极简复盘** | `/minimalist-review` | 对任何商业决策做直觉校验 |

**核心**：别先想「做什么产品」，先想「我是谁的朋友、他们痛在哪」。能手动为几个人解决，才有资格自动化。

---

## Part 2 · Playbook（AI 一人公司 · 打法）

源自实操拆解。回答「用 AI 怎么干」。核心理念：**文件夹即公司、技能即员工、做一次就技能化它**。

| 技能 | 命令 | 什么时候用 |
|-------|---------|-------------|
| **搭建 AI 操作系统** | `/setup-ai-os` | 刚开始用 AI 做独立开发，20 分钟搭好公司 |
| **构建任何东西** | `/build-anything` | 想做新产品、面对复杂项目不知从哪下手 |
| **技能化** | `/skillify` | 刚做完一个项目，想沉淀成永久可复用资产 |
| **自然获客引擎** | `/organic-engine` | 有产品没客户，想用内容让客户主动找你 |
| **冷触达引擎** | `/cold-outreach-engine` | 想搭一台「睡觉时也在干活」的获客管道 |
| **医生成交法** | `/doctor-selling` | 拿到线索但不会成交、丢单 |
| **交付与扩张** | `/deliver-and-scale` | 拿下客户要交付，或想从单次升级到月费/系统 |

**核心**：一个人公司的 IP 不是代码，是 SOP / 技能文件夹。每做两遍的事，就变成一个技能。

---

## 两部分怎么串起来用（完整链路）

```
[Part 1 · 想清楚]                [Part 2 · 用 AI 干]
/find-community  →  /validate-idea
        │                 │
        ▼                 ▼
                    /setup-ai-os   ← 搭好公司
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
   /processize       /mvp              /build-anything
   (手动跑通)        (最小产品)         (真的做出来)
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                     /skillify   ← 沉淀成永久资产
                          │
        ┌─────────────────┼─────────────────┐
        ▼                 ▼                 ▼
  /organic-engine  /cold-outreach    /first-customers
  (主动获客)       (被动获客)         (手动卖)
        │                 │                 │
        └─────────────────┼─────────────────┘
                          ▼
                  /doctor-selling  ← 拿下通话
                          │
                          ▼
                  /deliver-and-scale ← 交付 L1/L2/L3
                          │
                          ▼
              /pricing · /marketing-plan · /grow-sustainably
              (定价 · 放大 · 可持续)
                          │
                          ▼
                  /minimalist-review  ← 每个决策都复盘
```

---

## 本地化做了什么

| 类别 | 原版 | 中文版 |
|---|---|---|
| 理论框架 | 全部保留 | 100% 保留 |
| Sahil/Gumroad 案例 | 原创故事 | 保留（方法论原点） |
| 工具名 | Stripe/Carrd/Notion/Zapier | 微信支付/支付宝/上线了/腾讯文档/n8n 等 |
| 平台 | Twitter/Reddit/YouTube/Substack | 小红书/即刻/V2EX/B站/公众号/竹白 |
| 案例 | Nordstrom 接受轮胎退货 | 海底捞服务神话（同种「故事化价值观」） |
| 货币 | 美元 | 注释换算人民币，关键数字保留原值参考 |
| 语气 | 逼问式 | 保留（这是这套技能的力量来源） |
| frontmatter | 英文 | `name`/`part` 保留英文（加载器依赖），`description` 译成中文 |

---

## 用法建议（性价比最高）

1. **不必全装**——多数人卡在 `validate-idea`（该不该做）和 `build-anything`（怎么用 AI 做），挑你纠结的阶段调用。
2. **每个技能都逼你回答具体问题**，别糊弄，它的价值就在这。
3. **两部分可以分开用**：只想要哲学就用 Part 1，只想要打法就用 Part 2。
4. **想要 fork**：直接改 Markdown，结构是 17 个 `SKILL.md`，零代码依赖。

---

## 致谢与版权

**Part 1 (Mindset)** 的方法论与原创案例版权归原作者：
- 原作者：[Sahil Lavingia](https://sahillavingia.com/)
- 原仓库：[slavingia/skills](https://github.com/slavingia/skills)
- 原书：[The Minimalist Entrepreneur](https://www.minimalistentrepreneur.com/)

**Part 2 (Playbook)** 的打法源自公开实操拆解文的本地化重写。

本中文版仅为学习与本地化用途。完整的版权声明见 [LICENSE](./LICENSE)：原作者内容保留所有权利，我们的翻译与本地化增量内容采用 MIT。
