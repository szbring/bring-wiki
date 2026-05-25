---
id: huawei.dste.concept.dste-framework
doc_type: concept
title: DSTE 开发战略到执行
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process
canonical_name: DSTE
aliases:
- Develop Strategy to Execution
- 开发战略到执行
- 战略到执行
- 大 DSTE
parent_concept: null
relations:
- predicate: has_part
  object: huawei.dste.concept.sp-bp
- predicate: has_part
  object: huawei.dste.concept.blm
- predicate: has_part
  object: huawei.dste.concept.sp-dcp
- predicate: has_part
  object: huawei.dste.concept.bp-dcp
- predicate: has_part
  object: huawei.dste.concept.bp-qr-dcp
- predicate: has_part
  object: huawei.dste.concept.sa-dcp
- predicate: feeds
  object: huawei.ipd.concept.ipd-framework
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
applies_to:
- 公司级 / 业务单元级战略管理
- 跨年度战略落地
- 战略与年度计划的对齐
maturity_stage:
- L1
- L2
- L3
- L4
- L5
related_concepts:
- huawei.dste.concept.blm
- huawei.dste.concept.bp-dcp
- huawei.dste.concept.bp-qr-dcp
- huawei.dste.concept.sa-dcp
- huawei.dste.concept.sp-bp
- huawei.dste.concept.sp-dcp
- huawei.dste.refined.dste流程架构
- huawei.dste.refined.sp-bp战略规划体系
- huawei.ipd.concept.ipd-framework
- huawei.ltc.concept.ltc-framework
- huawei.overview.concept.dcp
---

# DSTE 开发战略到执行

## 定义
华为把战略从产生到落地端到端管理的流程体系，覆盖战略规划（SP）、年度业务计划（BP）、季度回顾（BP-QR）和战略审视（SA）四大节奏。

## 输入 / 输出
- **输入**：使命愿景、行业洞察（PEST/五看）、上一周期执行差距、客户与竞争情报、技术与商业模式趋势
- **输出**：发布的中长期战略（SP）、年度业务计划（BP）、季度回顾结论与调整方案、战略审视决议；下游 IPD/LTC/MTL 等流程的方向与资源约束
- **节奏**：年度 SP/BP（4-11 月）+ 季度 BP-QR + 不定期 SA

## 角色
- **决策方**：EMT（执行管理团队）/ 公司级战略与发展委员会
- **执行方**：战略与发展（S&D）部门，各业务单元（BG/BU）战略部
- **协同方**：财经（预算）、HR（组织/人才计划）、各业务流 Owner

## 上下游
- **上游**：使命愿景 + 行业洞察 + 客户/竞争/技术情报
- **下游**：[[id:huawei.ipd.concept.ipd-framework]] 接 SP/BP 方向 → 立项 / [[id:huawei.ltc.concept.ltc-framework]] 接 BP 销售目标 / [[id:huawei.dste.concept.sa-dcp]] 反馈调整 SP
- **治理关口**：[[id:huawei.overview.concept.dcp]] 家族（[[id:huawei.dste.concept.sp-dcp]] / [[id:huawei.dste.concept.bp-dcp]] / [[id:huawei.dste.concept.bp-qr-dcp]] / [[id:huawei.dste.concept.sa-dcp]]）

## 典型误区
- **战略 = 老板拍脑袋**：DSTE 强调结构化方法（[[id:huawei.dste.concept.blm]] 业务领先模型），靠流程而非天才
- **SP 与 BP 脱节**：BP 不承接 SP 必赢战役，年度做完发现没推进战略——必须用 [[id:huawei.dste.concept.sp-bp]] 衔接机制
- **战略只在战略部**：业务部门不参与制定，执行就敷衍——SP/BP 是高管深度参与的研讨会而非"汇报"
- **战略冻结**：发布后一年不动——[[id:huawei.dste.concept.sa-dcp]] 战略审视就是为了允许中途修正

## 出处
- [[id:huawei.dste.refined.dste流程架构]] — DSTE 流程架构（refined）
- [[id:huawei.dste.refined.sp-bp战略规划体系]] — SP/BP 战略规划体系
- 华为《价值为纲》战略管理章节
