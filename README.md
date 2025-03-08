<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp?version=0.1" width="400" border="0" alt="open-power">
  </a>
</p>

Other languages: [简体中文](README_zh.md), (Currently unable to translate more)

# open-power

This repository is used to record open source projects that excel in factors such as productivity, performance,
stability, or design.

You can quickly find the technology stack you need here.

Discussions and contributions are welcome.

# Index

<!-- TOC -->
* [open-power](#open-power)
* [Index](#index)
* [Projects](#projects)
  * [AI](#ai)
    * [AI Middleware](#ai-middleware)
    * [AI Tools](#ai-tools)
      * [General Tools](#general-tools)
      * [Image Processing](#image-processing)
      * [Audio Processing](#audio-processing)
      * [Others](#others)
  * [Access Control](#access-control)
  * [Network Control](#network-control)
  * [Message Middleware](#message-middleware)
  * [OPS](#ops)
  * [CI/CD](#cicd)
    * [CD](#cd)
    * [Container Runtime](#container-runtime)
* [AI Models](#ai-models)
  * [Generative AI Models](#generative-ai-models)
    * [Image Generation](#image-generation)
      * [Image Generation](#image-generation-1)
      * [Video Generation](#video-generation)
    * [LLMs & Multimodal Models](#llms--multimodal-models)
* [Language Capabilities](#language-capabilities)
  * [Cross-Language Frameworks](#cross-language-frameworks)
    * [RPC](#rpc)
  * [Python](#python)
    * [AI Capabilities](#ai-capabilities)
      * [AI Libraries](#ai-libraries)
      * [ML Frameworks](#ml-frameworks)
  * [Golang](#golang)
    * [AI Capabilities](#ai-capabilities-1)
      * [AI Libraries](#ai-libraries-1)
    * [Core Libraries](#core-libraries)
    * [Utilities](#utilities)
    * [HTTP](#http)
    * [GUI](#gui)
    * [OS Interfaces](#os-interfaces)
* [Java](#java)
  * [Android](#android)
    * [Permissions](#permissions)
* [Fonts](#fonts)
* [Protocol document link](#protocol-document-link)
<!-- TOC -->

# Projects

## AI

### AI Middleware

| Brief Description                                                                                                                                                                                                     | Main Features | Link (Click to Visit)                      | License                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|--------------------------------------------|---------------------------------------------------------|
| Dify is currently the most powerful (as of 20250309) open-source AI platform, capable of defining workflows, agent templates, etc. The project is not fully based on Apache 2.0 and has limitations on multi-tenancy. | AI Middleware | [dify](https://github.com/langgenius/dify) | [Multiple Licenses](https://github.com/langgenius/dify) |

### AI Tools

#### General Tools

| Brief Description                                                                                         | Main Features | Link (Click to Visit)                                | License                            |
|-----------------------------------------------------------------------------------------------------------|---------------|------------------------------------------------------|------------------------------------|
| A production-grade low-code node-based AI workflow editor with extensive community templates and plugins. | AI Workflow   | [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | [GPL 3.0](#Protocol-document-link) |

#### Image Processing

| Brief Description                                                                                                                                     | Main Features | Link (Click to Visit)                                                             | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|-----------------------------------------------------------------------------------|-------------------------------------|
| Stable-diffusion-webui provides a one-click web interface for AI image generation, with plugin support for video generation and a thriving ecosystem. | Image Gen     | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#Protocol-document-link) |
| A classic face-swapping project. Legal risks apply.                                                                                                   | Image Proc    | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                            | [GPL 3.0](#Protocol-document-link)  |

#### Audio Processing

| Brief Description                                                                                                | Main Features     | Link (Click to Visit)                                                              | License                               |
|------------------------------------------------------------------------------------------------------------------|-------------------|------------------------------------------------------------------------------------|---------------------------------------|
| A more powerful audio processing toolkit than UVR5-UI, actively maintained (as of 2025-02-22).                   | Audio Sep/Denoise | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#Protocol-document-link)   |
| An actively maintained SVC project (as of 2025-02-22) with out-of-the-box usability.                             | Voice Conversion  | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#Protocol-document-link)        |
| State-of-the-art text-to-speech system with active community (as of 2025-03-09).                                 | TTS               | [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)                               | [MIT](#Protocol-document-link)        |
| Currently one of the best text-to-speech systems still being updated, with an active community (as of 20250309). | TTS               | [CosyVoice](https://github.com/FunAudioLLM/CosyVoice)                              | [Apache 2.0](#Protocol-document-link) |

#### Others

| Brief Description                                                                                        | Main Features | Link (Click to Visit)                                                      | License                               |
|----------------------------------------------------------------------------------------------------------|---------------|----------------------------------------------------------------------------|---------------------------------------|
| A LangChain-based LLM project supporting RAG and Agent features (improved version of Langchain-ChatGLM). | ChatGPT-like  | [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) | [Apache 2.0](#Protocol-document-link) |
| An out-of-the-box ChatGPT-like project (API-based) with extensive features for rapid deployment.         | ChatGPT-like  | [open-webui](https://github.com/open-webui/open-webui)                     | [MIT](#Protocol-document-link)        |

## Access Control

| Brief Description                                                                         | Type  | Link (Click to Visit)                         | License                               |
|-------------------------------------------------------------------------------------------|-------|-----------------------------------------------|---------------------------------------|
| Casbin: A powerful and efficient open-source access control library supporting RBAC/ABAC. | AuthZ | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#Protocol-document-link) |
| Casdoor: Identity management (IAM/SSO) from the same developers as Casbin.                | AuthN | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#Protocol-document-link) |

## Network Control

| Brief Description                                          | Type          | Link (Click to Visit)                  | License                            |
|------------------------------------------------------------|---------------|----------------------------------------|------------------------------------|
| NPS: Intranet penetration proxy with web-based management. | Intranet Tool | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#Protocol-document-link) |

## Message Middleware

| Brief Description                                                                                         | Link (Click to Visit)                               | Type       | License                                          |
|-----------------------------------------------------------------------------------------------------------|-----------------------------------------------------|------------|--------------------------------------------------|
| TiDB: A financial-grade distributed SQL database with MySQL compatibility, supporting both OLAP and OLTP. | [tidb](https://github.com/pingcap/tidb)             | New-SQL-DB | [Apache 2.0](#Protocol-document-link)            |
| OceanBase: Ant Group's distributed relational database based on Paxos protocol.                           | [oceanbase](https://github.com/oceanbase/oceanbase) | New-SQL-DB | [Mulan PubL v2](#Protocol-document-link)         |
| Qdrant: Rust-based vector database with distributed capabilities.                                         | [qdrant](https://github.com/qdrant/qdrant)          | Vector-DB  | [Apache 2.0](#Protocol-document-link)            |
| Milvus: Go/C++ vector database with distributed capabilities.                                             | [milvus](https://github.com/milvus-io/milvus)       | Vector-DB  | [Apache 2.0](#Protocol-document-link)            |
| Redis: The de facto standard for in-memory key-value caching.                                             | [redis](https://github.com/redis/redis)             | KV-Cache   | [Custom License](https://github.com/redis/redis) |

## OPS

## CI/CD

### CD

| Brief Description                                                                                                       | Link (Click to Visit)                           | License                               |
|-------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|---------------------------------------|
| Kubernetes: The industry-standard container orchestration system, evolving toward stateful and GPU workload management. | [k8s](https://github.com/kubernetes/kubernetes) | [Apache 2.0](#Protocol-document-link) |

### Container Runtime

| Brief Description                                                                               | Link (Click to Visit)                                  | License                               |
|-------------------------------------------------------------------------------------------------|--------------------------------------------------------|---------------------------------------|
| Containerd: Container runtime for starting/stopping containers, typically used with Kubernetes. | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#Protocol-document-link) |

# AI Models

## Generative AI Models

### Image Generation

#### Image Generation

| Brief Description                                                                                     | Link (Click to Visit)                                                                           | License                                             |
|-------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| Stable Diffusion v1-5: The most toolchain-mature foundational image model (as of 2025-02-22).         | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#Protocol-document-link)   |
| Stable Diffusion XL 1.0: Stability AI's HD version with growing toolchain support (as of 2025-02-22). | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#Protocol-document-link) |

#### Video Generation

| Brief Description                                        | Link (Click to Visit)                         | License                                           |
|----------------------------------------------------------|-----------------------------------------------|---------------------------------------------------|
| CogVideo: Video generation model by Tsinghua University. | [CogVideo](https://github.com/THUDM/CogVideo) | [Multiple Licenses](https://huggingface.co/THUDM) |

### LLMs & Multimodal Models

| Brief Description                                                                                      | Multimodal | Link (Click to Visit)                      | License                                                                                     |
|--------------------------------------------------------------------------------------------------------|------------|--------------------------------------------|---------------------------------------------------------------------------------------------|
| DeepSeek: Leading LLM with multimodal capabilities.                                                    | Yes        | [deepseek](https://github.com/deepseek-ai) | [MIT](#Protocol-document-link)                                                              |
| LLaMA: Meta's foundational LLM with rich open-source ecosystem.                                        | Partial    | [Llama](https://www.llama.com/)            | [Custom License](https://www.llama.com/docs/how-to-guides/responsible-use-guide-resources/) |
| Qwen: Alibaba's LLM series with multimodal support (image/audio/math/code).                            | Yes        | [QwenLM](https://github.com/QwenLM)        | [Multiple Licenses](https://huggingface.co/Qwen)                                            |
| GLM: Tsinghua University's LLM with multimodal capabilities. May be deprecated in 2025 if not updated. | Yes        | [GLM4](https://github.com/THUDM/GLM-4)     | [Multiple Licenses](https://huggingface.co/THUDM)                                           |

# Language Capabilities

## Cross-Language Frameworks

### RPC

| Brief Description                                                              | Link (Click to Visit)                      | License                               |
|--------------------------------------------------------------------------------|--------------------------------------------|---------------------------------------|
| gRPC: Google's high-performance cross-language RPC framework using HTTP/2.     | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#Protocol-document-link) |
| Thrift: Meta's flexible cross-language RPC framework without native streaming. | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#Protocol-document-link) |

## Python

### AI Capabilities

#### AI Libraries

| Brief Description                                                                                     | Link (Click to Visit)                                  | License                               |
|-------------------------------------------------------------------------------------------------------|--------------------------------------------------------|---------------------------------------|
| Diffusers: Hugging Face's library for state-of-the-art diffusion models (images/audio/3D structures). | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#Protocol-document-link) |
| LangChain: Framework for LLM application development with standardized interfaces and toolchains.     | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#Protocol-document-link)        |

#### ML Frameworks

| Brief Description                                                      | Link (Click to Visit)                                  | License                                                                |
|------------------------------------------------------------------------|--------------------------------------------------------|------------------------------------------------------------------------|
| PyTorch: Meta's user-friendly ML framework for beginners.              | [pytorch](https://github.com/pytorch/pytorch)          | [Custom License](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow: Google's production-grade ML framework.                    | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#Protocol-document-link)                                  |
| JAX: Google's high-performance ML framework with steep learning curve. | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#Protocol-document-link)                                  |

## Golang

### AI Capabilities

#### AI Libraries

| Brief Description                                           | Link (Click to Visit)                     | License                               |
|-------------------------------------------------------------|-------------------------------------------|---------------------------------------|
| Eino: ByteDance's Go LLM framework (LangChain alternative). | [eino](https://github.com/cloudwego/eino) | [Apache 2.0](#Protocol-document-link) |

### Core Libraries

| Brief Description                | Link (Click to Visit)                                     | License                               |
|----------------------------------|-----------------------------------------------------------|---------------------------------------|
| Production-grade Goroutine pool. | [ants](https://github.com/panjf2000/ants)                 | [MIT](#Protocol-document-link)        |
| Map ↔ struct conversion library. | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#Protocol-document-link)        |
| Memory cache with size limits.   | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#Protocol-document-link) |
| Simplified memory cache.         | [freecache](https://github.com/coocood/freecache)         | [MIT](#Protocol-document-link)        |
| Lock-free concurrent Map.        | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#Protocol-document-link)        |

### Utilities

| Brief Description                                                      | Link (Click to Visit)                             | License                               |
|------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------|
| Smarter unique ID generator for string keys or Snowflake-like systems. | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#Protocol-document-link)        |
| Go FFmpeg wrapper for video processing.                                | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#Protocol-document-link) |

### HTTP

| Brief Description                                                              | Link (Click to Visit)                       | License                               |
|--------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------|
| ByteDance's high-performance HTTP framework surpassing fasthttp in benchmarks. | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#Protocol-document-link) |
| Popular HTTP client library.                                                   | [resty](https://github.com/go-resty/resty)  | [MIT](#Protocol-document-link)        |

### GUI

| Brief Description                                                                 | Link (Click to Visit)                   | License                          |
|-----------------------------------------------------------------------------------|-----------------------------------------|----------------------------------|
| Fyne: Cross-platform GUI framework supporting desktop/mobile apps (CGO required). | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#Protocol-document-link) |

### OS Interfaces

| Brief Description                                                                  | Link (Click to Visit)                          | License                          |
|------------------------------------------------------------------------------------|------------------------------------------------|----------------------------------|
| Go implementation of Python's psutil for system monitoring and process management. | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#Protocol-document-link) |

# Java

## Android

### Permissions

| Brief Description           | Link (Click to Visit)                                         | License                               |
|-----------------------------|---------------------------------------------------------------|---------------------------------------|
| Android permission library. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#Protocol-document-link) |

# Fonts

| Name          | Languages | Commercial Use | Link                                                 | License                                                      |
|---------------|-----------|----------------|------------------------------------------------------|--------------------------------------------------------------|
| Google Fonts  | Multiple  | Generally Yes  | [fonts.google.com](https://fonts.google.com)         | [Multiple Licenses](https://developers.google.com/fonts/faq) |
| Alibaba Fonts | Chinese   | Generally Yes  | [www.alibabafonts.com](https://www.alibabafonts.com) | [Custom License](https://www.alibabafonts.com/#/more)        |

# Protocol document link

| License                  | Official Link                                                                        |
|--------------------------|--------------------------------------------------------------------------------------|
| MIT                      | https://opensource.org/license/mit                                                   |
| AGPL 3.0                 | https://www.gnu.org/licenses/agpl-3.0.txt                                            |
| GPL 3.0                  | https://www.gnu.org/licenses/gpl-3.0.txt                                             |
| Apache 2.0               | https://www.apache.org/licenses/LICENSE-2.0.txt                                      |
| BSD 3                    | https://opensource.org/license/bsd-3-clause                                          |
| CreativeML Open RAIL-M   | https://github.com/CompVis/stable-diffusion/blob/main/LICENSE                        |
| CreativeML Open RAIL++-M | https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/blob/main/LICENSE.md |
| OFL 1.1 (2007)           | https://openfontlicense.org/documents/OFL.txt                                        |
| Mulan PubL v2            | http://license.coscl.org.cn/MulanPubL-2.0                                            |