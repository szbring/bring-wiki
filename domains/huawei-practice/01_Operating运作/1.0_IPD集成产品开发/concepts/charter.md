---
id: huawei.ipd.concept.charter
doc_type: concept
title: Charter 项目任务书/业务计划
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: artifact
canonical_name: Charter
aliases:
- 项目任务书
- 产品业务计划
- 产品 Charter
- Project Charter
- BP（Business Plan，部分企业混用）
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: produced_by
  object: huawei.ipd.concept.pdt
- predicate: feeds
  object: huawei.ipd.concept.cdcp
- predicate: feeds
  object: huawei.ipd.concept.pdcp
- predicate: fed_by
  object: huawei.ipd.concept.or
- predicate: fed_by
  object: huawei.ipd.concept.mm
applies_to:
- 产品立项
- DCP 评审决策材料
- 项目目标与边界定义
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.mm
- huawei.ipd.concept.or
- huawei.ipd.concept.pdt
- huawei.ipd.refined.charter-template
- huawei.ipd.refined.dcp-mechanism
---

# Charter 项目任务书/业务计划

## 定义
定义产品"做什么、不做什么、凭什么值得做"的立项决策文档。

## 输入 / 输出
- **输入**：[[id:huawei.ipd.concept.mm]] 输出的市场细分与机会选择；[[id:huawei.ipd.concept.or]] 输出的需求包；战略优先级；竞品与技术趋势
- **输出**：可被 [[id:huawei.ipd.concept.ipmt]] 评审的 Charter 文档，作为 CDCP/PDCP 的核心评审包
- **典型章节**：产品定位（含目标客户）、市场机会、竞争分析、产品概念、关键需求、技术方案要点、项目目标（Time/Scope/Quality/Cost）、资源预算、风险与假设、里程碑

## 角色
- **编写方**：[[id:huawei.ipd.concept.pdt]] 概念组（PDT 经理主笔，核心 Rep 贡献）
- **评审方**：[[id:huawei.ipd.concept.ipmt]] 在 CDCP/PDCP 决策
- **Charter 演化**：CDCP 时为初版（方向与商业可行性）→ PDCP 时为完整版（方案与承诺）→ 后续 DCP 持续更新

## 上下游
- **上游**：MM 的市场管理输出 + OR 的需求包 → 组合成 Charter 输入
- **下游**：Charter 是 CDCP/PDCP 的核心决策材料 → 批准后驱动后续阶段工作
- **伴随产物**：财务预测表、风险清单、技术方案摘要都是 Charter 的附件

## 典型误区
- **Charter 变成技术方案书**：工程思维堆满技术细节，缺市场机会和商业论证——Charter 首先是商业文档
- **"什么都做"的 Charter**：不写"不做什么"（Out of Scope）——产品边界模糊必定超时超预算
- **一次写完不再更新**：Charter 应是活文档，各 DCP 前更新为当时状态——CDCP 初版 vs PDCP 版差异大是正常的
- **财务预测脱节**：收入预测乐观、成本预测模糊、ROI 经不起压力测试——IPMT 首要质疑点
- **Charter 与需求脱节**：正文写"满足客户需求"但具体需求条目未列入、未排优先级——Charter 必须可追溯到具体需求 ID

## 出处
- [[id:huawei.ipd.refined.charter-template]] — Charter 模板与编写指南（待建/待完善）
- [[id:huawei.ipd.refined.dcp-mechanism]] — Charter 作为 DCP 评审包的角色
- 华为《Charter 编写与管理规定》
