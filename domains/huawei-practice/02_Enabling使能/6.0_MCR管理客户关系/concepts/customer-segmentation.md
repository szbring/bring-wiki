---
id: huawei.mcr.concept.customer-segmentation
doc_type: concept
title: 客户分级管理
domain: huawei-practice
process: 6.0_MCR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 客户分级管理
aliases:
- SABC分级
- 客户分级
- Customer Segmentation
parent_concept: huawei.mcr.concept.mcr-framework
relations:
- predicate: part_of
  object: huawei.mcr.concept.mcr-framework
- predicate: depends_on
  object: huawei.mcr.concept.customer-insight
- predicate: feeds
  object: huawei.mcr.concept.kam
applies_to:
- 客户差异化服务投入策略
- 资源分配优先级
- 大客户识别与经营
related_concepts:
- huawei.mcr.concept.mcr-framework
- huawei.mcr.concept.customer-insight
- huawei.mcr.concept.kam
- huawei.mcr.concept.three-layer-relationship
- huawei.ltc.concept.iron-triangle
- huawei.mcr.refined.大客户管理体系kam
- huawei.mcr.refined.客户关系管理
- huawei.mcr.refined.客户洞察与画像方法
---

# 客户分级管理

## 定义
基于客户价值评估对客户进行分级，实施差异化服务投入策略。华为采用 SABC 四级模型：S 类战略客户（营收贡献超 20% 或战略价值极高，高层定期拜访+专属资源）、A 类伙伴客户（核心客户且有扩展潜力，季度 QBR+重点跟进）、B 类普通客户（稳定客户以维护为主，半年回访+标准服务）、C 类长尾客户（贡献小数量多，标准化服务低接触）。客户价值评估综合三个维度：当前价值（营收、利润、份额，权重 40%）、战略价值（品牌背书、行业标杆、技术引领，30%）、成长价值（行业增长率、交叉销售机会，30%）。

## 输入与输出
- **输入**：客户价值评分卡（年营收贡献、利润率、品牌价值、成长性、交叉销售潜力、合作稳定性、付款信用，每项 1-5 分）
- **输出**：客户 SABC 分级结果、差异化服务投入策略、客户团队配置方案
- **分级标准**：S 类 30-35 分，A 类 22-29 分，B 类 15-21 分，C 类 15 分以下

## 角色
- **销售 VP（数据 Owner）**：定义数据标准，推动客户分级决策
- **客户总监**：S/A 类客户分级评审与资源分配
- **客户经理**：提供客户信息与评分依据，执行差异化策略
- **运营经理**：日常客户数据质量管理与分级维护

## 上下游
- **上游**：[[id:huawei.mcr.concept.customer-insight]] 四维洞察 → 提供客户价值评估输入
- **下游**：[[id:huawei.mcr.concept.kam]] KAM 体系 → S/A 类客户进入大客户管理体系；[[id:huawei.mcr.concept.three-layer-relationship]] 三层次关系 → 按客户级别差异化推进
- **关联**：客户分级直接决定 [[id:huawei.ltc.concept.iron-triangle]] 团队配置标准

## 典型误区
- **唯营收论**：只看当前营收不看战略价值和成长价值——可能漏掉未来战略级客户
- **分级一成不变**：客户价值动态变化但分级不更新——资源错配
- **C 类客户完全放弃**：长尾客户中可能隐藏成长型客户——应建立升降级机制
- **分级不与资源挂钩**：分了级但不匹配差异化投入——分级流于形式

## 出处
- [[id:huawei.mcr.refined.客户洞察与画像方法]] — 客户价值评估与 SABC 分级标准
- [[id:huawei.mcr.refined.客户关系管理]] — 客户分级管理框架
- [[id:huawei.mcr.refined.大客户管理体系kam]] — KAM 客户团队配置
