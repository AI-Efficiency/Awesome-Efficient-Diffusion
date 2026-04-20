# Awesome Efficient AIGC [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

This repo collects efficient approaches for large language models (LLMs) and diffusion models (DMs) to cope with the huge demand for computing resources. We are continuously improving the project. Welcome to PR the works (papers, repositories) missed by the repo.
## Table of Contents

  - [Survey](#survey)
  - [Language](#language)
    - [2024](#2024)
    - [2023](#2023)
    - [2022](#2022)
    - [2021](#2021)
    - [2020](#2020)
    - [2019](#2019)
  - [Vision](#vision)
    - [2024](#2024-1)
    - [2023](#2023-1)
 -  [Awesome-Repo](#Awesome-Repo)
  

## Survey

- [[Arxiv](https://arxiv.org/abs/2404.01077)] Efficient Prompting Methods for Large Language Models: A Survey
- [[Arxiv](https://arxiv.org/abs/2404.01077)] Efficient Diffusion Models for Vision: A Survey
- [[Arxiv](https://arxiv.org/abs/2402.01799)] Faster and Lighter LLMs: A Survey on Current Challenges and Way Forward [[code](https://github.com/nyunAI/Faster-LLM-Survey)] ![GitHub Repo stars](https://img.shields.io/github/stars/nyunAI/Faster-LLM-Survey)
- [[Arxiv](https://arxiv.org/abs/2402.13116)] A Survey on Knowledge Distillation of Large Language Models [[code](https://github.com/Tebmer/Awesome-Knowledge-Distillation-of-LLMs)] ![GitHub Repo stars](https://img.shields.io/github/stars/Tebmer/Awesome-Knowledge-Distillation-of-LLMs)
- [[Arxiv](https://arxiv.org/abs/2402.09748)] Model Compression and Efficient Inference for Large Language Models: A Survey
- [[Arxiv](https://arxiv.org/abs/2402.05964)] A Survey on Transformer Compression
- [[Arxiv](https://arxiv.org/abs/2401.15347)] A Comprehensive Survey of Compression Algorithms for Language Models
- [[Arxiv](https://arxiv.org/abs/2401.07851)] Unlocking Efficiency in Large Language Model Inference: A Comprehensive Survey of Speculative Decoding [[code](https://github.com/hemingkx/Spec-Bench)] ![GitHub Repo stars](https://img.shields.io/github/stars/hemingkx/Spec-Bench) [[Blog]](https://sites.google.com/view/spec-bench)
- [[Arxiv](https://arxiv.org/abs/2401.05459)] Personal LLM Agents: Insights and Survey about the Capability, Efficiency and Security [[code](https://github.com/MobileLLM/Personal_LLM_Agents_Survey)] ![GitHub Repo stars](https://img.shields.io/github/stars/MobileLLM/Personal_LLM_Agents_Survey)
- [[Arxiv](https://arxiv.org/abs/2401.09890)] A Survey on Hardware Accelerators for Large Language Models
- [[Arxiv](https://arxiv.org/abs/2401.08092)] A Survey of Resource-efficient LLM and Multimodal Foundation Models [[code](https://github.com/UbiquitousLearning/Efficient_Foundation_Model_Survey)] ![GitHub Repo stars](https://img.shields.io/github/stars/UbiquitousLearning/Efficient_Foundation_Model_Survey)
- [[Arxiv](https://arxiv.org/abs/2401.00625)] Beyond Efficiency: A Systematic Survey of Resource-Efficient Large Language Models [[code](https://github.com/tiingweii-shii/Awesome-Resource-Efficient-LLM-Papers)] ![GitHub Repo stars](https://img.shields.io/github/stars/tiingweii-shii/Awesome-Resource-Efficient-LLM-Papers)
- [[Arxiv](https://arxiv.org/abs/2312.15234)] Towards Efficient Generative Large Language Model Serving: A Survey from Algorithms to Systems
- [[Arxiv](https://arxiv.org/abs/2312.03863)] Efficient Large Language Models: A Survey [[code](https://github.com/AIoT-MLSys-Lab/Efficient-LLMs-Survey)] ![GitHub Repo stars](https://img.shields.io/github/stars/AIoT-MLSys-Lab/Efficient-LLMs-Survey)
- [[Arxiv](https://arxiv.org/abs/2312.00678)] The Efficiency Spectrum of Large Language Models: An Algorithmic Survey [[code](https://github.com/tding1/Efficient-LLM-Survey)] ![GitHub Repo stars](https://img.shields.io/github/stars/tding1/Efficient-LLM-Survey)
- [[Arxiv](https://arxiv.org/abs/2308.07633)] A Survey on Model Compression for Large Language Models
- [[Arxiv](https://arxiv.org/abs/2304.04262)] A Comprehensive Survey on Knowledge Distillation of Diffusion Models
- [[TACL](https://arxiv.org/abs/2002.11985)] Compressing Large-Scale Transformer-Based Models: A Case Study on BERT
- [[JSA](https://www.sciencedirect.com/science/article/abs/pii/S1383762123001698?casa_token=1Hdz_VnQpOIAAAAA:7OGh6gYWawUHYKBZ3biSHaq-F7UaT8-7O2XFbOvK5YTkAuofrm-Fj8KNyHoe3G5wGEJTMWEA4Pnt)] A Survey of Techniques for Optimizing Transformer Inference
- [[Arxiv](https://arxiv.org/abs/2401.02038)] Understanding LLMs: A Comprehensive Overview from Training to Inference

## Language

### 2024

- **[arXiv'26]** OneComp: One-Line Revolution for Generative AI Model Compression. *Ichikawa et al.* [[Paper](https://arxiv.org/abs/2603.28845)] [[Code](https://github.com/FujitsuResearch/OneCompression)]
- **[NeurIPS'25]** Quantization Error Propagation: Revisiting Layer-Wise Post-Training Quantization. *Arai & Ichikawa.* [[Paper](https://openreview.net/forum?id=a3l3K9khbL)] [[Code](https://github.com/FujitsuResearch/OneCompression)]

**Quantization**

- [[arXiv](https://arxiv.org/abs/2404.14047)] How Good Are Low-bit Quantized LLaMA3 Models? An Empirical Study [[code](https://github.com/Macaronlin/LLaMA3-Quantization)]![GitHub Repo stars](https://img.shields.io/github/stars/Macaronlin/LLaMA3-Quantization) [[HuggingFace](https://huggingface.co/LLMQ)]
- [[ArXiv](https://arxiv.org/abs/2402.05445)] Accurate LoRA-Finetuning Quantization of LLMs via Information Retention [[code](https://github.com/htqin/IR-QLoRA)]![GitHub Repo stars](https://img.shields.io/github/stars/htqin/IR-QLoRA)
- [[ArXiv](https://arxiv.org/abs/2402.04291)] BiLLM: Pushing the Limit of Post-Training Quantization for LLMs [[code](https://github.com/Aaronhuang-778/BiLLM)]![GitHub Repo stars](https://img.shields.io/github/stars/Aaronhuang-778/BiLLM)
- [[ArXiv](https://arxiv.org/abs/2402.11960)] DB-LLM: Accurate Dual-Binarization for Efficient LLMs
- [[ArXiv](https://arxiv.org/abs/2401.06118)] Extreme Compression of Large Language Models via Additive Quantization
- [[ArXiv](https://arxiv.org/abs/2401.07159)] Quantized Side Tuning: Fast and Memory-Efficient Tuning of Quantized Large Language Models
- [[ArXiv](https://arxiv.org/abs/2401.14112)] FP6-LLM: Efficiently Serving Large Language Models Through FP6-Centric Algorithm-System Co-Design
- [[ArXiv](https://arxiv.org/abs/2401.18079)] KVQuant: Towards 10 Million Context Length LLM Inference with KV Cache Quantization
- [[ArXiv](https://arxiv.org/abs/2402.10787)] EdgeQAT: Entropy and Distribution Guided Quantization-Aware Training for the Acceleration of Lightweight LLMs on the Edge [[code](https://github.com/shawnricecake/EdgeQAT)] ![GitHub Repo stars](https://img.shields.io/github/stars/shawnricecake/EdgeQAT)
- [[ArXiv](https://arxiv.org/abs/2402.10517)] Any-Precision LLM: Low-Cost Deployment of Multiple, Different-Sized LLMs
- [[ArXiv](https://arxiv.org/abs/2402.02446)] LQER: Low-Rank Quantization Error Reconstruction for LLMs
- [[ArXiv](https://arxiv.org/abs/2402.02750)] KIVI: A Tuning-Free Asymmetric 2bit Quantization for KV Cache [[code](https://github.com/jy-yuan/KIVI)] ![GitHub Repo stars](https://img.shields.io/github/stars/jy-yuan/KIVI)
- [[ArXiv](https://arxiv.org/abs/2402.04396)] QuIP#: Even Better LLM Quantization with Hadamard Incoherence and Lattice Codebooks [[code](https://github.com/Cornell-RelaxML/quip-sharp)] ![GitHub Repo stars](https://img.shields.io/github/stars/Cornell-RelaxML/quip-sharp)
- [[ArXiv](https://arxiv.org/abs/2402.04902)] L4Q: Parameter Efficient Quantization-Aware Training on Large Language Models via LoRA-wise LSQ
- [[ArXiv](https://arxiv.org/abs/2402.04925)] TP-Aware Dequantization
- [[ArXiv](https://arxiv.org/abs/2402.05147)] ApiQ: Finetuning of 2-Bit Quantized Large Language Model
- [[ArXiv](https://arxiv.org/abs/2402.10517)] Any-Precision LLM: Low-Cost Deployment of Multiple, Different-Sized LLMs
- [[ArXiv](https://arxiv.org/abs/2402.10631)] BitDistiller: Unleashing the Potential of Sub-4-Bit LLMs via Self-Distillation [[code](https://github.com/DD-DuDa/BitDistiller)] ![GitHub Repo stars](https://img.shields.io/github/stars/DD-DuDa/BitDistiller)
- [[ArXiv](https://arxiv.org/abs/2402.11295)] OneBit: Towards Extremely Low-bit Large Language Models
- [[ArXiv](https://arxiv.org/abs/2402.12065)] WKVQuant: Quantising Weight and Key/Value Cache for Large Language Models Gains More
- [[ArXiv](https://arxiv.org/abs/2402.15319)] GPTVQ: The Blessing of Dimensionality for LLM Quantization [[code](https://github.com/qualcomm-ai-research/gptvq)] ![GitHub Repo stars](https://img.shields.io/github/stars/qualcomm-ai-research/gptvq)
- [[DAC](https://arxiv.org/abs/2402.14866)] APTQ: Attention-aware Post-Training Mixed-Precision Quantization for Large Language Models
- [[DAC](https://arxiv.org/abs/2402.16775)] A Comprehensive Evaluation of Quantization Strategies for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2402.18096)] No Token Left Behind: Reliable KV Cache Compression via Importance-Aware Mixed Precision Quantization
- [[ArXiv](https://arxiv.org/abs/2402.18158)] Evaluating Quantized Large Language Models
- [[ArXiv](https://arxiv.org/abs/2402.17985)] FlattenQuant: Breaking Through the Inference Compute-bound for Large Language Models with Per-tensor Quantization
- [[ArXiv](https://arxiv.org/abs/2403.01136)] LLM-PQ: Serving LLM on Heterogeneous Clusters with Phase-Aware Partition and Adaptive Quantization
- [[ArXiv](https://arxiv.org/abs/2403.01241)] IntactKV: Improving Large Language Model Quantization by Keeping Pivot Tokens Intact
- [[ArXiv](https://arxiv.org/abs/2403.01384)] On the Compressibility of Quantized Large Language Models
- [[ArXiv](https://arxiv.org/abs/2403.02775)] EasyQuant: An Efficient Data-free Quantization Algorithm for LLMs
- [[ArXiv](https://arxiv.org/abs/2403.04643)] QAQ: Quality Adaptive Quantization for LLM KV Cache [[code](https://github.com/ClubieDong/QAQ-KVCacheQuantization)] ![GitHub Repo stars](https://img.shields.io/github/stars/ClubieDong/QAQ-KVCacheQuantization)
- [[ArXiv](https://arxiv.org/abs/2403.05527)] GEAR: An Efficient KV Cache Compression Recipefor Near-Lossless Generative Inference of LLM
- [[ArXiv](https://arxiv.org/abs/2403.06408)] What Makes Quantization for Large Language Models Hard? An Empirical Study from the Lens of Perturbation
- [[ArXiv](https://arxiv.org/abs/2403.07378)] SVD-LLM: Truncation-aware Singular Value Decomposition for Large Language Model Compression [[code](https://github.com/AIoT-MLSys-Lab/SVD-LLM)] ![GitHub Repo stars](https://img.shields.io/github/stars/AIoT-MLSys-Lab/SVD-LLM)
- [[ICLR](https://browse.arxiv.org/abs/2402.00858)] AffineQuant: Affine Transformation Quantization for Large Language Models [[code](https://github.com/bytedance/AffineQuant)] ![GitHub Repo stars](https://img.shields.io/github/stars/bytedance/AffineQuant)
- [[ICLR Practical ML for Low Resource Settings Workshop](https://arxiv.org/abs/2403.18159)] Oh! We Freeze: Improving Quantized Knowledge Distillation via Signal Propagation Analysis for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2403.20137)] Accurate Block Quantization in LLMs with Outliers
- [[ArXiv](https://arxiv.org/abs/2404.00456)] QuaRot: Outlier-Free 4-Bit Inference in Rotated LLMs [[code](https://github.com/spcl/QuaRot)] ![GitHub Repo stars](https://img.shields.io/github/stars/spcl/QuaRot)
- [[ArXiv](https://arxiv.org/abs/2404.01892)] Minimize Quantization Output Error with Bias Compensation [[code](https://github.com/GongCheng1919/bias-compensation)] ![GitHub Repo stars](https://img.shields.io/github/stars/GongCheng1919/bias-compensation)
- [[ArXiv](https://arxiv.org/abs/2404.02837)] Cherry on Top: Parameter Heterogeneity and Quantization in Large Language Models

**Fine-tuning**

- [[ArXiv](https://arxiv.org/abs/2402.10193)] BitDelta: Your Fine-Tune May Only Be Worth One Bit [[code](https://github.com/FasterDecoding/BitDelta)] ![GitHub Repo stars](https://img.shields.io/github/stars/FasterDecoding/BitDelta)
- [[AAAI EIW Workshop 2024](https://arxiv.org/abs/2402.10462)] QDyLoRA: Quantized Dynamic Low-Rank Adaptation for Efficient Large Language Model Tuning

**Other**

- [[ArXiv](https://arxiv.org/abs/2401.03868)] FlightLLM: Efficient Large Language Model Inference with a Complete Mapping Flow on FPGA
- [[ArXiv](https://arxiv.org/abs/2401.08294)] Inferflow: an Efficient and Highly Configurable Inference Engine for Large Language Models

### 2023

**Quantization**

- [[ICLR](https://arxiv.org/abs/2210.17323)] GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers [[code](https://github.com/IST-DASLab/gptq)] ![GitHub Repo stars](https://img.shields.io/github/stars/IST-DASLab/gptq)
- [[NeurIPS](https://nips.cc/virtual/2023/oral/73855)] QLORA: Efficient Finetuning of Quantized LLMs [[code](https://github.com/artidoro/qlora)] ![GitHub Repo stars](https://img.shields.io/github/stars/artidoro/qlora)
- [[NeurIPS](https://nips.cc/virtual/2023/poster/72931)] Memory-Efficient Fine-Tuning of Compressed Large Language Models via sub-4-bit Integer Quantization
- [[ICML](https://browse.arxiv.org/abs/2211.10438)] SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models [[code](https://github.com/mit-han-lab/smoothquant)] ![GitHub Repo stars](https://img.shields.io/github/stars/mit-han-lab/smoothquant)
- [[ICML](https://arxiv.org/abs/2306.00317)] FlexRound: Learnable Rounding based on Element-wise Division for Post-Training Quantization [[code](https://openreview.net/attachment?id=-tYCaP0phY_&name=supplementary_material)]
- [[ICML](https://arxiv.org/abs/2301.12017)] Understanding INT4 Quantization for Transformer Models: Latency Speedup, Composability, and Failure Cases [[code](https://github.com/microsoft/DeepSpeed)] ![GitHub Repo stars](https://img.shields.io/github/stars/microsoft/DeepSpeed)
- [[ICML](https://icml.cc/virtual/2023/28295)] GPT-Zip: Deep Compression of Finetuned Large Language Models
- [[ICML](https://arxiv.org/abs/2307.03738)] QIGen: Generating Efficient Kernels for Quantized Inference on Large Language Models [[code](https://github.com/IST-DASLab/QIGen)] ![GitHub Repo stars](https://img.shields.io/github/stars/IST-DASLab/QIGen)
- [[ICML](https://icml.cc/virtual/2023/poster/23915)] The case for 4-bit precision: k-bit Inference Scaling Laws
- [[ACL](https://arxiv.org/abs/2306.00014)] PreQuant: A Task-agnostic Quantization Approach for Pre-trained Language Models
- [[ACL](https://aclanthology.org/2023.findings-acl.15/)] Boost Transformer-based Language Models with GPU-Friendly Sparsity and Quantization
- [[EMNLP](https://arxiv.org/abs/2310.05079)] Revisiting Block-based Quantisation: What is Important for Sub-8-bit LLM Inference?
- [[EMNLP](https://arxiv.org/abs/2310.13315)] Zero-Shot Sharpness-Aware Quantization for Pre-trained Language Models
- [[EMNLP](https://arxiv.org/abs/2310.16836)] LLM-FP4: 4-Bit Floating-Point Quantized Transformers [[code](https://github.com/nbasyl/LLM-FP4)] ![GitHub Repo stars](https://img.shields.io/github/stars/nbasyl/LLM-FP4)
- [[EMNLP](https://arxiv.org/abs/2304.09145)] Outlier Suppression+: Accurate quantization of large language models by equivalent and optimal shifting and scaling
- [[ISCA](https://dl.acm.org/doi/abs/10.1145/3579371.3589038)] OliVe: Accelerating Large Language Models via Hardware-friendly Outlier-Victim Pair Quantization
- [[ArXiv](https://arxiv.org/abs/2303.08302)] ZeroQuant-V2: Exploring Post-training Quantization in LLMs from Comprehensive Study to Low Rank Compensation
- [[ArXiv](https://arxiv.org/abs/2206.09557)] LUT-GEMM: Quantized Matrix Multiplication based on LUTs for Efficient Inference in Large-Scale Generative Language Models
- [[ArXiv](https://arxiv.org/abs/2302.02390)] Quantized Distributed Training of Large Models with Convergence Guarantees
- [[ArXiv](https://arxiv.org/abs/2305.17888)] LLM-QAT: Data-Free Quantization Aware Training for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2306.00978)] AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration [[code](https://github.com/mit-han-lab/llm-awq)] ![GitHub Repo stars](https://img.shields.io/github/stars/mit-han-lab/llm-awq)
- [[ArXiv](https://arxiv.org/abs/2306.11987)] Training Transformers with 4-bit Integers [[code](https://github.com/xijiu9/Train_Transformers_with_INT4)] ![GitHub Repo stars](https://img.shields.io/github/stars/xijiu9/Train_Transformers_with_INT4)
- [[ArXiv](https://arxiv.org/abs/2306.07629)] SqueezeLLM: Dense-and-Sparse Quantization [[code](https://github.com/SqueezeAILab/SqueezeLLM)] ![GitHub Repo stars](https://img.shields.io/github/stars/SqueezeAILab/SqueezeLLM)
- [[ArXiv](https://arxiv.org/abs/2306.12929)] Quantizable Transformers: Removing Outliers by Helping Attention Heads Do Nothing
- [[ArXiv](https://arxiv.org/abs/2306.03078)] SpQR: A Sparse-Quantized Representation for Near-Lossless LLM Weight Compression [[code](https://github.com/Vahe1994/SpQR)] ![GitHub Repo stars](https://img.shields.io/github/stars/Vahe1994/SpQR)
- [[ArXiv](https://arxiv.org/abs/2307.13304)] QuIP: 2-Bit Quantization of Large Language Models With Guarantees [[code](https://github.com/jerry-chee/QuIP)] ![GitHub Repo stars](https://img.shields.io/github/stars/jerry-chee/QuIP)
- [[ArXiv](https://arxiv.org/abs/2306.02272)] OWQ: Lessons learned from activation outliers for weight quantization in large language models
- [[ArXiv](https://arxiv.org/abs/2308.13137)] OmniQuant: Omnidirectionally Calibrated Quantization for Large Language Models [[code](https://github.com/OpenGVLab/OmniQuant)] ![GitHub Repo stars](https://img.shields.io/github/stars/OpenGVLab/OmniQuant)
- [[ArXiv](https://arxiv.org/abs/2304.01089)] RPTQ: Reorder-based Post-training Quantization for Large Language Models [[code](https://github.com/hahnyuan/RPTQ4LLM)] ![GitHub Repo stars](https://img.shields.io/github/stars/hahnyuan/RPTQ4LLM)
- [[ArXiv](https://arxiv.org/abs/2305.12356)] Integer or Floating Point? New Outlooks for Low-Bit Quantization on Large Language Models
- [[ArXiv](https://arxiv.org/abs/2306.08162)] INT2.1: Towards Fine-Tunable Quantized Large Language Models with Error Correction through Low-Rank Adaptation
- [[ArXiv](https://arxiv.org/abs/2307.03712)] INT-FP-QSim: Mixed Precision and Formats For Large Language Models and Vision Transformers [[code](https://github.com/lightmatter-ai/INT-FP-QSim)] ![GitHub Repo stars](https://img.shields.io/github/stars/lightmatter-ai/INT-FP-QSim)
- [[ArXiv](https://arxiv.org/abs/2307.08072)] Do Emergent Abilities Exist in Quantized Large Language Models: An Empirical Study
- [[ArXiv](https://arxiv.org/abs/2307.09782)] ZeroQuant-FP: A Leap Forward in LLMs Post-Training W4A8 Quantization Using Floating-Point Formats
- [[ArXiv](https://arxiv.org/abs/2308.05600)] NUPES : Non-Uniform Post-Training Quantization via Power Exponent Search
- [[ArXiv](https://arxiv.org/abs/2308.06744)] Token-Scaled Logit Distillation for Ternary Weight Generative Language Models
- [[ArXiv](https://arxiv.org/abs/2308.07662)] Gradient-Based Post-Training Quantization: Challenging the Status Quo
- [[ArXiv](https://arxiv.org/abs/2308.09723)] FineQuant: Unlocking Efficiency with Fine-Grained Weight-Only Quantization for LLMs
- [[ArXiv](https://arxiv.org/abs/2308.14903)] MEMORY-VQ: Compression for Tractable Internet-Scale Memory
- [[ArXiv](https://arxiv.org/abs/2308.15987)] FPTQ: Fine-grained Post-Training Quantization for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2309.00964)] eDKM: An Efficient and Accurate Train-time Weight Clustering for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2309.01885)] QuantEase: Optimization-based Quantization for Language Models - An Efficient and Intuitive Algorithm
- [[ArXiv](https://arxiv.org/abs/2309.02784)] Norm Tweaking: High-performance Low-bit Quantization of Large Language Models
- [[ArXiv](https://arxiv.org/abs/2309.05210)] Understanding the Impact of Post-Training Quantization on Large Language Models
- [[ArXiv](https://arxiv.org/abs/2309.05516)] Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs [[code](https://github.com/intel/neural-compressor)] ![GitHub Repo stars](https://img.shields.io/github/stars/intel/neural-compressor)
- [[ArXiv](https://arxiv.org/abs/2309.14592)] Efficient Post-training Quantization with FP8 Formats [[code](https://github.com/intel/neural-compressor)] ![GitHub Repo stars](https://img.shields.io/github/stars/intel/neural-compressor)
- [[ArXiv](https://arxiv.org/abs/2309.14717)] QA-LoRA: Quantization-Aware Low-Rank Adaptation of Large Language Models [[code](https://github.com/yuhuixu1993/qa-lora)] ![GitHub Repo stars](https://img.shields.io/github/stars/yuhuixu1993/qa-lora)
- [[ArXiv](https://arxiv.org/abs/2309.15531)] Rethinking Channel Dimensions to Isolate Outliers for Low-bit Weight Quantization of Large Language Models
- [[ArXiv](https://arxiv.org/abs/2309.16119)] ModuLoRA: Finetuning 3-Bit LLMs on Consumer GPUs by Integrating with Modular Quantizers
- [[ArXiv](https://arxiv.org/abs/2310.00034)] PB-LLM: Partially Binarized Large Language Models [[code](https://github.com/hahnyuan/BinaryLLM)] ![GitHub Repo stars](https://img.shields.io/github/stars/hahnyuan/BinaryLLM)
- [[ArXiv](https://arxiv.org/abs/2310.04836)] Dual Grained Quantization: Efficient Fine-Grained Quantization for LLM
- [[ArXiv](https://arxiv.org/abs/2310.07147)] QFT: Quantized Full-parameter Tuning of LLMs with Affordable Resources
- [[ArXiv](https://arxiv.org/abs/2310.08041)] QLLM: Accurate and Efficient Low-Bitwidth Quantization for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2310.08659)] LoftQ: LoRA-Fine-Tuning-Aware Quantization for Large Language Models [[code](https://github.com/yxli2123/LoftQ)] ![GitHub Repo stars](https://img.shields.io/github/stars/yxli2123/LoftQ)
- [[ArXiv](https://arxiv.org/abs/2310.10944)] TEQ: Trainable Equivalent Transformation for Quantization of LLMs [[code](https://github.com/intel/neural-compressor)] ![GitHub Repo stars](https://img.shields.io/github/stars/intel/neural-compressor)
- [[ArXiv](https://arxiv.org/abs/2310.11453)] BitNet: Scaling 1-bit Transformers for Large Language Models [[code](https://github.com/kyegomez/BitNet)] ![GitHub Repo stars](https://img.shields.io/github/stars/kyegomez/BitNet)
- [[ArXiv](https://arxiv.org/abs/2310.18313)] FP8-LM: Training FP8 Large Language Models [[code](https://github.com/Azure/MS-AMP)] ![GitHub Repo stars](https://img.shields.io/github/stars/Azure/MS-AMP)
- [[ArXiv](https://arxiv.org/abs/2310.19102)] Atom: Low-bit Quantization for Efficient and Accurate LLM Serving [[code](https://github.com/efeslab/Atom)] ![GitHub Repo stars](https://img.shields.io/github/stars/efeslab/Atom)
- [[ArXiv](https://arxiv.org/abs/2310.08659)] LoftQ: LoRA-Fine-Tuning-Aware Quantization for Large Language Models [[code](https://github.com/yxli2123/LoftQ)] ![GitHub Repo stars](https://img.shields.io/github/stars/yxli2123/LoftQ)
- [[ArXiv](https://arxiv.org/abs/2311.01305)] AWEQ: Post-Training Quantization with Activation-Weight Equalization for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2311.01792)] AFPQ: Asymmetric Floating Point Quantization for LLMs [[code](https://github.com/zhangsichengsjtu/AFPQ)] ![GitHub Repo stars](https://img.shields.io/github/stars/zhangsichengsjtu/AFPQ)
- [[ArXiv](https://arxiv.org/abs/2311.12023)] LQ-LoRA: Low-rank Plus Quantized Matrix Decomposition for Efficient Language Model Finetuning [[code](https://github.com/HanGuo97/lq-lora)] ![GitHub Repo stars](https://img.shields.io/github/stars/HanGuo97/lq-lora)


**Pruning and Sparsity**

- [[ICML](https://icml.cc/virtual/2023/oral/25453)] Deja Vu: Contextual Sparsity for Efficient LLMs at Inference Time [[code](https://github.com/FMInference/DejaVu)] ![GitHub Repo stars](https://img.shields.io/github/stars/FMInference/DejaVu)
- [[ICML](https://arxiv.org/abs/2301.00774)] SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot [[code](https://github.com/IST-DASLab/sparsegpt)] ![GitHub Repo stars](https://img.shields.io/github/stars/IST-DASLab/sparsegpt)
- [[ICML](https://arxiv.org/abs/2306.11222)] LoSparse: Structured Compression of Large Language Models based on Low-Rank and Sparse Approximation [[code](https://github.com/yxli2123/LoSparse)] ![GitHub Repo stars](https://img.shields.io/github/stars/yxli2123/LoSparse)
- [[ICML](https://arxiv.org/abs/2306.11695)] A Simple and Effective Pruning Approach for Large Language Models [[code](https://github.com/locuslab/wanda)] ![GitHub Repo stars](https://img.shields.io/github/stars/locuslab/wanda)
- [[ICLR](https://arxiv.org/abs/2210.06313)] The Lazy Neuron Phenomenon: On Emergence of Activation Sparsity in Transformers [[code](https://github.com/IST-DASLab/gptq)] ![GitHub Repo stars](https://img.shields.io/github/stars/IST-DASLab/gptq)
- [[ICLR](https://openreview.net/forum?id=cKlgcx7nSZ)] Prune and Tune: Improving Efficient Pruning Techniques for Massive Language Models
- [[NeurIPS](https://arxiv.org/abs/2305.14314)] Outlier Suppression: Pushing the Limit of Low-bit Transformer Language Models [[code](https://github.com/wimh966/outlier_suppression)] ![GitHub Repo stars](https://img.shields.io/github/stars/wimh966/outlier_suppression)
- [[NeurIPS](https://arxiv.org/abs/2305.11627)] LLM-Pruner: On the Structural Pruning of Large Language Models [[code](https://github.com/horseee/LLM-Pruner)] ![GitHub Repo stars](https://img.shields.io/github/stars/horseee/LLM-Pruner)
- [[ACL](https://aclanthology.org/2023.findings-acl.15/)] Boost Transformer-based Language Models with GPU-Friendly Sparsity and Quantization
- [[AutoML](https://openreview.net/forum?id=SHlZcInS6C)] Structural Pruning of Large Language Models via Neural Architecture Search
- [[VLDB](https://arxiv.org/abs/2309.10285)] Flash-LLM: Enabling Cost-Effective and Highly-Efficient Large Generative Model Inference with Unstructured Sparsity [[code](https://github.com/AlibabaResearch/flash-llm)] ![GitHub Repo stars](https://img.shields.io/github/stars/AlibabaResearch/flash-llm)
- [[ArXiv](https://arxiv.org/abs/2302.03773)] What Matters In The Structured Pruning of Generative Language Models?
- [[ArXiv](https://arxiv.org/abs/2305.18403)] LoRAPrune: Pruning Meets Low-Rank Parameter-Efficient Fine-Tuning
- [[ArXiv](https://arxiv.org/abs/2306.03078)] SpQR: A Sparse-Quantized Representation for Near-Lossless LLM Weight Compression [[code](https://github.com/Vahe1994/SpQR)] ![GitHub Repo stars](https://img.shields.io/github/stars/Vahe1994/SpQR)
- [[ArXiv](https://arxiv.org/abs/2306.07629)] SqueezeLLM: Dense-and-Sparse Quantization [[code](https://github.com/SqueezeAILab/SqueezeLLM)] ![GitHub Repo stars](https://img.shields.io/github/stars/SqueezeAILab/SqueezeLLM)
- [[ArXiv](https://arxiv.org/abs/2309.09507)] Pruning Large Language Models via Accuracy Predictor
- [[ArXiv](https://arxiv.org/abs/2310.06694)] Sheared LLaMA: Accelerating Language Model Pre-training via Structured Pruning [[code](https://github.com/princeton-nlp/LLM-Shearing)] ![GitHub Repo stars](https://img.shields.io/github/stars/princeton-nlp/LLM-Shearing)
- [[ArXiv](https://arxiv.org/abs/2310.05175)] Outlier Weighed Layerwise Sparsity (OWL): A Missing Secret Sauce for Pruning LLMs to High Sparsity [[code](https://github.com/luuyin/OWL)] ![GitHub Repo stars](https://img.shields.io/github/stars/luuyin/OWL)
- [[ArXiv](https://arxiv.org/abs/2310.02277)] Junk DNA Hypothesis: A Task-Centric Angle of LLM Pre-trained Weights through Sparsity [[code](https://github.com/VITA-Group/Junk_DNA_Hypothesis)] ![GitHub Repo stars](https://img.shields.io/github/stars/VITA-Group/Junk_DNA_Hypothesis)
- [[ArXiv](https://arxiv.org/abs/2310.05015)] Compresso: Structured Pruning with Collaborative Prompting Learns Compact Large Language Models [[code](https://github.com/microsoft/Moonlit/tree/main/Compresso)] ![GitHub Repo stars](https://img.shields.io/github/stars/microsoft/Moonlit)
- [[ArXiv](https://arxiv.org/abs/2310.08915)] Dynamic Sparse No Training: Training-Free Fine-tuning for Sparse LLMs [[code](https://github.com/zyxxmu/DSnoT)] ![GitHub Repo stars](https://img.shields.io/github/stars/zyxxmu/DSnoT)
- [[ArXiv](https://arxiv.org/abs/2310.09499)] One-Shot Sensitivity-Aware Mixed Sparsity Pruning for Large Language Models
- [[ArXiv](https://arxiv.org/abs/2310.15929)] E-Sparse: Boosting the Large Language Model Inference through Entropy-based N:M Sparsity
- [[ArXiv](https://arxiv.org/abs/2310.18356)] LoRAShear: Efficient Large Language Model Structured Pruning and Knowledge Recovery [[code](https://github.com/microsoft/lorashear)]

**Distillation**

- [[ACL](https://aclanthology.org/2023.acl-long.150/)] Symbolic Chain-of-Thought Distillation: Small Models Can Also "Think" Step-by-Step [[code](https://github.com/allenai/cot_distillation)]
- [[ACL](https://aclanthology.org/2023.acl-long.249/)] Lifting the Curse of Capacity Gap in Distilling Language Models [[code](https://github.com/GeneZC/MiniMoE)]
- [[ACL](https://aclanthology.org/2023.acl-long.302/)] DISCO: Distilling Counterfactuals with Large Language Models [[code](https://github.com/eric11eca/disco)]
- [[ACL](https://aclanthology.org/2023.acl-long.304/)] SCOTT: Self-Consistent Chain-of-Thought Distillation [[code](https://github.com/wangpf3/consistent-CoT-distillation)]
- [[ACL](https://aclanthology.org/2023.acl-long.471/)] AD-KD: Attribution-Driven Knowledge Distillation for Language Model Compression
- [[ACL](https://aclanthology.org/2023.acl-long.830/)] Large Language Models Are Reasoning Teachers [[code](https://github.com/itsnamgyu/reasoning-teacher)]
- [[ACL](https://aclanthology.org/2023.findings-acl.441/)] Distilling Reasoning Capabilities into Smaller Language Models
- [[ACL](https://aclanthology.org/2023.findings-acl.463/)] Cost-effective Distillation of Large Language Models [[code](https://github.com/Sayan21/MAKD)]
- [[ACL](https://aclanthology.org/2023.findings-acl.507/)] Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes [[code](https://github.com/google-research/distilling-step-by-step)]
- [[EMNLP](https://arxiv.org/abs/2310.13332)] Democratizing Reasoning Ability: Tailored Learning from Large Language Model [[code](https://github.com/Raibows/Learn-to-Reason)]
- [[EMNLP](https://arxiv.org/abs/2310.14192)] PromptMix: A Class Boundary Augmentation Method for Large Language Model Distillation [[code](https://github.com/ServiceNow/PromptMix-EMNLP-2023)]
- [[EMNLP](https://arxiv.org/abs/2310.14747)] MCC-KD: Multi-CoT Consistent Knowledge Distillation
- [[EMNLP](https://arxiv.org/abs/2311.05161)] Enhancing Computation Efficiency in Large Language Models through Weight and Activation Quantization
- [[ArXiv](https://arxiv.org/abs/2304.14402)] LaMini-LM: A Diverse Herd of Distilled Models from Large-Scale Instructions [[code](https://github.com/mbzuai-nlp/LaMini-LM)]
- [[ArXiv](https://arxiv.org/abs/2305.12330)] Task-agnostic Distillation of Encoder-Decoder Language Models
- [[ArXiv](https://arxiv.org/abs/2305.12870)] Lion: Adversarial Distillation of Closed-Source Large Language Model [[code](https://github.com/YJiangcm/Lion)]
- [[ArXiv](https://arxiv.org/abs/2305.13888)] PaD: Program-aided Distillation Specializes Large Models in Reasoning
- [[ArXiv](https://arxiv.org/abs/2305.14864)] Large Language Model Distillation Doesn't Need a Teacher
 [[code](https://github.com/ananyahjha93/llm-distill)]
- [[ArXiv](https://arxiv.org/abs/2305.15717)] The False Promise of Imitating Proprietary LLMs
- [[ArXiv](https://arxiv.org/abs/2306.08543)] Knowledge Distillation of Large Language Models [[code](https://github.com/microsoft/LMOps/tree/main/minillm)]
- [[ArXiv](https://arxiv.org/abs/2306.13649)] GKD: Generalized Knowledge Distillation for Auto-regressive Sequence Models
- [[ArXiv](https://arxiv.org/abs/2306.14122)] Chain-of-Thought Prompt Distillation for Multimodal Named Entity Recognition and Multimodal Relation Extraction
- [[ArXiv](https://arxiv.org/abs/2308.04679)] Sci-CoT: Leveraging Large Language Models for Enhanced Knowledge Distillation in Small Models for Scientific QA
- [[ArXiv](https://arxiv.org/abs/2308.06744)] Token-Scaled Logit Distillation for Ternary Weight Generative Language Models
- [[ArXiv](https://arxiv.org/abs/2310.02421)] Can a student Large Language Model perform as well as it's teacher?
- [[ArXiv](https://arxiv.org/abs/2311.09550)] A Speed Odyssey for Deployable Quantization of LLMs
- [[ArXiv](https://arxiv.org/abs/2311.09755)] How Does Calibration Data Affect the Post-training Pruning and Quantization of Large Language Models?

**Fine-tuning**

- [[Nature](https://www.nature.com/articles/s42256-023-00626-4)] Parameter-efficient fine-tuning of large-scale pre-trained language models [[code](https://github.com/thunlp/OpenDelta)]
- [[NeurIPS](https://nips.cc/virtual/2023/oral/73855)] QLORA: Efficient Finetuning of Quantized LLMs [[code](https://github.com/artidoro/qlora)]
- [[NeurIPS](https://neurips.cc/virtual/2023/poster/72073)] Make Pre-trained Model Reversible: From Parameter to Memory Efficient Fine-Tuning [[code](https://github.com/BaohaoLiao/mefts)]
- [[ACL](https://aclanthology.org/2023.acl-long.830/)] Large Language Models Are Reasoning Teachers [[code](https://github.com/itsnamgyu/reasoning-teacher)]
- [[ArXiv](https://arxiv.org/abs/2305.18403)] LoRAPrune: Pruning Meets Low-Rank Parameter-Efficient Fine-Tuning
- [[ArXiv](https://arxiv.org/abs/2305.14152)] Memory-Efficient Fine-Tuning of Compressed Large Language Models via sub-4-bit Integer Quantization
- [[ArXiv](https://arxiv.org/abs/2306.08162)] INT2.1: Towards Fine-Tunable Quantized Large Language Models with Error Correction through Low-Rank Adaptation
- [[ArXiv](https://arxiv.org/abs/2309.12307)] LongLoRA: Efficient Fine-tuning of Long-Context Large Language Models [[code](https://github.com/dvlab-research/LongLoRA)]
- [[ArXiv](https://arxiv.org/abs/2309.14717)] QA-LoRA: Quantization-Aware Low-Rank Adaptation of Large Language Models [[code](https://github.com/yuhuixu1993/qa-lora)]
- [[ArXiv](https://arxiv.org/abs/2309.16119)] ModuLoRA: Finetuning 3-Bit LLMs on Consumer GPUs by Integrating with Modular Quantizers
- [[ArXiv](https://arxiv.org/abs/2310.07147)] QFT: Quantized Full-parameter Tuning of LLMs with Affordable Resources
- [[ArXiv](https://arxiv.org/abs/2310.08659)] LoftQ: LoRA-Fine-Tuning-Aware Quantization for Large Language Models [[code](https://github.com/yxli2123/LoftQ)]
- [[ArXiv](https://arxiv.org/abs/2311.03285)] S-LoRA: Serving Thousands of Concurrent LoRA Adapters [[code](https://github.com/S-LoRA/S-LoRA)]
- [[ArXiv](https://arxiv.org/abs/2311.12023)] LQ-LoRA: Low-rank Plus Quantized Matrix Decomposition for Efficient Language Model Finetuning [[code](https://github.com/HanGuo97/lq-lora)]

**Other**

- [[ACL](https://aclanthology.org/2023.acl-long.172/)] Did You Read the Instructions? Rethinking the Effectiveness of Task Definitions in Instruction Learning [[code](https://github.com/fanyin3639/Rethinking-instruction-effectiveness)]
- [[EMNLP](https://arxiv.org/abs/2305.14788)] Adapting Language Models to Compress Contexts [[code](https://github.com/princeton-nlp/AutoCompressors)]
- [[EMNLP](https://arxiv.org/abs/2310.05736)] LLMLingua: Compressing Prompts for Accelerated Inference of Large Language Models [[code](https://aka.ms/LLMLingua)]
- [[EMNLP](https://arxiv.org/abs/2310.06201)] Compressing Context to Enhance Inference Efficiency of Large Language Models [[code](https://github.com/)]
- [[EMNLP](https://arxiv.org/abs/2301.08721)] Batch Prompting: Efficient Inference with Large Language Model APIs [[code](https://github.com/xlang-ai/batch-prompting)]
- [[ArXiv](https://arxiv.org/abs/2304.08467
)] Learning to Compress Prompts with Gist Tokens [[code](https://github.com/jayelm/gisting)]
- [[ArXiv](https://arxiv.org/abs/2305.11170)] Efficient Prompting via Dynamic In-Context Learning
- [[ArXiv](https://arxiv.org/abs/2305.11186)] Compress, Then Prompt: Improving Accuracy-Efficiency Trade-off of LLM Inference with Transferable Prompt
- [[ArXiv](https://arxiv.org/abs/2307.06945)] In-context Autoencoder for Context Compression in a Large Language Model [[code](https://github.com/getao/icae)]
- [[ArXiv](https://arxiv.org/abs/2308.08758)] Discrete Prompt Compression with Reinforcement Learning
- [[ArXiv](https://arxiv.org/abs/2309.00384)] BatchPrompt: Accomplish more with less
- [[ArXiv](https://arxiv.org/abs/2310.00867)] (Dynamic) Prompting might be all you need to repair Compressed LLMs
- [[ArXiv](https://arxiv.org/abs/2310.01801)] Model Tells You What to Discard: Adaptive KV Cache Compression for LLMs
- [[ArXiv](https://arxiv.org/abs/2310.04408)] RECOMP: Improving Retrieval-Augmented LMs with Compression and Selective Augmentation [[code](https://github.com/carriex/recomp)]
- [[ArXiv](https://arxiv.org/abs/2310.05869)] HyperAttention: Long-context Attention in Near-Linear Time
- [[ArXiv](https://arxiv.org/abs/2310.06839)] LongLLMLingua: Accelerating and Enhancing LLMs in Long Context Scenarios via Prompt Compression [[code](https://aka.ms/LLMLingua)]

### 2022

**Quantization**

- [[ACL](https://aclanthology.org/2022.acl-long.331)] Compression of Generative Pre-trained Language Models via Quantization
- [[NeurIPS](https://arxiv.org/abs/2208.07339)] LLM.int8(): 8-bit Matrix Multiplication for Transformers at Scale
- [[NeurIPS](https://nips.cc/Conferences/2022/Schedule?showEvent=53407)] Towards Efficient Post-training Quantization of Pre-trained Language Models
- [[NeurIPS](https://nips.cc/Conferences/2022/Schedule?showEvent=54407)] ZeroQuant: Efficient and Affordable Post-Training Quantization for Large-Scale Transformers
- [[NeurIPS](https://nips.cc/Conferences/2022/Schedule?showEvent=55032)] BiT: Robustly Binarized Multi-distilled Transformer [[code](https://github.com/facebookresearch/bit)]
- [[ICLR](https://openreview.net/forum?id=5xEgrl_5FAJ)] BiBERT: Accurate Fully Binarized BERT [[code](https://github.com/htqin/BiBERT)]

**Distillation**

- [[ArXiv](https://arxiv.org/abs/2210.06726)] Explanations from Large Language Models Make Small Reasoners Better
- [[ArXiv](https://arxiv.org/abs/2212.10670)] In-context Learning Distillation: Transferring Few-shot Learning Ability of Pre-trained Language Models

**Fine-tuning**

- [[ACL](https://aclanthology.org/2023.acl-demo.54/)] Petals: Collaborative Inference and Fine-tuning of Large Models [[code](https://petals.ml/)]

**Other**

- [[ICML](https://proceedings.mlr.press/v162/liu22v.html)] GACT: Activation Compressed Training for Generic Network Architectures

### 2021

**Quantization**

- [[ICML](https://proceedings.mlr.press/v139/kim21d.html)] I-BERT: Integer-only BERT Quantization
- [[ACL](https://aclanthology.org/2021.acl-long.334/)] BinaryBERT: Pushing the Limit of BERT Quantization

**Pruning and Sparsity**

- [[ACL](https://aclanthology.org/2021.findings-acl.363)] On the Distribution, Sparsity, and Inference-time Quantization of Attention Values in Transformers

**Distillation**

- [[ACL](https://aclanthology.org/2021.findings-acl.387/)] One Teacher is Enough? Pre-trained Language Model Distillation from Multiple Teachers

### 2020

**Quantization**

- [[EMNLP](https://arxiv.org/abs/1910.10485)] Fully Quantized Transformer for Machine Translation
- [[IJCAI](https://www.ijcai.org/Proceedings/2020/0520.pdf)] Towards Fully 8-bit Integer Inference for the Transformer Model
- [[EMNLP](https://arxiv.org/abs/2009.12812)] TernaryBERT: Distillation-aware Ultra-low Bit BERT
- [[AAAI](https://arxiv.org/abs/1909.05840)] Q-BERT: Hessian Based Ultra Low Precision Quantization of BERT
- [[MICRO](http://arxiv.org/abs/2005.03842)] GOBO: Quantizing Attention-Based NLP Models for Low Latency and Energy Efficient Inference

**Pruning and Sparsity**

- [[ACL](https://arxiv.org/abs/2002.08307)] Compressing bert: Studying the effects of weight pruning on transfer learning

**Distillation**

- [[ICLR](https://arxiv.org/abs/1909.11687v1)] Extreme Language Model Compression with Optimal Subwords and Shared Projections

### 2019

**Quantization**

- [[ICML](https://arxiv.org/abs/1906.00532v2)] Efficient 8-Bit Quantization of Transformer Neural Machine Language Translation Model
- [[NeurIPS](https://www.emc2-ai.org/assets/docs/neurips-19/emc2-neurips19-paper-31.pdf)] Q8BERT: Quantized 8Bit BERT
- [[NeurIPS](https://www.emc2-ai.org/assets/docs/neurips-19/emc2-neurips19-paper-36.pdf)] Fully Quantized Transformer for Improved Translation

**Distillation**

- [[NeurIPS](https://arxiv.org/abs/1910.01108)] DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter

## Vision

### 2024

**Quantization**

- [[ArXiv](https://arxiv.org/abs/2404.05662)] BinaryDM: Towards Accurate Binarization of Diffusion Model [[code](https://github.com/Xingyu-Zheng/BinaryDM)]![GitHub Repo stars](https://img.shields.io/github/stars/Xingyu-Zheng/BinaryDM)

### 2023

**Quantization**

- [[ICLR](https://openreview.net/forum?id=3itjR9QxFw)] Analog Bits: Generating Discrete Data using Diffusion Models with Self-Conditioning
- [[CVPR](https://openaccess.thecvf.com/content/CVPR2023/papers/Shang_Post-Training_Quantization_on_Diffusion_Models_CVPR_2023_paper.pdf)] Post-training Quantization on Diffusion Models [[code](https://github.com/42Shawn/PTQ4DM)] ![GitHub Repo stars](https://img.shields.io/github/stars/42Shawn/PTQ4DM)
- [[CVPR](https://arxiv.org/abs/2303.06424)] Regularized Vector Quantization for Tokenized Image Synthesis
- [[ICCV](https://arxiv.org/abs/2302.04304)] Q-Diffusion: Quantizing Diffusion Models [[code](https://github.com/Xiuyu-Li/q-diffusion)] ![GitHub Repo stars](https://img.shields.io/github/stars/Xiuyu-Li/q-diffusion)
- [[NeurIPS](https://neurips.cc/virtual/2023/poster/70279)] Q-DM: An Efficient Low-bit Quantized Diffusion Model
- [[NeurIPS](https://neurips.cc/virtual/2023/poster/71314)] PTQD: Accurate Post-Training Quantization for Diffusion Models [[code](https://github.com/ziplab/PTQD)] ![GitHub Repo stars](https://img.shields.io/github/stars/ziplab/PTQD)
- [[NeurIPS](https://nips.cc/virtual/2023/poster/72396)] Temporal Dynamic Quantization for Diffusion Models
- [[ArXiv](https://arxiv.org/abs/2305.18723)] Towards Accurate Data-free Quantization for Diffusion Models
- [[ArXiv](https://arxiv.org/abs/2309.15505)] Finite Scalar Quantization: VQ-VAE Made Simple [[code](https://github.com/google-research/google-research/tree/master/fsq)] ![GitHub Repo stars](https://img.shields.io/github/stars/google-research/google-research)
- [[ArXiv](https://arxiv.org/abs/2310.03270)] EfficientDM: Efficient Quantization-Aware Fine-Tuning of Low-Bit Diffusion Models

**Pruning and Sparsity**

- [[TPAMI](https://arxiv.org/abs/2211.02048)] Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models [[code](https://github.com/lmxyy/sige)]
- [[ArXiv](https://arxiv.org/abs/2305.10924)] Structural Pruning for Diffusion Models [[code](https://github.com/VainF/Diff-Pruning)]

**Distillation**

- [[CVPR](https://openaccess.thecvf.com/content/CVPR2023/papers/Meng_On_Distillation_of_Guided_Diffusion_Models_CVPR_2023_paper.pdf)] On Distillation of Guided Diffusion Models
- [[ICME](https://arxiv.org/abs/2211.12039)] Accelerating Diffusion Sampling with Classifier-based Feature Distillation [[code](https://github.com/zju-SWJ/RCFD)]
- [[ICML](https://arxiv.org/abs/2308.06644)] Accelerating Diffusion-based Combinatorial Optimization Solvers by Progressive Distillation [[code](https://github.com/jwrh/Accelerating-Diffusion-based-Combinatorial-Optimization-Solvers-by-Progressive-Distillation)]
- [[ICML](https://arxiv.org/abs/2307.05977)] Towards Safe Self-Distillation of Internet-Scale Text-to-Image Diffusion Models [[code](https://github.com/nannullna/safe-diffusion)]
- [[ArXiv](https://arxiv.org/abs/2306.05544)] BOOT: Data-free Distillation of Denoising Diffusion Models with Bootstrapping
- [[ArXiv](https://arxiv.org/abs/2306.00980)] SnapFusion: Text-to-Image Diffusion Model on Mobile Devices within Two Seconds
- [[ArXiv](https://arxiv.org/abs/2305.10769)] Catch-Up Distillation: You Only Need to Train Once for Accelerating Sampling [[code](https://anonymous.4open.science/r/Catch-Up-Distillation-E31F)]
- [[ArXiv](https://arxiv.org/abs/2101.02388)] Knowledge Distillation in Iterative Generative Models for Improved Sampling Speed
- [[ArXiv](https://arxiv.org/abs/2305.15798)] On Architectural Compression of Text-to-Image Diffusion Models
- [[ArXiv](https://arxiv.org/abs/2202.00512)] Progressive Distillation for Fast Sampling of Diffusion Models

**Other**

- [[ArXiv](https://arxiv.org/abs/2309.10438)] AutoDiffusion: Training-Free Optimization of Time Steps and Architectures for Automated Diffusion Model Acceleration
- [[ArXiv](https://arxiv.org/abs/2308.10187)] Spiking-Diffusion: Vector Quantized Discrete Diffusion Model with Spiking Neural Networks [[code](https://github.com/Arktis2022/Spiking-Diffusion)]

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=Efficient-ML/Awesome-Efficient-LLM-Diffusion&type=Timeline)](https://star-history.com/#Efficient-ML/Awesome-Efficient-LLM-Diffusion&Timeline)

## Awesome-Repo

- https://github.com/htqin/Awesome-Model-Quantization ![GitHub Repo stars](https://img.shields.io/github/stars/htqin/awesome-model-quantization)
- https://github.com/Zhen-Dong/Awesome-Quantization-Papers ![GitHub Repo stars](https://img.shields.io/github/stars/Zhen-Dong/Awesome-Quantization-Papers)
- https://github.com/HuangOwen/Awesome-LLM-Compression ![GitHub Repo stars](https://img.shields.io/github/stars/HuangOwen/Awesome-LLM-Compression)
- https://github.com/horseee/Awesome-Efficient-LLM ![GitHub Repo stars](https://img.shields.io/github/stars/horseee/Awesome-Efficient-LLM)
- https://github.com/DefTruth/Awesome-LLM-Inference ![GitHub Repo stars](https://img.shields.io/github/stars/DefTruth/Awesome-LLM-Inference)
- https://github.com/A-suozhang/Awesome-Efficient-Diffusion ![GitHub Repo stars](https://img.shields.io/github/stars/A-suozhang/Awesome-Efficient-Diffusion)
