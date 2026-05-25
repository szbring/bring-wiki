# bring-wiki SCHEMA

> 本文件是知识库的**机器可读契约**，不是风格指南。
> 所有 `.md` 文件（`domains/` 下）必须遵守本 schema，否则视为未完成。
> 目标读者是 RAG agent，不是人。人能读懂只是副产品。

---

## 0. 核心原则

1. **frontmatter 是索引，不是装饰**。每个字段都必须对 AI 检索/过滤有用，否则不加。
2. **原子知识独立成卡**。一个概念一张卡（concept），长文只做导读和推理链，不做定义。
3. **原文归档与精炼内容分层**。raw 不进主检索，只作溯源。
4. **关系是显式三元组**，不是隐式 wikilink。
5. **所有枚举值封闭**。新增枚举需要改 schema 并全库迁移，不允许自由文本。

---

## 1. 文件类型（三类，`doc_type` 字段必填）

| doc_type | 用途 | 目录约定 | 正文长度 | 主检索 |
|---|---|---|---|---|
| `concept` | 原子知识卡（一个概念/工具/方法） | `{流程}/concepts/` | 150–500 字 | ✅ |
| `refined` | 方法论长文、流程概述、成熟度模型 | `{流程}/01_知识框架/` 等既有 6 层 | 800–3000 字 | ✅ |
| `raw` | 原文归档（公众号/书籍章节/报刊） | `{流程}/raw/` 或 `raw-archive/` | 不限 | ❌ 仅溯源 |
| `index` | 目录导航页、索引页 | 各级 `00_概述.md` / `_index_*.md` | 不限 | ❌ |

> 过渡期：现有 `01_知识框架/` 下混杂的 raw_article 必须迁到同级 `raw/` 子目录，不允许留在 refined 层。

---

## 2. 通用 frontmatter（所有文件必填）

```yaml
---
id: ipd.concept.dcp                    # 全局唯一，kebab-case，"."分层，见 §6
doc_type: concept                      # concept | refined | raw | index
title: DCP 决策评审点                   # 人可读标题
domain: huawei-practice                # 固定枚举，见 §7.1
process: 1.0_IPD                       # 固定枚举，见 §7.2
layer: 01_知识框架                      # 固定枚举，见 §7.3（raw 可省略）
source_authority: 华为官方             # 固定枚举，见 §7.4
confidence: high                       # high | medium | low
created: 2026-04-24
updated: 2026-04-24
---
```

**禁止字段**：`tags`（自由文本 tag 已被 `aliases` + `related` + `process` 取代）。

---

## 3. concept（原子卡）专属字段

```yaml
---
# 通用字段 (§2) +
entity_type: process_gate              # 见 §7.5 枚举
canonical_name: DCP                    # 规范名，英文缩写优先
aliases:                               # 所有可被提问时命中的别名
  - Decision Checkpoint
  - 决策评审点
  - 决策检查点
parent_concept: ipd.concept.ipd-framework   # 上位概念 id
child_concepts:                        # 可选，下位概念 id 列表
  - ipd.concept.dcp-charter
  - ipd.concept.dcp-plan
relations:                             # 三元组，见 §4
  - {predicate: gates, object: ipd.concept.ipd-stage}
  - {predicate: requires_role, object: ipd.concept.ipmt}
  - {predicate: produces, object: ipd.concept.charter}
applies_to:                            # 可选：适用场景枚举
  - 新产品立项
  - 版本规划
maturity_stage: [L2, L3, L4, L5]       # 从哪一级成熟度开始出现
---
```

**正文结构（强约束，顺序不可改）**：

```markdown
## 定义
一句话，≤40字。

## 输入 / 输出
- 输入：…
- 输出：…

## 角色
- 决策方：…
- 执行方：…
- 评审方：…

## 上下游
- 上游：[[id:上游concept]]
- 下游：[[id:下游concept]]

## 典型误区
- …（2-4 条，每条一句话）

## 出处
- [[id:某refined文档]]
- [[id:某raw文档]]  <!-- 原文溯源 -->
```

---

## 4. relations 三元组规范

