---
id: huawei.ipd.concept.pdt
doc_type: concept
title: PDT 产品开发团队
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: role
canonical_name: PDT
aliases:
- Product Development Team
- 产品开发团队
- 跨功能产品开发团队
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: supports
  object: huawei.ipd.concept.ipmt
- predicate: produces
  object: huawei.ipd.concept.charter
- predicate: role_in
  object: huawei.ipd.concept.cdcp
- predicate: role_in
  object: huawei.ipd.concept.pdcp
- predicate: role_in
  object: huawei.ipd.concept.adcp
- predicate: role_in
  object: huawei.ipd.concept.ldcp
applies_to:
- 新产品开发项目
- 重大版本开发
- 跨功能协同执行
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.charter
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.irt
- huawei.ipd.concept.or
- huawei.ipd.refined.dcp-mechanism
- huawei.ipd.refined.ipd-organization
---

# PDT 产品开发团队

## 定义
端到端对产品商业成功负责的跨功能产品开发执行团队。

## 输入 / 输出
- **输入**：IPMT 批准的 [[id:huawei.ipd.concept.charter]]；来自 [[id:huawei.ipd.concept.or]] 的需求包；TPP/TPD 提供的技术/平台
- **输出**：阶段交付物（需求、方案、代码、测试、上市物料）；各 DCP 的评审包；可发布的产品
- **端到端职责**：从概念立项到上市到生命周期末，同一个 PDT 负责（不是开发完就解散）

## 角色
- **PDT 经理**：团队唯一 leader，对商业结果负全责；通常由产品经理或资深项目经理担任
- **核心代表（7-10 人）**：市场 Rep、研发 Rep、测试 Rep、服务 Rep、供应 Rep、采购 Rep、财经 Rep、质量 Rep（关键：各 Rep 在本职能线有代表权）
- **扩展成员**：按需的技术专家、设计、用户研究等
- **与职能部门的关系**：矩阵式——PDT 经理负责项目目标，职能经理负责人员能力与资源池

## 上下游
- **上游**：IPMT 立项授权 → PDT 组建 → 接收 MM/OR 的市场与需求输入
- **下游**：PDT 产出经 DCP 放行 → 发布给市场/服务/供应 → 持续由 LMT 管理生命周期
- **关键协作**：
  - 与 [[id:huawei.ipd.concept.irt]]：TR 评审通过是 DCP 前置
  - 与 [[id:huawei.ipd.concept.ipmt]]：在 DCP 汇报并争取资源

## 典型误区
- **PDT 只是"项目组"**：PDT 是端到端跨功能团队，不是只含研发的项目组
- **核心代表层级不够**：派"打杂的"当 Rep，决策回去还要等职能老板——PDT 必须能在会上拍板
- **PDT 经理没实权**：只当协调员不当老板——必须有项目资源和绩效分配权
- **职能墙不破**：各 Rep 只代表本职能本位利益，不对产品整体负责——要求 PDT 用产品整体绩效而非职能 KPI
- **PDT 在 LDCP 后就解散**：研发完交给服务/市场就走——应负责到生命周期末，至少到第一次 EDCP

## 出处
- [[id:huawei.ipd.refined.ipd-organization]] — IPD 组织体系（PDT 组建、权责、绩效）
- [[id:huawei.ipd.refined.dcp-mechanism]] — PDT 在各 DCP 的职责
- 华为《PDT 运作手册》
