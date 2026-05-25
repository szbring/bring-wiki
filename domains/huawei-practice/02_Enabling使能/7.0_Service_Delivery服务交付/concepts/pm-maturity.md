---
id: huawei.sd.concept.pm-maturity
doc_type: concept
title: 项目管理成熟度模型
domain: huawei-practice
process: 7.0_ServiceDelivery
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 项目管理成熟度模型
aliases:
- PMMM
- 成熟度模型
- PM Maturity
parent_concept: huawei.sd.concept.sd-framework
relations:
- predicate: part_of
  object: huawei.sd.concept.sd-framework
applies_to:
- 组织级项目管理能力评估
- 成熟度诊断
- 能力提升规划
- PMO 建设
related_concepts:
- huawei.sd.concept.sd-framework
- huawei.sd.concept.evm
- huawei.sd.concept.service-quality
- huawei.sd.concept.c8-team
- huawei.sd.concept.gme-governance
- huawei.svcdel.refined.项目交付管理体系
- huawei.svcdel.refined.项目管理成熟度模型
---

# 项目管理成熟度模型

## 定义
华为融合 PMMM 和 CMMI 思想，形成适合交付项目管理的五级成熟度评估体系。L1 初始级：过程无序，依赖个人英雄，项目成功不可复制；L2 可重复级：有基本过程，项目经验可复用，但执行不一致；L3 已定义级：过程标准化，组织级流程统一，所有项目遵循；L4 已管理级：过程可量化，数据驱动，绩效可度量偏差可控；L5 优化级：持续改进，创新引领，基于数据持续优化行业领先。九维度评估框架覆盖：项目计划、进度管理、成本管理、质量管理、风险管理、范围管理、团队管理、沟通管理、知识管理。

## 输入 / 输出
- **输入**：成熟度问卷（九维度逐项评分）、项目绩效数据、访谈结果、对标分析
- **输出**：成熟度等级评定、九维度雷达图、提升路径与行动计划
- **快速诊断**：L1 无计划/无标准 → L2 有模板但不一致 → L3 流程统一 → L4 EVM 可量化 → L5 AI 赋能持续优化

## 角色
- **评估方**：PMO+项目团队自评（季度）、质量部内审（半年度）、第三方外评（年度）
- **改进方**：PMO 驱动流程标准化、PMO+管理层驱动度量体系、管理层驱动数字化平台

## 上下游
- **上游**：[[id:huawei.sd.concept.sd-framework]] 四代演进对应成熟度提升（PM1.0→L2/L3, 2.0→L3/L4, 3.0→L4, 4.0→L4/L5）
- **下游**：成熟度评估结果驱动流程改进与工具建设
- **平行**：[[id:huawei.sd.concept.evm]] 是 L3→L4 的关键提升项；[[id:huawei.sd.concept.c8-team]] 是 L2→L3 的团队建设要求；[[id:huawei.sd.concept.gme-governance]] 是 L4 沟通管理的标杆

## 典型误区
- **追求跨级跃迁**：跳过 L3 标准化直接做 L4 量化，根基不稳
- **评估与改进脱节**：评完等级但不制定提升行动，评估流于形式
- **只看总分不看短板**：九维度中某个 L1 短板被总分掩盖
- **混淆 CMMI 与 PMMM**：CMMI 面向研发过程域，PMMM 面向项目管理知识领域，不可简单套用

## 出处
- [[id:huawei.svcdel.refined.项目管理成熟度模型]] — 项目管理成熟度模型
- [[id:huawei.svcdel.refined.项目交付管理体系]] — 项目交付管理体系
