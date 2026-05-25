---
id: huawei.dste.concept.sp-bp
doc_type: concept
title: SP/BP 战略规划与年度业务计划
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: method
canonical_name: SP/BP
aliases:
- SP-BP
- Strategic Plan / Business Plan
- 战略规划与业务计划
- 战略规划体系
parent_concept: huawei.dste.concept.dste-framework
relations:
- predicate: part_of
  object: huawei.dste.concept.dste-framework
- predicate: gated_by
  object: huawei.dste.concept.sp-dcp
- predicate: gated_by
  object: huawei.dste.concept.bp-dcp
- predicate: feeds
  object: huawei.ipd.concept.mm
- predicate: feeds
  object: huawei.ipd.concept.ipd-framework
applies_to:
- 公司级与业务单元级战略规划
- 年度经营计划制定
- SP→BP→KPI 的逐级承接
related_concepts:
- huawei.dste.concept.bp-dcp
- huawei.dste.concept.sa-dcp
- huawei.dste.concept.sp-dcp
- huawei.dste.refined.blm战略管理模型
- huawei.dste.refined.sp-bp战略规划体系
- huawei.ipd.concept.mm
- huawei.ltc.concept.ltc-framework
---

# SP/BP 战略规划与年度业务计划

## 定义
SP（中长期战略规划，3-5 年）与 BP（年度业务计划，1 年）构成华为战略管理的"双轮驱动"——SP 定方向与必赢战役，BP 定年度目标与资源分配，BP 必须承接 SP。

## 输入 / 输出
- **SP 输入**：使命愿景、五看分析（看行业/市场/竞争/自己/机会）、上年度差距
- **SP 输出**：3-5 年战略目标、必赢战役清单、业务设计（客户选择/价值主张/盈利模式/控制点）、年度里程碑
- **BP 输入**：SP 已发布 + 上年度执行情况 + 当年外部约束
- **BP 输出**：年度 KPI、重点项目清单、组织/人才/预算计划
- **节奏**：SP 4-8 月制定，BP 9-11 月制定

## 角色
- **决策方**：EMT 评审并发布
- **制定方**：S&D 部门牵头 + 各 BG/BU 战略部 + 业务高管研讨
- **承接方**：业务流 Owner（IPD/LTC 等）把 SP/BP 拆解为各自计划

## 上下游
- **上游**：DSTE 整体节奏 → 启动 SP 或 BP 周期
- **下游**：BP → [[id:huawei.ipd.concept.mm]] 接战略意图做产品规划 / BP → [[id:huawei.ltc.concept.ltc-framework]] 接销售目标 / BP → 部门 KPI
- **关口**：[[id:huawei.dste.concept.sp-dcp]] 评审 SP 通过 → 才能启动 BP；[[id:huawei.dste.concept.bp-dcp]] 评审 BP 通过 → 锁定年度预算

## 典型误区
- **BP 不承接 SP**：BP 编制时只看上年实绩外推，不引用 SP 必赢战役，导致战略空转
- **SP 做成 PPT 表演**：研讨深度不够，高管签字了事——华为 SP 研讨持续 1-2 周，深度数据 + 反复辩论
- **必赢战役 ≠ 重点工作**：必赢战役是"赢了游戏就能赢"的少数关键点（≤5 个），不是部门重点工作清单
- **SP/BP 一发布就锁死**：[[id:huawei.dste.concept.sa-dcp]] 战略审视就是中期修正机制，不能僵化

## 出处
- [[id:huawei.dste.refined.sp-bp战略规划体系]] — SP/BP 战略规划体系（refined）
- [[id:huawei.dste.refined.blm战略管理模型]] — BLM 业务领先模型（SP 制定的核心方法）
- 华为《价值为纲》第二章 战略的逻辑
