---
id: huawei.ipd.concept.pdcp
doc_type: concept
title: PDCP 计划决策评审
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process_gate
canonical_name: PDCP
aliases:
- Plan DCP
- 计划决策评审
- IPD 计划阶段 DCP
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
  object: huawei.ipd.concept.cdcp
- predicate: precedes
  object: huawei.ipd.concept.adcp
applies_to:
- 详细方案与资源承诺决策
- 开发阶段启动
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.adcp
- huawei.ipd.concept.cdcp
- huawei.ipd.concept.charter
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.pdt
- huawei.ipd.refined.dcp-mechanism
---

# PDCP 计划决策评审

## 定义
IPD 计划阶段末，IPMT 对"方案可行、资源到位、可以启动开发"的投资决策。

## 输入 / 输出
- **输入**：详细技术方案（TR2 通过）、完整项目计划、BOM 与关键供应商确认、预算审批、风险清单、更新版 [[id:huawei.ipd.concept.charter]]
- **输出**：Go（进入 Available 阶段，释放开发资源）/ Kill（方案不可行，终止）/ Hold（回补方案或资源）
- **此点前累计资源投入**：约 15%

## 角色
- **决策方**：[[id:huawei.ipd.concept.ipmt]]
- **执行方**：[[id:huawei.ipd.concept.pdt]] 完整团队（已组建）
- **前置评审方**：IRT（技术评审团），负责 TR1/TR2 评审通过

## 上下游
- **上游**：[[id:huawei.ipd.concept.cdcp]] Go → 计划阶段工作 → TR1/TR2 通过
- **下游**：Go → 进入 Available 开发阶段，下一关口为 [[id:huawei.ipd.concept.adcp]]
- **关键依赖**：TR 不通过 PDCP 不排会——技术可行性是商业承诺的前提

## 典型误区
- **资源没到位就 Go**：PDCP 必须确认核心人员、关键物料、供应商、预算都已落实，不能"边走边凑"
- **计划文档完美但评审走形**：IPMT 成员必须读完评审包并带问题上会，避免 PDT 单向汇报
- **把 ADCP 的测试就绪前置到 PDCP**：PDCP 判"计划可行"，不是"已经开发完"，两者内容别混
- **Hold 不设期限**：任何 Hold 必须带"多久、补什么、达到什么标准再评"——否则项目就烂在 Hold 里

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制长文（PDCP 章节）
- 华为 IPD 产品开发流程手册——计划阶段定义
