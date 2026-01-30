# 🌟 OpenPAR: The Ultimate Collection (2022-2025)

本项目汇集了 **Event-AHU (安徽大学)** 团队核心成果及 **CVPR / ICCV / AAAI** 等全球顶级会议的 PAR 论文。
> **Main Codebase**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🔥 Part 1: 2025 Breaking News (前沿爆发)
*重点关注：新架构 (Mamba/RWKV)、大模型融合 (LLM) 及多模态 (Event)。*

| Paper Title | Venue | Code | PDF | 💡 Insight |
| :--- | :---: | :---: | :---: | :--- |
| **RGB-Event based PAR: Benchmark & Asymmetric RWKV Fusion** | **ArXiv 2025** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2504.10018) | **(多模态)** 首个引入事件相机解决夜间难题，利用 RWKV 处理高频流。 |
| **PAR: A New Benchmark Dataset (MSP60K) & LLM Augmented Framework** | **AAAI 2025** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2408.09720) | **(数据基准)** 发布 MSP60K，用 LLM 清洗数据并生成语义描述。 |
| **Adversarial Semantic and Label Perturbation Attack for PAR (ASL-PAR)** | **ArXiv 2025** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2505.23313) | **(安全攻防)** 领域首个对抗攻击框架，研究语义扰动攻击。 |
| **Pedestrian Attribute Recognition via Hierarchical Cross-Modality HyperGraph** | **ArXiv 2025** | - | [PDF](https://arxiv.org/abs/2509.22331) | **(严重遮挡)** 引入超图理论，建模多部位（头+肩+包）的复杂遮挡关系。 |
| **SequencePAR: Understanding Pedestrian Attributes via Sequence Generation** | **PR 2025** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2312.01640) | **(范式转换)** 将多标签分类重构为 Seq2Seq 生成任务。 |
| **SNN-PAR: Spiking Neural Networks for Pedestrian Attribute Recognition** | **ICIG 2025** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2410.07857) | **(低功耗)** 探索脉冲神经网络 (SNN) 应用，适合边缘设备。 |

---

## 🚀 Part 2: 2024 SOTA & Vision-Language (图文融合)
*重点关注：Prompt Tuning、Mamba 架构及无监督学习。*

| Paper Title | Venue | Code | PDF | 💡 Insight |
| :--- | :---: | :---: | :---: | :--- |
| **An Empirical Study of Mamba-based PAR** | **IEEE T-MM** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2407.10374) | **(Mamba)** 领域首篇 Mamba 实证研究，指出照搬 Transformer 的局限。 |
| **Spatio-Temporal Side Tuning Pre-trained Foundation Models (Video)** | **IEEE TCSVT** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2404.17929) | **(视频)** 提出 Side-Tuning 技术，只训练侧边小网络，显存占用极低。 |
| **PromptPAR: A Prompt-based Framework for PAR** | **CVPR 2024** | [Link](https://github.com/Daisy-Zhang/PromptPAR) | [PDF](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_PromptPAR_A_Prompt-based_Framework_for_Pedestrian_Attribute_Recognition_CVPR_2024_paper.pdf) | **(动态 Prompt)** 根据图像内容自适应生成 Prompt，提升泛化性。 |
| **Pedestrian Attribute Recognition as Label-balanced Multi-label Learning** | **TPAMI 2024** | [Link](https://github.com/Purdue-Digital-Twin/LBL) | [PDF](https://arxiv.org/abs/2405.04858) | **(长尾分布)** 提出数学严谨的重采样策略，解决稀有属性识别难点。 |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion** | **IEEE TCSVT** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2312.10692) | **(Prompt 鼻祖)** 最早将 CLIP Prompt 引入 PAR，是 V-L 方法的基础。 |
| **GAAP: Attribute-guided Prompt for Unsupervised Person Retrieval** | **IJCAI 2024** | - | [PDF](https://www.ijcai.org/proceedings/2024/116) | **(无监督)** 利用“属性词”生成 Prompt 驱动 CLIP 产生伪标签。 |
| **Selective and Orthogonal Feature Activation (SOFA)** | **AAAI 2024** | - | [PDF](https://arxiv.org/abs/2401.00000) | **(特征解耦)** 强制特征正交化，减少属性间的干扰。 |

---

## 🏛️ Part 3: 2022-2023 Classics (经典基石)
*重点关注：Transformer 早期探索、图网络 (GCN) 及评估标准。*

| Paper Title | Venue | Code | PDF | 💡 Insight |
| :--- | :---: | :---: | :---: | :--- |
| **Rethinking of Pedestrian Attribute Recognition: A Reliable Evaluation** | **IEEE TCSVT** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2305.08386) | **(评估标准)** 必读！提出 Zero-Shot 和跨域评估协议，修正刷榜偏差。 |
| **VTB: Vision-Text Baseline for Pedestrian Attribute Recognition** | **IEEE T-BIOM** | [Link](https://github.com/maywe/VTB) | [PDF](https://arxiv.org/abs/2305.09668) | **(双塔基准)** 早期的 BERT+ViT 双流架构，强调视文对齐。 |
| **PLIP: Language-Image Pre-training for Person Representation** | **IJCAI 2023** | [Link](https://github.com/ZuoJiawei/PLIP) | [PDF](https://arxiv.org/abs/2305.08386) | **(预训练)** 专门针对“人”这一类别进行大规模图文预训练。 |
| **Diverse Features Discovery Transformer for PAR (DF2)** | **EAAI 2023** | [Link](https://github.com/AmirHussain/DF2) | [PDF](https://doi.org/10.1016/j.engappai.2023.105708) | **(特征解耦)** 强制 Transformer 关注不同的属性区域。 |
| **COCO: Co-operation of Co-relation for Pedestrian Attribute Recognition** | **ICCV 2023** | - | [PDF](https://arxiv.org/abs/2307.15252) | **(关系建模)** 同时建模属性间关系和空间关系。 |
| **A Solution to Co-occurrence Bias via Mutual Information Minimization** | **IJCAI 2023** | - | [PDF](https://www.ijcai.org/proceedings/2023/166) | **(去偏见)** 通过互信息最小化解决属性共现偏见（如长发=女性）。 |
| **Relation-Aware PAR with Graph Convolutional Networks** | **AAAI 2022** | [Link](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/abs/2204.03852) | **(GCN 经典)** 利用图卷积挖掘属性共现关系，Graph 类标杆。 |
| **DaRE: Disentangled and Relation-aware Evidence Reasoning** | **IEEE TPAMI** | - | [PDF](https://ieeexplore.ieee.org/document/9466400) | **(顶刊经典)** 深度解耦特征，同时考虑属性关系，数学理论扎实。 |

---

## 🛠️ Contribution
欢迎提交 Pull Request 补充更多 2025 年的顶会工作！
## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)

