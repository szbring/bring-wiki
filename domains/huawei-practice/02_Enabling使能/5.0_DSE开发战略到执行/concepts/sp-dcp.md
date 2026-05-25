---
id: huawei.dste.concept.sp-dcp
doc_type: concept
title: SP-DCP 战略规划决策评审
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: SP-DCP
aliases:
- SP DCP
- 战略规划评审
- SP 决策评审点
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.dste.concept.dste-framework
- predicate: gates
  object: huawei.dste.concept.sp-bp
- predicate: precedes
  object: huawei.dste.concept.bp-dcp
applies_to:
- 中长期战略规划评审
- SP 文件批准发布
- 战略方向变更决策
related_concepts:
- huawei.dste.concept.bp-dcp
- huawei.dste.concept.sp-bp
- huawei.dste.refined.sp-bp战略规划体系
- huawei.ipd.refined.dcp-mechanism
- huawei.overview.concept.dcp
---

# SP-DCP 战略规划决策评审

## 定义
SP（中长期战略规划）周期末由 EMT 召开的决策评审点，对 SP 文件做 Go/Kill/Hold 决策，决定是否正式发布并启动后续 BP 编制。

## 输入 / 输出
- **输入**：SP 评审包（差距分析、五看洞察、战略意图、必赢战役、业务设计、3-5 年里程碑、资源诉求）
- **输出**：Go—SP 正式发布并启动 BP 编制 / Kill—驳回，重新研讨 / Hold—部分认可，列明补充条件
- **触发**：每年 8 月左右 SP 制定完成

## 角色
- **决策方**：EMT（执行管理团队）/ 公司战略与发展委员会
- **汇报方**：S&D 部门 + 业务单元一把手
- **质询方**：财经、HR、各业务流 Owner

## 上下游
- **上游**：[[id:huawei.dste.concept.sp-bp]] SP 制定阶段完成 + 内部研讨已收敛
- **下游**：通过后启动 BP 编制 → [[id:huawei.dste.concept.bp-dcp]]
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 DSTE 流程中的实例

## 典型误区
- **SP-DCP 走过场**：高管已私下沟通，评审会只是签字——评审会必须公开质询，挑战核心假设
- **只评 SP 数字目标**：忽略业务设计、必赢战役、关键任务等结构性内容
- **Hold 滥用**：明明该 Kill 但碍于面子给 Hold——Hold 必须列明明确的恢复条件和时间
- **只关注公司级 SP**：BG/BU 级 SP 也要走对应级别 DCP，不能只在公司开

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，DSTE 同构）
- [[id:huawei.dste.refined.sp-bp战略规划体系]] — SP/BP 战略规划体系
- 华为流程 Owner 体系——DSTE Owner 主持
