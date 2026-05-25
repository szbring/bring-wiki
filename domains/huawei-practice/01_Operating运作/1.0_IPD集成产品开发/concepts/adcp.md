---
id: huawei.ipd.concept.adcp
doc_type: concept
title: ADCP 可获得性决策评审
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process_gate
canonical_name: ADCP
aliases:
- Availability DCP
- Available DCP
- 可获得性决策评审
- 开发决策评审
- IPD 可获得性阶段 DCP
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: requires_role
  object: huawei.ipd.concept.ipmt
- predicate: depends_on
  object: huawei.ipd.concept.tr
- predicate: follows
  object: huawei.ipd.concept.pdcp
- predicate: precedes
  object: huawei.ipd.concept.ldcp
applies_to:
- 开发完成与发布前决策
- 小批量/试产/验证启动
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.ldcp
- huawei.ipd.concept.pdcp
- huawei.ipd.concept.pdt
- huawei.ipd.refined.dcp-mechanism
---

# ADCP 可获得性决策评审

## 定义
IPD 可获得性阶段末，IPMT 对"开发目标达成、产品可小批量/试产进入验证"的决策。

## 输入 / 输出
- **输入**：开发完成度报告、单元/集成测试结果、TR4/TR5 通过结论、试产或 β 验证计划、质量基线评估、更新版风险清单
- **输出**：Go（进入 Launch 阶段，启动试产/客户试用）/ Kill（质量不达标且无法补救，终止）/ Hold（回补开发或测试）
- **此点前累计资源投入**：约 50%

## 角色
- **决策方**：[[id:huawei.ipd.concept.ipmt]]
- **执行方**：[[id:huawei.ipd.concept.pdt]] 全员
- **前置评审方**：IRT（TR4 验证方案评审、TR5 产品发布就绪评审）

## 上下游
- **上游**：[[id:huawei.ipd.concept.pdcp]] Go → 开发执行 → TR3/TR4/TR5 通过
- **下游**：Go → Launch 阶段试产与上市准备，下一关口 [[id:huawei.ipd.concept.ldcp]]
- **关键依赖**：P0/P1 缺陷全部关闭或有明确规避方案是 Go 的底线

## 典型误区
- **把 ADCP 当"上市评审"**：ADCP 判"可以进入验证/试产"，不是"可以全面发货"——后者是 LDCP 的职责
- **缺陷堆积到 LDCP 再处理**：ADCP 是质量守门第一关，缺陷带进 Launch 成本飙升
- **试产计划缺失**：没有明确的试产客户、范围、评估指标就 Go，等于盲飞
- **供应链未 ready**：关键物料、产能、工装未到位，Go 了也发不出货，必须在 ADCP 核查

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制长文（ADCP 章节）
- 华为 IPD 产品开发流程手册——可获得性阶段定义
