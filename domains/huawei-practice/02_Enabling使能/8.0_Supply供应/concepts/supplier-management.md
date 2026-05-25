---
id: huawei.supply.concept.supplier-management
doc_type: concept
title: 供应商分级管理
domain: huawei-practice
process: 8.0_Supply
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 供应商分级管理
aliases:
- 供应商管理
- Supplier Management
- SQE
parent_concept: huawei.supply.concept.isc-framework
relations:
- predicate: part_of
  object: huawei.supply.concept.isc-framework
- predicate: part_of
  object: huawei.supply.concept.supply-chain-strategy
- predicate: feeds
  object: huawei.ipd.concept.ipd-framework
applies_to:
- 供应商分级与评估
- 战略供应商合作管理
- 供应商质量管理（SQE）
- 供应商开发与认证
related_concepts:
- huawei.supply.concept.isc-framework
- huawei.supply.concept.supply-chain-strategy
- huawei.ipd.concept.ipd-framework
- huawei.supply.refined.供应商管理
- huawei.supply.refined.供应链战略
- huawei.supply.refined.集成供应链isc方法论
---

# 供应商分级管理

## 定义
供应商分级管理是ISC使能流程的核心内容，聚焦供应商关系管理，是ISC运作流程的上游支撑。华为将供应商分为四级：战略供应商（Strategic）——长期战略合作，联合创新与产能保障；优选供应商（Preferred）——稳定供货，优先采购份额；合格供应商（Qualified）——满足基本要求，正常交易；观察供应商（Observed）——新引入或绩效下滑，需改善或淘汰。评估采用五维度加权：质量（30%）、交付（25%）、成本（20%）、技术（15%）、服务（10%）。华为实行双供应商策略，对关键物料至少保持两家合格供应商，避免单点依赖风险。供应商质量管理（SQE）贯穿供应商开发、认证、量产到退出的全生命周期。

## 输入与输出
- **输入**：供应商资质与认证材料、供货质量与交付绩效数据、技术与成本对标结果
- **输出**：供应商分级评定结果、采购份额分配方案、供应商改善要求与淘汰决策、SQE审核报告

## 角色
- **SQE（供应商质量工程师）**：负责供应商质量审核、制程审核与质量改进
- **采购品类经理**：负责供应商分级评定与份额分配
- **研发代表（IPD EPI）**：在研发早期介入供应商选型与技术评审

## 上下游
- **上游**：IPD流程中采购早期介入研发（EPI），在产品开发阶段即确定供应商选型方向
- **下游**：供应商分级与评估结果直接驱动采购执行中的份额分配和下单策略
- **与供应链战略的关系**：韧性战略要求多源供应与备选供应商，直接体现在双供应商策略中

## 典型误区
- **只看价格不看综合能力**：低价中标但交付与质量不达标，总成本反而更高
- **战略供应商无淘汰机制**：长期合作变成"舒适区"，缺乏绩效压力和持续改善动力
- **忽视供应商开发**：只在现有供应商池中选择，缺少新供应商引入与认证的持续投入
- **双供应商等于平均分配**：双供应商的核心是风险分散，份额分配应按绩效和能力差异化

## 出处
- [[id:huawei.supply.refined.供应商管理]] — 供应商管理核心内容与ISC关系
- [[id:huawei.supply.refined.集成供应链isc方法论]] — ISC与IPD的供应商界面（EPI机制）
- [[id:huawei.supply.refined.供应链战略]] — 韧性战略下的多源供应策略
