---
id: huawei.mtl.concept.mtl-framework
doc_type: concept
title: MTL 市场到线索
domain: huawei-practice
process: 2.0_MTL
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: process
canonical_name: MTL
aliases:
- Market to Lead
- 市场到线索
- 营销流程
- 大营销流程
parent_concept: null
relations:
- predicate: has_part
  object: huawei.mtl.concept.market-insight
- predicate: has_part
  object: huawei.mtl.concept.brand-management
- predicate: has_part
  object: huawei.mtl.concept.marketing-campaign
- predicate: has_part
  object: huawei.mtl.concept.lead-management
- predicate: feeds
  object: huawei.ipd.concept.mm
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
- predicate: fed_by
  object: huawei.dste.concept.sp-bp
applies_to:
- B2B 营销
- 品牌建设
- 线索生成与培育
- 与销售（LTC）的衔接
maturity_stage:
- L1
- L2
- L3
- L4
- L5
related_concepts:
- huawei.dste.concept.sp-bp
- huawei.ipd.concept.mm
- huawei.ltc.concept.ltc-framework
- huawei.mtl.concept.brand-management
- huawei.mtl.concept.lead-management
- huawei.mtl.concept.market-insight
- huawei.mtl.concept.marketing-campaign
- huawei.mtl.refined.mtl市场洞察方法论
- huawei.mtl.refined.mtl核心理念
- huawei.mtl.refined.mtl流程架构
---

# MTL 市场到线索

## 定义
华为以"客户洞察驱动"为内核构建的端到端营销流程，从市场洞察到品牌建设到营销活动到线索培育，承接 DSTE 战略 + 喂养 LTC 销售管道与 IPD 产品规划。

## 输入 / 输出
- **输入**：BP 营销目标（来自 [[id:huawei.dste.concept.sp-bp]]）、市场情报、客户与竞争数据、产品上市节奏
- **输出**：合格销售线索（喂给 LTC）、市场洞察（喂给 IPD MM 做产品规划）、品牌资产、客户认知改善
- **核心子流程**：[[id:huawei.mtl.concept.market-insight]] → [[id:huawei.mtl.concept.brand-management]] → [[id:huawei.mtl.concept.marketing-campaign]] → [[id:huawei.mtl.concept.lead-management]]

## 角色
- **决策方**：CMO / 营销委员会
- **执行方**：市场部（洞察、品牌、活动）+ 数字营销
- **协同方**：销售部门（线索接力）、产品部（[[id:huawei.ipd.concept.mm]]）、传播

## 上下游
- **上游**：[[id:huawei.dste.concept.sp-bp]] 战略 → 营销目标分解
- **下游**：合格线索 → [[id:huawei.ltc.concept.ltc-framework]] / 市场洞察 → [[id:huawei.ipd.concept.mm]]
- **平行**：MCR 客户关系（互补：MCR 关注存量大客户深耕，MTL 偏增量获客）

## 典型误区
- **MTL = 做活动**：把流程窄化为发布会 / 展会——丧失洞察 + 品牌 + 线索的端到端
- **市场与销售脱节**：营销做线索没人接，销售喊缺线索却不反馈——必须 SLA + 反馈闭环
- **不衡量营销 ROI**：只看活动数量不看转化漏斗——营销变成预算消耗中心
- **品牌虚化**：把品牌当成 logo + 口号——品牌是客户心智占位的累积，要长期投资

## 出处
- [[id:huawei.mtl.refined.mtl流程架构]] — MTL 流程架构
- [[id:huawei.mtl.refined.mtl核心理念]] — MTL 核心理念
- [[id:huawei.mtl.refined.mtl市场洞察方法论]] — MTL 市场洞察方法论
- 华为《以客户为中心》营销章节
