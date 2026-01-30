# 🌟 OpenPAR: The Ultimate Collection (2022-2025)

本项目旨在建立一个 **Pedestrian Attribute Recognition (PAR)** 领域的全景知识库。
核心内容基于 **Event-AHU (安徽大学)** 团队的开源成果，同时收录了 **CVPR / AAAI / TPAMI** 等顶级会议的 SOTA 工作。

> **🚀 Core Framework**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🗺️ Roadmap & Relationships (技术演进图谱)

技术是如何从 2022 演变到 2025 的？请看下图：

```mermaid
graph TD
    subgraph Phase1 ["Phase 1: Foundations (2022-2023)"]
        A["Relation Modeling<br>GCN (AAAI 2022)"]
        B["Vision Transformer<br>ViT Baseline"]
    end

    subgraph Phase2 ["Phase 2: Semantic Expansion (2023-2024)"]
        B --> C["CLIP-Prompt Fusion<br>TCSVT 2024 (Prompt Tuning)"]
        C --> C1["Video Side-Tuning<br>TCSVT 2024 (Efficiency)"]
        C --> C2["Unsupervised GAAP<br>IJCAI 2024 (Pseudo Label)"]
    end

    subgraph Phase3 ["Phase 3: New Era (2025)"]
        B --> D["Mamba & RWKV<br>T-MM 2024 (Linear Complexity)"]
        D --> D1["RGB-Event Fusion<br>ArXiv 2025 (Multi-Modal)"]
        
        C --> E["LLM Agent<br>AAAI 2025 (MSP60K Dataset)"]
        
        A --> F["HyperGraph<br>ArXiv 2025 (Structure Learning)"]
    end
    
    style D fill:#f9f,stroke:#333,stroke-width:2px
    style E fill:#bbf,stroke:#333,stroke-width:2px
    style D1 fill:#f96,stroke:#333,stroke-width:2px


## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)
## 🤝 如何贡献
1. 在 `papers` 文件夹中添加 PDF（可选）。
2. 在 `README.md` 表格中追加新论文。
3. 如果复现了代码，请链接到 `code/` 目录。