**语法**：frontmatter 里的 `relations:` 列表，每项 `{predicate, object}`，主语默认是当前文件的 `id`。

**封闭谓词表**（新增需改 schema）：

| predicate | 语义 | 反向谓词 |
|---|---|---|
| `part_of` | A 是 B 的组成部分 | `has_part` |
| `precedes` | A 在 B 之前发生 | `follows` |
| `produces` | A 产出 B（交付物） | `produced_by` |
| `requires_role` | A 需要角色 B 参与 | `role_in` |
| `gates` | A 是 B 的决策关口 | `gated_by` |
| `feeds` | A 的输出喂给 B | `fed_by` |
| `depends_on` | A 依赖 B 存在 | `supports` |
| `instantiates` | A 是 B 方法论的实例 | `instantiated_by` |
| `contradicts` | A 与 B 在语义上冲突（如不同版本） | `contradicts` |

> 反向关系不写在双方文件里——由构建脚本生成。只单向维护。

---

## 5. chunk 锚点

长文（`refined`，≥1000 字）必须在每个可独立回答问题的小节前加锚点：

```markdown
<!-- chunk: or.stage2.analysis -->
## 阶段 2：需求分析（Requirement Analysis）
...
```

- 锚点 id 规则：`{concept_id 或 doc_id}.{小节 slug}`，kebab-case。
- 每个 chunk 200–600 字为宜，超过 800 字必须再切。
- embedding 构建以 chunk 为单位，不以文件为单位。

---

## 6. ID 命名规则

```
{domain}.{process}.{type}.{slug}
```

- 所有段小写，点分隔，slug 用 kebab-case。
- 示例：
  - `huawei.ipd.concept.dcp`
  - `huawei.ipd.refined.or-process-overview`
  - `huawei.ltc.concept.iron-triangle`
  - `huawei.ipd.raw.cgzx-2024-03-ipd-reinterpretation`（公众号原文）
- 一旦分配，**永不改名**。改名走 `aliases_id:` 字段（重定向），不删旧 id。

---

## 7. 封闭枚举值

### 7.1 domain
- `huawei-practice`（当前唯一）
- 未来：`self-practice`（薄云自有方法）、`industry-benchmark`

### 7.2 process
与目录一一对应，去掉中文后缀：
`0.0_overview | 1.0_IPD | 2.0_MTL | 3.0_LTC | 4.0_ITR | 5.0_DSE | 6.0_MCR | 7.0_ServiceDelivery | 8.0_Supply | 9.0_Procurement | 10.0_HR | 11.0_Finances | 12.0_BTIT | 13.0_BusinessSupport | 14.0_ChannelSales | 15.0_MCI | 16.0_Retail | 17.0_CloudService`

**`0.0_overview` 的专属用法**：跨业务流通用概念（如 DCP、TR、流程 Owner 机制、BPA 架构）必须用 `process: 0.0_overview`，文件放在 `00_体系总览/concepts/` 或 `00_体系总览/` 对应层。各流程的具体实例（如 IPD 的 CDCP/PDCP、LTC 的 ATI/ATB）用各自 process 值，并通过 `instantiates` 关系指向 overview 父卡。

### 7.3 layer
`01_知识框架 | 02_诊断工具 | 03_解决方案 | 04_交付指南 | 05_销售材料 | 06_资产库 | concepts | raw`

### 7.4 source_authority
| 值 | 含义 | 可信度 |
|---|---|---|
| `华为官方` | 华为出版物/白皮书/任总讲话原文 | 最高 |
| `华为前员工` | 离职华为顾问撰写，一手经验 | 高 |
| `薄云实践` | 薄云咨询项目沉淀、讲师原创 | 高 |
| `业界咨询` | 麦肯锡/IBM/安谋等公开资料 | 中 |
| `二手解读` | 公众号/mbalib/woshipm 等二手整理 | 低 |
| `未知` | 来源不明，**不进主检索** | — |

