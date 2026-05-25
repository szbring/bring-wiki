---
id: huawei.supply.concept.scor-model
doc_type: concept
title: SCOR 供应链运作参考模型
domain: huawei-practice
process: 8.0_Supply
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: SCOR 供应链运作参考模型
aliases:
- SCOR
- Supply Chain Operations Reference
- 供应链运作模型
parent_concept: huawei.supply.concept.isc-framework
relations:
- predicate: part_of
  object: huawei.supply.concept.isc-framework
- predicate: feeds
  object: huawei.supply.concept.sop
applies_to:
- 供应链流程设计与评估
- ISC流程架构搭建
- 供应链绩效度量
related_concepts:
- huawei.supply.concept.isc-framework
- huawei.supply.concept.sop
- huawei.supply.concept.supply-chain-strategy
- huawei.supply.refined.供应链管理体系
- huawei.supply.refined.集成供应链isc方法论
---

# SCOR 供应链运作参考模型

## 定义
SCOR（Supply-Chain Operations Reference Model，供应链运作参考模型）是国际供应链理事会开发的标准化框架，用于设计和评价供应链系统。SCOR围绕五大基本管理流程构建：Plan（计划）、Source（采购）、Make（制造）、Deliver（交付）、Return（退货），其中Plan横向贯穿其余四个执行流程。SCOR还定义了四大要素：Performance（绩效——可靠性、响应性、柔性、成本、资产效率）、Process（流程——标准流程与流程关系描述）、Practice（实践——最佳实践指引）、People（人员——技能标准定义）。华为ISC变革即以SCOR为蓝本重构流程架构。

## 输入与输出
- **输入**：企业战略与业务模式、现有供应链流程与绩效数据
- **输出**：标准化流程架构（L2/L3分解）、绩效评价指标体系、最佳实践对标基线
- **Plan流程输出**：需求计划、供应计划、产能计划、库存计划

## 角色
- **流程设计者**：基于SCOR模型定义流程架构和分解层级
- **绩效管理者**：按SCOR五大绩效维度度量供应链表现
- **业务适配者**：根据业务模式裁剪SCOR标准流程（如MTS/MTO/CTO）

## 上下游
- **上游**：业务战略决定供应链战略取向，为SCOR流程设计提供方向
- **下游**：SCOR流程架构直接指导ISC流程落地和IT系统建设
- **Plan流程**横向贯穿Source/Make/Deliver/Return，是连接上下游的核心枢纽

## 典型误区
- **把SCOR当教条照搬**：SCOR是参考框架，需根据企业业务模式裁剪适配，华为就按物料分类和业务模式做了差异化分解
- **只关注流程要素忽略绩效要素**：Performance与Process同等重要，流程设计必须配以度量体系
- **SCOR只适用于大型企业**：中小企业可选取关键L2流程先行，不必一步到位构建完整模型

## 出处
- [[id:huawei.supply.refined.供应链管理体系]] — SCOR模型五大流程与四大要素详述
- [[id:huawei.supply.refined.集成供应链isc方法论]] — 基于SCOR的ISC流程框架与L2/L3分解
- Supply Chain Council, SCOR Model Reference
