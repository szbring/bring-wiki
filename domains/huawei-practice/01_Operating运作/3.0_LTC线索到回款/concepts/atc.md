---
id: huawei.ltc.concept.atc
doc_type: concept
title: ATC 合同决策评审
domain: huawei-practice
process: 3.0_LTC
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ATC
aliases:
- Authorize To Contract
- 合同签订决策
- 合同评审
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ltc.concept.ltc-framework
- predicate: gates
  object: huawei.ltc.concept.ltc-framework
- predicate: follows
  object: huawei.ltc.concept.atb
- predicate: precedes
  object: huawei.ltc.concept.atac
- predicate: requires_role
  object: huawei.ltc.concept.iron-triangle
applies_to:
- 合同最终条款评审
- 客户谈判最终方案锁定
- 合同签字授权
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.ltc.concept.atac
- huawei.ltc.concept.atb
- huawei.ltc.concept.iron-triangle
- huawei.ltc.refined.ltc流程架构
- huawei.overview.concept.dcp
---

# ATC 合同决策评审

## 定义
LTC 流程第三个 DCP，对客户谈判后的最终合同文本做 Go/Kill/Hold 决策，重点审视条款可执行性、付款节奏、风险敞口、毛利兑现。

## 输入 / 输出
- **输入**：最终合同文本（含技术规格、价格、付款、违约、知识产权等条款）、谈判让步记录、风险登记册更新版
- **输出**：Go—授权签字 / Kill—拒签（条款超出底线）/ Hold—回到客户重新谈判
- **重点审视**：付款节奏（首付/进度/尾款）、违约责任、不可抗力、知识产权归属

## 角色
- **决策方**：销项决策团 + 法务 + 财经（必要时上升至更高层）
- **汇报方**：[[id:huawei.ltc.concept.iron-triangle]]（AR 主谈，SR 解释技术，FR 解释交付可达性）
- **专业把关**：法务（合同合法）、财经（回款可达）、合规

## 上下游
- **上游**：[[id:huawei.ltc.concept.atb]] 中标 → 客户合同谈判
- **下游**：通过签字 → 进入合同执行（交付 + 回款）→ [[id:huawei.ltc.concept.atac]]
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 LTC 流程中的实例

## 典型误区
- **签了再说**：客户催签字，跳过 ATC 直接签——后续交付/回款问题无人兜底
- **只看价格不看条款**：违约/付款节奏比单价更影响最终利润
- **铁三角不参与法务/财经环节**：律师写合同律师评审——铁三角不理解条款无法对客户解释
- **ATC 通过 = 项目稳了**：实际只是开始，真正的考验在交付与回款

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，LTC 同构）
- [[id:huawei.ltc.refined.ltc流程架构]] — LTC 流程架构
