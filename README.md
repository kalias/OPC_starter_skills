# 极简创业者 — Claude Code 技能（中文本地化版）

基于 Sahil Lavingia 所著《The Minimalist Entrepreneur（极简创业者）》的 Claude Code 技能集，已做中文本地化。

> **原项目**：[slavingia/skills](https://github.com/slavingia/skills)（英文版）
> **作者背景**：Sahil Lavingia，17 岁辍学进 Pinterest 当首位设计师，19 岁一个周末做出 Gumroad。这本书讲的就是「先社区、先验证、先手动交付、第一天就收费」的极简创业方法论。
> **本仓库**：忠实保留原书理论与 Gumroad 原创案例，工具/平台/渠道/案例做国内化适配。

---

## 它是什么

把《极简创业者》这本书拆成 **10 个可调用的 Claude Code 技能**。每个技能是一个会提问、会给结论的「创业顾问」，对应书里创业旅程的一个阶段。

它不是「读完书自己理解」，而是「装上就能用 AI 按书里的框架逼你回答」。

## 安装

### 方式 A：作为 Claude Code 插件（推荐）

在 Claude Code 会话里：

```
/plugin marketplace add slavingia/skills
/plugin install minimalist-entrepreneur
```

（原英文版的安装命令；要装中文版，先 fork 这个目录到自己的仓库，再 `/plugin marketplace add <你的用户名>/<仓库名>`。）

### 方式 B：本地克隆

```bash
# 把本目录克隆到 Claude 插件目录
git clone <你的仓库地址> ~/.claude/plugins/zai-skills-zh
```

然后在 Claude Code 里：

```
/plugin marketplace add ~/.claude/plugins/zai-skills-zh
/plugin install minimalist-entrepreneur
```

### 方式 C：直接当提示词用（不装插件）

每个技能本质上就是 `skills/<名字>/SKILL.md` 一个 Markdown 文件。直接把它丢给 Claude/ChatGPT/任何 LLM，让它扮演那个「顾问」，效果一样。

---

## 10 个技能

| 技能 | 命令 | 什么时候用 |
|-------|---------|-------------|
| **找社区** | `/find-community` | 在找创业方向、找你的社区 |
| **验证想法** | `/validate-idea` | 在测试一个想法值不值得做 |
| **MVP** | `/mvp` | 准备做第一个产品、或在功能范围上挣扎 |
| **流程化** | `/processize` | 有产品想法，想在写代码前先手动交付价值 |
| **前 100 个客户** | `/first-customers` | 有产品了，要找头 100 个客户 |
| **定价** | `/pricing` | 在定价、或考虑调价 |
| **营销方案** | `/marketing-plan` | 已有产品-市场契合，准备用内容放大 |
| **可持续增长** | `/grow-sustainably` | 在做花费、招聘、融资、扩张的决策 |
| **公司价值观** | `/company-values` | 在定义文化、准备招聘 |
| **极简复盘** | `/minimalist-review` | 对任何商业决策做直觉校验 |

---

## 极简创业者之旅

技能顺序本身就是方法论——它和大多数人「想法 → 建产品 → 找客户」的直觉**相反**：

1. **社区** — 从「找到你的人」开始
2. **验证** — 确认问题值得解决
3. **构建** — 先交付手动流程，再产品化
4. **流程化** — 把产品想法转成今天就能手动交付的流程
5. **销售** — 一个一个地拿下 100 个客户
6. **定价** — 从第一天就收费
7. **营销** — 用内容建立受众
8. **增长** — 保持盈利、可持续扩张
9. **文化** — 建一座你想住的房子
10. **复盘** — 把极简原则用在每一个决策上

**反直觉核心**：别先想「做什么产品」，先想「我是谁的朋友、他们痛在哪」。能手动为几个人解决，才有资格自动化。

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
| frontmatter | 英文 | `name` 保留英文（插件加载依赖），`description` 译成中文 |

---

## 用法建议（性价比最高）

1. **不必全装**——多数人卡在 `validate-idea` 和 `pricing`，挑你纠结的阶段调用即可。
2. **每个技能都逼你回答具体问题**（「你能说出 10 个具体的有这个问题的人吗？」），别糊弄，它的价值就在这。
3. **想要 fork**：直接改 Markdown，结构是 10 个 `SKILL.md`，没有任何代码依赖。

---

## 致谢

- 原作者：[Sahil Lavingia](https://sahillavingia.com/)
- 原仓库：[slavingia/skills](https://github.com/slavingia/skills)
- 原书：[The Minimalist Entrepreneur](https://www.minimalistentrepreneur.com/)

本中文版仅为学习与本地化用途，方法论与原创案例版权归 Sahil Lavingia 所有。
