# 🌟 OpenPAR: The Ultimate Collection (2022-2025)

本项目旨在建立一个 **Pedestrian Attribute Recognition (PAR)** 领域的全景知识库。
核心内容基于 **Event-AHU (安徽大学)** 团队的开源成果，同时收录了 **CVPR / AAAI / TPAMI** 等顶级会议的 SOTA 工作。

> **🚀 Core Framework**: [https://github.com/Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR)

---

## 🗺️ Technical Roadmap (技术演进路线)

本项目记录了 PAR 领域从 2022 到 2025 年的三大技术演进阶段：

### **Phase 1: 基础奠基期 (2022-2023)**
* **核心任务**: 建立强 Baseline，挖掘属性间的逻辑关系。
* **代表技术**:
    * **GCN (图卷积)**: 利用图网络硬编码属性共现关系（如：长发 $\rightarrow$ 女性）。
    * **ViT (Vision Transformer)**: 确立了 Transformer 在 PAR 中的统治地位，取代 CNN。

### **Phase 2: 语义增强期 (2023-2024)**
* **核心痛点**: 纯视觉模型缺乏语义理解，且视频模型显存占用过高。
* **技术突破**:
    * **CLIP + Prompt**: 引入“提示学习”，将属性列表转化为自然语言句子，利用 CLIP 的知识库提升泛化性。
    * **Side-Tuning**: 针对视频 PAR，开发了“侧边微调”技术，冻结大模型，只训练轻量级时序模块。

### **Phase 3: 新范式爆发期 (2025 - Present)**
* **核心趋势**: 追求极致效率（线性复杂度）与解决极端场景（夜间/遮挡）。
* **前沿方向**:
    * **Mamba & RWKV**: 抛弃 Transformer，使用线性复杂度的 SSM 架构，推理速度大幅提升。
    * **RGB-Event**: 首次引入事件相机，利用高频脉冲解决夜间低光和运动模糊问题。
    * **LLM Agent**: 利用大语言模型清洗数据（MSP60K）并增强语义推理。
    * **HyperGraph**: 利用超图建模多部位遮挡关系。

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

## 🛠️ How to Contribute (如何贡献)

欢迎提交 Pull Request 补充更多 2025 年的新工作！
1. Fork 本仓库。
2. 将新论文添加到对应的表格分类中。
3. 提交 PR。
## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)

