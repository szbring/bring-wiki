---
id: huawei.ipd.refined.requirement-dcp-linkage-checklist
doc_type: refined
title: 需求与 DCP 节点联动清单
domain: huawei-practice
process: 1.0_IPD
layer: 02_诊断工具
source_authority: 薄云实践
confidence: high
created: '2026-04-24'
updated: '2026-04-24'
related_concepts:
- huawei.ipd.concept.ipd-framework
- huawei.ipd.refined.ipd-architecture
- huawei.ipd.refined.requirement-baseline
---

# 需求与 DCP 节点联动清单

> 所属流程：[[OR需求管理流程概述]] · [[IPD流程架构]]
> 标签：#华为 #IPD #[[IPD]] #需求评审 #TR

---

<!-- chunk: requirement-dcp-linkage-checklist.dcp-与需求的关系说明 -->
## DCP 与需求的关系说明

**DCP（Decision Check Point）** 是 IPD 的**商业决策评审点**，由 IPMT 主持，关注"值不值得投资"。
**TR（Technical Review）** 是**技术评审点**，由系统工程师/PDT 主持，关注"技术上能不能实现"。

> DCP 是需求的"门禁"——每个 DCP 通过前，需求输入必须达到对应质量标准，通过后建立对应层次的基线。

---

<!-- chunk: requirement-dcp-linkage-checklist.四大-dcp-节点需求输入-输出清单 -->
## 四大 DCP 节点需求输入/输出清单

### 1. Charter DCP（项目任务书决策评审）

| 项目 | 内容 |
|------|------|
| **阶段** | 概念前期，正式进入 IPD 流程之前 |
| **核心问题** | "这个产品方向值得投资吗？" |
| **需求输入** | 初步市场机会描述、客户痛点汇总、竞品分析初稿、初步价值主张 |
| **需求输出** | 批准 Charter，确定产品方向和初始投资边界 |
| **需求层次** | RR/IR 初步清单（粗颗粒度，方向性）|

---

### 2. CDCP（概念决策评审 Concept DCP）

| 项目 | 内容 |
|------|------|
| **阶段** | 概念阶段末 |
| **核心问题** | "产品概念可行吗？继续投入吗？" |
| **前置条件** | TR1（概念阶段技术评审）通过 |

**需求输入清单（Gate Input）**：
- 📥 需求收集报告（VoC 汇总，原始需求 RR 清单）
- 📥 初始需求清单（IR）及分析结论
- 📥 产品包需求初步定义（OR 初稿）
- 📥 主要 SF（系统特性）初步清单
- 📥 TR1 技术评审通过意见
- 📥 初步市场分析和客户价值主张

**需求输出清单（Gate Output）**：
- 📤 **OR 概念基线**（冻结 IR/SF 层需求）
- 📤 Charter 任务书（需求范围初步锁定）
- 📤 RMT 需求决策记录（接纳/拒绝/待定）
- 📤 需求分发计划（需求→版本/路标的初步映射）

---

### 3. PDCP（计划决策评审 Planning DCP）

| 项目 | 内容 |
|------|------|
| **阶段** | 计划阶段末 |
| **核心问题** | "开发计划可行吗？锁定投资了吗？" |
| **前置条件** | TR2（需求分解和需求规格评审）+ TR3（总体方案评审）均通过 |

**需求输入清单（Gate Input）**：
- 📥 OR/SF 层需求基线（CDCP 锁定版本）
- 📥 **SR 层完整需求规格说明书**（系统需求清单）
- 📥 AR 层需求分配方案（需求→子系统/模块分配矩阵）
- 📥 **需求追踪矩阵（RTM）**（OR→SF→SR→AR→测试用例）
- 📥 TR2 通过意见（需求分解和规格评审）
- 📥 TR3 通过意见（总体方案评审）
- 📥 详细项目计划（需求实现计划）
- 📥 资源配置方案和早期采购计划

**需求输出清单（Gate Output）**：
- 📤 **SR 基线（计划阶段基线）**（冻结 SR 层需求规格）
- 📤 AR 层需求分配方案确认（分发到各子系统/开发组）
- 📤 RTM 建立并通过评审
- 📤 锁定版本范围（Must/Should/Could 分级确认）
- 📤 绩效承诺签订（需求→团队→个人）

---

### 4. ADCP（可获得性决策评审 Availability DCP）

| 项目 | 内容 |
|------|------|
| **阶段** | 验证/发布阶段 |
| **核心问题** | "产品可以量产上市了吗？" |
| **前置条件** | TR4A + TR5 通过；β 测试/客户验证通过 |

**需求输入清单（Gate Input）**：
- 📥 SR 层 100% 实现状态跟踪报告
- 📥 AR 层各子系统实现完成证明
- 📥 **需求验证报告**（确认测试/系统测试/β 测试结果）
- 📥 非功能需求（性能/可靠性/安全性）验证通过证明
- 📥 TR4A + TR5 通过意见
- 📥 制造就绪（工艺/BOM/产能爬坡曲线）
- 📥 客户服务准备就绪（培训/资料/备件）
- 📥 产品规格书（最终版）

**需求输出清单（Gate Output）**：
- 📤 **需求实现完成确认**（All SR done，All AR done）
- 📤 可获得性基线锁定（产品规格书冻结）
- 📤 客户需求早期确认完成记录
- 📤 上市/发货计划批准
- 📤 生命周期管理计划（升级/退市策略）

---

### 5. LDCP（生命周期决策评审 Lifecycle DCP）

| 项目 | 内容 |
|------|------|
| **阶段** | 产品生命周期末期 |
| **核心问题** | "产品何时退市？" |
| **需求输入** | 产品市场表现/财务数据/竞争态势/替代产品就绪状况 |
| **需求输出** | 决策产品生命周期结束/退市计划 |

---

<!-- chunk: requirement-dcp-linkage-checklist.dcp-与-tr-的关系图 -->
## DCP 与 TR 的关系图

```
商业决策线（DCP）：
  Charter → CDCP → PDCP → ADCP → LDCP
    ↑          ↑      ↑       ↑
技术评审线（TR）：
   TR1      TR2+TR3  TR4A+TR5  TR6
   
需求层次演进：
   RR/IR     SF/SR    AR验证    退市
   (概念)    (计划)   (发布)    (EOL)
```

---

<!-- chunk: requirement-dcp-linkage-checklist.诊断问题-客户-dcp-需求管理评估 -->
## 诊断问题：客户 DCP 需求管理评估

| 问题 | 诊断目的 |
|------|---------|
| "DCP 评审时，会核查哪些需求相关材料？" | 了解 DCP 与需求管理的联动程度 |
| "PDCP 前有没有 SR 层完整需求规格书？" | 评估 SR 层分解成熟度 |
| "有没有需求追踪矩阵（RTM）？" | 评估需求可追溯性 |
| "需求变更时，有没有评估对 DCP 计划的影响？" | 评估变更管理机制 |

---

<!-- chunk: requirement-dcp-linkage-checklist.关联文档 -->
## 关联文档
- [[OR需求管理流程概述]] — 五阶段流程
- [[需求基线管理]] — 各 DCP 节点的基线建立
- [[../知识框架/IPD流程架构]] — DCP 完整流程
- [[RMT-RAT组织运作规范]] — 评审组织

---
_创建于 2026-03-29 | 来源：bring-A 收集整理_

<!-- chunk: requirement-dcp-linkage-checklist.参考资料 -->
## 参考资料

- [[华为的IPD]]
