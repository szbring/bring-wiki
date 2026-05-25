---
id: huawei.ltc.concept.ati
doc_type: concept
title: ATI 机会点立项决策评审
domain: huawei-practice
process: 3.0_LTC
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ATI
aliases:
- Authorize To Initiate
- 机会点立项决策
- LTC 第一关口
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ltc.concept.ltc-framework
- predicate: gates
  object: huawei.ltc.concept.ltc-framework
- predicate: precedes
  object: huawei.ltc.concept.atb
- predicate: requires_role
  object: huawei.ltc.concept.iron-triangle
applies_to:
- LTC 项目立项审批
- 机会点是否值得投入资源决策
- 销售管线进入立项门槛
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.ltc.concept.atb
- huawei.ltc.concept.iron-triangle
- huawei.ltc.refined.ltc流程架构
- huawei.ltc.refined.销售漏斗方法论
- huawei.overview.concept.dcp
---

# ATI 机会点立项决策评审

## 定义
LTC 流程第一个 DCP，对识别出的销售机会做"是否立项跟进"的 Go/Kill/Hold 决策——通过则正式投入资源（铁三角组建、解决方案投入），未通过则放弃或暂缓。

## 输入 / 输出
- **输入**：机会点信息（客户、需求、规模、竞争、可能金额）+ 客户决策链初判 + 资源诉求
- **输出**：Go—正式立项，组建铁三角并分配资源 / Kill—放弃机会 / Hold—暂存观察，不投入资源
- **门槛**：是否符合公司战略 + 是否值得投入 + 赢的概率

## 角色
- **决策方**：销项决策团（Sales Decision Team，区域级）
- **汇报方**：[[id:huawei.ltc.concept.iron-triangle]] AR（铁三角客户经理）
- **数据方**：市场情报、客户经理初步调研

## 上下游
- **上游**：MTL 营销活动产生线索 / 主动开发机会
- **下游**：通过 → 进入 [[id:huawei.ltc.concept.atb]] 投标准备阶段
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 LTC 流程中的实例

## 典型误区
- **来一个机会立一个**：不评估战略匹配和资源——铁三角资源被稀释
- **只看金额不看赢率**：金额大但赢率低也立项——投入产出比差
- **ATI 走过场**：销售部门已经做了所有事，ATI 只是签字——失去筛选意义
- **Hold 永远是 Hold**：长期挂账机会消耗管理注意力——必须有清退节奏

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，LTC 同构）
- [[id:huawei.ltc.refined.ltc流程架构]] — LTC 流程架构
- [[id:huawei.ltc.refined.销售漏斗方法论]] — 销售漏斗方法论
