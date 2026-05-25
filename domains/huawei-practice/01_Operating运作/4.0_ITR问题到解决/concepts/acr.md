---
id: huawei.itr.concept.acr
doc_type: concept
title: ACR 关闭与复盘决策评审
domain: huawei-practice
process: 4.0_ITR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ACR
aliases:
- Acknowledge, Close & Review
- 关闭与复盘
- 工单关闭
- ITR 末端关口
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.itr.concept.itr-framework
- predicate: gates
  object: huawei.itr.concept.itr-framework
- predicate: follows
  object: huawei.itr.concept.avr
- predicate: feeds
  object: huawei.ipd.concept.or
applies_to:
- 工单正式关闭
- 客户满意度收集
- 根因经验沉淀与产品改进输入
related_concepts:
- huawei.ipd.concept.or
- huawei.ipd.refined.dcp-mechanism
- huawei.itr.concept.avr
- huawei.itr.refined.itr核心理念
- huawei.overview.concept.dcp
---

# ACR 关闭与复盘决策评审

## 定义
ITR 流程末端 DCP，对客户已确认解决的工单做"正式关闭 + 复盘"决策——关闭工单、收集客户满意度、把根因/方案沉淀入库、把产品改进项推送到 [[id:huawei.ipd.concept.or]] 需求管理。

## 输入 / 输出
- **输入**：[[id:huawei.itr.concept.avr]] 已通过 + 客户书面确认 + 客户满意度问卷
- **输出**：Close—工单正式关闭 + 经验入库 + 产品改进项进 OR 需求池 / Reopen—客户后续反馈问题复现，重启工单
- **必须产出**：根因卡片入知识库、产品改进 backlog、流程问题改进建议

## 角色
- **决策方**：服务经理 + 流程 Owner
- **复盘组织方**：质量管理部
- **接收方**：研发（产品改进项）、流程改进委员会（流程问题）

## 上下游
- **上游**：[[id:huawei.itr.concept.avr]] 验证通过 + 客户确认
- **下游**：经验入库 → 服务知识库；产品改进项 → [[id:huawei.ipd.concept.or]] 需求管理；流程问题 → 流程优化
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 ITR 流程中的实例

## 典型误区
- **关单就完事**：不做经验沉淀——同样问题反复发生在不同客户
- **不收集满意度**：完工不问客户感受——客户不满未来流失
- **改进项推送不闭环**：把改进项扔给 IPD 就完事——OR 不接、不立项，长期不解决
- **重大问题没有复盘会**：关单流程走完即可——失去组织学习机会，建议 P1/P2 必复盘

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，ITR 同构）
- [[id:huawei.itr.refined.itr核心理念]] — ITR 核心理念
- 华为客户问题反向驱动产品改进机制