### 7.5 entity_type（concept 专用）
- `process` — 一级/二级流程本身（IPD、LTC）
- `sub_process` — 子流程（MM、OR、RDPM）
- `process_gate` — 决策关口（DCP、TR）
- `role` — 角色/团队（PDT、IPMT、IRB、铁三角）
- `artifact` — 交付物（Charter、业务计划书、PLM 规格）
- `method` — 方法论（BLM、五看三定、苹果树模型）
- `tool` — 工具/模板（成熟度问卷、访谈清单）
- `principle` — 原则/理念（以客户为中心、灰度管理）
- `metric` — 指标（研发投入产出比、NPS）
- `system` — IT 系统（PLM、CRM、ERP）

---

## 8. raw 文件的最小字段

raw 归档不进主检索，frontmatter 极简：

```yaml
---
id: huawei.ipd.raw.bycgzx-2024-ipd-reinterpretation
doc_type: raw
title: IPD解读——IPD重构产品研发与产品管理
domain: huawei-practice
process: 1.0_IPD
source_authority: 二手解读
source_url: https://mp.weixin.qq.com/s/xxx
source_publisher: 薄云咨询公众号
source_date: 2024-03-15
extracted_to:                          # 该 raw 被哪些 concept/refined 引用为出处
  - huawei.ipd.concept.dcp
  - huawei.ipd.refined.ipd-overview
created: 2026-04-23
---
```

> raw 正文允许口水话、营销尾巴，**不清洗**——保留原貌是溯源的核心价值。

---

## 9. 校验清单（lint 规则）

构建时必跑的检查（建议用 `health-monitor.py` 扩展）：

1. 所有 `.md` 必须有 frontmatter，且通过 schema 校验。
2. `id` 全局唯一。
3. `relations.object` 必须指向存在的 `id`。
4. `aliases` 不允许是 `canonical_name` 的子串重复（拒绝"IPD产品研发/IPD解读/IPD重构产品研发"这种）。
5. concept 正文必须包含 §3 的六个 H2 小节，顺序一致。
6. refined 文档若 ≥1000 字，必须至少有 2 个 chunk 锚点。
7. raw 文件必须可溯源，满足以下任一：(a) 有 `source_url`；(b) 有 `source_publisher + source_date`；(c) 有 `source_publisher + source_ingested`（`source_date: unknown` 合规，用于公众号/书籍原发日期无法考证的场景）。
8. 枚举字段不允许自由文本。
9. `source_authority: 未知` 或 `confidence: low` 的 concept/refined 会被主检索排除，只在降级时召回。

---

## 10. 迁移策略

不做全量重构。按以下顺序推进：

1. **现有 `01_知识框架/*` 中的 raw_article**（如 `IPD解读——IPD重构产品研发与产品管理.md`）先批量搬到同流程 `raw/`，frontmatter 按 §8 补齐。
2. **IPD 流程做样板**：按 §3 写 10–15 张 concept 原子卡（DCP / TR / PDT / IPMT / Charter / OR / MM / DCP阶段划分 / PLM / CBB / …），跑通 RAG 端到端检索。
3. **refined 层补 chunk 锚点**：先补 IPD 的 `00_概述.md` 和 `01_知识框架/OR_需求管理/*`。
4. **验证通过后**，把 §2–§7 的规范固化到 `classify_articles.py` / `extract_chapters.py` 的输出模板里，剩余 16 个流程批量产出时直接符合 schema。
5. **lint 入 pre-commit hook**：未通过的 md 不允许 commit。

---

## 11. 变更流程

- 本文件是契约。改枚举、改字段、改 id 规则都必须：
  1. 在本文件顶部更新 `## 变更日志`。
  2. 同步跑全库迁移（或留兼容期并在 `aliases_id:` 声明）。
  3. 重新构建索引与 embedding。

## 变更日志
- 2026-04-24: 初始版本。定义 doc_type 三分、frontmatter 索引字段、relations 三元组、chunk 锚点、id 命名、枚举值。
- 2026-04-24: §7.2 补充 `0.0_overview` 作为跨业务流通用概念的专属 process；§9 第 7 条放宽——允许 `source_date: unknown` + `source_ingested` 作为溯源替代。
