# Awesome Efficient Diffusion [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A collection of papers and code on efficient diffusion and flow matching models for image and video generation. Topics include fast sampling, distillation, caching, efficient attention, quantization, model compression, training, and deployment. Contributions are welcome.

- [Benchmarks](#benchmarks)
- [Survey Papers](#survey-papers)
- [Papers](#papers)
  - [2026](#2026)
  - [2025](#2025)
  - [2024](#2024)
  - [2023](#2023)
  - [2022](#2022)
- [Implementations](#implementations)
- [Related Repositories](#related-repositories)
- [Contributing](#contributing)

## Benchmarks

- **GenEval: An Object-Focused Framework for Evaluating Text-to-Image Alignment** [Paper](https://proceedings.nips.cc/paper_files/paper/2023/file/a3bf71c7c63f0c3bcb7ff67c67b1e7b1-Paper-Datasets_and_Benchmarks.pdf)<br>
  NeurIPS 2023, Datasets and Benchmarks. Objects, counts, colors, positions, and compositional text-image alignment.

- **VBench: Comprehensive Benchmark Suite for Video Generative Models** [Paper](https://openaccess.thecvf.com/content/CVPR2024/html/Huang_VBench_Comprehensive_Benchmark_Suite_for_Video_Generative_Models_CVPR_2024_paper.html)<br>
  CVPR 2024. Multiple dimensions of video generation quality.

## Survey Papers

- **Efficient Diffusion Models: A Comprehensive Survey From Principles to Practices** [Paper](https://arxiv.org/abs/2410.11795) [Published version](https://doi.org/10.1109/TPAMI.2025.3569700)<br>
  IEEE TPAMI 2025.

- **Efficient Diffusion Models: A Survey** [Paper](https://openreview.net/pdf?id=wHECkBOwyt)<br>
  TMLR 2025.

## Papers

Papers are grouped by publication year and topic. Preprints use their first release year and are labeled arXiv.

### 2026

#### Sampling and solvers

- [[arXiv]](https://arxiv.org/abs/2607.01642) Multi-Resolution Flow Matching: Training-Free Diffusion Acceleration via Staged Sampling (MrFlow) [Code](https://github.com/Xingyu-Zheng/MrFlow)

#### Distillation and few-step generation

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/html/Wang_VDOT_Efficient_Unified_Video_Creation_via_Optimal_Transport_Distillation_CVPR_2026_paper.html) VDOT: Efficient Unified Video Creation via Optimal Transport Distillation [Code](https://github.com/hhhh1138/VDOT)
- [[ECCV (accepted)]](https://arxiv.org/abs/2605.13724) AnyFlow: Any-Step Video Diffusion Model with On-Policy Flow Map Distillation
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/4a8244cd160c6862ff144e14322c32bb-Abstract-Conference.html) Joint Distillation for Fast Likelihood Evaluation and Sampling in Flow-based Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/0534abc9e6db91683d82186ef0d68202-Abstract-Conference.html) Large Scale Diffusion Distillation via Score-Regularized Continuous-Time Consistency [Code](https://github.com/NVlabs/rcm)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/935151cc6cb5d8b6816133b75233775a-Abstract-Conference.html) Rolling Forcing: Autoregressive Long Video Diffusion in Real Time
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/94a98f4338b6e5fba81344f961bac8e5-Abstract-Conference.html) SenseFlow: Scaling Distribution Matching for Flow-based Text-to-Image Distillation [Code](https://github.com/XingtongGe/SenseFlow)
- [[ICML]](https://arxiv.org/abs/2602.02214) Causal Forcing: Autoregressive Diffusion Distillation Done Right for High-Quality Real-Time Interactive Video Generation [Code](https://github.com/thu-ml/Causal-Forcing)

#### Caching and feature reuse

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/html/Nan_Accelerating_Autoregressive_Video_Diffusion_via_History-Guided_Cache_and_Residual_Correction_CVPR_2026_paper.html) Accelerating Autoregressive Video Diffusion via History-Guided Cache and Residual Correction
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/html/Liu_D2Cache_Second-Order_Delta_Caching_for_Higher_Video_Diffusion_Acceleration_CVPR_2026_paper.html) D2Cache: Second-Order Delta Caching for Higher Video Diffusion Acceleration
- [[CVPR]](https://arxiv.org/abs/2602.05449) DisCa: Accelerating Video Diffusion Transformers with Distillation-Compatible Learnable Feature Caching [Code](https://github.com/Tencent-Hunyuan/DisCa)
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/html/Haghighi_SenCache_Accelerating_Diffusion_Model_Inference_via_Sensitivity-Aware_Caching_CVPR_2026_paper.html) SenCache: Accelerating Diffusion Model Inference via Sensitivity-Aware Caching
- [[ECCV (accepted)]](https://arxiv.org/abs/2606.26769) ResilPhase: Plug-and-Play Phase Mapping and Noise-Resilient Macro-Trajectory Extrapolation for Diffusion Acceleration
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/78288ef33b18a351c3cd679dc9a15c8d-Abstract-Conference.html) DiCache: Let Diffusion Model Determine Its Own Cache
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/84d395725a9b40cb4a49d84478ac24c7-Abstract-Conference.html) ERTACache: Error Rectification and Timesteps Adjustment for Efficient Diffusion
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/999fcab97007ebef0cda9949550b4a9e-Abstract-Conference.html) Q&C: When Quantization Meets Cache in Efficient Generation
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/4019681ef05e8e347c3067d7f973a364-Abstract-Conference.html) Relational Feature Caching for Accelerating Diffusion Transformers
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/51373b6499708b6fcc38f1e8f8f5b376-Abstract-Conference.html) ScalingCache: Extreme Acceleration of DiTs through Difference Scaling and Dynamic Interval Caching

#### Efficient attention and token reduction

- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/37287) Sparse-vDiT: Unleashing the Power of Sparse Attention to Accelerate Video Diffusion Transformers
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/papers/Xiao_BinaryAttention_One-Bit_QK-Attention_for_Vision_and_Diffusion_Transformers_CVPR_2026_paper.pdf) BinaryAttention: One-Bit QK-Attention for Vision and Diffusion Transformers
- [[ICML]](https://arxiv.org/abs/2602.04789) Light Forcing: Accelerating Autoregressive Video Diffusion via Sparse Attention [Code](https://github.com/chengtao-lv/LightForcing)
- [[ICML]](https://arxiv.org/abs/2605.30325) Veda: Scalable Video Diffusion via Distilled Sparse Attention

#### Quantization and compression

- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/37841) TR-DQ: Time-Rotation Diffusion Quantization
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2026/html/Li_DeltaQuant_4-bit_Video_Diffusion_Models_with_Spatiotemporal_Delta_Smoothing_CVPR_2026_paper.html) DeltaQuant: 4-bit Video Diffusion Models with Spatiotemporal Delta Smoothing
- [[CVPR]](https://arxiv.org/abs/2507.14811) SegQuant: A Semantics-Aware and Generalizable Quantization Framework for Diffusion Models [Code](https://github.com/OptiSys-ZJU/segquant)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/58e5f95c8c4789af382ab48b4cbc6d9d-Abstract-Conference.html) Beyond Uniformity: Sample and Frequency Meta Weighting for Post-Training Quantization of Diffusion Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/3bd28dd5cc4e15f9e019da13cc0c4844-Abstract-Conference.html) DVD-Quant: Data-free Video Diffusion Transformers Quantization
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/dd3065a00d9b93e3d4d17faa907100bb-Abstract-Conference.html) Gradient-Aligned Calibration for Post-Training Quantization of Diffusion Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/94359ca6e248af69b8b6854668ae9782-Abstract-Conference.html) QuantSparse: Comprehensively Compressing Video Diffusion Transformer with Model Quantization and Attention Sparsification [Code](https://github.com/wlfeng0509/QuantSparse)

#### Efficient architectures and latent spaces

- [[ECCV (accepted)]](https://arxiv.org/abs/2509.25180) DC-Gen: Post-Training Diffusion Acceleration with Deeply Compressed Latent Space [Code](https://github.com/dc-ai-projects/DC-Gen)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2026/hash/41b93c59da0d0f835907fd661d419db2-Abstract-Conference.html) SANA-Video: Efficient Video Generation with Block Linear Diffusion Transformer [Code](https://github.com/NVlabs/Sana)

#### Systems and deployment

- [[ICML]](https://arxiv.org/abs/2512.05081) Deep Forcing: Training-Free Long Video Generation with Deep Sink and Participative Compression
- [[ICML]](https://arxiv.org/abs/2602.01801) FAST-AR: Fast Autoregressive Video Diffusion and World Models with Temporal Cache Compression and Sparse Attention

### 2025

#### Sampling and solvers

- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/f30307ac840b88f86f4ab5761b2d6595-Abstract-Conference.html) Faster Diffusion Sampling with Randomized Midpoints: Sequential and Parallel
- [[Machine Intelligence Research]](https://link.springer.com/article/10.1007/s11633-025-1562-4) DPM-Solver++: Fast Solver for Guided Sampling of Diffusion Probabilistic Models [Code](https://github.com/LuChengTHU/dpm-solver)

#### Distillation and few-step generation

- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/33722) Flash Diffusion: Accelerating Any Conditional Diffusion Model for Few Steps Image Generation [Code](https://github.com/gojasper/flash-diffusion)
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2025/html/Yin_From_Slow_Bidirectional_to_Fast_Autoregressive_Video_Diffusion_Models_CVPR_2025_paper.html) From Slow Bidirectional to Fast Autoregressive Video Diffusion Models
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/papers/Lu_Adversarial_Distribution_Matching_for_Diffusion_Distillation_Towards_Efficient_Image_and_ICCV_2025_paper.pdf) Adversarial Distribution Matching for Diffusion Distillation Towards Efficient Image and Video Synthesis
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Chen_SANA-Sprint_One-Step_Diffusion_with_Continuous-Time_Consistency_Distillation_ICCV_2025_paper.html) SANA-Sprint: One-Step Diffusion with Continuous-Time Consistency Distillation [Code](https://github.com/NVlabs/Sana)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/559a0998fab1d19b80e7e43a5852401c-Abstract-Conference.html) One Step Diffusion via Shortcut Models [Code](https://github.com/kvfrans/shortcut-models)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/a95ba79ea3881ffd9fb8620e1a0d4b36-Abstract-Conference.html) Simple ReFlow: Improved Techniques for Fast Flow Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/file/7e9c2053258b1bdd32ff2654802cd594-Paper-Conference.pdf) Simplifying, Stabilizing and Scaling Continuous-Time Consistency Models
- [[NeurIPS]](https://papers.neurips.cc/paper_files/paper/2025/hash/6d13e085b79d454da5910e4ca82a3d9d-Abstract-Conference.html) Mean Flows for One-step Generative Modeling
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2025/hash/f4823f831af67a3ef15e41a85434422a-Abstract-Conference.html) Self Forcing: Bridging the Train-Test Gap in Autoregressive Video Diffusion
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2025/file/e0d09183aea768b8eb3a7ae972a3d45c-Paper-Conference.pdf) Shortcutting Pre-trained Flow Matching Diffusion

#### Caching and feature reuse

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2025/html/Liu_CacheQuant_Comprehensively_Accelerated_Diffusion_Models_CVPR_2025_paper.html) CacheQuant: Comprehensively Accelerated Diffusion Models
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2025/html/Liu_Timestep_Embedding_Tells_Its_Time_to_Cache_for_Video_Diffusion_CVPR_2025_paper.html) Timestep Embedding Tells: It's Time to Cache for Video Diffusion Model [Code](https://github.com/ali-vilab/TeaCache)
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Kahatapitiya_Adaptive_Caching_for_Faster_Video_Generation_with_Diffusion_Transformers_ICCV_2025_paper.html) Adaptive Caching for Faster Video Generation with Diffusion Transformers
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Liu_From_Reusing_to_Forecasting_Accelerating_Diffusion_Models_with_TaylorSeers_ICCV_2025_paper.html) From Reusing to Forecasting: Accelerating Diffusion Models with TaylorSeers
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Wu_QuantCache_Adaptive_Importance-Guided_Quantization_with_Hierarchical_Latent_and_Layer_Caching_ICCV_2025_paper.html) QuantCache: Adaptive Importance-Guided Quantization with Hierarchical Latent and Layer Caching for Video Generation
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/file/bbe024e0517fe12ac3a8d388b19ff9fe-Paper-Conference.pdf) Accelerating Diffusion Transformers with Token-wise Feature Caching [Code](https://github.com/Shenyi-Z/ToCa)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/092c2d45005ea2db40fc24c470663416-Abstract-Conference.html) Real-Time Video Generation with Pyramid Attention Broadcast
- [[ICML]](https://proceedings.mlr.press/v267/jiang25h.html) SADA: Stability-guided Adaptive Diffusion Acceleration [Code](https://github.com/Ting-Justin-Jiang/sada-icml)

#### Efficient attention and token reduction

- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Xia_Training-free_and_Adaptive_Sparse_Attention_for_Efficient_Long_Video_Generation_ICCV_2025_paper.html) Training-free and Adaptive Sparse Attention for Efficient Long Video Generation
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/b286c344d38e10d2466c0514b78e2f36-Abstract-Conference.html) SageAttention: Accurate 8-Bit Attention for Plug-and-play Inference Acceleration [Code](https://github.com/thu-ml/SageAttention)
- [[ICML]](https://proceedings.mlr.press/v267/zhang25m.html) Fast Video Generation with Sliding Tile Attention [Code](https://github.com/hao-ai-lab/FastVideo)
- [[ICML]](https://arxiv.org/abs/2411.10958) SageAttention2: Efficient Attention with Thorough Outlier Smoothing and Per-thread INT4 Quantization [Code](https://github.com/thu-ml/SageAttention)
- [[ICML]](https://proceedings.mlr.press/v267/xi25c.html) Sparse Video-Gen: Accelerating Video Diffusion Transformers with Spatial-Temporal Sparsity [Code](https://github.com/svg-project/Sparse-VideoGen)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2025/hash/dfc310e81992d2e4cedc09ac47eff13e-Abstract-Conference.html) Faster Video Diffusion with Trainable Sparse Attention
- [[NeurIPS]](https://papers.neurips.cc/paper_files/paper/2025/hash/18a367688479c1b08b001584218a4443-Abstract-Conference.html) Radial Attention: O(n log n) Sparse Attention with Energy Decay for Long Video Generation
- [[NeurIPS]](https://arxiv.org/abs/2505.11594) SageAttention3: Microscaling FP4 Attention for Inference and An Exploration of 8-bit Training [Code](https://github.com/thu-ml/SageAttention)
- [[NeurIPS]](https://arxiv.org/abs/2505.18875) Sparse VideoGen2: Accelerate Video Generation with Sparse Attention via Semantic-Aware Permutation [Code](https://github.com/svg-project/Sparse-VideoGen)

#### Quantization and compression

- [[AAAI]](https://arxiv.org/abs/2501.08180) D2-DPM: Dual Denoising for Quantized Diffusion Probabilistic Models [Code](https://github.com/TaylorJocelyn/D2-DPM)
- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/33823) MPQ-DM: Mixed Precision Quantization for Extremely Low Bit Diffusion Models
- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/34039) Optimizing Quantized Diffusion Models via Distillation with Cross-Timestep Error Correction
- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/32658) Qua2SeDiMo: Quantifiable Quantization Sensitivity of Diffusion Models
- [[AAAI]](https://ojs.aaai.org/index.php/AAAI/article/view/33913) TCAQ-DM: Timestep-Channel Adaptive Quantization for Diffusion Models
- [[ACM MM]](https://arxiv.org/abs/2409.14307) DilateQuant: Accurate and Efficient Quantization-Aware Training for Diffusion Models via Weight Dilation
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2025/papers/Zhu_PassionSR_Post-Training_Quantization_with_Adaptive_Scale_in_One-Step_Diffusion_based_CVPR_2025_paper.pdf) PassionSR: Post-Training Quantization with Adaptive Scale in One-Step Diffusion based Image Super-Resolution [Code](https://github.com/libozhu03/PassionSR)
- [[ICCV]](https://arxiv.org/abs/2507.12933) DMQ: Dissecting Outliers of Diffusion Models for Post-Training Quantization [Code](https://github.com/LeeDongYeun/dmq)
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Wang_QuEST_Low-bit_Diffusion_Model_Quantization_via_Efficient_Selective_Finetuning_ICCV_2025_paper.html) QuEST: Low-bit Diffusion Model Quantization via Efficient Selective Finetuning [Code](https://github.com/hatchetProject/QuEST)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/b09df3a10e26204136540ca59bc5a646-Abstract-Conference.html) BinaryDM: Accurate Weight Binarization for Efficient Diffusion Models [Code](https://github.com/Xingyu-Zheng/BinaryDM)
- [[ICLR]](https://iclr.cc/virtual/2025/poster/29192) DGQ: Distribution-Aware Group Quantization for Text-to-Image Diffusion Models
- [[ICLR]](https://iclr.cc/virtual/2025/poster/27906) SVDQuant: Absorbing Outliers by Low-Rank Component for 4-Bit Diffusion Models [Code](https://github.com/nunchux-ai/nunchaku)
- [[ICLR]](https://iclr.cc/virtual/2025/poster/30429) ViDiT-Q: Efficient and Accurate Quantization of Diffusion Transformers for Image and Video Generation [Code](https://github.com/thu-nics/ViDiT-Q)
- [[ICML]](https://icml.cc/virtual/2025/poster/43551) Modulated Diffusion: Accelerating Generative Modeling with Modulated Quantization [Code](https://github.com/WeizhiGao/MoDiff)
- [[ICML]](https://icml.cc/virtual/2025/poster/45429) Q-VDiT: Towards Accurate Quantization and Distillation of Video-Generation Diffusion Transformers [Code](https://github.com/cantbebetter2/Q-VDiT)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2025/hash/31ed129feae64a7e44a15b148c15558d-Abstract-Conference.html) S²Q-VDiT: Accurate Quantized Video Diffusion Transformer with Salient Data and Sparse Token Distillation [Code](https://github.com/wlfeng0509/S2Q-VDiT)
- [[NeurIPS]](https://neurips.cc/virtual/2025/poster/115090) VETA-DiT: Variance-Equalized and Temporally Adaptive Quantization for Efficient 4-bit Diffusion Transformers

#### Efficient architectures and latent spaces

- [[ICLR]](https://arxiv.org/abs/2410.10733) Deep Compression Autoencoder for Efficient High-Resolution Diffusion Models [Code](https://github.com/mit-han-lab/efficientvit)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/34345e243156da67605d4b63d71c8d98-Abstract-Conference.html) SANA: Efficient High-Resolution Text-to-Image Synthesis with Linear Diffusion Transformers [Code](https://github.com/NVlabs/Sana)

#### Efficient training and adaptation

- [[ICCV]](https://arxiv.org/abs/2508.00413) DC-AE 1.5: Accelerating Diffusion Model Convergence with Structured Latent Space [Code](https://github.com/dc-ai-projects/DC-Gen)
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2025/html/Leng_REPA-E_Unlocking_VAE_for_End-to-End_Tuning_of_Latent_Diffusion_Transformers_ICCV_2025_paper.html) REPA-E: Unlocking VAE for End-to-End Tuning of Latent Diffusion Transformers [Code](https://github.com/End2End-Diffusion/REPA-E)
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2025/hash/d9e42b4d7163931f3689d6d6fbaa11d0-Abstract-Conference.html) Representation Alignment for Generation: Training Diffusion Transformers Is Easier Than You Think
- [[ICML]](https://proceedings.mlr.press/v267/xie25b.html) SANA 1.5: Efficient Scaling of Training-Time and Inference-Time Compute in Linear Diffusion Transformer [Code](https://github.com/NVlabs/Sana)

#### Systems and deployment

- [[NeurIPS]](https://proceedings.nips.cc/paper_files/paper/2025/hash/8da04a60948be713dc766f0c7e3a5b1f-Abstract-Conference.html) PipeFusion: Patch-level Pipeline Parallelism for Diffusion Transformers Inference [Code](https://github.com/xdit-project/xDiT)
- [[arXiv]](https://arxiv.org/abs/2512.16093) TurboDiffusion: Accelerating Video Diffusion Models by 100-200 Times [Code](https://github.com/thu-ml/TurboDiffusion)

### 2024

#### Sampling and solvers

- [[ICML]](https://proceedings.mlr.press/v235/sabour24a.html) Align Your Steps: Optimizing Sampling Schedules in Diffusion Models

#### Distillation and few-step generation

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/html/Yin_One-step_Diffusion_with_Distribution_Matching_Distillation_CVPR_2024_paper.html) One-step Diffusion with Distribution Matching Distillation
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/11557_ECCV_2024_paper.php) Adversarial Diffusion Distillation
- [[ECCV]](https://arxiv.org/abs/2405.05967) Distilling Diffusion Models into Conditional GANs
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2024/hash/c204d12afa0175285e5aac65188808b4-Abstract-Conference.html) Consistency Trajectory Models: Learning Probability Flow ODE Trajectory of Diffusion
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2024/hash/41bd71e7bf7f9fe68f1c936940fd06bd-Abstract-Conference.html) Improved Techniques for Training Consistency Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2024/hash/4dc37a7bc61057252ce043fa3b83aac2-Abstract-Conference.html) InstaFlow: One Step is Enough for High-Quality Diffusion-Based Text-to-Image Generation [Code](https://github.com/gnobitab/InstaFlow)
- [[ICML]](https://proceedings.mlr.press/v235/zhou24x.html) Score identity Distillation: Exponentially Fast Distillation of Pretrained Diffusion Models for One-Step Generation
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2024/file/d4e1c24ac41ff0b82ca1b171731f0b23-Paper-Conference.pdf) Hyper-SD: Trajectory Segmented Consistency Model for Efficient Image Synthesis
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/54dcf25318f9de5a7a01f0a4125c541e-Abstract-Conference.html) Improved Distribution Matching Distillation for Fast Image Synthesis [Code](https://github.com/tianweiy/DMD2)
- [[NeurIPS]](https://papers.neurips.cc/paper_files/paper/2024/hash/7343a5c976f8399880b695267f1f9e9f-Abstract-Conference.html) Improving the Training of Rectified Flows
- [[arXiv]](https://arxiv.org/abs/2403.12015) Fast High-Resolution Image Synthesis with Latent Adversarial Diffusion Distillation
- [[arXiv]](https://arxiv.org/abs/2402.13929) SDXL-Lightning: Progressive Adversarial Diffusion Distillation [Models](https://huggingface.co/ByteDance/SDXL-Lightning)

#### Caching and feature reuse

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/html/Ma_DeepCache_Accelerating_Diffusion_Models_for_Free_CVPR_2024_paper.html) DeepCache: Accelerating Diffusion Models for Free [Code](https://github.com/horseee/DeepCache)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2024/hash/f0b1515be276f6ba82b4f2b25e50bef0-Abstract-Conference.html) Learning-to-Cache: Accelerating Diffusion Transformer via Layer Caching [Code](https://github.com/horseee/learning-to-cache)

#### Efficient attention and token reduction

- [[NeurIPS]](https://proceedings.nips.cc/paper_files/paper/2024/hash/0267925e3c276e79189251585b4100bf-Abstract-Conference.html) DiTFastAttn: Attention Compression for Diffusion Transformer Models

#### Quantization and compression

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/html/Huang_TFMQ-DM_Temporal_Feature_Maintenance_Quantization_for_Diffusion_Models_CVPR_2024_paper.html) TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models
- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_Towards_Accurate_Post-training_Quantization_for_Diffusion_Models_CVPR_2024_paper.html) Towards Accurate Post-training Quantization for Diffusion Models
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/2494_ECCV_2024_paper.php) Memory-Efficient Fine-Tuning for Quantized Diffusion Model
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/2212_ECCV_2024_paper.php) MixDQ: Memory-Efficient Few-Step Text-to-Image Diffusion Models with Metric-Decoupled Mixed Precision Quantization
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7353_ECCV_2024_paper.php) Post-training Quantization with Progressive Calibration and Activation Relaxing for Text-to-Image Diffusion Models
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/8312_ECCV_2024_paper.php) Timestep-Aware Correction for Quantized Diffusion Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2024/hash/4494939e203ae3bce9c32512c21a352d-Abstract-Conference.html) EfficientDM: Efficient Quantization-Aware Fine-Tuning of Low-Bit Diffusion Models
- [[NeurIPS]](https://nips.cc/virtual/2024/poster/93620) BiDM: Pushing the Limit of Quantization for Diffusion Models
- [[NeurIPS]](https://neurips.cc/virtual/2024/poster/93008) Binarized Diffusion Model for Image Super-Resolution [Code](https://github.com/zhengchen1999/BI-DiffSR)
- [[NeurIPS]](https://nips.cc/virtual/2024/poster/96909) BitsFusion: 1.99 bits Weight Quantization of Diffusion Model
- [[NeurIPS]](https://nips.cc/virtual/2024/poster/95445) PTQ4DiT: Post-training Quantization for Diffusion Transformers
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2024/file/615675cc6e94ddb1a783904fb178b5f6-Paper-Conference.pdf) StepbaQ: Stepping backward as Correction for Quantized Diffusion Models

#### Efficient architectures and latent spaces

- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7138_ECCV_2024_paper.php) BK-SDM: A Lightweight, Fast, and Cheap Version of Stable Diffusion

#### Efficient training and adaptation

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/html/Karras_Analyzing_and_Improving_the_Training_Dynamics_of_Diffusion_Models_CVPR_2024_paper.html) Analyzing and Improving the Training Dynamics of Diffusion Models
- [[ICLR]](https://proceedings.iclr.cc/paper_files/paper/2024/hash/fe989bb038b5dcc44181255dd6913e43-Abstract-Conference.html) PixArt-α: Fast Training of Diffusion Transformer for Photorealistic Text-to-Image Synthesis
- [[NeurIPS]](https://papers.neurips.cc/paper_files/paper/2024/hash/a422a2f016c14406a01ddba731c0969a-Abstract-Conference.html) Immiscible Diffusion: Accelerating Diffusion Training with Noise Assignment

#### Systems and deployment

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_DistriFusion_Distributed_Parallel_Inference_for_High-Resolution_Diffusion_Models_CVPR_2024_paper.pdf) DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models
- [[ECCV]](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/7923_ECCV_2024_paper.php) MobileDiffusion: Instant Text-to-Image Generation on Mobile Devices

### 2023

#### Sampling and solvers

- [[ICLR]](https://arxiv.org/abs/2204.13902) Fast Sampling of Diffusion Models with Exponential Integrator [Code](https://github.com/qsh-zh/deis)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/ada8de994b46571bdcd7eeff2d3f9cff-Abstract-Conference.html) DPM-Solver-v3: Improved Diffusion ODE Solver with Empirical Model Statistics [Code](https://github.com/thu-ml/DPM-Solver-v3)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d6f764aae383d9ff28a0f89f71defbd9-Abstract-Conference.html) SEEDS: Exponential SDE Solvers for Fast High-Quality Sampling from Diffusion Models
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/9c2aa1e456ea543997f6927295196381-Abstract-Conference.html) UniPC: A Unified Predictor-Corrector Framework for Fast Sampling of Diffusion Models [Code](https://github.com/wl-zhao/UniPC)

#### Distillation and few-step generation

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2023/html/Meng_On_Distillation_of_Guided_Diffusion_Models_CVPR_2023_paper.html) On Distillation of Guided Diffusion Models
- [[ICLR]](https://arxiv.org/abs/2209.03003) Flow Straight and Fast: Learning to Generate and Transfer Data with Rectified Flow
- [[ICML]](https://proceedings.mlr.press/v202/song23a.html) Consistency Models
- [[arXiv]](https://arxiv.org/abs/2310.04378) Latent Consistency Models: Synthesizing High-Resolution Images with Few-Step Inference

#### Efficient attention and token reduction

- [[CVPR Workshop (ECV)]](https://openaccess.thecvf.com/content/CVPR2023W/ECV/html/Bolya_Token_Merging_for_Fast_Stable_Diffusion_CVPRW_2023_paper.html) Token Merging for Fast Stable Diffusion [Code](https://github.com/dbolya/tomesd)

#### Quantization and compression

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2023/html/Shang_Post-Training_Quantization_on_Diffusion_Models_CVPR_2023_paper.html) Post-training Quantization on Diffusion Models [Code](https://github.com/42Shawn/PTQ4DM)
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2023/papers/Li_Q-Diffusion_Quantizing_Diffusion_Models_ICCV_2023_paper.pdf) Q-diffusion: Quantizing Diffusion Models [Code](https://github.com/Xiuyu-Li/q-diffusion)
- [[NeurIPS]](https://neurips.cc/virtual/2023/poster/71314) PTQD: Accurate Post-Training Quantization for Diffusion Models [Code](https://github.com/ziplab/PTQD)
- [[NeurIPS]](https://neurips.cc/virtual/2023/poster/70279) Q-DM: An Efficient Low-bit Quantized Diffusion Model
- [[NeurIPS]](https://neurips.cc/virtual/2023/poster/72396) Temporal Dynamic Quantization for Diffusion Models

#### Efficient architectures and latent spaces

- [[NeurIPS]](https://papers.neurips.cc/paper_files/paper/2023/hash/35c1d69d23bb5dd6b9abcd68be005d5c-Abstract-Conference.html) Structural Pruning for Diffusion Models [Code](https://github.com/VainF/Diff-Pruning)

#### Efficient training and adaptation

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2023/html/Kumari_Multi-Concept_Customization_of_Text-to-Image_Diffusion_CVPR_2023_paper.html) Multi-Concept Customization of Text-to-Image Diffusion
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2023/papers/Xie_DiffFit_Unlocking_Transferability_of_Large_Diffusion_Models_via_Simple_Parameter-efficient_ICCV_2023_paper.pdf) DiffFit: Unlocking Transferability of Large Diffusion Models via Simple Parameter-Efficient Fine-Tuning
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2023/html/Hang_Efficient_Diffusion_Training_via_Min-SNR_Weighting_Strategy_ICCV_2023_paper.html) Efficient Diffusion Training via Min-SNR Weighting Strategy
- [[ICCV]](https://openaccess.thecvf.com/content/ICCV2023/html/Han_SVDiff_Compact_Parameter_Space_for_Diffusion_Fine-Tuning_ICCV_2023_paper.html) SVDiff: Compact Parameter Space for Diffusion Fine-Tuning
- [[ICLR]](https://arxiv.org/abs/2210.02747) Flow Matching for Generative Modeling

#### Systems and deployment

- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2023/hash/41bcc9d3bddd9c90e1f44b29e26d97ff-Abstract-Conference.html) SnapFusion: Text-to-Image Diffusion Model on Mobile Devices within Two Seconds

### 2022

#### Sampling and solvers

- [[ICLR]](https://arxiv.org/abs/2201.06503) Analytic-DPM: an Analytic Estimate of the Optimal Reverse Variance in Diffusion Probabilistic Models
- [[ICLR]](https://arxiv.org/abs/2202.05830) Learning Fast Samplers for Diffusion Models by Differentiating Through Sample Quality
- [[ICLR]](https://openreview.net/pdf/08c071f50f706076294158af529e4f1a2556df41.pdf) Pseudo Numerical Methods for Diffusion Models on Manifolds [Code](https://github.com/luping-liu/PNDM)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/260a14acce2a89dad36adc8eefe7c59e-Abstract-Conference.html) DPM-Solver: A Fast ODE Solver for Diffusion Probabilistic Model Sampling in Around 10 Steps [Code](https://github.com/LuChengTHU/dpm-solver)
- [[NeurIPS]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/a98846e9d9cc01cfb87eb694d946ce6b-Abstract-Conference.html) Elucidating the Design Space of Diffusion-Based Generative Models [Code](https://github.com/NVlabs/edm)

#### Distillation and few-step generation

- [[ICLR]](https://arxiv.org/abs/2202.00512) Progressive Distillation for Fast Sampling of Diffusion Models

#### Efficient architectures and latent spaces

- [[CVPR]](https://openaccess.thecvf.com/content/CVPR2022/html/Rombach_High-Resolution_Image_Synthesis_With_Latent_Diffusion_Models_CVPR_2022_paper.html) High-Resolution Image Synthesis With Latent Diffusion Models [Code](https://github.com/CompVis/latent-diffusion)

## Implementations

- [xDiT](https://github.com/xdit-project/xDiT): Parallel inference for diffusion transformers, including PipeFusion.
- [FastVideo](https://github.com/hao-ai-lab/FastVideo): Video generation inference and post-training, including sparse attention.
- [Nunchaku](https://github.com/nunchux-ai/nunchaku): Low-bit diffusion inference and SVDQuant kernels.
- [SageAttention](https://github.com/thu-ml/SageAttention): Low-precision attention kernels for inference acceleration.
- [Sparse VideoGen](https://github.com/svg-project/Sparse-VideoGen): Sparse attention implementations for video diffusion.
- [SANA](https://github.com/NVlabs/Sana): Efficient image/video model training and inference.
- [rCM](https://github.com/NVlabs/rcm): Continuous-time consistency distillation for video models.
- [TurboDiffusion](https://github.com/thu-ml/TurboDiffusion): Combined attention acceleration, distillation, and low-precision inference.

## Related Repositories

- [Awesome Model Quantization](https://github.com/AI-Efficiency/Awesome-Model-Quantization): Model quantization across architectures.
- [Awesome Efficient LLM](https://github.com/horseee/Awesome-Efficient-LLM): Efficient language models.
- [Efficient Diffusion Models](https://github.com/TsinghuaC3I/Efficient-Diffusion-Models): Resources accompanying the TPAMI survey.

## Contributing

Please open a pull request with the paper title, venue, year, paper link, and official code when available. We collect relevant publications at leading conferences and journals, as well as recent preprints with early community interest or adoption. For preprints, include a dated source documenting that interest. Keep one entry per paper and update it when the published version becomes available.

<details>
<summary>Preprint and other inclusion references</summary>

- [MrFlow](https://arxiv.org/abs/2607.01642): Released on July 2, 2026 and submitted to Hugging Face Daily Papers on July 3; the official repository records release-month Trending Papers coverage and community workflows. [Daily Papers](https://huggingface.co/papers/2607.01642) [Release history and community](https://github.com/Xingyu-Zheng/MrFlow#-news)
- [Latent Consistency Models](https://arxiv.org/abs/2310.04378): LCM ecosystem integration documented by Hugging Face in November 2023. [Evidence](https://huggingface.co/blog/lcm_lora)
- [Fast High-Resolution Image Synthesis with Latent Adversarial Diffusion Distillation](https://arxiv.org/abs/2403.12015): Hugging Face Daily Papers #1; submitted the day after release. [Evidence](https://huggingface.co/papers/2403.12015)
- [TurboDiffusion](https://arxiv.org/abs/2512.16093): Hugging Face Daily Papers #1; submitted within one week of release. [Evidence](https://huggingface.co/papers/2512.16093)
- [Token Merging for Fast Stable Diffusion](https://openaccess.thecvf.com/content/CVPR2023W/ECV/html/Bolya_Token_Merging_for_Fast_Stable_Diffusion_CVPRW_2023_paper.html): Release-week Diffusers community benchmarking, March 2023; workshop status is explicit. [Evidence](https://github.com/huggingface/diffusers/issues/2940)
- [SDXL-Lightning](https://arxiv.org/abs/2402.13929): Release-week public discussion and experimentation, February 2024. [Evidence](https://www.reddit.com/r/StableDiffusion/comments/1awpbg3)
- [DPM-Solver++](https://link.springer.com/article/10.1007/s11633-025-1562-4): Author-maintained history records Apple/Hugging Face Swift integration in December 2022; first preprint 2022. [Evidence](https://github.com/LuChengTHU/dpm-solver#news)

</details>
