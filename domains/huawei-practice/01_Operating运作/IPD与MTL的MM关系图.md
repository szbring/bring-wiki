---
id: huawei.overview.refined.ipd与mtl的mm关系图
doc_type: refined
title: IPD的MM与MTL的MM关系图
domain: huawei-practice
process: 0.0_overview
layer: 01_知识框架
source_authority: 薄云实践
confidence: high
created: '2026-04-27'
updated: '2026-04-27'
related_concepts:
- huawei.ipd.refined.ipd-architecture
- huawei.mtl.refined.mtl流程架构
---

# IPD的MM与MTL的MM关系图

## 总览：同一方法论，两个应用场景

```mermaid
flowchart TB
    subgraph DSTE["🖥️ DSTE 战略管理"]
        direction LR
        SP["SP 战略规划<br/>3-5年"]
        BP["BP 年度经营计划"]
    end

    subgraph MM_CORE["📐 MM 方法论（共用六步法）"]
        direction TB
        S1["Step 1<br/>理解市场"]
        S2["Step 2<br/>市场细分"]
        S3["Step 3<br/>组合分析"]
        S4["Step 4<br/>制定细分市场战略"]
        S5["Step 5<br/>制定业务计划"]
        S6["Step 6<br/>综合与优化"]
        S1 --> S2 --> S3 --> S4 --> S5 --> S6
    end

    subgraph IPD_MM["🔬 IPD 中的 MM — 回答「做什么产品」"]
        direction TB
        IPD_OUT1["📋 产品路标 Roadmap"]
        IPD_OUT2["📋 Charter 项目任务书"]
        IPD_OUT3["📋 OR 需求包"]
        IPD_OUT1 --> IPD_OUT2
        IPD_OUT1 --> IPD_OUT3
    end

    subgraph MTL_MM["📢 MTL 中的 MM — 回答「怎么卖出去」"]
        direction TB
        MTL_OUT1["🎯 H1/H2/H3 细分市场组合"]
        MTL_OUT2["🎯 市场计划 & GTM策略"]
        MTL_OUT3["🎯 营销资源分配"]
        MTL_OUT1 --> MTL_OUT2 --> MTL_OUT3
    end

    subgraph IPD_MAIN["🔧 IPD 主流程"]
        direction LR
        C["概念"] --> P["计划"] --> D["开发"] --> V["验证"] --> R["发布"]
    end

    subgraph MTL_FLOW["📣 MTL 后续模块"]
        direction LR
        JI["联合创新 JI"] --> SCE["销售赋能 SCE"] --> DG["激发需求 DG"]
    end

    LTC["💰 LTC 销售流程<br/>成交 · 回款"]

    %% 主链路
    DSTE -->|"战略方向"| MM_CORE
    MM_CORE -->|"产品投资决策"| IPD_MM
    MM_CORE -->|"市场投资决策"| MTL_MM
    IPD_MM -->|"Charter + 需求"| IPD_MAIN
    MTL_MM -->|"细分策略 + 营销计划"| MTL_FLOW
    IPD_MAIN -->|"产品/解决方案"| MTL_FLOW
    MTL_FLOW -->|"高质量线索"| LTC

    %% IPD → MTL 的信息流
    IPD_MM -.->|"产品路标<br/>客户需求<br/>GTM输入"| MTL_MM

    style MM_CORE fill:#E8F5E9,stroke:#4CAF50,stroke-width:2px
    style IPD_MM fill:#E3F2FD,stroke:#2196F3,stroke-width:2px
    style MTL_MM fill:#FFF3E0,stroke:#FF9800,stroke-width:2px
    style IPD_MAIN fill:#E3F2FD,stroke:#2196F3,stroke-width:1px
    style MTL_FLOW fill:#FFF3E0,stroke:#FF9800,stroke-width:1px
    style DSTE fill:#F3E5F5,stroke:#9C27B0,stroke-width:2px
    style LTC fill:#FFEBEE,stroke:#F44336,stroke-width:2px
```

---

## 端到端信息流转

```mermaid
flowchart LR
    subgraph 洞察层["🔍 洞察（共享）"]
        MI["市场洞察 MI"]
    end

    subgraph 决策层["📐 决策（MM 六步法）"]
        IPD_MM["IPD-MM<br/>产品投资决策"]
        MTL_MM["MTL-MM<br/>市场投资决策"]
    end

    subgraph 执行层["⚙️ 执行"]
        IPD_DEV["IPD 主流程<br/>开发产品"]
        MTL_MKT["MTL 营销<br/>生成线索"]
    end

    subgraph 变现层["💰 变现"]
        LTC["LTC<br/>成交回款"]
    end

    MI --> IPD_MM
    MI --> MTL_MM
    IPD_MM -->|"产品路标 + Charter"| IPD_DEV
    MTL_MM -->|"细分策略 + 营销计划"| MTL_MKT
    IPD_DEV -->|"产品/方案"| MTL_MKT
    IPD_MM -.->|"需求 · 路标 · GTM"| MTL_MM
    MTL_MKT -->|"销售线索"| LTC

    style 洞察层 fill:#E8F5E9,stroke:#4CAF50
    style 决策层 fill:#FFF8E1,stroke:#FFC107
    style 执行层 fill:#E3F2FD,stroke:#2196F3
    style 变现层 fill:#FFEBEE,stroke:#F44336
```

---

## 对比表：两个场景的差异

```mermaid
flowchart TB
    subgraph COMPARE["IPD-MM vs MTL-MM"]
        direction TB
        A["<b>相同点</b><br/>✅ 同一套 MM 六步法<br/>✅ 同一套分析工具（SWOT / $APPEALS / PESTEL）<br/>✅ 共享市场洞察数据<br/>✅ 共享细分市场结论"]
        B["<b>不同点</b>"]
        C["<b>IPD-MM</b><br/>🎯 核心问题：做什么产品？<br/>📤 关键输出：产品路标 + Charter<br/>👥 服务对象：PMT / PDT<br/>💰 投资视角：研发资源分配<br/>⬇️ 下游：IPD 主流程"]
        D["<b>MTL-MM</b><br/>🎯 核心问题：怎么卖出去？<br/>📤 关键输出：H1/H2/H3 组合 + 营销计划<br/>👥 服务对象：细分市场经理 / 营销团队<br/>💰 投资视角：营销资源分配<br/>⬇️ 下游：JI → SCE → DG"]
    end

    A --> B
    B --> C
    B --> D

    style A fill:#E8F5E9,stroke:#4CAF50
    style C fill:#E3F2FD,stroke:#2196F3
    style D fill:#FFF3E0,stroke:#FF9800
```

---

## 一句话总结

> **IPD 的 MM 和 MTL 的 MM 是同一套方法论的两个应用**——IPD 用它决定"做什么产品"（研发侧），MTL 用它决定"怎么卖出去"（营销侧）。两者共享洞察和分析，IPD-MM 的输出是 MTL-MM 的关键输入。

---

_关联：[[IPD流程架构]] · [[MTL流程架构]] · [[IPD解读——市场管理（MM）方法论]] · [[MM市场管理流程概述]]_
