---
id: huawei.ipd.concept.mm
doc_type: concept
title: MM 市场管理流程
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: sub_process
canonical_name: MM
aliases:
- Market Management
- 市场管理
- MM 流程
- 市场规划流程
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: feeds
  object: huawei.ipd.concept.or
- predicate: feeds
  object: huawei.ipd.concept.charter
- predicate: fed_by
  object: huawei.dste.concept.sp-bp
applies_to:
- 市场细分与机会选择
- 产品组合规划
- 年度/版本规划前置分析
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.cdcp
- huawei.ipd.concept.charter
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.or
- huawei.ipd.refined.mm-methodology
---

# MM 市场管理流程

## 定义
把市场机会转化为可执行产品规划的六步结构化方法（中 IPD 三大流程之一）。

## 输入 / 输出
- **输入**：DSTE 的 SP/BP 战略方向、市场数据、客户调研、竞争分析、技术演进趋势、现有产品业绩
- **输出**：细分市场选择、差异化价值主张、产品路标、版本规划建议；向 [[id:huawei.ipd.concept.or]] 和 [[id:huawei.ipd.concept.charter]] 输入
- **六步骤**：
  1. 市场细分与评估（Market Segmentation）
  2. 组合分析与目标选择（Portfolio Analysis）
  3. 差异化价值主张与业务设计
  4. 产品/解决方案规划（路标）
  5. 业务计划整合
  6. 管理业务计划（闭环）

## 角色
- **主责**：产品线/事业部的产品规划或 Marketing 团队
- **核心方法论成员**：市场分析师、产品经理、技术专家、财经代表
- **决策归口**：[[id:huawei.ipd.concept.ipmt]]（MM 输出的路标与产品组合在 IPMT 批准）

## 上下游
- **上游**：DSTE 战略规划（SP） + 业务计划（BP）→ 定方向和预算
- **下游**：MM 识别机会 → [[id:huawei.ipd.concept.or]] 做需求转化 → [[id:huawei.ipd.concept.charter]] 做立项承诺 → [[id:huawei.ipd.concept.cdcp]] 决策
- **周期性**：MM 通常按年滚动，重大市场变化时触发临时迭代

## 典型误区
- **把 MM 做成"市场调研报告"**：只写现状不做选择——MM 的输出必须是"做哪些不做哪些"的决策
- **没做细分直接选机会**：跳过细分导致机会评估同质化——六步方法第一步不可省
- **差异化等于"我们更便宜"**：低价不是差异化，应聚焦功能/体验/服务的结构性优势
- **路标画了没人跟**：MM 输出路标但 PDT 开发时不参照——必须在 Charter 里明确回指路标条目
- **MM 单点事件化**：一年做一次然后束之高阁——必须季度或半年滚动，市场变化快于计划周期

## 出处
- [[id:huawei.ipd.refined.mm-methodology]] — MM 方法论长文（待建/待完善）
- 华为《市场管理 MM 流程指南》
- 《华为能你也能 IPD》相关章节
