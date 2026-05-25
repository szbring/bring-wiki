---
id: huawei.overview.concept.dcp
doc_type: concept
title: DCP 决策评审点（跨业务流通用概念）
domain: huawei-practice
process: 0.0_overview
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-27
entity_type: process_gate
canonical_name: DCP
aliases:
- Decision Check Point
- Decision Checkpoint
- 决策评审点
- 决策检查点
- 流程决策关口
parent_concept: null
relations:
- predicate: instantiated_by
  object: huawei.ipd.concept.cdcp
- predicate: instantiated_by
  object: huawei.ipd.concept.pdcp
- predicate: instantiated_by
  object: huawei.ipd.concept.adcp
- predicate: instantiated_by
  object: huawei.ipd.concept.ldcp
- predicate: instantiated_by
  object: huawei.ipd.concept.edcp
- predicate: instantiated_by
  object: huawei.dste.concept.sp-dcp
- predicate: instantiated_by
  object: huawei.dste.concept.bp-dcp
- predicate: instantiated_by
  object: huawei.dste.concept.bp-qr-dcp
- predicate: instantiated_by
  object: huawei.dste.concept.sa-dcp
- predicate: instantiated_by
  object: huawei.ltc.concept.ati
- predicate: instantiated_by
  object: huawei.ltc.concept.atb
- predicate: instantiated_by
  object: huawei.ltc.concept.atc
- predicate: instantiated_by
  object: huawei.ltc.concept.atac
- predicate: instantiated_by
  object: huawei.itr.concept.asr
- predicate: instantiated_by
  object: huawei.itr.concept.aur
- predicate: instantiated_by
  object: huawei.itr.concept.aip
- predicate: instantiated_by
  object: huawei.itr.concept.avr
- predicate: instantiated_by
  object: huawei.itr.concept.acr
applies_to:
- 流程管理体系
- 阶段性投资/业务决策
- 跨职能评审机制
related_concepts:
- huawei.dste.concept.bp-dcp
- huawei.dste.concept.bp-qr-dcp
- huawei.dste.concept.sa-dcp
- huawei.dste.concept.sp-dcp
- huawei.ipd.concept.adcp
- huawei.ipd.concept.cdcp
- huawei.ipd.concept.edcp
- huawei.ipd.concept.ldcp
- huawei.ipd.concept.pdcp
- huawei.ipd.concept.tr
- huawei.ipd.refined.dcp-mechanism
- huawei.itr.concept.acr
- huawei.itr.concept.aip
- huawei.itr.concept.asr
- huawei.itr.concept.aur
- huawei.itr.concept.avr
- huawei.ltc.concept.atac
- huawei.ltc.concept.atb
- huawei.ltc.concept.atc
- huawei.ltc.concept.ati
---

# DCP 决策评审点（跨业务流通用概念）

## 定义
流程阶段末由跨职能评审团做 Go/Kill/Hold 决策的关口。

## 输入 / 输出
- **输入**：上一阶段的交付物、评审包（计划、方案、数据、风险清单），以及前置技术/专业评审（如 IPD 的 [[id:huawei.ipd.concept.tr]]）通过的结论
- **输出**：三选一的书面决策——Go（进入下一阶段并追加资源）/ Kill（终止并释放资源）/ Hold（暂停并列明恢复条件）

## 角色
- **决策方**：跨职能评审团（IPD 的 IPMT、LTC 的销项决策团、DSTE 的 EMT 等，随流程而定）
- **执行方**：业务流负责团队（IPD 的 PDT、LTC 的铁三角等）
- **前置评审方**：技术/专业评审团队，负责把技术与商业两类问题分离评审

## 上下游
- **上游**：业务流的阶段任务完成 + 前置专业评审通过
- **下游**：按决策结果分流——Go 进入下阶段 / Kill 终止并善后 / Hold 暂停并监控恢复条件
- **四大业务流的 DCP 实例**：
  - IPD 5 个：[[id:huawei.ipd.concept.cdcp]] / [[id:huawei.ipd.concept.pdcp]] / [[id:huawei.ipd.concept.adcp]] / [[id:huawei.ipd.concept.ldcp]] / [[id:huawei.ipd.concept.edcp]]
  - DSTE 4 个：[[id:huawei.dste.concept.sp-dcp]] / [[id:huawei.dste.concept.bp-dcp]] / [[id:huawei.dste.concept.bp-qr-dcp]] / [[id:huawei.dste.concept.sa-dcp]]
  - LTC 4 个：[[id:huawei.ltc.concept.ati]] / [[id:huawei.ltc.concept.atb]] / [[id:huawei.ltc.concept.atc]] / [[id:huawei.ltc.concept.atac]]
  - ITR 5 个：[[id:huawei.itr.concept.asr]] / [[id:huawei.itr.concept.aur]] / [[id:huawei.itr.concept.aip]] / [[id:huawei.itr.concept.avr]] / [[id:huawei.itr.concept.acr]]

## 典型误区
- **把 DCP 当流程专属术语**：DCP 是流程管理通用概念，各业务流有自己的 DCP 命名与实例；问 "DCP 是什么" 要先问哪个流程
- **第四种决策**："有条件通过""先做着看""小规模试一下"都不是决策，是逃避决策；Hold 必须带明确恢复条件
- **决策走过场**：评审团不提问就通过——必设必问清单，早期阶段顾问介入提升质量
- **技术评审与 DCP 合并开**：专业评审挤占商业讨论时间，两类决策都做不深；设计上要分离

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境下的长文详解，含五个 DCP 实例与薄云落地建议）
- 华为 BPA 流程架构——DCP 作为流程 Owner 体系的决策治理节点
