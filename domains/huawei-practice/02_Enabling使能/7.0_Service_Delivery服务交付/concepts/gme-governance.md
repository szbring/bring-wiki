---
id: huawei.sd.concept.gme-governance
doc_type: concept
title: GME 三层决策机制
domain: huawei-practice
process: 7.0_ServiceDelivery
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: GME 三层决策机制
aliases:
- GME
- Governance-Management-Execution
- 三层决策
parent_concept: huawei.sd.concept.sd-framework
relations:
- predicate: part_of
  object: huawei.sd.concept.sd-framework
- predicate: supports
  object: huawei.sd.concept.sd-framework
applies_to:
- 项目治理
- 客户沟通
- 升级决策
- 战略对齐
related_concepts:
- huawei.sd.concept.sd-framework
- huawei.sd.concept.c8-team
- huawei.sd.concept.evm
- huawei.svcdel.refined.项目交付管理体系
---

# GME 三层决策机制

## 定义
GME 是华为项目采用的三层决策模型，确保高层参与和战略对齐。G（Governance 战略层）：Sponsor 与客户 CXO 季度参与，决策战略对齐、重大变更、升级问题；M（Management 管理层）：PM 与客户 PM 双周/月沟通，决策项目运作、变更谈判、投诉处理；E（Execution 执行层）：项目团队与客户团队日常/周协作，执行进度推进、问题解决、风险应对。三层机制的核心价值在于：明确升级路径——E 层无法解决的问题升级至 M 层，M 层无法决策的升级至 G 层，避免问题淤积。

## 输入 / 输出
- **输入**：项目状态报告、风险/问题清单、变更请求、客户反馈
- **输出**：各层决策结论、升级记录、行动计划
- **核心机制**：E→M→G 逐层升级，G→M→E 逐层下达决策

## 角色
- **G 层参与者**：Sponsor（我方高层）+ 客户 CXO，季度会议
- **M 层参与者**：PM + 客户 PM，双周/月例会
- **E 层参与者**：C8 项目团队 + 客户执行团队，日常/周会
- **升级责任人**：PM 负责判断升级时机并推动决策

## 上下游
- **上游**：[[id:huawei.sd.concept.sd-framework]] 项目启动时建立 GME 沟通机制
- **下游**：各层决策驱动交付调整与资源调配
- **平行**：[[id:huawei.sd.concept.c8-team]] C8 团队在 E 层执行、M 层汇报

## 典型误区
- **G 层形同虚设**：高层不参加季度会议，战略问题无人决策
- **越级决策**：E 层问题直接跳到 G 层，跳过 M 层管理
- **GME 只沟通不决策**：三层会议变成汇报会，没有实质决策产出
- **升级标准模糊**：什么问题升到哪层没有明确规则，导致问题滞留或越级

## 出处
- [[id:huawei.svcdel.refined.项目交付管理体系]] — 项目交付管理体系（五、GME 决策机制）
