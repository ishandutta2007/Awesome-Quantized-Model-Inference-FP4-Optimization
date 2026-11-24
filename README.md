<p align="center">
  <img src="assets/banner.svg" alt="Awesome Quantized Model Inference and FP4 Optimization Banner" width="100%" />
</p>

<p align="center">
  <a href="https://github.com/ishandutta2007/Awesome-Awesome-Awesome"><img src="https://img.shields.io/badge/Awesome-%E2%9C%94-blueviolet?style=flat-square&logo=github" alt="Awesome"/></a><a href="https://discord.gg/jc4xtF58Ve"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Discord" /></a>
  <a href="https://github.com/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization/stargazers"><img src="https://img.shields.io/github/stars/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization?style=flat-square&color=yellow" alt="GitHub Stars"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization/network/members"><img src="https://img.shields.io/github/forks/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization?style=flat-square&color=blue" alt="GitHub Forks"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization/issues"><img src="https://img.shields.io/github/issues/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization?style=flat-square&color=red" alt="GitHub Issues"/></a>
  <a href="https://github.com/ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg?style=flat-square" alt="License: MIT"/></a>
  <a href="https://github.com/ishandutta2007"><img alt="GitHub followers" src="https://img.shields.io/github/followers/ishandutta2007?label=Follow" /></a>
</p>

---

# 🚀 Awesome Quantized Model Inference & FP4 Optimization

> **A comprehensive, SEO-optimized, community-curated index of production-ready SaaS platforms, cloud inference engines, and open-source frameworks pioneering low-bit quantization (NVFP4, MXFP4, INT4, FP8, AWQ, GPTQ) and high-throughput LLM serving.**

**Last updated: November 2026** 📅

This repository tracks notable **cloud SaaS platforms** and **open-source repositories** for **Quantized Model Inference & FP4 Optimization**. These cutting-edge tools maximize LLM, VLM, and multimodal generative throughput while drastically cutting VRAM requirements using 4-bit floating-point formats (`NVFP4`, `MXFP4`), weight-only/activation quantization (`AWQ`, `GPTQ`, `FP8`, `GGUF`), speculative decoding (`EAGLE`, `Medusa`), and fused attention/GEMM kernels (`Marlin`, `FlashInfer`, `FlashAttention`).

---

