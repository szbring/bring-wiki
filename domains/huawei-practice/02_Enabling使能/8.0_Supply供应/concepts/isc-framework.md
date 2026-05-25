---
id: huawei.supply.concept.isc-framework
doc_type: concept
title: ISC 集成供应链
domain: huawei-practice
process: 8.0_Supply
layer: concepts
source_authority: 华为官方
confidence: high
created: 2026-04-28
updated: 2026-04-28
entity_type: process
canonical_name: ISC 集成供应链
aliases:
- ISC
- Integrated Supply Chain
- 集成供应链
parent_concept: null
relations:
- predicate: depends_on
  object: huawei.supply.concept.scor-model
- predicate: part_of
  object: huawei.supply.concept.sop
- predicate: feeds
  object: huawei.ipd.concept.ipd-framework
- predicate: feeds
  object: huawei.ltc.concept.ltc-framework
- predicate: depends_on
  object: huawei.dste.concept.dste-framework
applies_to:
- 端到端供应链管理
- 需求到交付全流程
- 采购到付款全流程
- 退货到处置全流程
related_concepts:
- huawei.supply.concept.scor-model
- huawei.supply.concept.sop
- huawei.supply.concept.supply-chain-strategy
- huawei.supply.concept.supplier-management
- huawei.ipd.concept.ipd-framework
- huawei.ltc.concept.ltc-framework
- huawei.btit.concept.btit-framework
- huawei.supply.refined.供应链管理体系
- huawei.supply.refined.集成供应链isc方法论
---

# ISC 集成供应链

## 定义
ISC（Integrated Supply Chain，集成供应链）是华为供应链管理的核心方法论，由IBM顾问引入，基于SCOR模型重构而成。核心是三个"集成"：流程集成（打通计划-采购-制造-交付-退货端到端流程）、组织集成（合并制造/计划/采购/物流为供应链管理部）、IT集成（ERP/MRP/WMS/TMS/SRM系统打通）。变革目标为"质量好、成本低、服务好、对客户需求反应快"。ISC+数字化阶段进一步实现六大转变：被动到主动、经验驱动到数据驱动、局部优化到全局优化等，构建灵鲲数智云脑（决策层）与灵蜂智能引擎（执行层）两层智能体系。

## 输入与输出
- **输入**：客户需求与销售预测、BOM与产品数据（来自IPD）、订单与交付需求（来自LTC）
- **输出**：齐套交付、供应链总成本与绩效指标、库存周转与现金周转数据
- **ISC与IPD界面**：采购早期介入研发（EPI）、BOM传递、可供应性评估
- **ISC与LTC界面**：订单传递、交付承诺、物流跟踪、交付方案评审（DRB）

## 角色
- **供应链管理部**：集成后统一组织，统筹计划/采购/制造/物流
- **计划人员**：需求预测、S&OP协调、产能规划
- **采购人员**：寻源认证、采购执行、供应商管理
- **制造人员**：生产执行、质量控制
- **物流人员**：仓储、运输、安装调试

## 上下游
- **上游**：IPD流程提供产品数据与BOM，确定可供应性；战略规划（DSTE）确定供应链战略方向
- **下游**：LTC流程承接订单交付承诺与物流执行
- **三大端到端链条**：需求到交付、采购到付款、退货到处置

## 典型误区
- **把ISC等同于采购管理**：ISC覆盖计划/采购/制造/交付/退货全链条，采购仅是其中一环
- **流程集成但组织不集成**：流程打通但部门墙仍在，信息共享无法落地
- **忽视ISC与IPD/LTC的界面**：供应链不参与研发早期和销售前端，导致供需脱节
- **ISC+仅理解为上系统**：数字化转型的核心是决策模式转变，不是单纯IT建设

## 出处
- [[id:huawei.supply.refined.集成供应链isc方法论]] — ISC方法论长文
- [[id:huawei.supply.refined.供应链管理体系]] — 供应链管理体系与变革历程
- 任正非："集成供应链（ISC）解决了，公司的管理问题基本上就解决了"
