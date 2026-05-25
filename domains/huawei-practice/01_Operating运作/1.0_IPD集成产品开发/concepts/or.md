---
id: huawei.ipd.concept.or
doc_type: concept
title: OR 需求管理流程
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: sub_process
canonical_name: OR
aliases:
- Offering Requirement
- Requirement Management
- RM
- 需求管理
- OR 需求管理流程
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: fed_by
  object: huawei.ipd.concept.mm
- predicate: feeds
  object: huawei.ipd.concept.charter
- predicate: feeds
  object: huawei.ipd.concept.cdcp
applies_to:
- 客户需求收集与转化
- 版本规划输入
- 需求变更管理
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.charter
- huawei.ipd.concept.mm
- huawei.ipd.concept.pdt
- huawei.ipd.refined.or-process-overview
- huawei.ipd.refined.requirement-priority
---

# OR 需求管理流程

## 定义
连接市场/客户与研发的五阶段漏斗，确保客户真实需求被识别、分析、分发、实现、验证。

## 输入 / 输出
- **输入**：客户反馈、市场调研、竞品分析、协议标准、法规、运维数据、内部反馈、[[id:huawei.ipd.concept.mm]] 输出的路标
- **输出**：分类分级的需求包——按长/中/短期分发进入 SP/BP、路标、[[id:huawei.ipd.concept.charter]]；需求可追溯记录
- **五阶段漏斗**：
  1. 收集（Raw Requirement，RR）
  2. 分析（Initial Requirement，IR + 价值评估）
  3. 分发（按时间维度：长期→SP/BP、中期→路标、短期→Charter、紧急→变更评审）
  4. 实现（[[id:huawei.ipd.concept.pdt]] 负责）
  5. 验证（通过各级测试闭环）

## 角色
- **全员职责**：需求收集是全员的事，不是产品经理独家
- **RAT**（Requirement Analysis Team）：需求审核团队，由产品经理、市场、研发、测试、服务代表组成，负责第二阶段分析
- **与 PDT 的关系**：PDT 负责第四阶段实现；需求变更需经 RAT 评估后决定是否纳入当前项目

## 上下游
- **上游**：MM 提供市场细分与价值定位 → OR 在此范围内收集和转化具体需求
- **下游**：
  - 长期（3-5年）→ SP/BP 业务规划
  - 中期（1-3年）→ 产品路标
  - 短期（1年内）→ Charter 立项
  - 紧急 → 变更评审后纳入当前开发
- **与 DCP 的关系**：OR 输出的 IR 是 CDCP/PDCP 的核心输入，需求价值评估支撑 Go/Kill 决策

## 典型误区
- **只收集功能需求**：漏掉 DFX（可靠性、可维护性、安全性等）——产品 = 功能需求 + DFX 需求
- **需求不过滤全部接单**：客户提什么做什么——需求资源永远稀缺，必须做价值评估和排序
- **需求不追溯**：Charter 里说"满足客户需求"但具体 RR/IR ID 断档——后续验证无从对照
- **紧急需求占比失控**：大量需求走变更插入当前项目——应保持紧急占比 ≤10%，否则项目永远做不完
- **RAT 没权威**：RAT 评估结论经常被销售/高层覆盖——必须授予 RAT 拒绝权，覆盖必须书面记录原因

## 出处
- [[id:huawei.ipd.refined.or-process-overview]] — OR 需求管理流程概述长文
- [[id:huawei.ipd.refined.requirement-priority]] — 需求优先级方法论（待完善）
- 华为《需求管理流程手册》
