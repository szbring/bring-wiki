---
id: huawei.supply.concept.sop
doc_type: concept
title: S&OP 销售与运营计划
domain: huawei-practice
process: 8.0_Supply
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: method
canonical_name: S&OP 销售与运营计划
aliases:
- S&OP
- Sales and Operations Planning
- 产销协调
parent_concept: huawei.supply.concept.isc-framework
relations:
- predicate: part_of
  object: huawei.supply.concept.isc-framework
- predicate: depends_on
  object: huawei.supply.concept.scor-model
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
applies_to:
- 月度产销平衡
- 需求预测与供应能力匹配
- 库存与产能规划
related_concepts:
- huawei.supply.concept.isc-framework
- huawei.supply.concept.scor-model
- huawei.ltc.concept.ltc-framework
- huawei.supply.refined.供应链管理体系
- huawei.supply.refined.集成供应链isc方法论
---

# S&OP 销售与运营计划

## 定义
S&OP（Sales and Operations Planning，销售与运营计划）是ISC的核心运营机制，以月度滚动方式平衡销售预测与供应能力。流程为：销售预测到需求汇总，再到供应能力评估，进行差距分析，制定行动方案，最后更新各部门计划。S&OP的核心价值在于将销售端的"想要多少"与供应端的"能供多少"显性化对齐，避免产销脱节。行业经验表明，预测准确率每提升1%，可在库存水平、采购效率、交付及时率等方面带来约5%的综合改善。S&OP输出五大计划：客户订单计划、生产计划、采购计划、库存管理计划、交付计划。

## 输入与输出
- **输入**：销售预测与历史需求、当前库存与在途数据、产能约束与供应商交付能力、业务战略目标
- **输出**：客户订单计划（需求分类与优先级）、生产计划（排产与产能分配）、采购计划（采购需求与到货计划）、库存管理计划（安全库存与补货策略）、交付计划（发货与物流计划）

## 角色
- **销售部门**：提供需求预测与客户优先级
- **供应链计划**：汇总需求、评估供应能力、制定平衡方案
- **制造部门**：确认产能与排产可行性
- **采购部门**：确认物料可获取性与到货周期
- **高管层**：裁决重大供需差距的决策方案

## 上下游
- **上游**：LTC流程提供销售预测与客户需求信息；DSTE流程提供年度经营目标
- **下游**：S&OP输出驱动采购执行、生产排程、物流调度等日常运营
- **与SCOR的关系**：S&OP是SCOR中Plan流程的核心机制，贯穿需求计划/供应计划/产能计划/库存计划

## 典型误区
- **把S&OP开成汇报会**：S&OP的核心是差距分析与决策，不是进度汇报
- **只做销售预测不评估供应能力**：单方面推动需求，忽视产能与物料约束，导致承诺无法兑现
- **S&OP仅限供应链内部**：销售不参与或不重视，产销协调名存实亡
- **月度滚动但调整迟缓**：市场变化快时应缩短滚动周期或增加临时S&OP会议

## 出处
- [[id:huawei.supply.refined.供应链管理体系]] — S&OP流程与月度滚动机制详述
- [[id:huawei.supply.refined.集成供应链isc方法论]] — ISC流程框架中S&OP的定位
