---
id: huawei.ipd.concept.ipmt
doc_type: concept
title: IPMT 投资决策团
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: role
canonical_name: IPMT
aliases:
- Integrated Portfolio Management Team
- 投资决策团
- 产品投资管理团
- 组合决策团
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: role_in
  object: huawei.ipd.concept.cdcp
- predicate: role_in
  object: huawei.ipd.concept.pdcp
- predicate: role_in
  object: huawei.ipd.concept.adcp
- predicate: role_in
  object: huawei.ipd.concept.ldcp
- predicate: role_in
  object: huawei.ipd.concept.edcp
- predicate: supports
  object: huawei.ipd.concept.pdt
applies_to:
- 产品投资决策
- 跨产品组合资源分配
- DCP 评审会主持
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.charter
- huawei.ipd.concept.pdt
- huawei.ipd.refined.dcp-mechanism
- huawei.ipd.refined.ipd-organization
- huawei.overview.concept.dcp
---

# IPMT 投资决策团

## 定义
代表公司行使产品投资决策权的跨职能高层团队，是 DCP 的决策方。

## 输入 / 输出
- **输入**：[[id:huawei.ipd.concept.pdt]] 提交的 [[id:huawei.ipd.concept.charter]]、业务计划、技术方案、财务预测、风险清单
- **输出**：Go/Kill/Hold 书面决策；资源（人/钱/物）的授权或回收；跨产品线优先级调整
- **决策权限**：投资、立项、Kill、关键里程碑放行、跨项目资源再分配

## 角色
- **组成**：通常 7-11 人，覆盖市场、研发、服务、供应、财经、质量、HR 等关键职能的高层代表
- **主任**：产品线总经理或事业部总裁（不是研发负责人）
- **常设秘书**：PDT 经理对接人（不含投票权）
- **基本要求**：成员在各自职能线有最终签字权，避免"会上答应回去被老板推翻"

## 上下游
- **上游**：DSTE 的 SP/BP 输出 → IPMT 拿到投资预算与战略优先级
- **下游**：IPMT 决策 → [[id:huawei.ipd.concept.pdt]] 执行 / 产品线资源再分配
- **评审范围**：[[id:huawei.overview.concept.dcp]] 家族全部关口都由 IPMT 决策
- **与 IRT 的分工**：IRT 判"做得对不对"（TR），IPMT 判"值不值得做"（DCP），两者分离

## 典型误区
- **IPMT 被架空成橡皮图章**：成员不读材料、不提问、全票通过——必设必问清单，前 3 次评审建议顾问介入
- **用研发总监当 IPMT 主任**：产品投资决策是跨职能事务，研发单点决策会偏向技术理想化
- **成员层级不够**：派代表参会但代表无签字权——等于没开
- **IPMT 会议变成项目汇报会**：必须带三选一明确决议，不得"带回去研究"
- **多头 IPMT**：一个产品被多个 IPMT 评审——必须唯一归属，否则互相推诿

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（含 IPMT 职责与决策流程）
- [[id:huawei.ipd.refined.ipd-organization]] — IPD 组织体系（IPMT 组建与运作规范）
- 华为 IPMT 运作指南
