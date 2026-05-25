---
id: huawei.ipd.concept.ipd-framework
doc_type: concept
title: IPD 集成产品开发体系
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process
canonical_name: IPD
aliases:
- Integrated Product Development
- 集成产品开发
- 华为 IPD
- 大 IPD
parent_concept: null
relations:
- predicate: has_part
  object: huawei.ipd.concept.mm
- predicate: has_part
  object: huawei.ipd.concept.or
- predicate: has_part
  object: huawei.ipd.concept.tr
- predicate: has_part
  object: huawei.ipd.concept.plm
- predicate: has_part
  object: huawei.ipd.concept.cbb
- predicate: fed_by
  object: huawei.dste.concept.sp-bp
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
- predicate: feeds
  object: huawei.itr.concept.itr-framework
applies_to:
- 产品型企业
- 跨功能研发管理
- 从机会到上市到退市的端到端产品管理
maturity_stage:
- L1
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.cbb
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.irt
- huawei.ipd.concept.mm
- huawei.ipd.concept.or
- huawei.ipd.concept.pdt
- huawei.ipd.concept.plm
- huawei.ipd.concept.tr
- huawei.ipd.refined.ipd-overview
- huawei.overview.concept.dcp
---

# IPD 集成产品开发体系

## 定义
把产品开发作为投资来管理的端到端跨功能产品创新流程体系。

## 输入 / 输出
- **输入**：战略方向与业务计划（来自 DSTE 的 SP/BP）、市场机会、客户需求、技术演进趋势
- **输出**：满足市场需求并实现商业回报的产品；经 EDCP 退市的老产品；可复用的 [[id:huawei.ipd.concept.cbb]] 与技术资产
- **范围三层**：
  - **小 IPD**：狭义产品开发流程（Concept → Plan → Available → Launch → Lifecycle）
  - **中 IPD**：产品开发 + [[id:huawei.ipd.concept.mm]] + [[id:huawei.ipd.concept.or]] 三大流程
  - **大 IPD**：中 IPD + 技术规划 (TPP)+ 技术开发 (TPD)+ [[id:huawei.ipd.concept.plm]] + 组织与绩效激励

## 角色
- **决策层**：[[id:huawei.ipd.concept.ipmt]]（投资决策团）
- **执行层**：[[id:huawei.ipd.concept.pdt]]（产品开发团队，跨职能）
- **评审层**：[[id:huawei.ipd.concept.irt]]（独立技术评审团）
- **生命周期层**：LMT（生命周期管理团，EDCP 后接手）

## 上下游
- **上游**：DSTE 提供战略方向 → IPD 的 [[id:huawei.ipd.concept.mm]] 识别具体机会
- **下游**：IPD 产出产品 → LTC 转化为订单回款 / ITR 处理上市后问题
- **平行**：供应、采购、财经、HR 等使能/支撑流程与 IPD 协同
- **治理关口**：[[id:huawei.overview.concept.dcp]] 家族（CDCP/PDCP/ADCP/LDCP/EDCP）+ [[id:huawei.ipd.concept.tr]] 家族

## 典型误区
- **把 IPD 等同于产品开发流程**：这是小 IPD，漏掉市场管理和需求管理就做不成端到端
- **技术驱动研发**：IPD 的核心是"需求驱动"，技术可行性是前提不是起点
- **照搬华为阶段划分**：中小企业照抄 6 阶段 5 DCP 必然过度，要按规模裁剪（保 CDCP/LDCP/EDCP 三个关键关口最有效）
- **只改流程不改组织**：IPD 必然打破部门墙，不配套 PDT 团队机制就只是开评审会
- **变革没有高层决心**：IPD 变革周期 1-3 年，业绩短期下降不可避免，缺高层支持必然失败

## 出处
- [[id:huawei.ipd.refined.ipd-overview]] — IPD 集成产品开发（00_概述长文）
- [[id:huawei.ipd.raw.bycgzx-ipd-reinterpretation]] — IPD 解读公众号原文（溯源）
- 华为《IPD 产品开发流程手册》、《华为能你也能 IPD》
