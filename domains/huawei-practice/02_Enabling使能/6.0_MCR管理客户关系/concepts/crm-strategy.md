---
id: huawei.mcr.concept.crm-strategy
doc_type: concept
title: CRM 策略与数字化
domain: huawei-practice
process: 6.0_MCR
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: CRM策略与数字化
aliases:
- CRM策略
- 客户关系数字化
- Customer Relationship Digitization
parent_concept: huawei.mcr.concept.mcr-framework
relations:
- predicate: part_of
  object: huawei.mcr.concept.mcr-framework
- predicate: feeds
  object: huawei.mcr.concept.kam
- predicate: depends_on
  object: huawei.mcr.concept.three-layer-relationship
applies_to:
- 客户关系管理流程固化与提效
- 客户数据治理与分析驱动
- 客户健康度量化评估
related_concepts:
- huawei.mcr.concept.mcr-framework
- huawei.mcr.concept.kam
- huawei.mcr.concept.three-layer-relationship
- huawei.mcr.concept.customer-insight
- huawei.mcr.refined.大客户管理体系kam
- huawei.mcr.refined.客户关系数字化
---

# CRM 策略与数字化

## 定义
CRM（Customer Relationship Management）不是软件系统，而是管理策略——系统只是工具，策略才是灵魂。华为实践表明客户关系管理的科学部分（流程、数据、规则）可以数字化和复制，艺术部分（人际互动、情感连接）则需要数字化工具提供支撑。CRM 四层架构：策略层（客户分级、差异化服务策略）、流程层（MCR 流程标准化与固化）、数据层（客户信息采集、治理与应用）、工具层（CRM 软件系统）。落地三阶段：规范期（数据在线、流程在线，3-6 月）→ 效率期（流程提效、数据驱动，6-12 月）→ 智能期（AI 辅助决策，12-24 月）。

## 输入与输出
- **输入**：客户主数据（基本信息、组织信息、交易信息、互动记录）、MCR 流程规范
- **输出**：360 度客户视图、客户健康度评分（互动活跃度 20%+项目参与度 15%+满意度 20%+增长趋势 15%+续约风险 15%+竞争渗透 15%）、Pipeline 分析、流失预警
- **健康度阈值**：< 60 分红色预警需立即行动，60-80 分黄色关注需主动跟进，> 80 分绿色健康保持维护

## 角色
- **数据 Owner（销售 VP）**：定义数据标准，推动数据质量提升
- **数据 Steward（运营经理）**：日常数据质量管理与问题处理
- **系统 Admin（IT）**：系统配置、权限管理、集成维护
- **数据录入人（客户经理）**：按规范录入和更新客户数据

## 上下游
- **上游**：[[id:huawei.mcr.concept.customer-insight]] 客户洞察 → 提供数据采集维度；[[id:huawei.mcr.concept.three-layer-relationship]] 三层关系 → 流程固化对象
- **下游**：[[id:huawei.mcr.concept.kam]] KAM 体系 → CRM 提供客户健康度与 Pipeline 数据支撑 QBR 决策
- **关联**：CRM 数据层打通 ERP/财务/交付系统，支撑全流程数据驱动

## 典型误区
- **CRM 等于买软件**：系统只是工具层，没有策略层和流程层的 CRM 必然失败
- **销售不愿意用**：录入负担重看不到价值——应简化录入让销售先用起来看到价值
- **数据质量无人管**：缺乏数据 Owner 制度——纳入考核，建立数据治理六维度（完整性/准确性/一致性/及时性/唯一性/合规性）
- **CRM 与其他系统孤岛**：不与 ERP/财务打通——规划集成方案，分步实施

## 出处
- [[id:huawei.mcr.refined.客户关系数字化]] — CRM 四层架构、客户健康度评分、落地路径
- [[id:huawei.mcr.refined.大客户管理体系kam]] — KAM 运营机制与 CRM 集成
- 华为 CRM 落地实践
