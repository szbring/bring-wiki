---
id: huawei.ipd.concept.irt
doc_type: concept
title: IRT 独立技术评审团
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: role
canonical_name: IRT
aliases:
- Independent Review Team
- 独立技术评审团
- 技术评审团
- TRT
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: role_in
  object: huawei.ipd.concept.tr
- predicate: supports
  object: huawei.ipd.concept.ipmt
applies_to:
- 技术方案独立评审
- 质量守门
- 跨项目技术一致性保障
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.pdt
- huawei.ipd.refined.ipd-organization
- huawei.ipd.refined.tr-mechanism
- huawei.overview.concept.dcp
---

# IRT 独立技术评审团

## 定义
独立于项目团队、由资深技术专家组成、对 TR 技术评审负责的评审团。

## 输入 / 输出
- **输入**：[[id:huawei.ipd.concept.pdt]] 提交的技术方案、设计文档、测试报告、质量数据
- **输出**：TR 通过/不通过/有条件通过的评审结论；技术风险清单；改进建议
- **原则**：判"做得对不对"（技术正确性），不判"值不值得做"（那是 [[id:huawei.ipd.concept.ipmt]] 的职责）

## 角色
- **组成**：5-9 人资深技术专家，跨领域（架构、硬件、软件、测试、质量、供应、制造等）
- **IRT 主任**：通常由 CTO 办公室或产品线技术总监兼任
- **独立性要求**：成员不得在当前被评审项目中承担具体开发任务，避免"运动员兼裁判"
- **固定 vs 临时**：产品线级 IRT 通常固定常设；大型技术评审可临时扩充外部专家

## 上下游
- **上游**：PDT 完成阶段性技术工作 → 提交 TR 评审包 → IRT 预审
- **下游**：TR 通过 → 进入 [[id:huawei.overview.concept.dcp]] 评审；TR 不通过 → PDT 整改后重评
- **与 IPMT 的分工**：TR 评审结论是 DCP 的前置输入——TR 不通过则 DCP 不排会

## 典型误区
- **IRT 成员不独立**：被评审项目的 PDT 成员进 IRT——必须排除，否则评审失去意义
- **IRT 变成技术答辩**：评审变成团队汇报、专家点头——必须预审材料、带问题上会
- **IRT 越权做商业决策**："这个产品没必要做"不是 IRT 该说的——那是 IPMT 的决策范围，IRT 只判技术可行性
- **IRT 与 DCP 合并开**：技术与商业两类决策必须分离评审，合并会丢失专业深度
- **IRT 专家层级不够**：派中级工程师当评审——评审结论不权威，PDT 不服

## 出处
- [[id:huawei.ipd.refined.tr-mechanism]] — TR 技术评审体系（含 IRT 运作）
- [[id:huawei.ipd.refined.ipd-organization]] — IPD 组织体系（IRT 组建与独立性要求）
- 华为《技术评审管理规定》
