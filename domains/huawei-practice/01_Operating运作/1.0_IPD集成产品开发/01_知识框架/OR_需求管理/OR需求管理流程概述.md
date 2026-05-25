---
id: huawei.ipd.refined.or-process-overview
doc_type: refined
title: OR 需求管理流程概述
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
- huawei.ipd.refined.requirement-baseline
- huawei.ipd.refined.requirement-classification
- huawei.ipd.refined.requirement-priority
---

# OR 需求管理流程概述

> 所属流程：[[IPD流程架构]]
> 适用阶段：贯穿 [[IPD]] 全流程
> 标签：#华为 #[[IPD]] #需求管理 #OR流程

---

<!-- chunk: or-process-overview.一句话定义 -->
## 一句话定义
OR（Opportunity Requirement）需求管理是 IPD 体系中连接市场/客户与研发团队的关键桥梁，通过五阶段漏斗型结构，确保客户真实需求被准确识别、分析、分发并实现。

<!-- chunk: or-process-overview.核心价值 -->
## 核心价值
- 防止研发"做了市场不需要"的浪费
- 将无限的客户需求转化为有限资源能支撑的版本计划
- 建立需求可追溯机制，支撑 DCP 决策质量

---

<!-- chunk: or-process-overview.五阶段流程-漏斗型结构 -->
## 五阶段流程（漏斗型结构）

```
外部/内部原始声音
        ↓
【阶段1】需求收集  →  RR（原始需求清单）
        ↓
【阶段2】需求分析  →  IR（初始需求清单）+ 价值评估报告
        ↓
【阶段3】需求分发  →  需求包（按版本/路标/SP-BP分发）
        ↓
【阶段4】需求实现  →  满足需求规格的产品/版本
        ↓
【阶段5】需求验证  →  通过各级测试的交付物
```

---

<!-- chunk: or-process-overview.阶段-1-需求收集-requirement-gathering -->
## 阶段 1：需求收集（Requirement Gathering）

| 项目 | 内容 |
|------|------|
| **输入** | 客户原始反馈、市场调研、竞品分析、协议标准、法律法规、招标书、技术演进趋势、运营维护数据 |
| **对外渠道** | 客户拜访、焦点小组、问卷调查、β测试、原型验证、高层拜访 |
| **对内渠道** | 领导层/研发/市场/测试反馈 |
| **输出物** | **RR（Raw Requirement，原始需求清单）**—— 站在客户视角描述的痛点和期望，未经标准化 |
| **要点** | 需求收集是全员职责；产品需求 = **功能需求 + DFX需求**，不能只收集功能需求 |

---

<!-- chunk: or-process-overview.阶段-2-需求分析-requirement-analysis -->
## 阶段 2：需求分析（Requirement Analysis）

| 项目 | 内容 |
|------|------|
| **输入** | RR 原始需求清单 |
| **执行者** | **RAT（需求审核团队）** |
| **核心活动** | 解释（还原真实业务场景）→ 过滤（剔除无价值/不可行）→ 分类（领域/类型/紧急程度）→ 排序（价值/工作量/战略符合度）→ 证实（必要时市场调研） |
| **输出物** | **IR（Initial Requirement，初始需求清单）**—— 标准格式和语言重新描述；**需求价值评估报告** |
| **要点** | 核心是判断需求价值——"市场需求是无限的，投资和资源永远是有限的" |

---

<!-- chunk: or-process-overview.阶段-3-需求分发-requirement-distribution -->
## 阶段 3：需求分发（Requirement Distribution）

| 时间维度 | 分发目标 |
|----------|----------|
| 🔵 长期需求（3-5年）| 进入 SP/BP 业务规划 |
| 🟡 中期需求（1-3年）| 进入产品路标 |
| 🟠 短期需求（1年内）| 纳入 Charter 任务书，立项进入 [[IPD]] 流程 |
| 🔴 紧急需求 | 通过变更评审纳入当前开发项目（尽量降低此类占比）|

**原则**：看五步，理三步，走一步（平衡长中短期需求分配）

---

<!-- chunk: or-process-overview.阶段-4-需求实现-requirement-implementation -->
## 阶段 4：需求实现（Requirement Implementation）

- PDT（产品开发团队）负责全过程
- 产品经理主导原型设计/文档输出
- 重点跟进变更的需求和阻塞问题
- 有重大外部资源阻塞的需求须纳入需求池记录

---

<!-- chunk: or-process-overview.阶段-5-需求验证-requirement-validation -->
## 阶段 5：需求验证（Requirement Validation）

| 验证层次 | 内容 |
|----------|------|
| 模块需求验证 | 单元测试 |
| 子系统需求验证 | 子系统集成测试 |
| 确认测试 | 检验是否满足需求特性规格 |
| 系统需求验证 | 系统测试，检验非功能需求符合度 |
| 特性验证 | α 测试 |
| 客户验证 | β 测试 |

---

<!-- chunk: or-process-overview.关键角色 -->
## 关键角色
- **RMT（需求管理团队）**：需求决策责任团队，见 [[RMT-RAT组织运作规范]]
- **RAT（需求审核团队）**：专业分析支撑团队，见 [[RMT-RAT组织运作规范]]
- **PDT Leader**：需求实现过程的责任人
- **产品经理**：连接客户与研发的核心接口

<!-- chunk: or-process-overview.关联文档 -->
## 关联文档
- [[需求分类标准]] — 功能/非功能/约束条件分类
- [[需求优先级方法论]] — KANO + MoSCoW
- [[需求分解规范OR-SR-EPR]] — 三层分解体系
- [[需求基线管理]] — 版本控制与变更
- [[../OR_需求诊断/RMT-RAT组织运作规范]] — 评审机制
- [[../OR_需求诊断/需求与DCP联动清单]] — DCP 节点输入输出

---
_创建于 2026-03-29 | 来源：bring-A 收集整理，参考 [[IPD]] 百科网、翰德恩咨询等公开资料_

<!-- chunk: or-process-overview.参考资料 -->
## 参考资料

- [[华为的IPD]]
- [[华为研发管理]]
- [[IPD]]
