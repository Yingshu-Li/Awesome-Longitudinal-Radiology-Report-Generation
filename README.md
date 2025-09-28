# Awesome Longitudinal Report Generation [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome) <!-- omit in toc -->

## [A Survey of Longitudinal Report Generation]


This is a repository for organizing papers, codes and other resources related to Longitudinal Report Generation, particularly focusing on medical imaging and radiology report generation using temporal data.

Longitudinal Report Generation involves generating textual reports from sequences of medical images taken over time, leveraging temporal information to provide more accurate and comprehensive diagnoses.

## 📖 **The main structure of this survey!**


📂 **Datasets**

Strategies for constructing longitudinal datasets:
- **Modality Composition**: prior images, prior reports, or both  
- **Case Inclusion**: only longitudinal cases vs. mixed  
- **Number of Priors**: single prior vs. multiple temporal priors  
- **Multi-View**: frontal only vs. multi-view (frontal + lateral)  

<p align="center">
  <img src="Dataset.png" alt="TAX" style="display: block; margin: 0 auto;" />
</p>

⚡ **Core Challenges**

Longitudinal report generation introduces unique difficulties that go beyond single-image settings, requiring models to cope with incomplete data, misaligned features, and complex temporal reasoning.  
- **Missing priors** → zero-padding, placeholder tokens, pseudo-priors  
- **Feature misalignment** → contrastive learning across time & modalities  
- **Temporal fusion** → attention, gating, concatenation  
- **Auxiliary modules** → temporal change classification, retrieval-based augmentation, time-gap encoding  

<p align="center">
  <img src="method_tree1.png" alt="TAX" style="display: block; margin: 0 auto;" />
</p>

#### :books: How to read?
The papers are organized by year and methodology approach. Each paper includes links to the original publication and code repository (when available). The papers are listed in chronological order from newest to oldest to track the evolution of the field.

#### :high_brightness: This project is still on-going, pull requests are welcomed!!

If you have any suggestions (missing papers, new papers, key researchers or typos), please feel free to edit and pull a request. Just letting us know the title of papers can also be a great contribution to us.

#### :star: If you find this repo useful, please star it!!!

## Papers

### Longitudinal Method

