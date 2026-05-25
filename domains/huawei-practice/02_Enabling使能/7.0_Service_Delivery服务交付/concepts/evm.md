---
id: huawei.sd.concept.evm
doc_type: concept
title: 挣值管理 EVM
domain: huawei-practice
process: 7.0_ServiceDelivery
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 挣值管理
aliases:
- EVM
- Earned Value Management
- 挣值法
parent_concept: huawei.sd.concept.sd-framework
relations:
- predicate: part_of
  object: huawei.sd.concept.sd-framework
- predicate: supports
  object: huawei.sd.concept.c8-team
applies_to:
- 项目进度监控
- 成本控制
- 绩效度量
- 偏差分析
related_concepts:
- huawei.sd.concept.sd-framework
- huawei.sd.concept.c8-team
- huawei.sd.concept.pm-maturity
- huawei.svcdel.refined.项目交付管理体系
- huawei.svcdel.refined.项目管理成熟度模型
---

# 挣值管理 EVM

## 定义
挣值管理（Earned Value Management）是华为项目监控阶段的核心量化方法，通过综合度量范围、进度和成本，客观评估项目绩效。三个基础变量：PV（Planned Value，计划价值，即预算成本）、EV（Earned Value，挣值，即已完成工作的预算价值）、AC（Actual Cost，实际成本，即已完成工作的实际花费）。由此推导四个关键指标：SV=EV-PV（进度偏差，<0 表示落后）、CV=EV-AC（成本偏差，<0 表示超支）、SPI=EV/PV（进度绩效指数，<1 表示落后）、CPI=EV/AC（成本绩效指数，<1 表示超支）。当偏差超出阈值时触发纠正措施。

## 输入 / 输出
- **输入**：项目基准计划（WBS+预算）、实际进度与成本数据
- **输出**：进度周报/月报中的 EVM 分析、偏差预警、纠正行动建议
- **核心公式**：SV=EV-PV, CV=EV-AC, SPI=EV/PV, CPI=EV/AC

## 角色
- **项目控制（PC）**：EVM 数据采集、计算分析与报告
- **项目经理（PM）**：基于 EVM 结果决策纠正措施
- **财务代表（FR）**：提供实际成本数据，协助成本偏差分析

## 上下游
- **上游**：[[id:huawei.sd.concept.sd-framework]] DR1 批准项目基准计划后启用 EVM
- **下游**：EVM 偏差预警 → 纠正措施 → 更新计划或申请变更
- **平行**：[[id:huawei.sd.concept.c8-team]] PC 角色负责 EVM 执行；[[id:huawei.sd.concept.pm-maturity]] 成熟度 L4 要求 EVM 挣值管理

## 典型误区
- **只看进度不看成本**：只跟踪进度偏差 SV/SPI，忽视成本偏差 CV/CPI
- **EV 计算口径不一致**：不同项目 EV 确认方式（0/100 法、50/50 法等）不统一，数据不可比
- **偏差预警无阈值**：没有设定偏差容忍区间，所有偏差都报警或都忽略
- **EVM 数据滞后**：AC 采集不及时，EVM 分析基于过期数据，决策失准

## 出处
- [[id:huawei.svcdel.refined.项目交付管理体系]] — 项目交付管理体系（监控阶段 EVM 挣值分析）
- [[id:huawei.svcdel.refined.项目管理成熟度模型]] — 成熟度模型（L3→L4 提升项含 EVM）