## 📑 Table of Contents
- [🌐 Sector Overview & Market Dynamics](#-sector-overview--market-dynamics)
- [☁️ SaaS & Hosted Inference Platforms](#️-saas--hosted-inference-platforms)
- [💻 Open-Source GitHub Projects](#-open-source-github-projects)
- [🛠️ How to Contribute](#️-how-to-contribute)
- [💖 Support & Sponsorship](#-support--sponsorship)
- [📈 Star History](#-star-history)
- [⚠️ Disclaimer](#️-disclaimer)

---

## 🌐 Sector Overview & Market Dynamics

The AI inference infrastructure and hardware-accelerated serving market is projected to expand from **$15 billion in 2024 to over $110 billion by 2030** (growing at a ~38% CAGR), rapidly eclipsing AI model training expenditure as enterprise deployment moves into real-time production. The sector exhibits **moderate fragmentation with emergent winner-take-most dynamics**: foundational hardware and compiler microservices remain heavily consolidated around NVIDIA (Blackwell/Hopper architecture and CUDA ecosystem), while the cloud API serving layer features aggressive contestation between hyperscalers, custom silicon providers (e.g., Groq LPUs, SambaNova RDUs), and independent low-latency serverless clouds (Fireworks AI, Together AI, Modal, Baseten).

---

## ☁️ SaaS & Hosted Inference Platforms

The following SaaS platforms offer managed low-bit inference APIs, custom FP4/FP8 runtime acceleration, and autoscaling GPU microservices. Entries are sorted descending by company size (valuation / market capitalization / revenue).

| 🏢 Platform | 💰 Company Size (Valuation / Revenue) | 🏷️ Starting Tier Price | 🎁 Free Tier Limits | 🔍 Core Specialization & FP4/Low-Bit Highlights |
| :--- | :--- | :--- | :--- | :--- |
| **[NVIDIA NIM & TensorRT Cloud](https://nvidia.com)** | **~$3.5 Trillion** Market Cap (NVIDIA) | **$1.00 / GPU-hour** (NVIDIA AI Enterprise starts at $4,500/GPU/year or $1.00/GPU-hr on cloud) | **Dynamic Free Tier** (~40 RPM rate limit across hosted model catalog via NVIDIA Developer Program at `build.nvidia.com`, no credit card required) | Enterprise microservices featuring pre-optimized TensorRT-LLM engines with native Blackwell NVFP4, Hopper FP8, and SmoothQuant acceleration. |
| **[Fireworks AI](https://fireworks.ai)** | **$17.5 Billion** Valuation ($1B+ ARR) | **$0.15 / 1M input tokens** (Flash/small models; standard models scale $0.50-$2.00/1M tokens) | **$1.00 Free Trial Credit** (Instant signup credit without upfront credit card, subject to ~10 RPM ceiling until billing profile verified) | Ultra-low-latency generative inference cloud powered by custom quantized CUDA kernels (`FireAttention`), speculative decoding, and FP4/FP8 pipelines. |
| **[Modal](https://modal.com)** | **$15.75 Billion** Valuation ($1B+ ARR) | **$0.0000028 / vCPU-sec** (~$0.01/hr CPU, GPUs starting at $0.15/hr T4 up to H100s, pay-per-second) | **$30.00 / month Recurring Free Credits** on Starter Plan (Max 10 concurrent GPUs, 100 containers, 3 workspace seats; resets monthly) | High-performance serverless Python infrastructure running containerized vLLM, SGLang, TensorRT-LLM, and custom FP4/CUDA kernels on demand. |
| **[SambaNova Cloud](https://sambanova.ai)** | **$11.0 Billion** Valuation | **$0.10 / 1M input tokens** (Pay-as-you-go Developer tier; Llama-3.1 70B starting at $0.60/1M tokens) | **Permanent Free Tier** (20 RPM, 20 RPD, and up to 200,000 tokens/day cap on preview models without entering a payment method) | Native inference cloud running massive quantized models on Reconfigurable Dataflow Units (RDUs) with extreme on-chip SRAM bandwidth. |
| **[Together AI](https://together.ai)** | **$8.3 Billion** Valuation | **$0.18 / 1M input tokens** (Llama 3 8B; requires $15 mandatory initial prepaid deposit, refills min $5) | **No Free Tier / No Trial Credits** (Direct prepaid model; external qualifying early-stage startups can apply for $15,000-$50,000 credits) | High-throughput cloud inference engine utilizing custom FP4/FP8 quantization, FlashAttention kernels, and sub-second token generation. |
| **[Hugging Face Inference Endpoints](https://huggingface.co)** | **$4.5 Billion** Valuation | **$0.06 / hour** (CPU instances; GPU instances start at $0.50/hr for T4, scaling to A100/H100) | **No Dedicated Free Tier** (Paid hourly dedicated instances; accounts get serverless community API rate allowances or $2/mo credit with PRO plan) | Fully managed dedicated model hosting backed by Text Generation Inference (TGI) with built-in BitsAndBytes, AWQ, GPTQ, and Marlin quantization. |
| **[GroqCloud](https://groq.com)** | **$3.5 Billion** Valuation | **$0.05 / 1M input tokens** (Llama 8B; larger 70B models start at $0.59/1M tokens on Developer Plan) | **Permanent Free Tier** (30 RPM, 1,000-14,400 RPD, and 6,000-30,000 TPM depending on model tier, no credit card required) | Hosted Language Processing Unit (LPU) inference platform delivering ultra-high-speed deterministic token generation with hardware low-precision execution. |
| **[Baseten](https://baseten.co)** | **$2.15 Billion** Valuation | **$0.000108 / sec** ($0.39/hr for T4 GPU; A100 at $3.25/hr, pay-per-second compute with $0 monthly platform fee) | **$30.00 One-time Free Trial Credit** (Granted upon initial workspace creation to test model APIs and dedicated deployments before card billing) | Managed model deployment and inference infrastructure offering one-click TensorRT-LLM, vLLM, and FP4/FP8 quantized model autoscaling. |
| **[RunPod Serverless](https://runpod.io)** | **$1.0 Billion** Valuation | **$0.0002 / second** (~$0.20/hr for entry GPUs; Flex serverless starts at $0.00016/sec, storage at $0.05/GB/mo) | **No Permanent Free Tier** (Prepaid pay-per-second compute model; periodic $5-$10 promo vouchers and startup accelerator grants available) | Distributed GPU cloud offering serverless endpoints, vLLM/ExLlama worker templates, and custom Docker execution for quantized GGUF/AWQ models. |
| **[FriendliAI](https://friendli.ai)** | **~$80 Million** Valuation | **$0.20 / 1M input tokens** (Pay-as-you-go serverless model endpoints; dedicated container licenses available) | **Free Starter Access** (Free serverless trial quota provided upon initial registration for testing open-weight models before paid tiers) | Commercial LLM serving engine featuring iteration-level scheduling, custom low-bit CUDA engines, and proprietary FP8/INT4/FP4 quantization. |

---

## 💻 Open-Source GitHub Projects

The open-source community is the driving force behind quantized model inference, delivering state-of-the-art fused CUDA/Triton kernels, post-training quantization (PTQ) algorithms, and production-grade serving architectures. 

Projects below are equipped with live social star badges linking directly to their stargazer pages and are **sorted descending by star counts**.

- **[llama.cpp](https://github.com/ggml-org/llama.cpp)** <a href="https://github.com/ggml-org/llama.cpp/stargazers"><img src="https://img.shields.io/github/stars/ggml-org/llama.cpp?style=social&color=white" alt="Stars"/></a>  
  Premier open-source C/C++ LLM inference engine enabling 1.5-bit to 8-bit GGUF, IQ, and MXFP4 quantized execution across NVIDIA, AMD ROCm, Apple Silicon Metal, and CPUs.

- **[vLLM](https://github.com/vllm-project/vllm)** <a href="https://github.com/vllm-project/vllm/stargazers"><img src="https://img.shields.io/github/stars/vllm-project/vllm?style=social&color=white" alt="Stars"/></a>  
  Industry-standard high-throughput LLM serving engine featuring PagedAttention, native NVFP4/MXFP4, Hopper FP8, AWQ, GPTQ, and Marlin fused kernel integration.

- **[DeepSpeed](https://github.com/deepspeedai/DeepSpeed)** <a href="https://github.com/deepspeedai/DeepSpeed/stargazers"><img src="https://img.shields.io/github/stars/deepspeedai/DeepSpeed?style=social&color=white" alt="Stars"/></a>  
  Microsoft's deep learning optimization suite featuring DeepSpeed-FastGen, ZeroQuant, SmoothQuant, and SplitFuse high-throughput quantized inference.

- **[SGLang](https://github.com/sgl-project/sglang)** <a href="https://github.com/sgl-project/sglang/stargazers"><img src="https://img.shields.io/github/stars/sgl-project/sglang?style=social&color=white" alt="Stars"/></a>  
  High-performance serving framework for LLMs and VLMs featuring RadixAttention prefix caching, zero-overhead scheduling, and hardware-accelerated FP4/FP8 quantization.

- **[FlashAttention](https://github.com/Dao-AILab/flash-attention)** <a href="https://github.com/Dao-AILab/flash-attention/stargazers"><img src="https://img.shields.io/github/stars/Dao-AILab/flash-attention?style=social&color=white" alt="Stars"/></a>  
  Fast, memory-efficient IO-aware exact attention CUDA library accelerating transformer training and low-bit inference runtimes.

- **[MLC-LLM](https://github.com/mlc-ai/mlc-llm)** <a href="https://github.com/mlc-ai/mlc-llm/stargazers"><img src="https://img.shields.io/github/stars/mlc-ai/mlc-llm?style=social&color=white" alt="Stars"/></a>  
  Universal LLM deployment and machine learning compilation engine compiling 3-bit and 4-bit quantized models natively across WebGPU, iOS, Android, Vulkan, and CUDA.

- **[TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM)** <a href="https://github.com/NVIDIA/TensorRT-LLM/stargazers"><img src="https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM?style=social&color=white" alt="Stars"/></a>  
  NVIDIA's flagship library for defining and serving optimized LLMs with native Blackwell NVFP4, Hopper FP8, in-flight batching, and custom GEMM kernels.

- **[Text Generation Inference (TGI)](https://github.com/huggingface/text-generation-inference)** <a href="https://github.com/huggingface/text-generation-inference/stargazers"><img src="https://img.shields.io/github/stars/huggingface/text-generation-inference?style=social&color=white" alt="Stars"/></a>  
  Production-grade Rust and Python LLM serving container by Hugging Face supporting Marlin, EXL2, AWQ, GPTQ, EETQ, and FP8 quantization out of the box.

- **[BitsAndBytes](https://github.com/bitsandbytes-foundation/bitsandbytes)** <a href="https://github.com/bitsandbytes-foundation/bitsandbytes/stargazers"><img src="https://img.shields.io/github/stars/bitsandbytes-foundation/bitsandbytes?style=social&color=white" alt="Stars"/></a>  
  Accessible k-bit quantization library for PyTorch enabling 4-bit NormalFloat (NF4), FP4, 8-bit matrix multiplication, and QLoRA fine-tuning.

- **[LMDeploy](https://github.com/InternLM/lmdeploy)** <a href="https://github.com/InternLM/lmdeploy/stargazers"><img src="https://img.shields.io/github/stars/InternLM/lmdeploy?style=social&color=white" alt="Stars"/></a>  
  Open-source toolkit by InternLM for compressing, deploying, and serving LLMs and VLMs powered by the TurboMind C++/CUDA engine and W4A16/FP8 quantization.

- **[FlashInfer](https://github.com/flashinfer-ai/flashinfer)** <a href="https://github.com/flashinfer-ai/flashinfer/stargazers"><img src="https://img.shields.io/github/stars/flashinfer-ai/flashinfer?style=social&color=white" alt="Stars"/></a>  
  High-performance kernel library engineered for LLM serving, offering specialized FP8/FP4 KV-cache compression, ragged batch decoding, and fused attention.

- **[NVIDIA Model Optimizer](https://github.com/NVIDIA/Model-Optimizer)** <a href="https://github.com/NVIDIA/Model-Optimizer/stargazers"><img src="https://img.shields.io/github/stars/NVIDIA/Model-Optimizer?style=social&color=white" alt="Stars"/></a>  
  Unified library of state-of-the-art model compression techniques (PTQ, QAT, distillation, sparsity) preparing models for TensorRT-LLM and vLLM NVFP4/FP8 deployment.

- **[AutoGPTQ](https://github.com/AutoGPTQ/AutoGPTQ)** <a href="https://github.com/AutoGPTQ/AutoGPTQ/stargazers"><img src="https://img.shields.io/github/stars/AutoGPTQ/AutoGPTQ?style=social&color=white" alt="Stars"/></a>  
  Easy-to-use 4-bit post-training quantization package for LLMs with custom CUDA, Marlin, and Triton kernels integrated across the Hugging Face ecosystem.

- **[ExLlamaV2](https://github.com/turboderp-org/exllamav2)** <a href="https://github.com/turboderp-org/exllamav2/stargazers"><img src="https://img.shields.io/github/stars/turboderp-org/exllamav2?style=social&color=white" alt="Stars"/></a>  
  Fast inference engine designed for running EXL2 (mixed 2-to-8 bit precision) and GPTQ quantized models locally with minimal VRAM on modern consumer GPUs.

- **[LLM Compressor](https://github.com/vllm-project/llm-compressor)** <a href="https://github.com/vllm-project/llm-compressor/stargazers"><img src="https://img.shields.io/github/stars/vllm-project/llm-compressor?style=social&color=white" alt="Stars"/></a>  
  State-of-the-art model compression library built directly for production vLLM inference, supporting NVFP4, MXFP4, FP8, INT4, and 2:4 structural sparsity.

- **[AWQ (LLM-AWQ)](https://github.com/mit-han-lab/llm-awq)** <a href="https://github.com/mit-han-lab/llm-awq/stargazers"><img src="https://img.shields.io/github/stars/mit-han-lab/llm-awq?style=social&color=white" alt="Stars"/></a>  
  MIT HAN Lab's seminal Activation-aware Weight Quantization algorithm for 4-bit LLM compression, preserving outlier activation weights without retraining.

- **[TorchAO](https://github.com/pytorch/ao)** <a href="https://github.com/pytorch/ao/stargazers"><img src="https://img.shields.io/github/stars/pytorch/ao?style=social&color=white" alt="Stars"/></a>  
  PyTorch native Architecture Optimization library offering first-class `MXFP4`, `INT4`, `FP8`, dynamic quantization, and sparsity kernels compatible with `torch.compile`.

- **[GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa)** <a href="https://github.com/qwopqwop200/GPTQ-for-LLaMa/stargazers"><img src="https://img.shields.io/github/stars/qwopqwop200/GPTQ-for-LLaMa?style=social&color=white" alt="Stars"/></a>  
  Pioneering 4-bit post-training quantization implementation for LLaMA-based architectures using approximate second-order weight updates.

- **[EAGLE](https://github.com/SafeAILab/EAGLE)** <a href="https://github.com/SafeAILab/EAGLE/stargazers"><img src="https://img.shields.io/github/stars/SafeAILab/EAGLE?style=social&color=white" alt="Stars"/></a>  
  Leading speculative decoding framework (EAGLE-1, EAGLE-2, and EAGLE-3) accelerating LLM token generation up to 3x without degrading output quality.

- **[AutoAWQ](https://github.com/casper-hansen/AutoAWQ)** <a href="https://github.com/casper-hansen/AutoAWQ/stargazers"><img src="https://img.shields.io/github/stars/casper-hansen/AutoAWQ?style=social&color=white" alt="Stars"/></a>  
  Turnkey 4-bit AWQ post-training quantization tool with Marlin CUDA kernel backend providing up to 2x-3x speedups during low-bit batched serving.

- **[Aphrodite Engine](https://github.com/dphnAI/sonar)** <a href="https://github.com/dphnAI/sonar/stargazers"><img src="https://img.shields.io/github/stars/dphnAI/sonar?style=social&color=white" alt="Stars"/></a>  
  Large-scale LLM inference engine supporting extensive community quantization formats (GGUF, EXL2, IQ4, AWQ, Marlin, and QuIP#).

- **[FSDP-QLoRA](https://github.com/AnswerDotAI/fsdp_qlora)** <a href="https://github.com/AnswerDotAI/fsdp_qlora/stargazers"><img src="https://img.shields.io/github/stars/AnswerDotAI/fsdp_qlora?style=social&color=white" alt="Stars"/></a>  
  Answer.AI's open-source framework combining PyTorch FSDP with 4-bit quantized parameters for efficient multi-GPU training and inference.

- **[AQLM](https://github.com/Vahe1994/AQLM)** <a href="https://github.com/Vahe1994/AQLM/stargazers"><img src="https://img.shields.io/github/stars/Vahe1994/AQLM?style=social&color=white" alt="Stars"/></a>  
  Additive Quantization for Large Language Models, delivering accurate extreme 2-bit and 3-bit multi-codebook vector compression with fast CUDA/Triton kernels.

- **[GPTQModel](https://github.com/ModelCloud/GPTQModel)** <a href="https://github.com/ModelCloud/GPTQModel/stargazers"><img src="https://img.shields.io/github/stars/ModelCloud/GPTQModel?style=social&color=white" alt="Stars"/></a>  
  Multi-backend model compression toolkit featuring hardware-accelerated quantization for NVIDIA CUDA, AMD ROCm, Intel XPU, and Apple Silicon.

- **[Marlin](https://github.com/IST-DASLab/marlin)** <a href="https://github.com/IST-DASLab/marlin/stargazers"><img src="https://img.shields.io/github/stars/IST-DASLab/marlin?style=social&color=white" alt="Stars"/></a>  
  Groundbreaking FP16xINT4 CUDA kernel achieving near-ideal 4x memory bandwidth speedup across batch sizes 16-32 tokens in batched LLM serving.

- **[HQQ](https://github.com/dropbox/hqq)** <a href="https://github.com/dropbox/hqq/stargazers"><img src="https://img.shields.io/github/stars/dropbox/hqq?style=social&color=white" alt="Stars"/></a>  
  Half-Quadratic Quantization: calibration-free, ultra-fast 1-bit to 4-bit weight compression library with custom Triton and CUDA fused kernels.

- **[QuIP#](https://github.com/Cornell-RelaxML/quip-sharp)** <a href="https://github.com/Cornell-RelaxML/quip-sharp/stargazers"><img src="https://img.shields.io/github/stars/Cornell-RelaxML/quip-sharp?style=social&color=white" alt="Stars"/></a>  
  2-bit and 4-bit lattice-based vector quantization with randomized Hadamard transforms and fast decoding kernels for extreme memory savings.

- **[bitdecoding-fp4](https://github.com/openbitsys/bitdecoding-fp4)** <a href="https://github.com/openbitsys/bitdecoding-fp4/stargazers"><img src="https://img.shields.io/github/stars/openbitsys/bitdecoding-fp4?style=social&color=white" alt="Stars"/></a>  
  Specialized open-source CUDA kernels and low-level decoding primitives optimized specifically for ultra-fast FP4 quantized LLM inference.

---

## 🛠️ How to Contribute

We welcome community contributions, benchmarks, and updates to ensure this directory remains the gold standard for quantized model inference! 🤝

1. 🍴 **Fork the repository** to your GitHub account.
2. 🌿 **Create a new branch** (`git checkout -b feature/add-new-tool`).
3. 📝 **Add or update entries** in `README.md` following the tabular or list format (ensure descriptions are factual, link to official sites, and badges follow conventions).
4. 💾 **Commit your changes** (`git commit -m "Add new FP4 inference engine"`).
5. 🚀 **Push to the branch** (`git push origin feature/add-new-tool`).
6. 📬 **Submit a Pull Request** with a concise explanation of the added tool or benchmark.

---

## 💖 Support & Sponsorship

If this curated repository saved you hours of research, reduced your VRAM footprint, or helped you scale high-throughput low-bit inference, please consider supporting the project:

- ⭐ **Star this repository** to help others discover it!
- 🍴 **Fork and share** it with your fellow ML systems engineers, kernel developers, and AI researchers.
- ☕ **Buy a coffee & sponsor**: Support continuous curation and development via the [GitHub Sponsor Dashboard](https://github.com/sponsors/ishandutta2007).

Thank you for being part of the open AI systems community! 🙌

---

## 📈 Star History

[![Star History Chart](https://star-history.dera.page/svg?repos=ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization&type=date&legend=top-left)](https://star-history.dera.page/#ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization&type=date&legend=top-left)
[![Star History Chart](https://www.star-history.com/svg?repos=ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Awesome-Quantized-Model-Inference-FP4-Optimization&type=date&legend=top-left)

---

## ⚠️ Disclaimer

- This is an **independently curated community list** and does not constitute an endorsement of any vendor, SaaS platform, or open-source software.
- Native hardware FP4 (`NVFP4` / `MXFP4`) tensor-core acceleration requires modern microarchitectures (such as NVIDIA Blackwell B200/GB200 or AMD CDNA4); older architectures utilize software emulation or mixed-precision W4A16 / Marlin execution.
- Always benchmark quantized models on domain-specific validation suites (perplexity, accuracy, needle-in-a-haystack, and reasoning tasks) prior to deploying into production.

---

<p align="center">
  <b>Built with ❤️ for ML systems engineers, CUDA/Triton kernel developers, AI infrastructure architects, and local LLM builders worldwide.</b>
</p>
