---
id: huawei.itr.concept.asr
doc_type: concept
title: ASR 问题接收决策评审
domain: huawei-practice
process: 4.0_ITR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ASR
aliases:
- Acquire Service Request
- 接收服务请求
- 问题接收
- ITR 第一关口
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.itr.concept.itr-framework
- predicate: gates
  object: huawei.itr.concept.itr-framework
- predicate: precedes
  object: huawei.itr.concept.aur
applies_to:
- 客户问题工单接收
- 问题初步分级
- 受理与拒绝决策
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.itr.concept.aur
- huawei.itr.refined.问题分类与升级机制
- huawei.overview.concept.dcp
---

# ASR 问题接收决策评审

## 定义
ITR 流程第一个 DCP，对接收的客户问题做"是否受理 + 初步分级"的 Go/Reject/Defer 决策——受理则建立工单进入处理，拒绝则告知客户原因，延后则等待补充信息。

## 输入 / 输出
- **输入**：客户报障信息（客户、产品、症状、紧急度、影响范围、联系人）
- **输出**：Go—建工单 + 初步分级（紧急度 P1-P4）+ 分派给对应处理团队 / Reject—告知客户该问题不在服务范围 / Defer—需要客户补充信息
- **关键动作**：分级决定后续 SLA 时钟启动

## 角色
- **决策方**：服务台 / 服务经理（分级权限）
- **录入方**：客服坐席 / 客户自助（在线提单）
- **协同方**：CRM 系统（客户身份与合同核对）

## 上下游
- **上游**：客户报障 / 监控告警 / 主动巡检发现
- **下游**：通过 → [[id:huawei.itr.concept.aur]] 问题理解与分配
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 ITR 流程中的实例

## 典型误区
- **来单就受理**：不做初步分级——所有工单平等处理，紧急的被淹没
- **客户级别决定问题级别**：只看 VIP 客户优先——忽视普通客户的真严重问题
- **拒绝就拒绝**：不解释原因——客户体验差，下次绕过流程
- **ASR 仅是录单动作**：不做决策——失去关口意义

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，ITR 同构）
- [[id:huawei.itr.refined.问题分类与升级机制]] — 问题分类与升级机制
- ITIL 服务台最佳实践（参考）