+ **DDaTR** [Dynamic Difference-aware Temporal Residual Network for Longitudinal Radiology Report Generation](https://arxiv.org/abs/2505.03401) (May 06, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.03401)
  [![Star](https://img.shields.io/github/stars/xmed-lab/ddatr.svg?style=social&label=Star)](https://github.com/xmed-lab/ddatr)

+ **RADAR** [Enhancing Radiology Report Generation with Supplementary Knowledge Injection](https://arxiv.org/abs/2505.14318) (May 20, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.14318)
  [![Star](https://img.shields.io/github/stars/wjhou/Radar.svg?style=social&label=Star)](https://github.com/wjhou/Radar)

+ **MedVersa** [A Generalist Foundation Model for Medical Image Interpretation](https://arxiv.org/pdf/2405.07988) (Jun 10, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2405.07988)

+ **STREAM** [Spatio-Temporal and Retrieval-Augmented Modeling for Chest X-Ray Report Generation](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10938723) (Mar 25, 2025)
  [![IEEE](https://img.shields.io/badge/IEEE-006699.svg)](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10938723)
  [![Star](https://img.shields.io/github/stars/yangyan22/STREAM.svg?style=social&label=Star)](https://github.com/yangyan22/STREAM)

+ **MLRG** [Enhanced Contrastive Learning with Multi-view Longitudinal Data for Chest X-ray Report Generation](https://arxiv.org/abs/2502.20056) (Feb 27, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2502.20056)
  [![Star](https://img.shields.io/github/stars/mk-runner/MLRG.svg?style=social&label=Star)](https://github.com/mk-runner/MLRG)

+ **HC-LLM** [Historical-Constrained Large Language Models for Radiology Report Generation](https://arxiv.org/pdf/2412.11070) (Dec 15, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2412.11070)
  [![Star](https://img.shields.io/github/stars/TengfeiLiu966/HC-LLM.svg?style=social&label=Star)](https://github.com/TengfeiLiu966/HC-LLM)

+ **LLM-RG4** [Flexible and Factual Radiology Report Generation Across Diverse Input Contexts](https://arxiv.org/abs/2412.12001) (Dec 16, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2412.12001)
  [![Star](https://img.shields.io/github/stars/zh-Wang-Med/LLM-RG4.svg?style=social&label=Star)](https://github.com/zh-Wang-Med/LLM-RG4)

+ **Libra** [Leveraging Temporal Images for Biomedical Radiology Analysis](https://arxiv.org/abs/2411.19378v2) (Nov 28, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.19378v2)
  [![Star](https://img.shields.io/github/stars/X-iZhang/Libra.svg?style=social&label=Star)](https://github.com/X-iZhang/Libra)

+ **HIST-AID** [Leveraging Historical Patient Reports for Enhanced Multi-Modal Automatic Diagnosis](https://arxiv.org/abs/2411.10684) (Nov 26, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.10684)
  [![Star](https://img.shields.io/github/stars/NoTody/HIST-AID.svg?style=social&label=Star)](https://github.com/NoTody/HIST-AID)

+ **EVOKE** [Elevating Chest X-ray Report Generation via Multi-View Contrastive Learning and Patient-Specific Knowledge](https://arxiv.org/abs/2411.10224) (Nov 15, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2411.10224)
  [![Star](https://img.shields.io/github/stars/mk-runner/EVOKE.svg?style=social&label=Star)](https://github.com/mk-runner/EVOKE)

+ **TiBiX** [Leveraging Temporal Information for Bidirectional X-Ray and Report Generation](https://link.springer.com/chapter/10.1007/978-3-031-72744-3_17) (Oct 09, 2024)
  [![Springer](https://img.shields.io/badge/Springer-FF6B00.svg)](https://link.springer.com/chapter/10.1007/978-3-031-72744-3_17)
  [![Star](https://img.shields.io/github/stars/BioMedIA-MBZUAI/TiBiX.svg?style=social&label=Star)](https://github.com/BioMedIA-MBZUAI/TiBiX)

+ **MAIRA-2** [Grounded Radiology Report Generation](https://arxiv.org/pdf/2406.04449) (Sep 20, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2406.04449)
  [![Star](https://img.shields.io/github/stars/microsoft/RadFact.svg?style=social&label=Star)](https://github.com/microsoft/RadFact)

+ **M4CXR** [Exploring Multi-task Potentials of Multi-modal Large Language Models for Chest X-ray Interpretation](https://arxiv.org/abs/2408.16213) (Aug 29, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2408.16213)

+ **HERGen** [Elevating Radiology Report Generation with Longitudinal Data](https://arxiv.org/abs/2407.15158) (Jul 21, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2407.15158)
  [![Star](https://img.shields.io/github/stars/HKU-MedAI/HERGen.svg?style=social&label=Star)](https://github.com/HKU-MedAI/HERGen)

+ **LGVT** [Enhancing Radiology Report Generation: The Impact of Locally Grounded Vision and Language Training](https://bmva-archive.org.uk/bmvc/2024/papers/Paper_857/paper.pdf) (2024)
  [![PDF](https://img.shields.io/badge/PDF-EC1C24.svg)](https://bmva-archive.org.uk/bmvc/2024/papers/Paper_857/paper.pdf)

+ **RECAP** [Towards Precise Radiology Report Generation via Dynamic Disease Progression Reasoning](https://arxiv.org/pdf/2310.13864) (Oct 21, 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2310.13864)
  [![Star](https://img.shields.io/github/stars/wjhou/Recap.svg?style=social&label=Star)](https://github.com/wjhou/Recap)

+ **LXRCXR** [Utilizing Longitudinal Chest X-Rays and Reports to Pre-Fill Radiology Reports](https://arxiv.org/abs/2306.08749) (Oct 10, 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2306.08749)
  [![Star](https://img.shields.io/github/stars/CelestialShine/Longitudinal-Chest-X-Ray.svg?style=social&label=Star)](https://github.com/CelestialShine/Longitudinal-Chest-X-Ray)

+ **CCLR** [Controllable Chest X-Ray Report Generation from Longitudinal Representations](https://arxiv.org/pdf/2310.05881) (Oct 09, 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2310.05881)

+ **CXRMate** [Longitudinal Data and a Semantic Similarity Reward for Chest X-Ray Report Generation](https://arxiv.org/abs/2307.09758) (Jul 19, 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2307.09758)
  [![Star](https://img.shields.io/github/stars/aehrc/cxrmate.svg?style=social&label=Star)](https://github.com/aehrc/cxrmate)

+ **BioVil-T** [Learning to Exploit Temporal Structure for Biomedical Vision–Language Processing](https://arxiv.org/pdf/2301.04558) (Mar 16, 2023)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2301.04558)

+ **PriorRG** [Prior-Guided Contrastive Pre-training and Coarse-to-Fine Decoding for Chest X-ray Report Generation](https://arxiv.org/pdf/2508.05353) (Aug 7, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/pdf/2508.05353)
  [![Star](https://img.shields.io/github/stars/mk-runner/PriorRG.svg?style=social&label=Star)](https://github.com/mk-runner/PriorRG)

+ **DPE** [Disease probability-enhanced follow-up chest X-ray radiology report summary generation](https://www.nature.com/articles/s41598-025-12684-2) (Jul 24, 2025)
  [![Paper](https://img.shields.io/badge/Nature-Article-blue)](https://www.nature.com/articles/s41598-025-12684-2)

+ **Diff-RRG** [Longitudinal Disease-Wise Patch Difference as Guidance for LLM-Based Radiology Report Generation](https://link.springer.com/chapter/10.1007/978-3-032-04981-0_15) (Sep 20, 2025)
  [![MICCAI](https://img.shields.io/badge/MICCAI-2025-brightgreen)](https://link.springer.com/chapter/10.1007/978-3-032-04981-0_15)
  [![Star](https://img.shields.io/github/stars/ku-milab/Diff-RRG.svg?style=social&label=Star)](https://github.com/ku-milab/Diff-RRG)

### Longitudinal-related Metrics

+ **Mrscore** [Mrscore: Evaluating radiology report generation with llm-based reward system](https://arxiv.org/abs/2404.17778) (Apr 27, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2404.17778)

+ **Lunguage** [Lunguage: A Benchmark for Structured and Sequential Chest X-ray Interpretation](https://arxiv.org/abs/2505.21190) (May 27, 2025)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2505.21190)

+ **FineRadScore** [FineRadScore: A Radiology Report Line-by-Line Evaluation Technique Generating Corrections with Severity Scores](https://arxiv.org/abs/2405.20613) (May 31, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.20613)

+ **Green** [Green: Generative radiology report evaluation and error notation](https://arxiv.org/abs/2405.20613) (May 6, 2024)
  [![arXiv](https://img.shields.io/badge/arXiv-b31b1b.svg)](https://arxiv.org/abs/2405.20613)
  [![Star](https://img.shields.io/github/stars/Stanford-AIMI/GREEN.svg?style=social&label=Star)](https://github.com/Stanford-AIMI/GREEN)

  
*This list is continuously updated. Please feel free to contribute by opening issues or pull requests!*
