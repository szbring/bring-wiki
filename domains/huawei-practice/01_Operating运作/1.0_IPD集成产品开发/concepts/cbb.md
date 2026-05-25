---
id: huawei.ipd.concept.cbb
doc_type: concept
title: CBB 共用基础模块
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: method
canonical_name: CBB
aliases:
- Common Building Block
- 共用基础模块
- 共享构建块
- 平台化组件
parent_concept: huawei.ipd.concept.ipd-framework
relations:
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: supports
  object: huawei.ipd.concept.pdt
applies_to:
- 跨产品复用
- 异步开发
- 平台化建设
maturity_stage:
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.pdt
- huawei.ipd.refined.ipd-overview
---

# CBB 共用基础模块

## 定义
跨产品/跨版本可复用的标准化技术/功能模块，是 IPD 异步开发与平台化的载体。

## 输入 / 输出
- **输入**：多个产品的共性需求识别、现有成熟模块抽取、技术规划（TPP）规划的平台组件
- **输出**：标准化模块（含接口、文档、测试、版本管理）；可被多个 PDT 直接调用的技术资产
- **常见形态**：硬件模组、软件库、算法、协议栈、接口规范、工具链、设计模板

## 角色
- **拥有方**：CBB Owner（通常由技术委员会或平台部门任命的技术 leader）
- **使用方**：各 [[id:huawei.ipd.concept.pdt]]（按接口规范调用）
- **治理方**：CTO 办公室或技术管理部——评审 CBB 立项、版本升级、生命周期

## 上下游
- **上游**：技术规划（TPP）或若干产品项目的"从项目抽取平台"行动 → 抽象为 CBB
- **下游**：CBB 被多个 PDT 集成到具体产品 → 产品研发周期缩短、质量提升
- **异步开发**：CBB 独立演进（Beat），产品 PDT 按需选择 CBB 版本集成——这是 IPD "异步开发"的基础机制

## 典型误区
- **"CBB"只是内部叫法没实质**：没有 Owner、没有版本管理、没有接口规范——本质还是代码拷贝
- **为抽象而抽象**：只被 1 个产品用过就立项 CBB——应至少识别 3+ 个产品的共性再抽
- **CBB 无生命周期管理**：老版本无人维护、新版本无人升级——CBB 必须像产品一样有 LDCP 和 EDCP
- **PDT 抵制复用**：项目组觉得改造时间>自己写，宁可重做——要在绩效上奖励 CBB 使用率
- **CBB 变成"代码仓库"**：只有代码无文档无测试用例——CBB 必须含接口文档、样例、测试套，否则复用门槛太高

## 出处
- [[id:huawei.ipd.refined.cbb-methodology]] — CBB 应用研讨与平台抽取培训（待完善）
- [[id:huawei.ipd.refined.ipd-overview]] — IPD 概述中"大 IPD"章节
- 华为《平台化开发与 CBB 管理规定》
