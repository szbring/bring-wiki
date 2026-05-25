---
id: huawei.dste.concept.sa-dcp
doc_type: concept
title: SA-DCP 战略审视决策评审
domain: huawei-practice
process: 5.0_DSE
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: SA-DCP
aliases:
- SA DCP
- 战略审视
- Strategic Audit
- 战略再检验
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.dste.concept.dste-framework
- predicate: follows
  object: huawei.dste.concept.bp-qr-dcp
applies_to:
- 重大外部变化下战略修正
- SP 中期检视
- 必赢战役方向调整
related_concepts:
- huawei.dste.concept.bp-qr-dcp
- huawei.dste.concept.sp-dcp
- huawei.ipd.refined.dcp-mechanism
- huawei.overview.concept.dcp
---

# SA-DCP 战略审视决策评审

## 定义
当外部环境发生重大变化或 BP 季度回顾持续偏差时触发的战略审视评审，对当前 SP 的方向、必赢战役、业务设计做 Confirm/Adjust/Reset 决策。

## 输入 / 输出
- **输入**：触发事件（市场剧变 / 竞争颠覆 / 技术拐点 / 持续业绩偏差）+ 重新做的市场洞察 + SP 偏差分析
- **输出**：Confirm—SP 方向不变，加强执行 / Adjust—修正必赢战役或业务设计（不重做整个 SP）/ Reset—启动 SP 重新制定
- **触发**：非定期，由触发事件驱动；常见每年 6 月或 12 月

## 角色
- **决策方**：EMT / 公司战略与发展委员会
- **汇报方**：S&D 部门 + 业务一把手
- **质询方**：财经、独立战略顾问、董事会

## 上下游
- **上游**：[[id:huawei.dste.concept.bp-qr-dcp]] Escalate 触发，或外部重大事件触发
- **下游**：Adjust 输出 → 修订 SP 中关键模块；Reset 输出 → 重启 [[id:huawei.dste.concept.sp-dcp]] 周期
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 DSTE 流程中的实例

## 典型误区
- **从不开 SA**：环境变了也死守原 SP——僵化
- **SA 频繁开**：动不动就重做 SP——失去战略定力，团队疲惫
- **SA 只调数字不调方向**：跌了就降目标，涨了就提目标——这是预算调整不是战略审视
- **Reset 走过场**：决议要 Reset 但实际没启动 SP 重新制定——管理层失信

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，DSTE 同构）
- 华为《价值为纲》战略审视章节
- DSTE 流程 Owner 体系
