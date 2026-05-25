---
id: huawei.ipd.concept.ldcp
doc_type: concept
title: LDCP 发布决策评审
domain: huawei-practice
process: 1.0_IPD
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-24
updated: 2026-04-24
entity_type: process_gate
canonical_name: LDCP
aliases:
- Launch DCP
- 发布决策评审
- 上市决策评审
- IPD 发布阶段 DCP
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ipd.concept.ipd-framework
- predicate: requires_role
  object: huawei.ipd.concept.ipmt
- predicate: depends_on
  object: huawei.ipd.concept.tr
- predicate: follows
  object: huawei.ipd.concept.adcp
- predicate: precedes
  object: huawei.ipd.concept.edcp
applies_to:
- 产品全面上市决策
- GA（General Availability）放行
maturity_stage:
- L2
- L3
- L4
- L5
related_concepts:
- huawei.ipd.concept.adcp
- huawei.ipd.concept.edcp
- huawei.ipd.concept.ipmt
- huawei.ipd.concept.pdt
- huawei.ipd.refined.dcp-mechanism
---

# LDCP 发布决策评审

## 定义
IPD 发布阶段末，IPMT 对"产品质量达标、全面上市（GA）放行"的决策。

## 输入 / 输出
- **输入**：试产/β 客户验证结果、全部 P0/P1 缺陷关闭证据、上市物料（官网、销售话术、渠道培训）就绪报告、售后服务准备度、供应产能报告、最终版财务预测
- **输出**：Go（GA 发布，全面放货）/ Kill（验证失败且不可接受，项目终止/撤市）/ Hold（回补缺陷或市场准备）
- **此点前累计资源投入**：约 85%

## 角色
- **决策方**：[[id:huawei.ipd.concept.ipmt]]（多数场景由更高一级——产品线总裁或 EMT——联合决策）
- **执行方**：[[id:huawei.ipd.concept.pdt]] + 市场/销售/服务/供应就绪代表
- **前置评审方**：IRT（TR6 发布评审），服务/供应/市场各自准入评审

## 上下游
- **上游**：[[id:huawei.ipd.concept.adcp]] Go → 试产/β 验证 → TR6 通过
- **下游**：Go → 产品进入生命周期管理阶段，由 [[id:huawei.ipd.concept.edcp]] 定期评估
- **关键依赖**：销售、服务、供应链三条路径必须同步 ready，缺一不 Go

## 典型误区
- **技术 Go、市场没 ready 就上市**：销售话术、渠道培训、官网素材没到位，产品上市也卖不动——LDCP 必须检查市场端就绪度
- **Kill 不下去**：此时已投 85%，团队和管理层都难接受 Kill；但如果验证数据说明方向错了，继续投剩下 15% 是追加损失
- **P2 缺陷当 P1 处理**：不是所有缺陷都要在 LDCP 关闭；P2 可带规避方案上市，否则永远发布不了
- **把 LDCP 和 ADCP 合并开**：阶段不同、评审焦点不同（量产可能 vs 全面放行），合并会丢失阶梯式收紧的效果

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制长文（LDCP 章节）
- 华为 IPD 产品开发流程手册——发布阶段定义
