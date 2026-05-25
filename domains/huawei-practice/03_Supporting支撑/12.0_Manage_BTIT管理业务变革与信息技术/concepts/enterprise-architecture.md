---
id: huawei.btit.concept.enterprise-architecture
doc_type: concept
title: EA 企业架构方法论
domain: huawei-practice
process: 12.0_BTIT
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: EA
aliases:
- Enterprise Architecture
- 企业架构
- TOGAF
- 业务架构 + 应用架构 + 数据架构 + 技术架构
parent_concept: huawei.btit.concept.btit-framework
relations:
- predicate: part_of
  object: huawei.btit.concept.btit-framework
- predicate: supports
  object: huawei.btit.concept.it-governance
- predicate: supports
  object: huawei.btit.concept.digital-transformation
applies_to:
- 公司级 IT 蓝图设计
- 跨流程系统对齐
- 重大变革方案的架构评审
related_concepts:
- huawei.btit.concept.btit-framework
- huawei.btit.refined.企业架构ea方法论
- huawei.dste.concept.dste-framework
---

# EA 企业架构方法论

## 定义
通过业务架构、应用架构、数据架构、技术架构（BADT 四视图）系统化描述企业现状与未来蓝图，为变革规划与 IT 投资提供决策框架，避免点状建设造成系统割裂与重复投资。

## 输入 / 输出
- **输入**：业务战略 + 现有系统盘点 + 组织能力诊断 + 行业架构最佳实践
- **输出**：业务架构（流程地图）+ 应用架构（系统组合）+ 数据架构（核心域 + 流向）+ 技术架构（基础设施）+ 蓝图差距分析 + 演进路线图
- **方法基础**：TOGAF（华为深度定制版）+ Zachman + DoDAF（部分参考）

## 角色
- **架构师**：EA 团队（首席架构师 + 各域架构师）
- **使用方**：BTC、变革项目方案设计者、IT 投资决策者
- **协同方**：业务流 Owner（提供业务架构输入）

## 上下游
- **上游**：[[id:huawei.dste.concept.dste-framework]] 战略 + [[id:huawei.btit.concept.btit-framework]] 变革蓝图诉求
- **下游**：架构蓝图 → 指导变革项目方案 / 指导 IT 投资优先级
- **关联**：所有重大变革项目立项前需通过架构评审

## 典型误区
- **EA = 画图练习**：画了一堆漂亮架构图但没人参考——必须嵌入决策流程才有意义
- **架构与业务脱节**：架构师纯技术视角，不懂业务——做出的蓝图业务不接受
- **过度详细**：试图把每个系统每个接口都画清楚——蓝图维护成本超过价值
- **架构评审走形式**：项目都开发了才补架构评审——评审应在 charter / 方案阶段嵌入

## 出处
- [[id:huawei.btit.refined.企业架构ea方法论]] — 企业架构 EA 方法论
- TOGAF 9.x 标准
- 华为 IFS 变革架构案例
