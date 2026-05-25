---
id: huawei.sd.concept.service-quality
doc_type: concept
title: 服务质量管理体系
domain: huawei-practice
process: 7.0_ServiceDelivery
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: 服务质量管理体系
aliases:
- 服务质量
- 交付质量
- Service Quality
parent_concept: huawei.sd.concept.sd-framework
relations:
- predicate: part_of
  object: huawei.sd.concept.sd-framework
- predicate: feeds
  object: huawei.itr.concept.itr-framework
applies_to:
- 交付质量保障
- 过程质量控制
- 客户满意度管理
- 持续改进
related_concepts:
- huawei.sd.concept.sd-framework
- huawei.sd.concept.pm-maturity
- huawei.itr.concept.itr-framework
- huawei.svcdel.refined.服务质量管理体系
- huawei.svcdel.refined.项目交付管理体系
---

# 服务质量管理体系

## 定义
华为基于 ITIL 和 ISO20000，结合交付实践建立的覆盖服务全生命周期的质量管理体系。三层质量保障：事前预防（标准化流程、评审机制、能力认证，由质量经理/PM 负责）、事中控制（过程审计、里程碑评审、缺陷管理，由质量经理负责）、事后改进（客户满意度、复盘改进、经验固化，由 PM/质量部负责）。遵循 PDCA 循环（Plan→Do→Check→Act）持续改进。

## 输入 / 输出
- **输入**：项目基准计划、质量标准与基线、客户验收标准
- **输出**：质量记录、缺陷报告、评审通过记录、CSAT/NPS 评分、改进措施
- **核心指标**：里程碑按时达成率(≥90%)、评审通过率(≥85%)、交付物合格率(≥95%)、验收一次通过率(≥80%)、CSAT(≥8/10)、NPS(≥30)

## 角色
- **质量经理（QM）**：质量保证、过程审计、评审把关
- **PM**：对项目质量负总责，驱动复盘改进
- **评审人**：同行评审（技术专家）、里程碑评审（PM+QM+客户）、管理评审（PMO+管理层）
- **质量部**：组织级质量审计、质量基线维护

## 上下游
- **上游**：[[id:huawei.sd.concept.sd-framework]] 项目立项时设定质量基线与验收标准
- **下游**：质量评审结果驱动改进 → 交付验收 → [[id:huawei.itr.concept.itr-framework]] 售后问题质量闭环
- **平行**：[[id:huawei.sd.concept.pm-maturity]] 成熟度 L3 要求过程评审+验收标准

## 典型误区
- **质量=事后检查**：只做验收检查，忽视事前标准化和事中控制
- **评审走过场**：同行评审流于形式，零缺陷出口原则未落实
- **指标收集不闭环**：质量指标仅统计不改进，PDCA 只走到 C 没有 A
- **与 ITR 割裂**：交付质量问题不进入 ITR 问题处理流程，改进无闭环

## 出处
- [[id:huawei.svcdel.refined.服务质量管理体系]] — 服务质量管理体系
- [[id:huawei.svcdel.refined.项目交付管理体系]] — 项目交付管理体系
