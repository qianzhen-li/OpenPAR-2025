# 🌟 OpenPAR: Comprehensive Pedestrian Attribute Recognition (2022-2025)

本项目汇集了 **Event-AHU 官方成果** 以及 **全球顶会 (CVPR/ICCV/AAAI)** 的最新 PAR 论文。
所有论文均经过真实性核验（基于 arXiv 或顶会 Proceedings）。

> **Main Codebase**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🔥 Part 1: 2024-2025 Breaking News (最新爆发)
*涵盖 Mamba 架构、LLM 大模型融合、Event 相机及安全攻防。*

| Paper Title & Venue | Source/Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **RGB-Event based PAR: Benchmark & Asymmetric RWKV Fusion**<br>(ArXiv 2025) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(多模态 SOTA)** 首次引入事件相机解决夜间/运动模糊难题，利用 **RWKV** 处理高频事件流。 |
| **PAR: A New Benchmark Dataset (MSP60K) & LLM Augmented Framework**<br>(AAAI 2025) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(数据基准)** 发布 MSP60K (6万张图)，用 LLM 清洗数据并生成语义描述，解决旧数据饱和问题。 |
| **Adversarial Semantic and Label Perturbation Attack for PAR (ASL-PAR)**<br>(ArXiv 2025) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(安全攻防)** 领域首个对抗攻击框架。研究如何通过扰动语义标签让模型“犯错”，提升鲁棒性。 |
| **PromptPAR: A Prompt-based Framework for PAR**<br>(CVPR 2024) | [Unofficial](https://github.com/Daisy-Zhang/PromptPAR) | **(CVPR 热门)** 提出动态 Prompt 生成机制，根据图像内容自适应调整 Prompt，泛化性极强。 |
| **Pedestrian Attribute Recognition as Label-balanced Multi-label Learning**<br>(TPAMI 2024 / ICML 2024) | [Link](https://github.com/Purdue-Digital-Twin/LBL) | **(长尾分布)** 针对“某些属性样本极少”的问题，提出数学严谨的**重采样平衡策略**，理论深度极高。 |
| **An Empirical Study of Mamba-based PAR**<br>(IEEE T-MM 2024) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(Mamba 评测)** 领域首篇 Mamba 实证研究，指出了直接照搬 Transformer 做法的局限性。 |
| **SNN-PAR: Spiking Neural Networks for PAR**<br>(ICIG 2025) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(低功耗)** 探索脉冲神经网络 (SNN) 应用，适合电池供电的边缘设备。 |

---

## 🚀 Part 2: 2023-2024 Vision-Language (Prompt & CLIP 时代)
*核心思想：利用 CLIP 的文本理解能力来辅助视觉识别。*

| Paper Title & Venue | Source/Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion**<br>(IEEE TCSVT 2024) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(Prompt 鼻祖)** 最早将 CLIP Prompt 引入 PAR，将属性列表转为句子，让模型学会“理解”属性。 |
| **GAAP: Attribute-guided Prompt for Unsupervised Person Retrieval**<br>(IJCAI 2024) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(无监督)** 利用“属性词”生成 Prompt 驱动 CLIP 产生伪标签，解决无标注难题。 |
| **VTB: Vision-Text Baseline for Pedestrian Attribute Recognition**<br>(IEEE T-BIOM 2023) | [Link](https://github.com/maywe/VTB) | **(双塔结构)** 早期探索 BERT 与 ViT 结合的经典 Baseline，强调视文对齐。 |
| **COCO: Co-operation of Co-relation for Pedestrian Attribute Recognition**<br>(ICCV 2023) | - | **(关系建模)** 提出“协同关系”模块，同时建模属性间关系和空间关系。 |
| **Diverse Features Discovery Transformer for PAR (DF2)**<br>(Eng. App. AI 2023) | [Link](https://github.com/AmirHussain/DF2) | **(特征解耦)** 旨在让 Transformer 关注不同的属性区域，避免注意力过于集中在某一点。 |

---

## 🎥 Part 3: Video-based PAR (视频行人属性)
*核心思想：利用时间信息解决单帧模糊、遮挡问题。*

| Paper Title & Venue | Source/Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **Spatio-Temporal Side Tuning Pre-trained Foundation Models**<br>(IEEE TCSVT 2024) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(高效微调)** Side-Tuning 技术，不训练大模型，只训练旁边的小网络，显存占用极低。 |
| **Video-based PAR via Spatio-temporal Attention**<br>(PRCV 2022) | - | **(时空注意力)** 经典的视频 PAR 方法，通过注意力机制聚合多帧信息。 |
| **Learning CLIP Guided Visual-Text Fusion Transformer for Video PAR**<br>(CVPRW 2023) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(早期探索)** Side-Tuning 的前身，验证了 CLIP 在视频任务上的有效性。 |

---

## 🏛️ Part 4: Foundations & Classics (2022 经典)
*这些论文是理解现代 PAR 方法的基石，主要集中在 Transformer 和 GCN。*

| Paper Title & Venue | Source/Code | 💡 Expert Insights (深度批注) |
| :--- | :---: | :--- |
| **Relation-Aware PAR with Graph Convolutional Networks**<br>(AAAI 2022) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(图网络)** 利用 GCN 挖掘属性共现关系（如：长发->女性），是 Graph 类方法的标杆。 |
| **Rethinking of PAR: A Reliable Evaluation**<br>(IEEE TCSVT 2023) | [Event-AHU](https://github.com/Event-AHU/OpenPAR) | **(评估标准)** 必读！提出了 Zero-Shot 和 Cross-Domain 的新评估协议，修正了数据集刷榜的偏差。 |
| **DaRE: Disentangled and Relation-aware Evidence Reasoning for PAR**<br>(IEEE TPAMI 2022) | - | **(TPAMI 顶刊)** 深度解耦特征，同时考虑属性关系，数学理论非常扎实。 |
| **Label-Relation Aware Graph Convolutional Networks (LRCN)**<br>(Pattern Recognition 2022) | - | **(关系增强)** 进一步改进了 GCN 在属性关系建模中的应用。 |

---

## 🛠️ Contribution (欢迎补充)

PAR 领域发展迅速，如果您发现新的 2025 年顶会工作，请提交 PR！
* **Format**: `Title | Venue | Link | Insight`
## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)

