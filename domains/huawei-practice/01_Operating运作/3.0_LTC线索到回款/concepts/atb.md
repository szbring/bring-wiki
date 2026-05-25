---
id: huawei.ltc.concept.atb
doc_type: concept
title: ATB 投标决策评审
domain: huawei-practice
process: 3.0_LTC
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ATB
aliases:
- Authorize To Bid
- 投标决策
- 投标授权
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ltc.concept.ltc-framework
- predicate: gates
  object: huawei.ltc.concept.ltc-framework
- predicate: follows
  object: huawei.ltc.concept.ati
- predicate: precedes
  object: huawei.ltc.concept.atc
- predicate: requires_role
  object: huawei.ltc.concept.iron-triangle
applies_to:
- 投标方案与商务条件审批
- 报价底线与让步空间决策
- 投标资源最终投入决策
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.ltc.concept.atc
- huawei.ltc.concept.ati
- huawei.ltc.concept.iron-triangle
- huawei.ltc.refined.ltc流程架构
- huawei.overview.concept.dcp
---

# ATB 投标决策评审

## 定义
LTC 流程第二个 DCP，对完成的投标方案（技术方案 + 商务报价 + 风险评估）做"是否提交投标"的 Go/Kill/Hold 决策，并锁定报价底线和让步空间。

## 输入 / 输出
- **输入**：完整投标方案、报价分析（成本/竞争/期望）、风险登记册、客户决策链分析
- **输出**：Go—授权投标，锁定底价与让步规则 / Kill—放弃投标（成本超预算或赢率太低）/ Hold—需要修订方案后再评审
- **特别条款**：低毛利/超规模/特殊条款项目要上升评审层级

## 角色
- **决策方**：销项决策团（高于 ATI 层级或同层）
- **汇报方**：[[id:huawei.ltc.concept.iron-triangle]] 三人共同汇报
- **质询方**：财经（毛利）、法务（合同条款）、交付（可交付性）

## 上下游
- **上游**：[[id:huawei.ltc.concept.ati]] 通过 → 投标方案准备
- **下游**：通过 → 提交投标 → 中标后进入 [[id:huawei.ltc.concept.atc]]
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 LTC 流程中的实例

## 典型误区
- **只评技术不评商务**：技术 OK 就投——忽视毛利、付款条件等关键风险
- **铁三角私下定底价**：不上 ATB 评审，自己拍板——风险无人兜底
- **ATB 拖到投标截止前**：评审仓促，质询不充分——要求至少投标前 5 天完成
- **不评赢率**：明知赢率 <30% 也投，浪费投标成本

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，LTC 同构）
- [[id:huawei.ltc.refined.ltc流程架构]] — LTC 流程架构
