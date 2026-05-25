---
id: huawei.ipd.refined.ipd-organization
doc_type: refined
title: IPD组织体系
domain: huawei-practice
process: 1.0_IPD
layer: 01_知识框架
source_authority: 薄云实践
confidence: high
created: '2026-04-24'
updated: '2026-04-24'
related_concepts:
- huawei.ipd.refined.ipd-architecture
- huawei.ipd.refined.ipd-principles
- huawei.ipd.refined.tr-mechanism
---

# IPD组织体系

<!-- chunk: ipd-organization.一句话定义 -->
## 一句话定义
IPD组织体系是支撑IPD流程运转的组织保障，核心是建立跨功能团队（PDT）和投资决策委员会（IPMT）的双层结构，确保"流程有人走、决策有人担"。

---

<!-- chunk: ipd-organization.核心组织架构 -->
## 核心组织架构

```
            IPMT（投资决策委员会）
               │ 战略方向与投资决策
    ┌──────────┼──────────┐
    │          │          │
 PDT-A      PDT-B      PDT-C        ← 产品开发团队（跨功能）
    │          │          │
 ┌──┼──┐   ┌──┼──┐   ┌──┼──┐
 研发 市场  研发 市场  研发 市场    ← 功能部门（资源池）
 供应链 财务 供应链 财务 供应链 财务
```

**关键原则**：矩阵式管理——PDT是"纵向执行"，功能部门是"横向资源供给"。

---

<!-- chunk: ipd-organization.ipmt-集成组合管理团队-integrated-portfolio-management-team -->
## IPMT — 集成组合管理团队（Integrated Portfolio Management Team）

### 定义与职责
IPMT是产品投资决策的最高权力机构，对产品线的商业成功负责。

| 职责 | 说明 |
|---|---|
| 投资决策 | 在DCP评审点做出Go/Kill/Hold决策 |
| 资源分配 | 在多个PDT之间分配研发资源 |
| 产品路标审批 | 审批产品系列路标和Charter |
| 绩效考核 | 对PDT Leader的商业结果负责评价 |

### 组成人员

| 角色 | 通常由谁担任 | 职责 |
|---|---|---|
| IPMT主任 | 产品线总裁/BU负责人 | 最终决策权，对产品线P&L负责 |
| 研发VP | 技术负责人 | 技术可行性评审 |
| 市场VP | 市场/销售负责人 | 市场机会与竞争评审 |
| 供应链VP | 供应链负责人 | 交付能力评审 |
| 财务总监 | CFO或财务负责人 | 投资回报评审 |
| 质量总监 | 质量负责人 | 质量风险评审 |

### IPMT运作规则
- **会议频率**：按DCP节点触发，非定期会议
- **决策机制**：IPMT主任有一票否决权，但需说明理由；无异议则Go
- **决策结果**：只有Go/Kill/Hold三种，不接受"有条件通过"
- **决策记录**：每次DCP决策必须文档化，作为后续审计依据

---

<!-- chunk: ipd-organization.pdt-产品开发团队-product-development-team -->
## PDT — 产品开发团队（Product Development Team）

### 定义与职责
PDT是IPD的核心执行单元，跨功能组建，对产品从立项到上市的商业成功端到端负责。

### PDT核心角色

| 角色 | 英文 | 职责 | 来自部门 |
|---|---|---|---|
| PDT Leader | — | 团队核心，对商业成功负责 | 产品管理/研发 |
| 研发代表 | R&D Representative | 技术方案与开发执行 | 研发部 |
| 市场代表 | Marketing Representative | 市场需求与上市策略 | 市场部 |
| 系统工程师 | System Engineer | 系统架构与子系统协调 | 研发/架构组 |
| 采购代表 | Procurement Representative | 物料选型与供应商管理 | 采购部 |
| 制造代表 | Manufacturing Representative | 可制造性设计与量产导入 | 制造/供应链 |
| 财务代表 | Finance Representative | 预算管理与ROI跟踪 | 财务部 |
| 质量代表 | Quality Representative | 质量计划与质量评审 | 质量部 |

### PDT运作的关键原则

1. **PDT Leader有实权**：不是协调员，而是指挥官，有资源调度权和团队成员绩效打分权
2. **全职投入**：核心成员（PDT Leader + 研发代表 + 市场代表）至少70%时间投入PDT
3. **对商业成功负责**：PDT的考核指标不是"按时做完"，而是"产品上市后的商业结果"
4. **内部解决冲突**：跨部门问题在PDT内部解决，不升级到IPMT
5. **单一责任人**：每个模块只有一个代表，避免推诿

### PDT组建时点
- DCP0之前：PDT Leader和核心成员到位
- DCP0通过后：全员到位，启动概念阶段工作
- DCP4之后：PDT逐步解散，转入生命周期管理团队

