---
id: huawei.dste.concept.bp-qr-dcp
doc_type: concept
title: BP-QR-DCP 季度业务回顾决策评审
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: BP-QR-DCP
aliases:
- BP QR DCP
- 季度业务回顾
- QBR
- Quarterly Business Review
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.dste.concept.dste-framework
- predicate: follows
  object: huawei.dste.concept.bp-dcp
- predicate: precedes
  object: huawei.dste.concept.sa-dcp
applies_to:
- 季度业务复盘
- BP 执行偏差识别
- 资源/指标动态调整
related_concepts:
- huawei.dste.concept.bp-dcp
- huawei.dste.concept.sa-dcp
- huawei.ipd.refined.dcp-mechanism
- huawei.overview.concept.dcp
---

# BP-QR-DCP 季度业务回顾决策评审

## 定义
每季度对 BP 执行情况做 Go/Adjust/Escalate 决策的评审点——业绩好继续推进、偏差小做战术调整、偏差大上升到战略审视（SA-DCP）。

## 输入 / 输出
- **输入**：本季度 KPI 完成情况 + 重点项目进展 + 风险预警 + 偏差归因分析
- **输出**：Go—维持 BP 节奏 / Adjust—调整资源/优先级（不动 BP 大盘）/ Escalate—问题超出 BP 调整范围，上升至 [[id:huawei.dste.concept.sa-dcp]]
- **触发**：每季度末（4/7/10/次年 1 月）

## 角色
- **决策方**：BU 一把手 + 业务 EMT
- **汇报方**：各业务流 Owner / 项目经理
- **数据方**：财经（业绩数据）、市场（外部变化）

## 上下游
- **上游**：[[id:huawei.dste.concept.bp-dcp]] BP 已锁定执行
- **下游**：调整决议 → 业务流执行调整；如 Escalate → [[id:huawei.dste.concept.sa-dcp]]
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 DSTE 流程中的实例

## 典型误区
- **QBR 做成业绩汇报会**：只讲数字达成，不解释偏差原因和调整动作——失去复盘价值
- **不允许调整**：把 BP 当圣经，季度发现偏差也不动——一年下来差距越拉越大
- **每季度都 Escalate**：动不动就上升到 SA——SA 是战略层面，频繁触发说明 BP 本身有问题
- **只看本季不看趋势**：单季完成就过——必须看 YTD 累计趋势

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，DSTE 同构）
- 华为《华为执行力》季度复盘机制章节
- DSTE 流程 Owner 体系
