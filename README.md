<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp?version=0.3" width="80" border="0" alt="open-power">
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
    * [Others](#others)
* [Infrastructure](#infrastructure)
  * [Access Control](#access-control)
  * [Network Control](#network-control)
  * [Data Storage and Caching](#data-storage-and-caching)
  * [Delivery and Image Building](#delivery-and-image-building)
    * [CD](#cd)
    * [Container Capabilities](#container-capabilities)
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
    * [Toolkits](#toolkits)
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
| HunyuanImage-3.0 is a native multimodal autoregressive image generation model requiring substantial compute resources.             | [HunyuanImage-3.0](https://github.com/Tencent-Hunyuan/HunyuanImage-3.0)                         | [Proprietary License](https://github.com/Tencent-Hunyuan/HunyuanImage-3.0/blob/main/LICENSE) |
| HiDream-I1 is a 17B-parameter text-to-image foundation model using Sparse DiT architecture, supporting bilingual prompts, with Full / Dev / Fast variants. | [HiDream-I1](https://github.com/HiDream-ai/HiDream-I1)                                          | [MIT](#protocol-document-links)                      |

##### Video Generation

| Project Summary                                                        | Link (Click to Visit)               | License                              |
| ---------------------------------------------------------------------- | ----------------------------------- | ------------------------------------ |
| Alibaba's open-source video generation model family, available in multiple variants. | [Wan-Video](https://github.com/Wan-Video) | [Apache 2.0](#protocol-document-links) |
| LTX-Video is a DiT-based video generation model supporting image-to-video, multi-keyframe conditioning, video extension, and video-to-video transformations, with up to 4K resolution at 50 FPS. | [LTX-Video](https://github.com/Lightricks/ltx-video) | [Apache 2.0](#protocol-document-links) |

## AI Protocols and Standards

### Protocols

| Project Summary                                                                                                                                                | Type                | Link (Click to Visit)                                           | License                              |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | --------------------------------------------------------------- | ------------------------------------ |
| Model Context Protocol (MCP) is an open protocol for integrating LLM applications with external data sources and tools, defining a unified context exchange and client/server interaction model. | AI Protocol Standard | [MCP](https://github.com/modelcontextprotocol/modelcontextprotocol) | [MIT](#protocol-document-links)      |
| Agent2Agent (A2A) is an open protocol enabling communication and interoperability between opaque agentic applications, allowing agents to discover capabilities and collaborate on long-running tasks. | AI Protocol Standard | [A2A](https://github.com/a2aproject/A2A) | [Apache 2.0](#protocol-document-links) |
| Agent Client Protocol (ACP) standardizes communication between code editors and coding agents, providing SDKs in Kotlin, Java, Python, Rust, and TypeScript. | AI Protocol Standard | [ACP](https://github.com/agentclientprotocol/agent-client-protocol) | [Apache 2.0](#protocol-document-links) |

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
| An open-source project for text-to-speech generation.                          | Text-to-Speech | [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)      | [MIT](#protocol-document-links)      |
| Voxtral-4B-TTS is Mistral's open-weight multilingual text-to-speech model supporting 9 languages and zero-shot voice cloning from 3 seconds of reference audio, with ~70 ms latency. | Text-to-Speech | [Voxtral-4B-TTS](https://huggingface.co/mistralai/Voxtral-4B-TTS-2603) | [CC BY-NC 4.0](#protocol-document-links) |
| Fish Speech (Fish Audio S2 Pro) is a multilingual text-to-speech system with Dual-AR architecture and RL alignment, supporting natural language prosody control and multi-speaker generation across 80+ languages. | Text-to-Speech | [fish-speech](https://github.com/fishaudio/fish-speech) | [FISH AUDIO RESEARCH LICENSE](https://github.com/fishaudio/fish-speech/blob/main/LICENSE) |

### Coding Agents

| Project Summary                                                                                                                   | Main Features  | Link (Click to Visit)                          | License                              |
| --------------------------------------------------------------------------------------------------------------------------------- | -------------- | ---------------------------------------------- | ------------------------------------ |
| OpenCode is an open-source AI coding agent focused on terminal workflows and client/server architecture for local and remote execution. | AI Coding Agent | [opencode](https://github.com/anomalyco/opencode) | [MIT](#protocol-document-links)      |

### Others

| Project Summary                                                                               | Main Features | Link (Click to Visit)                                  | License                              |
| --------------------------------------------------------------------------------------------- | ------------- | ------------------------------------------------------ | ------------------------------------ |
| A ChatGPT-like web application for building a general-purpose chat UI on top of APIs.                | ChatGPT-like  | [open-webui](https://github.com/open-webui/open-webui) | [MIT](#protocol-document-links)      |

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
| An in-memory KV database and caching system for caching, messaging, and data structure workloads.                                              | [redis](https://github.com/redis/redis)             | KV-Cache   | [Proprietary License](https://github.com/redis/redis) |

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
| An in-memory cache library with simpler configuration than BigCache.                                                 | [freecache](https://github.com/coocood/freecache)         | [MIT](#protocol-document-links)      |
| A lock-free and concurrency-safe map.                                                                                | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#protocol-document-links)      |

### Toolkits

| Project Summary                                                                                                                                                             | Link (Click to Visit)                             | License                              |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|--------------------------------------|
| A Go implementation of ffmpeg-python. [FFmpeg](https://github.com/FFmpeg/FFmpeg) is an open-source audio and video processing library written in C.                       | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#protocol-document-links) |

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
| CC BY-NC 4.0             | https://creativecommons.org/licenses/by-nc/4.0/                                      |
| FISH AUDIO RESEARCH LICENSE | https://github.com/fishaudio/fish-speech/blob/main/LICENSE                        |
