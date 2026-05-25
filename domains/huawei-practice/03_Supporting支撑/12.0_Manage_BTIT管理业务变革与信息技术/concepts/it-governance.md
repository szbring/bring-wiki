---
id: huawei.btit.concept.it-governance
doc_type: concept
title: IT 治理体系
domain: huawei-practice
process: 12.0_BTIT
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: IT 治理
aliases:
- IT Governance
- IT 投资决策
- IT 管理体系
parent_concept: huawei.btit.concept.btit-framework
relations:
- predicate: part_of
  object: huawei.btit.concept.btit-framework
- predicate: supports
  object: huawei.btit.concept.business-transformation
- predicate: supports
  object: huawei.btit.concept.digital-transformation
applies_to:
- IT 投资优先级决策
- IT 与业务对齐
- IT 服务运营
related_concepts:
- huawei.btit.concept.btit-framework
- huawei.btit.concept.enterprise-architecture
- huawei.btit.refined.it治理体系
---

# IT 治理体系

## 定义
华为为确保 IT 投资始终服务于业务变革目标而构建的决策、问责、监督机制，覆盖 IT 战略、IT 投资组合管理、IT 项目交付、IT 运营。

## 输入 / 输出
- **输入**：业务变革诉求 + IT 现状评估 + 资源约束（预算、人才）+ 技术趋势
- **输出**：IT 战略蓝图（与业务战略对齐）+ IT 投资清单（按价值排序）+ 项目交付计划 + 运营 KPI
- **核心机制**：IT 投资决策委员会、IT 架构评审委员会、IT 服务交付治理

## 角色
- **决策方**：IT 委员会 / CIO + EMT 重点项目共审
- **执行方**：IT 部门各模块（基础设施 / 应用 / 数据 / 安全）
- **业务方**：作为 IT 客户提需求并验收

## 上下游
- **上游**：[[id:huawei.btit.concept.btit-framework]] BTC 决定整体变革优先级 → IT 治理决策具体投资
- **下游**：IT 投资 → 落地的应用系统 → 支撑业务流程数字化
- **关联**：[[id:huawei.btit.concept.enterprise-architecture]] EA 提供 IT 战略输入

## 典型误区
- **IT 治理 = IT 部门 KPI**：治理不只是 IT 内部管事，是 IT 与业务的协同治理
- **业务部门把 IT 当外包**：提需求不参与设计，最后系统不用——治理要求业务共担
- **预算导向**：按预算花钱不看价值——应转 ROI 导向
- **架构评审走过场**：项目都已开发完才上架构评审——评审应在方案阶段嵌入

## 出处
- [[id:huawei.btit.refined.it治理体系]] — IT 治理体系
- 华为 IFS 变革（IT 与业务一体化的代表案例）
- COBIT / ISO38500 IT 治理标准（参考）
