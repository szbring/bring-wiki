---
id: huawei.ipd.concept.edcp
doc_type: concept
title: EDCP 生命周期/退市决策评审
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process_gate
canonical_name: EDCP
aliases:
- End of Life DCP
- EOL DCP
- 生命周期决策评审
- 退市决策评审
- IPD 生命周期阶段 DCP
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: requires_role
  object: huawei.ipd.concept.ipmt
- predicate: follows
  object: huawei.ipd.concept.ldcp
applies_to:
- 生命周期管理
- 继续投资/退市决策
- 产品组合管理
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.ldcp
- huawei.ipd.refined.dcp-mechanism
---

# EDCP 生命周期/退市决策评审

## 定义
产品上市后，IPMT 定期对"继续投资、优化调整或退市"的决策（至少每年一次）。

## 输入 / 输出
- **输入**：销售业绩、市场份额、毛利/净利、客户满意度（NPS）、竞争态势、技术演进趋势、维护成本、产品组合重叠度
- **输出**：继续投资（追加开发/营销投入）/ 优化调整（降本、精简 SKU、切换市场）/ 计划退市（设退市时间表，启动 EOL 流程）
- **评审频率**：每年至少 1 次，有重大市场变化时临时触发

## 角色
- **决策方**：[[id:huawei.ipd.concept.ipmt]]（多数场景由产品线总裁+产品组合委员会联合决策）
- **执行方**：产品管理团队（PM）主责，PDT 转为维护模式后配合
- **支持方**：财经（成本与利润）、市场（竞争与客户）、服务（维护成本与服役客户影响）

## 上下游
- **上游**：[[id:huawei.ipd.concept.ldcp]] Go → 产品进入市场 → 运营数据累积 1 年
- **下游**：继续投资 → 触发版本规划，回到 IPD 循环；退市 → 启动 EOL 流程，处理老客户迁移、备件保障、知识沉淀
- **与产品组合的关系**：EDCP 不能只看单产品，必须在产品组合下做相对决策

## 典型误区
- **退市没人推**：退市比立项难——销售舍不得、老客户抵触、团队有感情；必须靠制度硬推，设退市窗口期
- **把 EDCP 开成业绩汇报**：数据展示不等于决策，必须带三选一的明确决议
- **忽略客户迁移**：退市决策必须附迁移方案——替代产品、服务承诺、备件供应年限，否则损伤品牌
- **数据不全就决策**：财经/市场/服务三条线数据缺一就不决策，避免"感觉还不错就继续投"

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制长文（EDCP 章节）
- 华为 IPD 产品生命周期管理（PLM）——EOL 流程衔接
