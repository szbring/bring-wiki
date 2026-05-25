---
id: huawei.ipd.concept.cdcp
doc_type: concept
title: CDCP 概念决策评审
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process_gate
canonical_name: CDCP
aliases:
- Concept DCP
- 概念决策评审
- 立项评审
- IPD 概念阶段 DCP
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: requires_role
  object: huawei.ipd.concept.ipmt
- predicate: fed_by
  object: huawei.ipd.concept.charter
- predicate: precedes
  object: huawei.ipd.concept.pdcp
applies_to:
- 新产品立项决策
- 产品机会评估
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.charter
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.pdcp
- huawei.ipd.concept.pdt
- huawei.ipd.refined.dcp-mechanism
- huawei.overview.concept.dcp
---

# CDCP 概念决策评审

## 定义
IPD 概念阶段末，IPMT 对"产品是否值得立项"的首次投资决策。

## 输入 / 输出
- **输入**：[[id:huawei.ipd.concept.charter]] 初稿、市场机会分析、初步产品定义、商业可行性分析、竞争格局评估
- **输出**：Go（立项进入 Plan 阶段，批准计划阶段资源）/ Kill（放弃该机会）/ Hold（补充前置调研后再评）
- **此点前累计资源投入**：约 5%

## 角色
- **决策方**：[[id:huawei.ipd.concept.ipmt]]（产品线或事业部级投资决策团）
- **执行方**：[[id:huawei.ipd.concept.pdt]] 概念组（尚未完整组建，由产品经理+关键代表组成）
- **支持方**：市场、研发、服务、供应各 Rep 提供初步评估

## 上下游
- **上游**：市场洞察（MM/OR）→ 业务机会识别 → 概念阶段启动
- **下游**：Go → 进入 Plan 阶段并召开 [[id:huawei.ipd.concept.pdcp]]；Kill → 机会归档；Hold → 回补调研
- **与同级关系**：通过 [[id:huawei.overview.concept.dcp]] instantiate 跨流程父卡

## 典型误区
- **CDCP 走过场，把 Kill 留到后面**：越晚 Kill 沉没成本越大，CDCP 是 ROI 最高的 Kill 点
- **材料深度超标**：此时详细技术方案和完整项目计划不是必须的，避免把 PDCP 的内容前置到 CDCP
- **商业论证靠直觉**：必须回答"客户是谁、痛点真实吗、市场多大、我们能赢吗、财务回报合理吗"五个问题，缺一不可
- **把技术可行性当商业可行性**：CDCP 判的是值不值得做，不是能不能做

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制长文（CDCP 章节）
- 华为 IPD 产品开发流程手册——概念阶段定义
