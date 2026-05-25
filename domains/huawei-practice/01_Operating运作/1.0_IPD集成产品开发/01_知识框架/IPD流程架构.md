---
id: huawei.ipd.refined.ipd-architecture
doc_type: refined
title: IPD流程架构
domain: huawei-practice
process: 1.0_IPD
layer: 01_知识框架
source_authority: 薄云实践
confidence: high
created: '2026-04-24'
updated: '2026-04-24'
related_concepts:
- huawei.ipd.refined.ipd-principles
- huawei.btit.refined.变革项目charter模板
- huawei.ipd.refined.ipd-maturity-assessment
---

# IPD流程架构

<!-- chunk: ipd-architecture.三大核心流程 -->
## 三大核心流程

```
市场管理流程 (MM) ──→ 产品路标/Charter
                              ↓
需求管理流程 (OR) ──→ 需求包
                              ↓
         IPD主流程 ──→ 产品/解决方案
```

---

<!-- chunk: ipd-architecture.mm-市场管理流程-market-management -->
## MM — 市场管理流程（Market Management）

**作用**：做正确的事，确保研发方向与市场需求一致

| 步骤 | 内容 |
|---|---|
| 理解市场 | 市场细分、客户需求、竞争态势分析 |
| 市场细分 | 识别有价值的细分市场和目标客户 |
| 组合分析 | 现有产品+在研产品的投资优先级 |
| 制定业务计划 | SPa（战略产品规划）/ BPb（业务计划） |
| 融合与优化 | 跨产品线资源协调，输出产品路标 |

**输出物**：产品系列路标 + Charter（项目任务书）

---

<!-- chunk: ipd-architecture.or-需求管理流程-opportunity-requirement -->
## OR — 需求管理流程（Opportunity Requirement）

**作用**：确保客户真实需求被正确传递给研发团队

- 需求收集：来自销售、市场、客户反馈、竞品分析
- 需求分析：功能需求 + 非功能需求 + 约束条件
- 需求分配：哪个版本实现哪些需求
- 需求变更管理：变更影响评估与审批

---

<!-- chunk: ipd-architecture.ipd主流程-阶段与dcp -->
## IPD主流程 — 阶段与DCP

```
概念阶段 → DCP0 → 计划阶段 → DCP1 → 开发阶段 → DCP2 → 验证阶段 → DCP3 → 发布阶段 → DCP4 → 生命周期管理
```

| DCP | 名称 | 核心问题 |
|---|---|---|
| DCP0 | 立项评审 | 这个产品值得做吗？市场机会是否存在？ |
| DCP1 | 计划评审 | 计划可行吗？资源是否到位？ |
| DCP2 | 开发完成评审 | 开发目标达成了吗？可以测试了吗？ |
| DCP3 | 发布评审 | 产品质量达标了吗？可以上市了吗？ |
| DCP4 | 生命周期评审 | 产品是否继续投资？何时退市？ |

**每个DCP的决策只有三种**：Go（继续）/ Kill（终止）/ Hold（暂停）

---

<!-- chunk: ipd-architecture.pdt-跨功能产品开发团队 -->
## PDT — 跨功能产品开发团队

**组成**：
- PDT Leader（产品经理，对商业成功负责）
- 研发代表
- 市场/销售代表
- 供应链/制造代表
- 财务代表
- 采购代表（硬件产品）
- 质量代表

**核心原则**：
- PDT Leader有资源调度权，不是协调员
- 团队成员在项目期间对PDT负责，而非对职能部门负责
- 跨部门问题在PDT内部解决，不升级

---

<!-- chunk: ipd-architecture.charter-项目任务书 -->
## Charter — 项目任务书

Charter是IPD立项的核心文件，包含：

| 模块 | 内容 |
|---|---|
| 市场机会 | 目标市场规模、客户需求、竞争分析 |
| 产品定义 | 功能特性、差异化卖点、价格定位 |
| 商业计划 | 收入预测、成本估算、投资回报周期 |
| 开发计划 | 里程碑、资源需求、关键风险 |
| 成功标准 | 可量化的成功指标（市场份额/营收/客户满意度） |

---

_关联：[[IPD核心理念]] · [[IPD成熟度评估]] · [[Charter模板]]_

---

<!-- chunk: ipd-architecture.产品生命周期管理-plm-dcp4后续 -->
## 产品生命周期管理（PLM）— DCP4后续

[详细内容见：[[产品生命周期管理PLM]]]

> DCP4标志着IPD主流程的结束，PLM的开始。产品正式进入市场后，生命周期管理机制接管，持续评估产品的商业价值与投资优先级。

### DCP4 生命周期评审触发条件

- 年度例行评审（每年至少一次）
- 市场重大变化触发（竞品颠覆、技术换代）
- 财务指标持续恶化触发

### 退市决策流程

1. 产品团队提交退市建议（含影响分析）
2. IPMT评审并决策
3. 发布EoL通知（提前18-24个月）
4. 客户迁移支持计划
5. 停止新订单接收
6. 维护期结束，完全退市

<!-- chunk: ipd-architecture.参考资料 -->
## 参考资料

- [[华为的IPD]]
- [[华为研发管理]]
