---
id: huawei.dste.concept.bp-dcp
doc_type: concept
title: BP-DCP 年度业务计划决策评审
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: BP-DCP
aliases:
- BP DCP
- 年度计划评审
- BP 决策评审点
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.dste.concept.dste-framework
- predicate: gates
  object: huawei.dste.concept.sp-bp
- predicate: follows
  object: huawei.dste.concept.sp-dcp
- predicate: precedes
  object: huawei.dste.concept.bp-qr-dcp
applies_to:
- 年度业务计划评审
- 年度预算与组织调整批准
- BP 锁定后下发
related_concepts:
- huawei.dste.concept.bp-qr-dcp
- huawei.dste.concept.sp-dcp
- huawei.dste.refined.sp-bp战略规划体系
- huawei.ipd.refined.dcp-mechanism
- huawei.overview.concept.dcp
---

# BP-DCP 年度业务计划决策评审

## 定义
BP（年度业务计划）编制完成后的决策评审点，对 BP 文件、年度 KPI、预算、组织调整与人才计划做 Go/Kill/Hold 决策，通过后正式锁定下发执行。

## 输入 / 输出
- **输入**：BP 文件（年度 KPI、重点项目、预算、组织/人才计划）+ 与 SP 的衔接说明 + 财经预算审计
- **输出**：Go—BP 锁定下发，开启执行 / Kill—驳回重做（罕见）/ Hold—部分通过，指标项需修订
- **触发**：每年 11-12 月

## 角色
- **决策方**：EMT
- **汇报方**：各 BG/BU 一把手
- **质询方**：财经（预算合理性）、HR（组织/人才）、战略部（与 SP 一致性）

## 上下游
- **上游**：[[id:huawei.dste.concept.sp-dcp]] 通过 → SP 已发布；BP 编制完成
- **下游**：BP 锁定 → 各业务流执行 → [[id:huawei.dste.concept.bp-qr-dcp]] 季度回顾
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 DSTE 流程中的实例

## 典型误区
- **BP 与 SP 脱节**：BP 评审只看数字，不审"是否承接必赢战役"——SP 等于无效
- **预算游戏**：业务部门留余量、财经压指标，最后达成协议而非真实预测——评审应聚焦逻辑而非博弈
- **BP 锁死**：BP 通过后任何调整都被视为"违规"——应保留 [[id:huawei.dste.concept.bp-qr-dcp]] 调整窗口
- **不做组织/人才计划**：BP 只做财务数字，组织调整年中再说——结果项目无人执行

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，DSTE 同构）
- [[id:huawei.dste.refined.sp-bp战略规划体系]] — SP/BP 战略规划体系
- 华为流程 Owner 体系——DSTE Owner 主持
