---
id: huawei.itr.concept.aur
doc_type: concept
title: AUR 问题理解决策评审
domain: huawei-practice
process: 4.0_ITR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: AUR
aliases:
- Acknowledge & Understand Request
- 问题确认与理解
- 问题诊断准入
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.itr.concept.itr-framework
- predicate: gates
  object: huawei.itr.concept.itr-framework
- predicate: follows
  object: huawei.itr.concept.asr
- predicate: precedes
  object: huawei.itr.concept.aip
applies_to:
- 工单确认 + 现象复现
- 问题归类与责任团队确定
- 是否需要升级
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.itr.concept.aip
- huawei.itr.concept.asr
- huawei.itr.refined.问题分类与升级机制
- huawei.overview.concept.dcp
---

# AUR 问题理解决策评审

## 定义
ITR 流程第二个 DCP，对工单做深入理解后的决策——是否能复现/确认问题、是否归对了团队、是否需要升级、SLA 时钟是否需要调整。

## 输入 / 输出
- **输入**：工单初判 + 客户补充信息 + 复现尝试 + 历史相似案例
- **输出**：Confirm—问题确认，分配处理团队，进入诊断 / Reassign—归类错误，转给正确团队 / Escalate—复杂度超出当前层级，上升至专家组 / Close-No-Issue—无法复现且非真实问题
- **关键动作**：现象复现 + 责任团队定位

## 角色
- **决策方**：服务经理 + 一线技术团队 Leader
- **执行方**：一线工程师（尝试复现）
- **协同方**：客户运维方（提供环境信息）

## 上下游
- **上游**：[[id:huawei.itr.concept.asr]] 已分派工单
- **下游**：通过 → [[id:huawei.itr.concept.aip]] 进入分析与方案制定
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 ITR 流程中的实例

## 典型误区
- **直接跳到方案**：没复现就开始改——可能改错地方
- **轻易 Close-No-Issue**：客户报的"无法复现"被关单——客户体验差，可能漏真实问题
- **不调整 SLA**：发现问题严重度比初判高，但 SLA 不调整——后续处理时间不足
- **AUR 是工程师私下判断**：没有正式评审记录——后续追溯不到

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，ITR 同构）
- [[id:huawei.itr.refined.问题分类与升级机制]] — 问题分类与升级机制
