---
id: huawei.ltc.concept.atac
doc_type: concept
title: ATAC 合同关闭决策评审
domain: huawei-practice
process: 3.0_LTC
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-27
updated: 2026-04-27
entity_type: process_gate
canonical_name: ATAC
aliases:
- Authorize To Account Closure
- 合同关闭
- 项目结算关闭
- 销售闭环
parent_concept: huawei.overview.concept.dcp
relations:
- predicate: instantiates
  object: huawei.overview.concept.dcp
- predicate: part_of
  object: huawei.ltc.concept.ltc-framework
- predicate: gates
  object: huawei.ltc.concept.ltc-framework
- predicate: follows
  object: huawei.ltc.concept.atc
- predicate: requires_role
  object: huawei.ltc.concept.iron-triangle
applies_to:
- 合同执行完成后正式关闭
- 项目复盘与经验沉淀
- 客户满意度收尾
related_concepts:
- huawei.ipd.refined.dcp-mechanism
- huawei.ltc.concept.atc
- huawei.ltc.concept.iron-triangle
- huawei.ltc.refined.ltc流程架构
- huawei.overview.concept.dcp
---

# ATAC 合同关闭决策评审

## 定义
LTC 流程末端 DCP，对合同交付完成、回款全部到账、客户验收完毕的项目做"是否正式关闭"的评审决策，并完成项目复盘与销售经验沉淀。

## 输入 / 输出
- **输入**：交付完成证明 + 回款全部到账记录 + 客户验收文件 + 风险事项处理结果
- **输出**：Go—合同正式关闭，资源释放 / Hold—尾款未到账或客户问题未关闭，挂账继续跟踪
- **必须产出**：项目复盘报告（赢/输/差距分析）、客户满意度记录、销售经验入库

## 角色
- **决策方**：销项决策团 + 财经
- **汇报方**：[[id:huawei.ltc.concept.iron-triangle]]（FR 主报交付与验收，AR 主报回款与客户关系）
- **复盘组织方**：销售管理部 + 流程 Owner

## 上下游
- **上游**：[[id:huawei.ltc.concept.atc]] 合同签订 → 交付与回款执行 → 验收完成
- **下游**：合同关闭 → 经验入库 → 反馈下一周期 SP/BP 与铁三角能力建设
- **关联**：是 [[id:huawei.overview.concept.dcp]] 在 LTC 流程中的实例

## 典型误区
- **回款未到账就关闭**：交付完成 = 关闭——结果尾款拖欠几年没人跟
- **不做复盘**：项目结束就解散——经验只在个人脑子里，组织不沉淀
- **只复盘赢的项目**：失败项目大家不愿提——但失败案例的学习价值更大
- **ATAC 是仪式性的**：项目早就实质结束，ATAC 只是档案动作——丧失复盘价值

## 出处
- [[id:huawei.ipd.refined.dcp-mechanism]] — DCP 决策评审机制（IPD 语境，LTC 同构）
- [[id:huawei.ltc.refined.ltc流程架构]] — LTC 流程架构
- 华为项目复盘机制