---

<!-- chunk: ipd-organization.irt-集成评审团队-integration-review-team -->
## IRT — 集成评审团队（Integration Review Team）

### 定义
IRT是技术评审的执行组织，负责在IPD各阶段对技术方案进行评审，确保技术可行性和质量达标。

### IRT与IPMT的区别

| 维度 | IPMT | IRT |
|---|---|---|
| 评审性质 | 商业决策评审 | 技术评审 |
| 决策权限 | Go/Kill/Hold | 通过/不通过/附条件通过 |
| 评审对象 | Charter、DCP | TR（技术评审点） |
| 关注焦点 | 市场机会与投资回报 | 技术方案与产品质量 |
| 主席 | IPMT主任 | 首席工程师/技术VP |

### IRT组成
- IRT主任（首席工程师或技术VP）
- 系统架构师
- 各子系统技术专家
- 质量代表
- 外部专家（必要时邀请）

---

<!-- chunk: ipd-organization.pmt-组合管理团队-portfolio-management-team -->
## PMT — 组合管理团队（Portfolio Management Team）

### 定义
PMT负责产品组合的投资决策与资源平衡，是IPMT的参谋机构。

### 职责
- 制定产品系列路标（Roadmap）
- 在多个项目之间进行优先级排序
- 管理产品组合的财务回报
- 为IPMT的DCP决策提供分析输入

### PMT与IPMT的关系
```
PMT（分析建议）→ IPMT（决策批准）
```
PMT不做决策，但提供专业的组合分析，是IPMT决策的"大脑"。

---

<!-- chunk: ipd-organization.rmt-rat-需求管理团队 -->
## RMT/RAT — 需求管理团队

| 角色 | 全称 | 职责 |
|---|---|---|
| RMT | Requirement Management Team | 需求分析、分解、分配 |
| RAT | Requirement Analysis Team | 需求收集、初步分析、分类 |

**关系**：RAT是一线需求收集的前哨，RMT是需求分析决策的中枢。详细运作见[[RMT-RAT组织运作规范]]。

---

<!-- chunk: ipd-organization.功能部门的角色 -->
## 功能部门的角色

### 核心原则：双轨考核
功能部门不是IPD的对立面，而是资源保障的"大后方"：

| 功能部门 | IPD中的角色 | 考核方式 |
|---|---|---|
| 研发部 | 提供研发代表和开发人员 | 双轨：PDT项目绩效 + 部门能力建设 |
| 市场部 | 提供市场代表和需求输入 | 双轨：PDT项目绩效 + 市场体系能力 |
| 供应链 | 提供制造/采购代表 | 双轨：PDT项目绩效 + 供应链响应能力 |
| 财务部 | 提供财务代表 | 双轨：PDT项目绩效 + 预算管控能力 |

**关键**：功能部门主管必须向PDT输出合格人才，而非把能力弱的人"塞"给PDT。

---

<!-- chunk: ipd-organization.华为与一般企业的差异 -->
## 华为与一般企业的差异

| 维度 | 华为实践 | 一般企业现状 | 差距 |
|---|---|---|---|
| IPMT | 有真正的决策权，可Kill项目 | 立项审批走形式 | 决策权威性 |
| PDT Leader | 有资源调度权，对商业结果负责 | 只是项目经理，协调为主 | 权责对等 |
| 跨部门协作 | 制度化嵌入，非靠个人关系 | 靠催、靠关系、靠领导协调 | 制度vs人治 |
| 功能部门 | 资源池定位，双轨考核 | 部门利益优先，不愿输出人才 | 矩阵管理成熟度 |

---

<!-- chunk: ipd-organization.薄云咨询的应用建议 -->
## 薄云咨询的应用建议

### 常见误区
1. **照搬华为组织**：华为有数万研发人员，中小企业不需要完整的IPMT/PMT/IRT架构
2. **PDT虚设**：组建了PDT但不给实权，变成了"跨部门协调会"
3. **功能部门不配合**：没有双轨考核，部门主管不放人

### 分级落地建议

| 企业规模 | IPMT | PDT | IRT/PMT |
|---|---|---|---|
| <50人研发 | CEO+技术VP+市场VP | 3-5人核心团队 | 不需要，CEO兼 |
| 50-200人 | 5-7人委员会 | 5-8人，核心全职 | 兼职IRT |
| 200-1000人 | 正式IPMT | 完整PDT | 正式IRT+PMT |
| >1000人 | 多产品线IPMT | 多PDT并行 | 完整组织体系 |

---

_关联：[[IPD核心理念]] · [[IPD流程架构]] · [[DCP决策评审机制]] · [[TR技术评审体系]]_

<!-- chunk: ipd-organization.参考资料 -->
## 参考资料

- [[华为的IPD]]
- [[华为研发管理]]
