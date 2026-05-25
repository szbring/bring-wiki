---
id: huawei.itr.concept.aip
doc_type: concept
title: AIP 问题分析与方案决策评审
domain: huawei-practice
process: 4.0_ITR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: AIP
aliases:
- Analyze, Investigate, Plan
- 问题分析与方案
- 解决方案评审
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.itr.concept.itr-framework
- predicate: gates
  object: huawei.itr.concept.itr-framework
- predicate: follows
  object: huawei.itr.concept.aur
- predicate: precedes
  object: huawei.itr.concept.avr
applies_to:
- 根因分析评审
- 修复方案选型决策
- 影响面与回退方案评审
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.itr.concept.aur
- huawei.itr.concept.avr
- huawei.itr.refined.itr流程架构
- huawei.overview.concept.dcp
---

# AIP 问题分析与方案决策评审

## 定义
ITR 流程第三个 DCP，对完成的根因分析、备选方案、影响面、回退预案做评审——通过则授权实施修复，未通过则需要补充分析或换方案。

## 输入 / 输出
- **输入**：根因分析报告（5Why / 鱼骨图等）+ 备选解决方案对比 + 影响范围 + 回退方案 + 实施时间窗
- **输出**：Approve—授权实施 / Reject—方案不可行，重新分析 / Conditional—附加约束（如必须在维护窗口内做）
- **关键审视**：根因是否找到（不是只治表象）、方案是否最小变更、回退是否可行

## 角色
- **决策方**：服务经理 + 技术专家 / TR（如涉及产品变更）
- **汇报方**：处理工程师
- **协同方**：研发（涉及代码修改）、运维（涉及环境变更）、客户（确认接受）

## 上下游
- **上游**：[[id:huawei.itr.concept.aur]] 问题已确认
- **下游**：通过 → [[id:huawei.itr.concept.avr]] 实施验证
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 ITR 流程中的实例

## 典型误区
- **症状级修复**：只解决表象不查根因——同样问题反复出现
- **没有备选方案**：第一个想到的方案就实施——错过更优解
- **不做回退预案**：实施失败无法回退——故障扩大
- **AIP 太重**：所有问题都走严格 AIP——简单问题流程负担大于价值；按问题级别裁剪

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，ITR 同构）
- [[id:huawei.itr.refined.itr流程架构]] — ITR 流程架构
- ITIL 问题管理（参考）
