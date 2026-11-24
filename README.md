# Awesome-Quantized-Model-Inference-FP4-Optimization

# Awesome-Quantized-Model-Inference-FP4-Optimization

## Top Quantized Model Inference & FP4 Optimization Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on NVFP4 / MXFP4 / INT4 Quantization, High-Throughput LLM Serving, Custom CUDA Kernels & Low-Bit Inference*  

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Quantized Model Inference & FP4 Optimization**. These tools maximize LLM and multimodal throughput while slashing VRAM footprints using 4-bit floating-point formats (`NVFP4`, `MXFP4`), weight-only/activation quantization (`AWQ`, `GPTQ`, `FP8`, `GGUF`), speculative decoding, and fused attention/GEMM kernels.



**Examples** include vLLM, TensorRT-LLM, DeepSpeed, LMDeploy, Text Generation Inference (TGI), FlashAttention Cloud, ExLlamaV2, Aphrodite Engine, SGLang, Marlin, and `openbitsys/bitdecoding-fp4` (the category leaders). 



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosted low-bit inference engines, FP4/INT4 CUDA kernels, post-training quantization toolkits, and local CPU/GPU runtimes — ideal for ML systems engineers, kernel developers, AI infrastructure teams, and local LLM enthusiasts.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[NVIDIA NIM & TensorRT Cloud](https://nvidia.com)**  

  Enterprise-managed inference microservices featuring pre-optimized TensorRT-LLM engines with native Blackwell NVFP4 and Hopper FP8 acceleration.



- **[Together AI (Together Inference Engine)](https://together.ai)**  

  High-throughput cloud inference platform utilizing custom FP4/FP8 quantization and FlashAttention kernels for sub-second model serving.



- **[Fireworks AI](https://fireworks.ai)**  

  Low-latency generative AI inference cloud powered by custom quantized CUDA kernels (`FireAttention`) and speculative decoding pipelines.



- **[GroqCloud](https://groq.com)**  

  Hosted LPU (Language Processing Unit) inference service delivering deterministic, ultra-high-speed token generation with hardware-level low-precision execution.



- **[SambaNova Cloud](https://sambanova.ai)**  

  Cloud AI inference platform running massive quantized foundation models on Reconfigurable Dataflow Units (RDUs) with fast memory bandwidth.



- **[Baseten](https://baseten.co)**  

  Managed model deployment and inference infrastructure offering one-click TensorRT-LLM, vLLM, and FP4/FP8 quantized model autoscaling.



- **[Modal](https://modal.com)**  

  Serverless GPU cloud platform optimized for running custom vLLM, SGLang, TensorRT-LLM, and custom CUDA FP4 inference containers on demand.



- **[RunPod Serverless](https://runpod.io)**  

  Distributed GPU cloud offering pre-built, high-speed serverless endpoints for vLLM, ExLlamaV2, and quantized GGUF/AWQ models.



- **[Hugging Face Inference Endpoints (TGI Cloud)](https://huggingface.co)**  

  Dedicated managed cloud hosting backed by Text Generation Inference (TGI) with built-in BitsAndBytes, AWQ, GPTQ, and Marlin quantization.



- **[FriendliAI (Friendli Dedicated Endpoints)](https://friendli.ai)**  

  Commercial LLM serving engine and cloud platform featuring iteration-level batching and proprietary FP8/INT4/FP4 quantization pipelines.





## Open-Source GitHub Projects



- **[openbitsys/bitdecoding-fp4](https://github.com)**  

  High-performance open-source CUDA kernels and decoding primitives engineered specifically for ultra-fast FP4 quantized LLM inference.



- **[vLLM](https://github.com)**  

  Industry-standard open-source high-throughput LLM serving engine featuring PagedAttention, NVFP4/MXFP4, FP8, AWQ, GPTQ, and Marlin kernel integration.



- **[SGLang](https://github.com)**  

  Fast open-source serving framework for LLMs and VLMs featuring RadixAttention prefix caching, zero-overhead scheduling, and native FP4/FP8 quantization.



- **[NVIDIA TensorRT-LLM](https://github.com)**  

  Open-source library for assembling optimized LLM inference workflows with native Blackwell NVFP4, Hopper FP8, SmoothQuant, and in-flight batching.



- **[Marlin (IST-DASLab)](https://github.com)**  

  Ultra-fast open-source FP16xINT4 matrix-multiplication CUDA kernel achieving near-ideal 4x memory-bandwidth speedups for batched LLM inference.



- **[LMDeploy (InternLM)](https://github.com)**  

  Open-source toolkit for compressing, deploying, and serving LLMs/VLMs powered by the TurboMind C++/CUDA engine and W4A16/FP8 quantization.



- **[ExLlamaV2](https://github.com)**  

  High-speed open-source inference library for running EXL2 (mixed-precision 2-to-8 bit) and GPTQ quantized models locally on consumer GPUs.



- **[Hugging Face Text Generation Inference (TGI)](https://github.com)**  

  Production-grade open-source Rust and Python inference server supporting Marlin, EXL2, AWQ, GPTQ, EETQ, and FP8 quantization out of the box.



- **[DeepSpeed & DeepSpeed-FastGen](https://github.com)**  

  Microsoft's open-source deep learning optimization suite featuring ZeroQuant, SmoothQuant, and SplitFuse high-throughput quantized inference.



- **[Aphrodite Engine](https://github.com)**  

  Open-source large-scale inference engine built on vLLM with broad support for community quantization formats (GGUF, EXL2, IQ4, AQLM, QuIP#).



- **[llama.cpp](https://github.com)**  

  Premier open-source C/C++ LLM inference engine enabling 1.5-bit to 8-bit GGUF/IQ/MXFP4 quantized execution across NVIDIA, AMD, Apple Silicon, and CPUs.



- **[FlashAttention & FlashInfer](https://github.com)**  

  Open-source high-performance CUDA kernel libraries for IO-aware exact attention, FP8/FP4 KV-cache compression, and sparse/ragged decoding.



- **[AutoAWQ](https://github.com)**  

  Popular open-source Activation-Aware Weight Quantization (AWQ) toolkit for compressing LLMs to 4-bit with minimal accuracy degradation.



- **[GPTQModel (AutoGPTQ Successor)](https://github.com)**  

  Actively maintained open-source post-training quantization framework supporting GPTQ, Marlin, ExLlama, and hardware-accelerated 4-bit inference.



- **[LLM Compressor (Neural Magic / vLLM)](https://github.com)**  

  Unified open-source library for applying NVFP4, MXFP4, FP8, INT4/INT8 quantization, and sparsity directly for vLLM deployment.



- **[BitsAndBytes](https://github.com)**  

  Lightweight open-source CUDA wrapper enabling NF4 (NormalFloat 4-bit), FP4, and LLM.int8() quantized inference and QLoRA fine-tuning.



- **[HQQ (Half-Quadratic Quantization)](https://github.com)**  

  Calibration-free, ultra-fast open-source quantization toolkit supporting 1-bit to 4-bit weights with custom Triton and CUDA fused kernels.



### Additional Strong Open-Source Options



- **[MLC-LLM](https://github.com)** for compiling 3-bit and 4-bit quantized LLMs natively across WebGPU, iOS, Android, Vulkan, and CUDA.

- **[TorchAO (PyTorch Architecture Optimization)](https://github.com)** for native PyTorch-first `MXFP4`, `INT4`, `FP8`, and sparsity kernels integrated with `torch.compile`.

- **[QuIP#](https://github.com)** and **[AQLM](https://github.com)** for extreme 2-bit and 3-bit vector/lattice quantization with high perplexity retention.

- **[NVIDIA Model Optimizer (TensorRT ModelOpt)](https://github.com)** for open-source PTQ/QAT pipelines targeting `NVFP4` and `FP8` weights and KV caches.

- Many community **FP8/FP4 KV-cache quantization patches**, **Triton low-bit GEMM kernels**, and **speculative decoding (`EAGLE-3` / `Medusa`)** plugins for maximizing tokens per second.



**Frameworks for building custom systems**: Combine **LLM Compressor / TorchAO**, **vLLM** or **SGLang**, **FlashInfer**, and **Marlin / openbitsys/bitdecoding-fp4** with **llama.cpp** for ultra-dense, low-latency quantized inference across edge and datacenter GPUs.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Native hardware FP4 (`NVFP4` / `MXFP4`) tensor-core acceleration requires modern GPU architectures (e.g., NVIDIA Blackwell SM100/SM120 or AMD CDNA4/RDNA4); older GPUs fall back to software emulation or W4A16 (`INT4`/`Marlin`) kernels.

- Always benchmark quantized models on domain-specific evaluation suites (perplexity, reasoning, tool-calling accuracy) before deploying into production.



---



**Made for ML systems engineers, CUDA/Triton kernel developers, AI infrastructure architects, and local LLM builders.**  

Let's make model inference faster, leaner, and radically open.
