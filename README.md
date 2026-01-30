# 🌟 OpenPAR: The Ultimate Collection (2022-2025)

本项目旨在建立一个 **Pedestrian Attribute Recognition (PAR)** 领域的全景知识库。
核心内容基于 **Event-AHU (安徽大学)** 团队的开源成果，同时收录了 **CVPR / AAAI / TPAMI** 等顶级会议的 SOTA 工作。

> **🚀 Core Framework**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🔥 Part 1: Event-AHU Core Works (2024-2025)
*基于 OpenPAR 框架的最新前沿进展，涵盖 Mamba、RWKV、LLM 及复杂场景。*

### 1. New Architectures (Mamba / RWKV / SNN)
> **趋势解读**: 抛弃沉重的 Transformer，转向线性复杂度的 Mamba 和 RWKV，追求极致的推理效率。

| Paper Title & Venue | Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **RGB-Event based PAR: Benchmark & Asymmetric RWKV Fusion**<br>(ArXiv 2025) [\[PDF\]](https://arxiv.org/abs/2504.10018) | [Link](https://github.com/Event-AHU/OpenPAR) | **(最新)** 首次引入事件相机解决夜间/运动模糊难题。**亮点**：设计了“非对称 RWKV”架构，专门处理高频稀疏的事件流数据，比纯 RGB 方法在夜间提升显著。 |
| **An Empirical Study of Mamba-based PAR**<br>(IEEE T-MM 2024) [\[PDF\]](https://arxiv.org/abs/2407.10374) | [Link](https://github.com/Event-AHU/OpenPAR) | **(基准)** PAR 领域首篇 Mamba 评测。**避坑**：实验发现直接将属性标签作为 Token 拼接到 VMamba 中并不能提升性能，这打破了 ViT 时代的经验主义。 |
| **SNN-PAR: Spiking Neural Networks for PAR**<br>(ICIG 2025) [\[PDF\]](https://arxiv.org/abs/2410.07857) | [Link](https://github.com/Event-AHU/OpenPAR) | **(低功耗)** 探索脉冲神经网络 (SNN) 在 PAR 中的应用。适合部署在对功耗极其敏感的边缘监控设备上。 |

### 2. LLM & Vision-Language (Prompt / CLIP)
> **趋势解读**: 利用大模型 (LLM) 的知识库来弥补视觉特征的不足，解决“长尾属性”和“语义理解”问题。

| Paper Title & Venue | Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **PAR: A New Benchmark Dataset (MSP60K) & LLM Augmented Framework**<br>(AAAI 2025) [\[PDF\]](https://arxiv.org/abs/2408.09720) | [Link](https://github.com/Event-AHU/OpenPAR) | **(重磅数据)** 发布了 MSP60K (6万张图)，是 PA100K 之后最大的新基准。**亮点**：不仅用 LLM 增强训练，还用 LLM 清洗了数据标签，解决了旧数据集标注混乱的问题。 |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion**<br>(IEEE TCSVT 2024) [\[PDF\]](https://arxiv.org/abs/2312.10692) | [Link](https://github.com/Event-AHU/OpenPAR) | **(经典)** Prompt Tuning 在 PAR 的奠基之作。将属性列表转化为句子喂给 CLIP，让预训练模型“零样本”或“少样本”也能识别属性。 |
| **GAAP: Attribute-guided Prompt for Unsupervised Person Retrieval**<br>(IJCAI 2024) [\[PDF\]](https://www.ijcai.org/proceedings/2024/116) | [Link](https://github.com/Event-AHU/OpenPAR) | **(无监督)** 解决无标注难题。利用“属性词”生成 Prompt 驱动 CLIP 产生伪标签。**启示**：证明了属性可以作为跨模态检索的中间桥梁。 |

### 3. Hard Settings (Video / Occlusion / Attack)
> **趋势解读**: 解决真实落地场景中的“硬骨头”：视频帧冗余、严重遮挡和安全对抗。

| Paper Title & Venue | Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **Spatio-Temporal Side Tuning Pre-trained Foundation Models**<br>(IEEE TCSVT 2024) [\[PDF\]](https://arxiv.org/abs/2404.17929) | [Link](https://github.com/Event-AHU/OpenPAR) | **(视频高效)** 针对视频 PAR，提出了 Side-Tuning (侧边微调)。不训练大模型，只训练旁边的小网络，显存占用极低，工程价值极高。 |
| **Pedestrian Attribute Recognition via Hierarchical Cross-Modality HyperGraph**<br>(ArXiv 2025) [\[PDF\]](https://arxiv.org/abs/2509.22331) | - | **(遮挡处理)** 引入超图 (HyperGraph)。普通图只能连两点，超图能把（头、帽子、眼镜）打包成一个超边，专门解决多部位同时遮挡的问题。 |
| **Adversarial Semantic and Label Perturbation Attack for PAR (ASL-PAR)**<br>(ArXiv 2025) [\[PDF\]](https://arxiv.org/abs/2505.23313) | [Link](https://github.com/Event-AHU/OpenPAR) | **(安全攻防)** PAR 领域的首个对抗攻击框架。对于研究模型鲁棒性和安全性的同学是必读的开山之作。 |

---

## 🌍 Part 2: Global SOTA Extensions (2022-2025)
*收录 Event-AHU 之外的顶会 (CVPR, TPAMI, AAAI) 核心工作，补全视野。*

| Paper Title & Venue | Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **Label-Balanced Multi-Label Learning for PAR**<br>(TPAMI 2024) [\[Link\]](https://ieeexplore.ieee.org/document/10856608) | [Link](https://github.com/Purdue-Digital-Twin/LBL) | **(长尾分布)** 专门解决属性不平衡问题（如“戴帽子”的人很少）。提出了基于重采样的平衡策略，数学推导严谨。 |
| **PromptPAR: A Prompt-based Framework for PAR**<br>(CVPR 2024) | - | **(动态Prompt)** 相比于 Event-AHU 的固定 Prompt，这篇工作尝试根据图片内容动态生成 Prompt，进一步提升了泛化性。 |
| **Rethinking of PAR: A Reliable Evaluation**<br>(IEEE TCSVT 2023) [\[PDF\]](https://arxiv.org/abs/2305.08386) | [Link](https://github.com/Event-AHU/OpenPAR) | **(评估标准)** 必读！指出了现有数据集刷榜的虚高现象，并提出了 Zero-Shot 和 Cross-Domain 的新评估协议。 |
| **Relation-Aware PAR with Graph Convolutional Networks**<br>(AAAI 2022) [\[PDF\]](https://arxiv.org/abs/2204.03852) | [Link](https://github.com/Event-AHU/OpenPAR) | **(图网络经典)** 2022年的标杆之作。利用 GCN 挖掘属性共现关系（如：长发->女性），是后续所有 Graph 类工作的鼻祖。 |

---

## 🗺️ Roadmap & Relationships (论文关系图谱)

技术是如何从 2022 演变到 2025 的？请看下图：

```mermaid
graph TD
    subgraph "Phase 1: Foundations (2022-2023)"
        A[<b>Relation Modeling</b><br>GCN (AAAI'22)]
        B[<b>Vision Transformer</b><br>ViT Baseline]
    end

    subgraph "Phase 2: Semantic Expansion (2023-2024)"
        B --> C[<b>CLIP-Prompt Fusion</b><br>TCSVT'24 (Prompt Tuning)]
        C --> C1[<b>Video Side-Tuning</b><br>TCSVT'24 (Efficiency)]
        C --> C2[<b>Unsupervised GAAP</b><br>IJCAI'24 (Pseudo Label)]
    end

    subgraph "Phase 3: New Era (2025)"
        B --> D[<b>Mamba & RWKV</b><br>T-MM'24 (Linear Complexity)]
        D --> D1[<b>RGB-Event Fusion</b><br>ArXiv'25 (Multi-Modal)]
        
        C --> E[<b>LLM Agent</b><br>AAAI'25 (MSP60K Dataset)]
        
        A --> F[<b>HyperGraph</b><br>ArXiv'25 (Structure Learning)]
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
