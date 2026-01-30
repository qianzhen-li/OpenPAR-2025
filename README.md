# 🌟 OpenPAR 2025: Pedestrian Attribute Recognition Collection

本项目旨在整理 2025 年及近期行人属性识别 (PAR) 领域的最新进展。重点关注 Mamba 架构、CLIP-based 视觉语言融合以及复杂场景下的属性识别。

> **核心代码库 (Base Framework):** > [Event-AHU/OpenPAR](https://github.com/Event-AHU/OpenPAR) (我们主要基于此框架进行复现和扩展)

## 🔥 重点关注 (Highlight)

这里存放我们需要重点研究、复现或魔改的核心论文。

| Paper Title | Year/Venue | Category | Code | Link | 备注 |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion** | 2024/ArXiv | **VL-Fusion** | [Coming Soon](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/html/2312.10692v2)| **(重点)** 基于 CLIP 提示学习，需精读 |
| **An Empirical Study of Mamba-based Pedestrian Attribute Recognition** | 2024/ArXiv | **Mamba** | [Check OpenPAR](https://github.com/Event-AHU/OpenPAR) | [PDF](https://arxiv.org/pdf/2407.10374) | 探索 Mamba 在 PAR 的有效性 |

---

## 📅 2025 论文清单 (Paper List)

### 1. Vision-Language & Prompt (CLIP 相关)
利用大模型知识引导属性识别，解决数据稀缺或语义鸿沟问题。

| 论文名 (Title) | 年限/会议 | 归类 (Category) | Code | Paper | 简述/笔记 |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Pedestrian Attribute Recognition via CLIP based Prompt Vision-Language Fusion** | 2024/ArXiv | Prompt Tuning | - | [Link](https://arxiv.org/abs/xxxx) | 利用 CLIP 融合视觉与文本提示 |
| **GAAP: Cross-modal Generation and Alignment via Attribute-guided Prompt...** | 2023/IJCAI | Text-ReID/PAR | [Link](https://github.com/xxxx) | [Link](https://www.ijcai.org/proceedings/xxxx) | 虽然是 ReID，但其属性引导提示的思想可借鉴 |

### 2. New Architectures (Mamba / Transformer)
探索 CNN 之外的骨干网络。

| 论文名 (Title) | 年限/会议 | 归类 (Category) | Code | Paper | 简述/笔记 |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **An Empirical Study of Mamba-based Pedestrian Attribute Recognition** | 2024/ArXiv | State Space Model | [Official](https://github.com/Event-AHU/OpenPAR) | [Link](https://arxiv.org/abs/xxxx) | 验证 Mamba 相比 ViT 的效率优势 |

### 3. Hard Settings (Occlusion, Low-light)
解决监控环境中的实际困难（遮挡、模糊、低光照）。

| 论文名 (Title) | 年限/会议 | 归类 (Category) | Code | Paper | 简述/笔记 |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Based on Hierarchical Cross-Modal Hypergraph Learning...** | 2024/ArXiv | Hypergraph | - | [Link](https://arxiv.org/abs/xxxx) | **层次化跨模态超图学习**，针对低光照、运动模糊、遮挡场景 |

---

## 📚 经典资源回溯 (Before 2022)
如果你需要查找 2022 年以前的经典 Baseline，请参考：
* [Older Works Collection 1](https://github.com/wangxiao5791509/Pedestrian-Attribute-Recognition-Paper-List)
## 🤝 如何贡献
1. 在 `papers` 文件夹中添加 PDF（可选）。
2. 在 `README.md` 表格中追加新论文。
3. 如果复现了代码，请链接到 `code/` 目录。
