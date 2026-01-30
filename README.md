# 🌟 OpenPAR 2025: Pedestrian Attribute Recognition Collection

本项目旨在整理 2025 年及近期行人属性识别 (PAR) 领域的最新进展。重点关注 Mamba 架构、CLIP-based 视觉语言融合以及复杂场景下的属性识别。

> **核心代码库 (Base Framework):** > [Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR) (我们主要基于此框架进行复现和扩展)

## 🔥 重点关注 (Highlight)

这里存放我们需要重点研究、复现或魔改的核心论文。

| Paper Title | Year/Venue | Category | Code | Link | 备注 |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion** | 2024/ArXiv | **VL-Fusion** | [Coming Soon](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/html/2312.10692v2)| **(重点)** 基于 CLIP 提示学习，需精读 |
| **An Empirical Study of Mamba-based Pedestrian Attribute Recognition** | 2024/ArXiv | **Mamba** | [Check OpenPAR](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/pdf/2407.10374) | 探索 Mamba 在 PAR 的有效性 |


## 🗺️ 技术演进图谱 (Technology Roadmap)

在阅读论文前，建议先理解技术发展的脉络：

```mermaid
graph TD
    A[<b>CNN Era</b><br>ResNet baseline] --> B[<b>Transformer Era (2022-2023)</b><br>ViT / VTFPAR]
    A --> C[<b>Graph / GCN (2022)</b><br>Relation Modeling]
    
    B --> D{<b>2024-2025 New Paradigms</b>}
    
    D -->|Efficiency| E[<b>Mamba & RWKV (2025)</b><br>Linear Complexity]
    D -->|Semantics| F[<b>LLM & CLIP (2024)</b><br>Prompt Tuning / GAAP]
    D -->|Hard Case| G[<b>Multi-Modal (2025)</b><br>RGB-Event / HyperGraph]
    
    E --> E1[Empirical Mamba]
    E --> E2[RGB-Event RWKV]
    
    F --> F1[MSP60K Dataset]
    F --> F2[Video Side-Tuning]

## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)
## 🤝 如何贡献
1. 在 `papers` 文件夹中添加 PDF（可选）。
2. 在 `README.md` 表格中追加新论文。
3. 如果复现了代码，请链接到 `code/` 目录。
