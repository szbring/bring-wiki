---
id: huawei.ltc.concept.ltc-framework
doc_type: concept
title: LTC 线索到回款
domain: huawei-practice
process: 3.0_LTC
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process
canonical_name: LTC
aliases:
- Lead to Cash
- 线索到回款
- 销售流程
- 大销售流程
parent_concept: null
relations:
- predicate: has_part
  object: huawei.ltc.concept.iron-triangle
- predicate: has_part
  object: huawei.ltc.concept.ati
- predicate: has_part
  object: huawei.ltc.concept.atb
- predicate: has_part
  object: huawei.ltc.concept.atc
- predicate: has_part
  object: huawei.ltc.concept.atac
- predicate: fed_by
  object: huawei.dste.concept.sp-bp
- predicate: fed_by
  object: huawei.ipd.concept.ipd-framework
applies_to:
- B2B 大客户销售
- 项目型销售管理
- 从机会点到现金回款的端到端
maturity_stage:
- L1
- L2
- L3
- L4
- L5
related_concepts:
- huawei.dste.concept.sp-bp
- huawei.ipd.concept.ipd-framework
- huawei.ltc.concept.atac
- huawei.ltc.concept.atb
- huawei.ltc.concept.atc
- huawei.ltc.concept.ati
- huawei.ltc.concept.iron-triangle
- huawei.ltc.refined.ltc关键角色与铁三角
- huawei.ltc.refined.ltc核心理念
- huawei.ltc.refined.ltc流程架构
- huawei.overview.concept.dcp
---

# LTC 线索到回款

## 定义
华为以"客户为中心"重构的端到端销售流程，从机会点识别到合同回款全流程跨职能协同，由[[id:huawei.ltc.concept.iron-triangle]]担纲项目级运作。

## 输入 / 输出
- **输入**：BP 销售目标（来自 [[id:huawei.dste.concept.sp-bp]]）、IPD 提供的产品（[[id:huawei.ipd.concept.ipd-framework]]）、市场线索、客户需求
- **输出**：签订合同 → 交付 → 回款；销售经验沉淀；客户关系深化
- **核心阶段**：[[id:huawei.ltc.concept.ati]] → [[id:huawei.ltc.concept.atb]] → [[id:huawei.ltc.concept.atc]] → [[id:huawei.ltc.concept.atac]]
- **三大子流程**：MLE（管理线索）/ MO（管理机会）/ MCE（管理合同执行）

## 角色
- **决策层**：销项决策团 / 各级 DCP 评审团
- **执行层**：[[id:huawei.ltc.concept.iron-triangle]]（客户经理 AR + 解决方案经理 SR + 交付经理 FR）
- **支持层**：技术专家、财经、法务、供应链
- **客户层**：客户决策链各角色（经办/技术/采购/高层）

## 上下游
- **上游**：DSTE 提供战略目标 → MTL 营销活动产生线索 → IPD 提供可销售产品
- **下游**：合同 → ServiceDelivery（服务交付）/ Supply（供应）/ ITR（问题处理）
- **平行**：MCR 管理客户关系（客户级长期关系，与 LTC 项目级运作互补）
- **治理关口**：[[id:huawei.overview.concept.dcp]] 家族（[[id:huawei.ltc.concept.ati]] / [[id:huawei.ltc.concept.atb]] / [[id:huawei.ltc.concept.atc]] / [[id:huawei.ltc.concept.atac]]）

## 典型误区
- **LTC 只是销售部门的事**：没有跨职能就没有 LTC——必须把 SR/FR 拉进来共担目标
- **照搬华为铁三角到小公司**：3 个全职角色对 SMB 太重，关键是"职责到位"而非"必有 3 人"
- **只做线索到合同，不管交付与回款**：那是 LTOC 不是 LTC——回款没到不算闭环
- **机会点不分级**：所有机会同等投入资源，结果重要客户被稀释

## 出处
- [[id:huawei.ltc.refined.ltc流程架构]] — LTC 流程架构（refined）
- [[id:huawei.ltc.refined.ltc关键角色与铁三角]] — LTC 关键角色与铁三角
- [[id:huawei.ltc.refined.ltc核心理念]] — LTC 核心理念
