---
id: huawei.sd.concept.c8-team
doc_type: concept
title: C8 项目核心团队
domain: huawei-practice
process: 7.0_ServiceDelivery
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: C8 项目核心团队
aliases:
- C8团队
- 项目八核心
- Project Core Team
parent_concept: huawei.sd.concept.sd-framework
relations:
- predicate: part_of
  object: huawei.sd.concept.sd-framework
- predicate: requires_role
  object: huawei.sd.concept.sd-framework
applies_to:
- 项目团队组建
- 交付执行
- 矩阵管理
related_concepts:
- huawei.sd.concept.sd-framework
- huawei.sd.concept.gme-governance
- huawei.sd.concept.evm
- huawei.svcdel.refined.项目交付管理体系
---

# C8 项目核心团队

## 定义
C8 是华为交付项目的核心团队模式，由 8 个关键角色组成，代表项目拉动功能部门工作。八个角色为：项目经理（PM，整体管理与经营负责）、技术经理（TM，技术方案与架构设计）、系统工程师（SE，系统集成与测试验证）、项目控制（PC，进度/成本/风险监控）、财务代表（FR，预算管理与成本核算）、质量经理（QM，质量保证与过程审计）、配置经理（CM，配置管理与版本控制）、交付经理（DM，现场交付与客户协调）。C8 的本质是"项目拉动资源"——以项目为核心，功能部门向项目提供合格资源。

## 输入 / 输出
- **输入**：项目章程/启动报告、RACI 矩阵、资源需求计划
- **输出**：各角色分管领域的交付物与管控记录（质量记录、变更记录、成本报告等）
- **核心机制**：PM 作为 CEO 统筹 C8，C8 各角色拉动对应功能部门

## 角色
- **PM**：项目 CEO，整体管理与客户沟通、经营负责
- **TM**：技术方案、架构设计、技术风险把控
- **SE**：系统集成、测试验证、系统思维
- **PC**：进度/成本/风险监控，EVM 数据分析
- **FR**：预算管理、成本核算、收入确认
- **QM**：质量保证、过程审计、评审把关
- **CM**：配置管理、版本控制、基线管理
- **DM**：现场交付执行、客户关系协调

## 上下游
- **上游**：[[id:huawei.sd.concept.sd-framework]] 项目立项阶段组建 C8 团队
- **下游**：C8 各角色输出管控交付物 → 项目验收与关闭
- **平行**：[[id:huawei.sd.concept.gme-governance]] GME 决策机制中 E 层由 C8 执行

## 典型误区
- **C8 只挂名不履职**：角色名存实亡，仍按功能部门各自为战
- **PM 事必躬亲**：PM 替代 C8 其他角色工作，团队形同虚设
- **C8 与功能部门边界不清**：C8 角色和功能部门主管权责冲突
- **缺 FR/QM/CM**：只配 PM+TM+DM 三角，财务、质量、配置无人管

## 出处
- [[id:huawei.svcdel.refined.项目交付管理体系]] — 项目交付管理体系（四、C8 项目核心团队）
