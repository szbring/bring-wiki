---
id: huawei.mtl.concept.lead-management
doc_type: concept
title: 线索管理
domain: huawei-practice
process: 2.0_MTL
layer: concepts
source_authority: 薄云实践
confidence: medium
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 线索管理
aliases:
- Lead Management
- 线索培育
- Lead Nurturing
- MQL / SQL
parent_concept: huawei.mtl.concept.mtl-framework
relations:
- predicate: part_of
  object: huawei.mtl.concept.mtl-framework
- predicate: fed_by
  object: huawei.mtl.concept.marketing-campaign
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
applies_to:
- 营销线索的捕获、评分、培育、移交
- 营销-销售协作（MQL→SQL→OPP）
- 线索质量与转化漏斗管理
related_concepts:
- huawei.ltc.concept.ati
- huawei.ltc.concept.ltc-framework
- huawei.mtl.concept.marketing-campaign
- huawei.mtl.refined.mtl流程架构
---

# 线索管理

## 定义
对营销活动产生的潜在客户线索进行捕获、评分、培育、移交销售的端到端机制，确保营销投资最终兑现为合格销售机会，并在营销与销售之间建立可衡量的协作 SLA。

## 输入 / 输出
- **输入**：营销活动产生的原始线索（landing page 表单 / 名片 / 内容下载等）+ 客户画像规则 + 评分模型
- **输出**：MQL（Marketing Qualified Lead，营销合格线索）→ SQL（Sales Qualified Lead，销售合格线索）→ 移交 LTC 立项
- **关键漏斗**：原始线索 → MQL → SQL → 商机（OPP）→ 中标，每层转化率为关键 KPI

## 角色
- **执行方**：营销运营 / 数字营销团队
- **协同方**：销售开发代表（SDR / BDR，MQL→SQL 阶段电话/邮件培育）+ 客户经理（SQL 接力到 LTC）
- **决策方**：CMO + 销售 VP（MQL/SQL 定义 + SLA 约定）

## 上下游
- **上游**：[[id:huawei.mtl.concept.marketing-campaign]] 营销活动 → 原始线索
- **下游**：SQL → [[id:huawei.ltc.concept.ltc-framework]] 进入 [[id:huawei.ltc.concept.ati]] 立项评审
- **系统**：CRM 线索池 + 营销自动化平台

## 典型误区
- **MQL/SQL 定义不清**：营销和销售对"什么是合格"标准不一致——线索移交后销售拒收，互相甩锅
- **没有 SLA**：销售跟进时效不定，线索冷却变垃圾——必须约定移交后多少小时内联系
- **线索评分纯靠表单字段**：忽视行为数据（多次访问、深度浏览）——评分准确度低
- **没有反馈闭环**：销售拒收的线索原因没回流——营销下次还在生产同样质量的线索

## 出处
- [[id:huawei.mtl.refined.mtl流程架构]] — MTL 流程架构
- 薄云项目实践
- SiriusDecisions Demand Waterfall 漏斗模型（参考）
