---
id: huawei.ipd.concept.plm
doc_type: concept
title: PLM 产品生命周期管理
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: method
canonical_name: PLM
aliases:
- Product Lifecycle Management
- 产品生命周期管理
- 全生命周期管理
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: supports
  object: huawei.ipd.concept.edcp
- predicate: follows
  object: huawei.ipd.concept.ldcp
applies_to:
- 产品上市后运营
- 版本演进与退市
- 产品组合优化
maturity_stage:
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.edcp
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.ldcp
- huawei.ipd.concept.or
- huawei.ipd.refined.plm-overview
---

# PLM 产品生命周期管理

## 定义
产品从上市到退市的全生命周期运营管理体系，是"大 IPD"的后段。

## 输入 / 输出
- **输入**：[[id:huawei.ipd.concept.ldcp]] 放行的产品、市场反馈、竞争变化、销售/服务/财务数据
- **输出**：版本演进规划、降本改进方案、老产品退市路径、客户迁移计划；向下一版本 IPD 反馈需求
- **四阶段视角**：导入期 → 成长期 → 成熟期 → 衰退/退市期，每个阶段运营重点不同

## 角色
- **主责**：LMT（Lifecycle Management Team，产品上市后由 PDT 转为 LMT 继续负责）
- **产品经理**：从 PDT 经理延续到 LMT 经理，保持端到端责任
- **关键协作**：市场/销售（推广与渠道）、服务（售后质量）、供应（产能与成本）、财经（利润分析）
- **决策层**：[[id:huawei.ipd.concept.ipmt]] 在 [[id:huawei.ipd.concept.edcp]] 做生命周期决策

## 上下游
- **上游**：LDCP 放行产品 → 进入 PLM 阶段
- **下游**：EDCP 决策"继续投资 / 优化调整 / 退市"；退市触发 EOL 流程（备件保障、客户迁移、技术沉淀）
- **反馈闭环**：PLM 阶段发现的问题与机会 → 反馈给 [[id:huawei.ipd.concept.or]] → 进入下一版本 IPD 循环

## 典型误区
- **PDT 上市就解散**：项目经理转岗，产品无人端到端负责——必须延续到至少第一次 EDCP
- **只管新产品不管老产品**：资源都给新品，老产品维护缺位——老产品贡献利润大头，不能忽视
- **退市没有流程**：销售舍不得、服务担心客户、财务靠惯性——必须设退市机制化流程（EDCP + EOL Playbook）
- **PLM 系统与流程脱节**：买了 PLM IT 系统但组织没变——系统只是载体，LMT/LDCP/EDCP 机制才是本质
- **客户迁移方案缺失**：退市决定后才告诉客户——应提前 12-18 个月通知，提供替代产品和数据迁移

## 出处
- [[id:huawei.ipd.refined.plm-overview]] — PLM 产品生命周期管理概述（待完善）
- [[id:huawei.ipd.refined.edcp-process]] — EDCP 生命周期决策流程
- 华为《PLM 管理规定》
