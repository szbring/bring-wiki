---
id: huawei.supply.concept.supply-chain-strategy
doc_type: concept
title: 供应链战略取向
domain: huawei-practice
process: 8.0_Supply
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 供应链战略取向
aliases:
- 供应链战略
- Lean/Agile/Resilient
- 供应链战略选择
parent_concept: huawei.supply.concept.isc-framework
relations:
- predicate: part_of
  object: huawei.supply.concept.isc-framework
- predicate: depends_on
  object: huawei.dste.concept.dste-framework
applies_to:
- 供应链体系设计方向选择
- 分品类分场景差异化策略
- 业务战略与供应链对齐
related_concepts:
- huawei.supply.concept.isc-framework
- huawei.supply.concept.sop
- huawei.supply.concept.supplier-management
- huawei.dste.concept.dste-framework
- huawei.supply.refined.供应链战略
- huawei.supply.refined.集成供应链isc方法论
---

# 供应链战略取向

## 定义
供应链战略取向决定了供应链体系的设计方向和投入重点。三种基本取向：精益（Lean）以消除浪费和最低成本为目标，适用于需求稳定、产品标准化的场景，做法包括JIT、零库存；敏捷（Agile）以快速响应需求变化为目标，适用于需求波动大、产品定制化的场景，做法包括延迟分化、模块化设计、安全库存；韧性（Resilient）以抵抗冲击和快速恢复为目标，适用于供应中断风险高的场景，做法包括多源供应、备选供应商、产能冗余。华为采用"精益+敏捷+韧性"复合战略：持续降本与库存优化（精益）、CTO按订单配置与快速交付（敏捷）、多源供应与国产替代（韧性）。战略制定可基于Fisher模型匹配产品类型，或基于不确定性矩阵选择组合。

## 输入与输出
- **输入**：客户需求特征（稳定性/定制化程度/交付期望）、供应不确定性、竞争维度（成本/速度/安全）
- **输出**：供应链战略取向选择（精益/敏捷/韧性或组合）、供应网络设计方案、重点投入方向

## 角色
- **供应链战略制定者**：分析需求与供应不确定性，选择战略取向组合
- **业务负责人**：提供业务战略输入，确保供应链战略与业务战略对齐
- **品类管理者**：按品类特征差异化应用不同战略取向

## 上下游
- **上游**：DSTE流程输出的业务战略决定供应链战略方向；产品类型与市场特征影响取向选择
- **下游**：供应链战略取向指导ISC流程设计、供应网络布局、供应商策略和库存策略
- **战略执行框架**：供应网络设计、流程能力建设、组织能力建设、数字化能力、风险管理

## 典型误区
- **追求单一取向**：只选精益导致柔性不足，突发事件冲击巨大；只选韧性则成本过高
- **战略与业务不对齐**：成本领先业务却走敏捷路线，或快速响应业务却走精益路线
- **不分品类一刀切**：不同产品线需求特征差异大，应分品类差异化选型
- **战略制定后不执行**：缺少从战略到供应网络设计、流程建设的落地路径

## 出处
- [[id:huawei.supply.refined.供应链战略]] — 三种战略取向、华为复合战略与Fisher模型详述
- [[id:huawei.supply.refined.集成供应链isc方法论]] — ISC变革中的战略取向体现
