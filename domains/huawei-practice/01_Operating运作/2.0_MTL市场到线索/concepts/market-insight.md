---
id: huawei.mtl.concept.market-insight
doc_type: concept
title: 市场洞察（五看）
domain: huawei-practice
process: 2.0_MTL
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 市场洞察
aliases:
- Market Insight
- 五看
- 五看分析
- 五看三定
- MTL 洞察
parent_concept: huawei.mtl.concept.mtl-framework
relations:
- predicate: part_of
  object: huawei.mtl.concept.mtl-framework
- predicate: feeds
  object: huawei.dste.concept.sp-bp
- predicate: feeds
  object: huawei.ipd.concept.mm
- predicate: supports
  object: huawei.dste.concept.blm
applies_to:
- SP / BP 制定输入
- IPD MM 市场管理输入
- 重大投资决策的市场依据
related_concepts:
- huawei.dste.concept.blm
- huawei.dste.concept.sp-bp
- huawei.ipd.concept.mm
- huawei.mtl.refined.mtl市场洞察方法论
- huawei.mtl.refined.市场洞察五看模型
---

# 市场洞察（五看）

## 定义
华为标准化的市场分析方法，从五个维度（看行业 / 看市场 / 看竞争 / 看自己 / 看机会）系统性扫描外部环境，输出 SP/BP 与 MM 决策所需的事实基础与机会清单。

## 输入 / 输出
- **输入**：行业研究报告、客户访谈、竞争情报、内部能力盘点、技术趋势报告
- **输出**：五看分析报告（含行业地图 / 市场细分 / 竞争格局 / SWOT / 机会清单）+ 三定（定目标 / 定策略 / 定计划）输入
- **五看维度**：
  - **看行业**：宏观规模、增长、价值链、监管、技术拐点
  - **看市场**：客户细分、需求未满足点、地理分布
  - **看竞争**：直接竞争、潜在颠覆者、对手能力对比
  - **看自己**：资源、能力、品牌、客户关系、组织
  - **看机会**：可投资机会清单 + 风险评估

## 角色
- **主导方**：市场洞察团队 / 战略部
- **协同方**：业务部门（提需求 + 验证假设）、客户经理（一手客户声音）、研发（技术趋势）
- **客户方**：DSTE 战略团队、IPD MM 团队

## 上下游
- **上游**：DSTE 启动 SP/BP 周期 → 触发五看
- **下游**：五看输出 → [[id:huawei.dste.concept.sp-bp]] SP/BP / [[id:huawei.ipd.concept.mm]] MM 市场管理 / [[id:huawei.dste.concept.blm]] BLM 市场洞察模块

## 典型误区
- **五看 = 报告堆砌**：只做信息收集不做判断——核心是辩论与洞察输出
- **不更新**：一份报告用一年——市场动态变，应至少季度迭代关键模块
- **看自己看不清**：靠业务部门自评——必须对标外部基准 + 客户声音
- **机会清单 = 业务愿望清单**：把"想做的"列成机会，不是"市场允许 + 自己能赢"的——应做赢率打分

## 出处
- [[id:huawei.mtl.refined.市场洞察五看模型]] — 市场洞察五看模型
- [[id:huawei.mtl.refined.mtl市场洞察方法论]] — MTL 市场洞察方法论
- 华为《价值为纲》战略洞察章节
