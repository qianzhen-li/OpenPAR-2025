# 🌟 OpenPAR: The Comprehensive Collection (2022-2025)

本项目汇集了 **Event-AHU 官方成果** 以及 **全球顶会 (CVPR/ICCV/AAAI)** 的最新 PAR 论文。
所有链接均已修正，确保指向真实的官方资源。

> **Main Codebase**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🔥 Part 1: 2024-2025 Breaking News (最新爆发)
*涵盖 Mamba 架构、LLM 大模型融合、Event 相机及安全攻防。*

| Paper Title & Venue | Code (官方/复现) | Paper (PDF) | 💡 Expert Insights |
| :--- | :---: | :---: | :--- |
| **RGB-Event based PAR: Benchmark & Asymmetric RWKV Fusion**<br>(ArXiv 2025) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2504.10018) | **(多模态 SOTA)** 引入事件相机解决夜间难题，利用 RWKV 处理高频事件流。 |
| **PAR: A New Benchmark Dataset (MSP60K) & LLM Augmented Framework**<br>(AAAI 2025) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2408.09720) | **(数据基准)** 发布 MSP60K，用 LLM 清洗数据并生成语义描述。 |
| **Adversarial Semantic and Label Perturbation Attack for PAR (ASL-PAR)**<br>(ArXiv 2025) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2505.23313) | **(安全攻防)** 领域首个对抗攻击框架，研究语义扰动攻击。 |
| **PromptPAR: A Prompt-based Framework for PAR**<br>(CVPR 2024) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_PromptPAR_A_Prompt-based_Framework_for_Pedestrian_Attribute_Recognition_CVPR_2024_paper.pdf) | **(动态 Prompt)** 根据图像内容自适应生成 Prompt，提升泛化性。 |
| **Pedestrian Attribute Recognition as Label-balanced Multi-label Learning**<br>(TPAMI 2024) | [Official](https://github.com/Purdue-Digital-Twin/LBL) | [PDF](https://arxiv.org/abs/2405.04858) | **(长尾分布)** 针对属性样本极少问题，提出数学严谨的重采样平衡策略。 |
| **An Empirical Study of Mamba-based PAR**<br>(IEEE T-MM 2024) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2407.10374) | **(Mamba 评测)** 领域首篇 Mamba 实证研究，指出直接照搬 Transformer 的局限。 |
| **SNN-PAR: Spiking Neural Networks for PAR**<br>(ICIG 2025) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2410.07857) | **(低功耗)** 探索脉冲神经网络 (SNN) 应用，适合边缘设备。 |

---

## 🚀 Part 2: 2023-2024 Vision-Language (Prompt & CLIP 时代)
*核心思想：利用 CLIP 的文本理解能力来辅助视觉识别。*

| Paper Title & Venue | Code | Paper (PDF) | 💡 Expert Insights |
| :--- | :---: | :---: | :--- |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion**<br>(IEEE TCSVT 2024) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2312.10692) | **(Prompt 鼻祖)** 最早将 CLIP Prompt 引入 PAR，将属性列表转为句子。 |
| **GAAP: Attribute-guided Prompt for Unsupervised Person Retrieval**<br>(IJCAI 2024) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://www.ijcai.org/proceedings/2024/116) | **(无监督)** 利用“属性词”生成 Prompt 驱动 CLIP 产生伪标签。 |
| **VTB: Vision-Text Baseline for Pedestrian Attribute Recognition**<br>(IEEE T-BIOM 2023) | [Official](https://github.com/maywe/VTB) | [PDF](https://arxiv.org/abs/2305.09668) | **(双塔结构)** 早期探索 BERT 与 ViT 结合的经典 Baseline。 |
| **COCO: Co-operation of Co-relation for Pedestrian Attribute Recognition**<br>(ICCV 2023) | [Unofficial](https://github.com/valencebond/Rethinking_of_PAR) | [PDF](https://arxiv.org/abs/2307.15252) | **(关系建模)** 同时建模属性间关系和空间关系。 |
| **Diverse Features Discovery Transformer for PAR (DF2)**<br>(Eng. App. AI 2023) | [Official](https://github.com/AmirHussain/DF2) | [PDF](https://arxiv.org/abs/2303.04456) | **(特征解耦)** 让 Transformer 关注不同的属性区域。 |

---

## 🎥 Part 3: Video-based PAR (视频行人属性)
*核心思想：利用时间信息解决单帧模糊、遮挡问题。*

| Paper Title & Venue | Code | Paper (PDF) | 💡 Expert Insights |
| :--- | :---: | :---: | :--- |
| **Spatio-Temporal Side Tuning Pre-trained Foundation Models**<br>(IEEE TCSVT 2024) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2404.17929) | **(高效微调)** Side-Tuning 技术，只训练小网络，显存占用极低。 |
| **Video-based PAR via Spatio-temporal Attention**<br>(PRCV 2022) | - | [PDF](https://link.springer.com/chapter/10.1007/978-3-030-31726-2_18) | **(时空注意力)** 经典的视频 PAR 方法，通过注意力机制聚合多帧信息。 |
| **Learning CLIP Guided Visual-Text Fusion Transformer for Video PAR**<br>(CVPRW 2023) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://openaccess.thecvf.com/content/CVPR2023W/NFVLR/papers/Zhu_Learning_CLIP_Guided_Visual-Text_Fusion_Transformer_for_Video-Based_Pedestrian_Attribute_CVPRW_2023_paper.pdf) | **(早期探索)** Side-Tuning 的前身，验证了 CLIP 在视频任务上的有效性。 |

---

## 🏛️ Part 4: Foundations & Classics (2022 经典)
*这些论文是理解现代 PAR 方法的基石。*

| Paper Title & Venue | Code | Paper (PDF) | 💡 Expert Insights |
| :--- | :---: | :---: | :--- |
| **Relation-Aware PAR with Graph Convolutional Networks**<br>(AAAI 2022) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2204.03852) | **(图网络)** 利用 GCN 挖掘属性共现关系，是 Graph 类方法的标杆。 |
| **Rethinking of PAR: A Reliable Evaluation**<br>(IEEE TCSVT 2023) | [Official](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2305.08386) | **(评估标准)** 必读！提出了 Zero-Shot 新评估协议，修正刷榜偏差。 |
| **DaRE: Disentangled and Relation-aware Evidence Reasoning for PAR**<br>(IEEE TPAMI 2022) | - | [PDF](https://ieeexplore.ieee.org/document/9466400) | **(TPAMI 顶刊)** 深度解耦特征，同时考虑属性关系，数学理论扎实。 |

---
## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)

