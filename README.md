<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.svg" width="80" border="0" alt="open-power">
  </a>
</p>

Other languages: [简体中文](README_zh.md)

# open-power

> A curated open-source technology selection index focused on AI models, MCP, coding agents, infrastructure, and language ecosystems.

Covering open-source projects, protocols, and toolchains for research, comparison, and technology selection.

This project uses AI tools to assist with documentation editing. All project selections and curation are performed 100% manually.

# Table of Contents

<!-- TOC -->
* [open-power](#open-power)
* [Table of Contents](#table-of-contents)
* [AI](#ai)
  * [AI Models](#ai-models)
    * [Large Language Models and Multimodal Models](#large-language-models-and-multimodal-models)
    * [Generative AI Models](#generative-ai-models)
      * [Image Generation Models](#image-generation-models)
        * [Image Generation](#image-generation)
        * [Video Generation](#video-generation)
  * [AI Protocols and Standards](#ai-protocols-and-standards)
    * [Protocols](#protocols)
  * [AI Workflows](#ai-workflows)
  * [AI Tools](#ai-tools)
    * [Image Generation](#image-generation-1)
    * [Audio Processing](#audio-processing)
      * [Audio Separation and Noise Reduction](#audio-separation-and-noise-reduction)
      * [Voice Conversion](#voice-conversion)
      * [Text to Speech](#text-to-speech)
    * [Coding Agents](#coding-agents)
    * [OCR](#ocr)
* [Infrastructure](#infrastructure)
  * [Access Control](#access-control)
  * [Network Control](#network-control)
  * [Data Storage and Caching](#data-storage-and-caching)
  * [Delivery and Image Building](#delivery-and-image-building)
    * [CD](#cd)
    * [Container Capabilities](#container-capabilities)
  * [Toolkits](#toolkits)
* [Language Capabilities](#language-capabilities)
  * [Cross-Language Frameworks](#cross-language-frameworks)
    * [RPC](#rpc)
  * [Python](#python)
    * [AI Capabilities](#ai-capabilities)
      * [LLM Application Frameworks](#llm-application-frameworks)
      * [Model Training and Inference Tools](#model-training-and-inference-tools)
      * [Algorithm Frameworks](#algorithm-frameworks)
  * [Golang](#golang)
    * [AI Capabilities](#ai-capabilities-1)
      * [LLM Application Frameworks](#llm-application-frameworks-1)
    * [Basic Capabilities](#basic-capabilities)
    * [HTTP](#http)
      * [Server](#server)
      * [Client](#client)
    * [RPC](#rpc-1)
      * [Server](#server-1)
    * [Service Frameworks](#service-frameworks)
    * [GUI](#gui)
    * [OS Interfaces](#os-interfaces)
* [Java](#java)
  * [Android](#android)
    * [Permission Management](#permission-management)
* [Fonts](#fonts)
* [License Source Links](#protocol-document-links)
<!-- TOC -->

# AI

## AI Models

### Large Language Models and Multimodal Models

Multimodal models are usually extended from large language models.

| Project Summary                                                                                           | Multimodal                    | Link (Click to Visit)                      | License Status      |
| --------------------------------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------ | ------------------- |
| DeepSeek is an open-source model family covering reasoning and multimodal directions.                     | Experimental multimodal lines | [deepseek](https://github.com/deepseek-ai) | Depends on the model |
| Qwen is Alibaba's open-source model family, covering text, image understanding, audio, math, and code.  | Multimodal versions available | [QwenLM](https://github.com/QwenLM)        | Depends on the model |
| GLM is an open-source model family from zai-org, covering general-purpose, multimodal, and agent use.   | Multimodal versions available | [GLM](https://huggingface.co/zai-org)      | Depends on the model |
| Kimi is an open-source model family from Moonshot AI, covering general and reasoning-oriented models.    | Multimodal versions available | [KIMI](https://github.com/MoonshotAI)      | Depends on the model |
| Gemma is an open-weights large language model family by Google DeepMind, based on Gemini research and technology, with a JAX library for inference and fine-tuning. | Multimodal versions available | [gemma](https://github.com/google-deepmind/gemma) | [Apache 2.0](#protocol-document-links) |

### Generative AI Models

#### Image Generation Models

##### Image Generation

| Project Summary                                                                                                                       | Link (Click to Visit)                                                                           | License                                 |
| ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | --------------------------------------- |
| Stable Diffusion v1-5 is an image generation base model compatible with WebUI, ComfyUI, LoRA, and ControlNet workflows.           | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#protocol-document-links)   |
| Stable Diffusion XL Base 1.0 is a high-resolution image generation base model compatible with common SDXL tooling and workflows.   | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#protocol-document-links) |
| Alibaba's unified text-to-image generation and image editing model, with a 7B-parameter visual component built on 32 single-stream DiT layers, supporting text rendering, native RGBA transparent generation, and editing with up to 10 reference images, at resolutions up to 2752×1536. | [Qwen-Image-2.1](https://huggingface.co/Qwen/Qwen-Image-2.1) | [Qwen Research License](#protocol-document-links) |

##### Video Generation

| Project Summary                                                        | Link (Click to Visit)               | License                              |
| ---------------------------------------------------------------------- | ----------------------------------- | ------------------------------------ |
| MiniMax's synchronized audio-video generation model built on a 33B-parameter dense single-stream Transformer, supporting text-to-video, first/last-frame-to-video, and omni-reference conditioning with up to 12 mixed reference files, outputting 4–15 seconds at 24 FPS up to 2K resolution, with dialogue support in 11 languages. | [MiniMax-H3](https://huggingface.co/MiniMaxAI/MiniMax-H3) | [MiniMax H3 Community License](#protocol-document-links) |

## AI Protocols and Standards

### Protocols

| Project Summary                                                                                                                                                | Type                | Link (Click to Visit)                                           | License                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | --------------------------------------------------------------- | ------------------------------------ |
| Model Context Protocol (MCP) is an open protocol for integrating LLM applications with external data sources and tools, defining a unified context exchange and client/server interaction model. | AI Protocol Standard | [MCP](https://github.com/modelcontextprotocol/modelcontextprotocol) | [MIT](#protocol-document-links)      |
| Agent2Agent (A2A) is an open protocol enabling communication and interoperability between opaque agentic applications, allowing agents to discover capabilities and collaborate on long-running tasks. | AI Protocol Standard | [A2A](https://github.com/a2aproject/A2A) | [Apache 2.0](#protocol-document-links) |
| Agent Client Protocol (ACP) standardizes communication between code editors and coding agents, providing SDKs in Kotlin, Java, Python, Rust, and TypeScript. | AI Protocol Standard | [ACP](https://github.com/agentclientprotocol/agent-client-protocol) | [Apache 2.0](#protocol-document-links) |
| Agent Skills is an open specification, originally developed by Anthropic, for packaging agent capabilities: a skill is a folder containing a SKILL.md file with name/description metadata plus instructions, optionally bundling scripts, references, and assets, loaded via progressive disclosure across discovery, activation, and execution. | AI Protocol Standard | [Agent Skills](https://github.com/agentskills/agentskills) | [Apache 2.0](#protocol-document-links) |

## AI Workflows

| Project Summary                                                                                                                          | Main Features | Link (Click to Visit)                             | License                              |
| ---------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ------------------------------------------------- | ------------------------------------ |
| ComfyUI is a low-code node-based workflow tool for generative AI, supporting community workflows and plugins.                            | AI Workflow   | [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | [GPL 3.0](#protocol-document-links)  |

## AI Tools

### Image Generation

| Project Summary                                                                                                      | Main Features    | Link (Click to Visit)                                                             | License                              |
| -------------------------------------------------------------------------------------------------------------------- | ---------------- | --------------------------------------------------------------------------------- | ------------------------------------ |
| Stable-diffusion-webui is an image generation web UI supporting plugins and extensions for video-related workflows.                    | Image Generation | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#protocol-document-links) |

### Audio Processing

#### Audio Separation and Noise Reduction

| Project Summary                                                    | Main Features                    | Link (Click to Visit)                                     | License                              |
| ------------------------------------------------------------------ | -------------------------------- | --------------------------------------------------------- | ------------------------------------ |
| An integrated audio processing project covering common separation and noise reduction capabilities. | Audio Separation/Noise Reduction | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI) | [AGPL 3.0](#protocol-document-links) |

#### Voice Conversion

| Project Summary                                  | Main Features    | Link (Click to Visit)                                                              | License                              |
| ------------------------------------------------ | ---------------- | ----------------------------------------------------------------------------------- | ------------------------------------ |
| An open-source project for voice conversion workflows.                | Voice Conversion | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#protocol-document-links)      |

#### Text to Speech

| Project Summary                                          | Main Features  | Link (Click to Visit)                                     | License                              |
| -------------------------------------------------------- | -------------- | --------------------------------------------------------- | ------------------------------------ |
| Alibaba's open-source text-to-speech model built on Qwen3-TTS-Tokenizer-12Hz with a discrete multi-codebook LM and a lightweight non-DiT architecture, supporting zero-shot voice cloning from 3 seconds of reference audio, streaming generation with first-packet latency as low as 97 ms, and ten languages: Chinese, English, Japanese, Korean, German, French, Russian, Portuguese, Spanish, and Italian. | Text-to-Speech | [Qwen3-TTS-12Hz-1.7B-Base](https://huggingface.co/Qwen/Qwen3-TTS-12Hz-1.7B-Base) | [Apache 2.0](#protocol-document-links) |

### Coding Agents

| Project Summary                                                                                                                   | Main Features  | Link (Click to Visit)                          | License                              |
| --------------------------------------------------------------------------------------------------------------------------------- | -------------- | ---------------------------------------------- | ------------------------------------ |
| Pi is an AI agent toolkit and coding-agent harness; its TypeScript monorepo splits a unified multi-provider LLM API, agent runtime, differential-rendering TUI, and coding agent CLI into separate packages. | AI Coding Agent | [pi](https://github.com/earendil-works/pi) | [MIT](#protocol-document-links) |
| DeepSeek's open-source agent harness (CLI: dsh) built on an everything-is-a-plugin architecture, with a built-in web UI and a plugin ecosystem tracked via the dsh-plugin topic. | AI Coding Agent | [deepseek-harness](https://github.com/deepseek-ai/deepseek-harness) | [MIT](#protocol-document-links) |
| YYLO is a command-line orchestrator for coding agents, repeatable workflows, and receipt-backed repository changes. It is for developers who want a quick agent loop and for project operators who need typed task, validation, merge, and release-readiness boundaries. | AI Coding Agent | [yylo](https://github.com/yylo-dev/yylo) | [MIT](#protocol-document-links) |

### OCR

| Project Summary | Main Features | Link (Click to Visit) | License |
| --------------- | ------------- | --------------------- | ------- |
| light-ocr is a fast offline OCR toolkit for Node.js and C++, using PP-OCRv6 with a bundled OCR runtime and optional Core ML and WebGPU hardware acceleration. | OCR | [light-ocr](https://github.com/arcships/light-ocr) | [Apache 2.0](#protocol-document-links) |

# Infrastructure

## Access Control

| Project Summary                                                   | Type                    | Link (Click to Visit)                         | License                              |
| ----------------------------------------------------------------- | ----------------------- | --------------------------------------------- | ------------------------------------ |
| Casbin is an open-source access control library supporting common models such as RBAC and ABAC. | Permission Management   | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#protocol-document-links) |
| An identity and authentication project (IAM/SSO) from the same ecosystem as Casbin. | Identity Authentication | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#protocol-document-links) |

## Network Control

| Project Summary                                                        | Type                 | Link (Click to Visit)                  | License                              |
| ---------------------------------------------------------------------- | -------------------- | -------------------------------------- | ------------------------------------ |
| NPS can be used to build an intranet penetration proxy with a web-based backend. | Intranet Penetration | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#protocol-document-links)  |

## Data Storage and Caching

| Project Summary                                                                                                                                | Link (Click to Visit)                               | Type       | License                                               |
| ---------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ---------- | ----------------------------------------------------- |
| TiDB is a financial-grade distributed database compatible with the MySQL API, supporting both OLAP and OLTP.                                  | [tidb](https://github.com/pingcap/tidb)             | New-SQL-DB | [Apache 2.0](#protocol-document-links)                |
| OceanBase Database is a distributed relational database developed by Ant Group, based on Paxos and a distributed architecture for HA and linear scaling. | [oceanbase](https://github.com/oceanbase/oceanbase) | New-SQL-DB | [Mulan PubL v2](#protocol-document-links)             |
| Qdrant is a vector database written in Rust for distributed deployments.                                                                        | [qdrant](https://github.com/qdrant/qdrant)          | Vector-DB  | [Apache 2.0](#protocol-document-links)                |
| Milvus is a vector database written in Go and C++ for distributed deployments.                                                                  | [milvus](https://github.com/milvus-io/milvus)       | Vector-DB  | [Apache 2.0](#protocol-document-links)                |
| An open-source column-oriented DBMS for real-time analytics, executing SQL queries over columnar storage with data compression, supporting distributed deployments, primarily implemented in C++. | [clickhouse](https://github.com/ClickHouse/ClickHouse) | OLAP-DB | [Apache 2.0](#protocol-document-links) |
| An in-memory data structure server forked from Redis 7.2.4 and hosted by the Linux Foundation (LF Projects), compatible with the Redis protocol and API, supporting Lua, Sentinel, Cluster, and the module API. | [valkey](https://github.com/valkey-io/valkey)       | KV-Cache   | [BSD 3](#protocol-document-links)         |

## Delivery and Image Building

### CD

| Project Summary                                                                                                                   | Link (Click to Visit)                           | License                              |
| --------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- | ------------------------------------ |
| Kubernetes is a platform for container orchestration and cluster management, supporting declarative deployment, service discovery, autoscaling, self-healing, and rolling updates.            | [k8s](https://github.com/kubernetes/kubernetes) | [Apache 2.0](#protocol-document-links) |

### Container Capabilities

| Project Summary                                                                                                                              | Link (Click to Visit)                                  | License                              |
| -------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------ |
| containerd is a container runtime responsible for image pulling, container lifecycle management, and execution. It can be used as the runtime for Kubernetes nodes and also in local or single-node environments.                            | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#protocol-document-links) |
| BuildKit is an image build toolkit supporting cache reuse, parallel builds, multi-platform builds, and rootless execution. Docker Engine 23.0 and later use Buildx/BuildKit by default for `docker build`. | [buildkit](https://github.com/moby/buildkit)           | [Apache 2.0](#protocol-document-links) |

## Toolkits

| Project Summary                                                                                                                                                              | Link (Click to Visit)              | License                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- | ---------------------------------------------- |
| Open-source audio/video codec and processing framework implemented in C, comprising the libavcodec, libavformat, libavutil, libavfilter, libavdevice, libswresample and libswscale libraries plus the ffmpeg, ffplay and ffprobe command-line tools, covering mainstream container formats, streaming protocols and codecs. | [ffmpeg](https://github.com/FFmpeg/FFmpeg) | [LGPL 2.1+ / GPL 2.0+](#protocol-document-links) |

# Language Capabilities

## Cross-Language Frameworks

### RPC

| Project Summary                                                                                                               | Link (Click to Visit)                      | License                              |
| ----------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------ |
| gRPC is a cross-language RPC framework from Google, based on HTTP/2 and supporting bidirectional streaming, timeouts, authentication, and code generation. | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#protocol-document-links) |
| Thrift was originally developed at Facebook and is now an Apache Foundation project, providing IDL, code generation, and replaceable transport and protocol layers. | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#protocol-document-links) |

## Python

### AI Capabilities

#### LLM Application Frameworks

| Project Summary                                                                                                                     | Link (Click to Visit)                                  | License                              |
| ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------ |
| LangChain is a framework for developing and managing applications based on large language models, with standardized interfaces and toolchains for model interaction, data processing, and application development. | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#protocol-document-links)      |

#### Model Training and Inference Tools

| Project Summary                                                                                                           | Link (Click to Visit)                                  | License                              |
| ------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------ |
| Diffusers is Hugging Face's open-source training and inference toolkit for diffusion models, covering images, audio, and 3D workloads. | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#protocol-document-links) |
| Unsloth is a local training and inference toolkit for open models, supporting fine-tuning, reinforcement learning, export, and unified local interfaces, with a focus on low VRAM usage and training efficiency. | [unsloth](https://github.com/unslothai/unsloth)        | [Multiple Licenses](https://github.com/unslothai/unsloth) |
| vLLM is a large language model inference and serving engine originating from UC Berkeley's Sky Computing Lab, managing the KV cache with PagedAttention and supporting continuous batching, chunked prefill, prefix caching, speculative decoding, and FP8, INT4, GPTQ, AWQ, and GGUF quantization, covering 200+ Hugging Face model architectures on NVIDIA, AMD, and Intel hardware with an OpenAI-compatible API. | [vllm](https://github.com/vllm-project/vllm) | [Apache 2.0](#protocol-document-links) |
| SGLang is an LLM and multimodal model serving framework from LMSYS, using RadixAttention prefix caching and a zero-overhead CPU scheduler, supporting prefill-decode disaggregation, speculative decoding, structured output, and FP8, INT4, AWQ, and GPTQ quantization on NVIDIA, AMD, Intel, TPU, and Ascend hardware, compatible with the OpenAI API. | [sglang](https://github.com/sgl-project/sglang) | [Apache 2.0](#protocol-document-links) |
| LMDeploy is an OpenMMLab toolkit for compressing, deploying, and serving LLMs, built on TurboMind and PyTorch inference engines, supporting persistent batching, blocked KV cache, 4-bit/AWQ weight quantization and KV cache quantization, tensor parallelism, CUDA graphs, and prefill-decode disaggregation on NVIDIA GPUs and Huawei Ascend, covering InternLM, Qwen, Llama, and DeepSeek models. | [lmdeploy](https://github.com/InternLM/lmdeploy) | [Apache 2.0](#protocol-document-links) |

#### Algorithm Frameworks

| Project Summary                                                                                             | Link (Click to Visit)                                  | License                                                                     |
| ----------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------- |
| PyTorch is a deep learning framework with open governance under the PyTorch Foundation.               | [pytorch](https://github.com/pytorch/pytorch)          | [Proprietary License](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow is Google's engineered machine learning framework covering training, inference, deployment, and mobile scenarios. | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#protocol-document-links)                                      |
| JAX is a high-performance array computing and program transformation library for accelerators, focused on JIT compilation, autodiff, vectorization, and parallelization. | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#protocol-document-links)                                      |

## Golang

### AI Capabilities

#### LLM Application Frameworks

| Project Summary                                                                                           | Link (Click to Visit)                     | License                              |
| --------------------------------------------------------------------------------------------------------- | ----------------------------------------- | ------------------------------------ |
| Eino is ByteDance's open-source Go toolchain framework for large model applications, comparable to LangChain. | [eino](https://github.com/cloudwego/eino) | [Apache 2.0](#protocol-document-links) |

### Basic Capabilities

| Project Summary                                                                                                      | Link (Click to Visit)                                     | License                              |
| -------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- | ------------------------------------ |
| A Go coroutine pool library.                                                                                         | [ants](https://github.com/panjf2000/ants)                 | [MIT](#protocol-document-links)      |
| A Go library for parsing between maps and structs.                                                                   | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#protocol-document-links)      |
| Sonic is a JSON library using JIT and SIMD acceleration to provide serialization and deserialization without code generation.                    | [sonic](https://github.com/bytedance/sonic)               | [Apache 2.0](#protocol-document-links) |
| An in-memory cache library that supports configuring a maximum cache size.                                           | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#protocol-document-links) |
| A lock-free and concurrency-safe map.                                                                                | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#protocol-document-links)      |

### HTTP

#### Server

| Project Summary                                                                                                                                    | Link (Click to Visit)                       | License                              |
|----------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|--------------------------------------|
| Hertz is ByteDance's open-source Go microservice HTTP framework for production services.                                                  | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#protocol-document-links) |

#### Client

| Project Summary                      | Link (Click to Visit)                      | License                         |
|--------------------------------------|--------------------------------------------|---------------------------------|
| An HTTP client library.          | [resty](https://github.com/go-resty/resty) | [MIT](#protocol-document-links) |

### RPC

#### Server

| Project Summary                                                                                                                                       | Link (Click to Visit)                    | License                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------|--------------------------------------|
| Kitex is ByteDance's open-source Go RPC framework, supporting Thrift, Kitex Protobuf, and gRPC, with code generation, governance extensions, and streaming support. | [kitex](https://github.com/cloudwego/kitex) | [Apache 2.0](#protocol-document-links) |

### Service Frameworks

| Project Summary                                                                                                                                        | Link (Click to Visit)                      | License                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|---------------------------------|
| Kratos is a Go framework for microservices, with built-in support for HTTP and gRPC plus foundational capabilities such as project layout, config, logging, service discovery, and middleware. | [kratos](https://github.com/go-kratos/kratos) | [MIT](#protocol-document-links) |

### GUI

| Project Summary                                                                                                     | Link (Click to Visit)                   | License                           |
|---------------------------------------------------------------------------------------------------------------------|-----------------------------------------|-----------------------------------|
| Fyne is a Go GUI framework supporting desktop and mobile application development with unified widgets, layout, and packaging. | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#protocol-document-links) |

### OS Interfaces

| Project Summary                                                                                                                                   | Link (Click to Visit)                          | License                           |
|---------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|-----------------------------------|
| Gopsutil is a library for system monitoring, analysis, limiting process resources, and managing processes. It is the Go implementation of Python's [psutil](https://github.com/giampaolo/psutil). | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#protocol-document-links) |

# Java

## Android

### Permission Management

| Project Summary                              | Link (Click to Visit)                                         | License                              |
|----------------------------------------------|---------------------------------------------------------------|--------------------------------------|
| An Android permission request library. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#protocol-document-links) |

# Fonts

| Project Summary    | Language     | Commercial Use | Link                                                        | License                                                      |
|--------------------|--------------|----------------|-------------------------------------------------------------|--------------------------------------------------------------|
| Google Free Fonts  | Multilingual | Mostly Allowed | [fonts.google.com](https://fonts.google.com)                | [Multiple Licenses](https://developers.google.com/fonts/faq) |
| Alibaba Free Fonts | Chinese      | Mostly Allowed | [www.alibabafonts.co](https://www.alibabafonts.com)         | [Proprietary License](https://www.alibabafonts.com/#/more)   |

<a id="protocol-document-links"></a>

# License Source Links

| License                  | Original Link                                                                        |
|--------------------------|--------------------------------------------------------------------------------------|
| MIT                      | https://opensource.org/license/mit                                                   |
| AGPL 3.0                 | https://www.gnu.org/licenses/agpl-3.0.txt                                            |
| GPL 3.0                  | https://www.gnu.org/licenses/gpl-3.0.txt                                             |
| Apache 2.0               | https://www.apache.org/licenses/LICENSE-2.0.txt                                      |
| BSD 3                    | https://opensource.org/license/bsd-3-clause                                          |
| CreativeML Open RAIL-M   | https://github.com/CompVis/stable-diffusion/blob/main/LICENSE                        |
| CreativeML Open RAIL++-M | https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/blob/main/LICENSE.md |
| OFL1.1 2007              | https://openfontlicense.org/documents/OFL.txt                                        |
| Mulan PubL v2            | https://license.coscl.org.cn/MulanPubL-2.0                                            |
| Qwen Research License    | https://huggingface.co/Qwen/Qwen-Image-2.1/blob/main/LICENSE                       |
| MiniMax H3 Community License | https://huggingface.co/MiniMaxAI/MiniMax-H3/blob/main/LICENSE                  |
| LGPL 2.1+ / GPL 2.0+   | https://github.com/FFmpeg/FFmpeg/blob/master/LICENSE.md                                      |
