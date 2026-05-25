---
id: huawei.ipd.refined.mm-methodology
doc_type: refined
title: MM 市场管理流程概述
domain: huawei-practice
process: 1.0_IPD
layer: 01_知识框架
source_authority: 薄云实践
confidence: high
created: '2026-04-24'
updated: '2026-04-24'
related_concepts:
- huawei.ipd.concept.ipd-framework
- huawei.ipd.refined.ipd-architecture
---

# MM 市场管理流程概述

> 所属体系：华为 [[IPD]] + DSTE
> 标签：#华为 #MM #市场管理 #市场洞察 #细分市场

---

<!-- chunk: mm-methodology.一句话定义 -->
## 一句话定义
MM（Market Management，市场管理）是 IPD 体系的前端输入流程，解决"做什么产品、做给谁、怎么赢"的战略性问题，确保研发方向与市场机会一致。

<!-- chunk: mm-methodology.核心价值 -->
## 核心价值
- 将有限资源集中于最有价值的市场机会
- 为 IPD 主流程提供市场需求输入（Charter/路标）
- 打通战略（DSTE）与产品开发（IPD）之间的断层

---

<!-- chunk: mm-methodology.mm-六步框架 -->
## MM 六步框架

```
Step 1：理解市场（Understand the Market）
           ↓
Step 2：市场细分（Market Segmentation）
           ↓
Step 3：组合分析（Portfolio Analysis）
           ↓
Step 4：制定细分市场战略（Develop Segmentation Strategies）
           ↓
Step 5：制定业务计划（Develop Business Plans）
           ↓
Step 6：综合与优化（Integrate and Optimize）
```

---

<!-- chunk: mm-methodology.step-1-理解市场-四大洞察维度 -->
## Step 1：理解市场（四大洞察维度）

| 维度 | 目标 | 核心工具 |
|------|------|---------|
| **客户与市场** | 理解客户业务目标、痛点和购买决策逻辑 | SWOT、客户旅程图、$APPEALS |
| **竞争** | 全面了解竞争格局，识别优劣势 | 竞争对手画像、竞争定位图 |
| **技术** | 识别可能颠覆行业的技术趋势 | 技术雷达、Gartner曲线 |
| **宏观环境** | 理解政策/经济/社会/法规影响 | PESTEL分析 |

**输出物**：市场洞察报告（含市场规模/客户需求/竞争格局/技术趋势）

---

<!-- chunk: mm-methodology.step-2-市场细分 -->
## Step 2：市场细分

**MACS 有效细分原则：**
- **M（Measurable）** — 细分市场规模可量化
- **A（Accessible）** — 有渠道和能力触达
- **C（Competitive）** — 在该市场有相对竞争优势
- **S（Substantial）** — 规模足以支撑投资回报

**华为常用细分维度：** 地区/行业/客户规模/技术成熟度/购买力

**输出物**：细分市场地图 + 各细分市场规模估算（TAM/SAM/SOM）

---

<!-- chunk: mm-methodology.step-3-组合分析 -->
## Step 3：组合分析

**市场吸引力 × 竞争地位矩阵：**

```
              竞争地位
              强       中       弱
市场  高   ■优先投入  ■选择投入  □考虑放弃
吸引  中   ■选择投入  □维持现状  □逐步退出
力    低   □维持现状  □逐步退出  □放弃
```

**输出物**：产品/市场组合优先级决策，各细分市场投资建议

---

<!-- chunk: mm-methodology.step-4-制定细分市场战略 -->
## Step 4：制定细分市场战略

**核心问题：**
- Where to Play：在哪些细分市场重点投入？
- How to Win：用什么差异化策略赢得竞争？

**差异化策略选项：** 技术领先 / 低成本 / 客户亲密 / 生态平台

**输出物**：各细分市场竞争策略 + 差异化价值主张

---

<!-- chunk: mm-methodology.step-5-制定业务计划-sp-bp -->
## Step 5：制定业务计划（SP/BP）

| 计划类型 | 周期 | 核心内容 |
|---------|------|---------|
| **SP（战略规划）** | 3-5年 | 市场方向、产品路标、资源大盘 |
| **BP（年度经营计划）** | 1年 | 销售目标、产品发布计划、预算分配 |

**SP/BP 核心章节：**
1. 市场分析摘要（洞察结论）
2. 战略选择（Where to Play / How to Win）
3. 产品/解决方案路标
4. 财务预测（收入/成本/利润）
5. 资源需求
6. 关键里程碑与风险

**输出物**：SP/BP 文件 → 直接输入 [[IPD]] Charter 和产品路标规划

---

<!-- chunk: mm-methodology.step-6-综合与优化 -->
## Step 6：综合与优化

- 跨产品线资源协调，避免内耗
- SP/BP 与 [[IPD]] 产品路标对齐
- 年度 review 机制（Strategy Review）

**输出物**：整合后的资源分配计划 + 产品线路标（输入 [[IPD]] 立项）

---

<!-- chunk: mm-methodology.mm-与-ipd-的关系 -->
## MM 与 IPD 的关系

```
【MM 市场管理】                    【IPD 产品开发】
理解市场 → 细分 → 组合 → 战略        Charter → DCP0 → 开发 → 发布
                    ↓                    ↑
              SP/BP 业务计划 ──────→ 产品路标 + 立项需求
              产品路标规划  ──────→ OR 需求输入
```

**MM 是 [[IPD]] 的"上游"**：MM 确定做什么，IPD 决定怎么做。

---

<!-- chunk: mm-methodology.市场洞察节奏 -->
## 市场洞察节奏

| 洞察类型 | 频率 | 输出 |
|---------|------|------|
| 战略级市场洞察 | 年度 | 年度市场洞察报告，输入 SP/BP |
| 细分市场更新 | 季度 | 季度市场动态简报 |
| 竞争情报 | 月度 | 月度竞情简报 |
| 客户反馈整合 | 实时 | 客户反馈数据库 |

---

<!-- chunk: mm-methodology.关联文档 -->
## 关联文档
- [[IPD流程架构]] — IPD 主流程与 MM 的接口
- [[OR需求管理流程概述]] — MM 输出进入 OR 流程
- [[../../2.0_MTL市场到线索/01_知识框架/MTL市场洞察方法论]] — 详细方法论
- [[MM_市场细分方法论]] — 细分市场分析工具
- [[MM_竞争分析框架]] — 竞争洞察方法
- [[MM_产品组合管理]] — 组合分析详解

---
_创建于 2026-03-29 | 综合整理自知识库现有内容_

<!-- chunk: mm-methodology.参考资料 -->
## 参考资料

- [[IPD]]
