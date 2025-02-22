<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp?version=0.1" width="400" border="0" alt="open-power">
  </a>
</p>

Other languages: [简体中文](README_zh.md), (Currently unable to translate more)

# open-power

This repository records open-source projects that excel in productivity/performance/stability/design. Here you can
quickly find production-ready solutions. I advocate for efficiently completing tasks rather than delving into trivial
details.

For projects with overlapping functionalities, only 1-2 will be listed. Listing all similar projects is not meaningful.

Our evaluation principles: Simplicity > Complexity; Ease of Use > Professionalism; Stability > Performance.

Including but not limited to AI, blockchain, graphics, algorithms, development tools, O&M tools, protocols, fonts, and
documentation.

# Index

<!-- TOC -->
* [open-power](#open-power)
* [Index](#index)
* [AI](#ai)
  * [Out-of-the-Box Solutions](#out-of-the-box-solutions)
  * [Generative AI Models](#generative-ai-models)
    * [Image Generation](#image-generation)
      * [Image Generation](#image-generation-1)
      * [Video Generation](#video-generation)
    * [Large Language Models & Multimodal Models](#large-language-models--multimodal-models)
  * [Utility Libraries](#utility-libraries)
  * [Algorithm Frameworks](#algorithm-frameworks)
* [DEV](#dev)
  * [Protocols](#protocols)
    * [RPC](#rpc)
  * [Databases](#databases)
  * [Golang](#golang)
    * [Core Utilities](#core-utilities)
    * [Utility Libraries](#utility-libraries-1)
    * [HTTP](#http)
    * [Container Capabilities](#container-capabilities)
    * [GUI](#gui)
    * [OS Interfaces](#os-interfaces)
    * [Out-of-the-Box Solutions](#out-of-the-box-solutions-1)
    * [Development Tools](#development-tools)
  * [Web Scraping](#web-scraping)
    * [Targeted Scraping](#targeted-scraping)
  * [Android](#android)
    * [Utility Libraries](#utility-libraries-2)
* [Font](#font)
* [Protocol Document Links](#protocol-document-links)
<!-- TOC -->

# AI

## Out-of-the-Box Solutions

| Brief Description                                                                                                                                      | Main Functionality | Link (Click to Visit)                                                              | License                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|------------------------------------------------------------------------------------|-----------------------------------------------------|
| Stable-diffusion-webui: A one-click web UI for AI image generation with rich plugin support and video generation.                                      | Image Generation   | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)  | [AGPL 3.0](#protocol-document-links)                |
| A production-grade low-code node-based AI workflow editor with extensive community templates and plugins.                                              | AI Workflow        | [ComfyUI](https://github.com/comfyanonymous/ComfyUI)                               | [GPL 3.0](#protocol-document-links)                 |
| Advanced audio processing toolkit surpassing UVR5-UI, actively maintained (as of 2025-02-22).                                                          | Audio Separation   | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#protocol-document-links)                |
| A classic face-swapping project. Legal risks apply.                                                                                                    | Image Processing   | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                             | [GPL 3.0](#protocol-document-links)                 |
| Actively maintained SVC project (as of 2025-02-22), ready for deployment.                                                                              | Voice Conversion   | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#protocol-document-links)                     |
| Langchain-based LLM project supporting RAG and Agent functionalities (improved version of Langchain-ChatGLM).                                          | ChatGPT-like       | [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat)         | [Apache 2.0](#protocol-document-links)              |
| Out-of-the-box ChatGPT-like project with extensive API support. Ideal for quick deployment.                                                            | ChatGPT-like       | [open-webui](https://github.com/open-webui/open-webui)                             | [MIT](#protocol-document-links)                     |
| Dify: The most powerful (as of 2025-02-22) open-source AI-API aggregation platform with workflow and Agent templates. Multi-tenant restrictions apply. | AI Middleware      | [dify](https://github.com/langgenius/dify)                                         | [Multi-license](https://github.com/langgenius/dify) |

## Generative AI Models

### Image Generation

#### Image Generation

| Brief Description                                                                                                                   | Link (Click to Visit)                                                                           | License                                              |
|-------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|------------------------------------------------------|
| Stable Diffusion v1-5: An improved version of CompVis's original model, still the most robust image base model (as of 2025-02-22).  | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#protocol-document-links)   |
| Stable Diffusion XL 1.0: HD version by Stability AI. Toolchain maturity (e.g., ControlNet) second only to SD1.5 (as of 2025-02-22). | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#protocol-document-links) |

#### Video Generation

| Brief Description               | Link (Click to Visit)                         | License                                       |
|---------------------------------|-----------------------------------------------|-----------------------------------------------|
| CogVideo by Tsinghua University | [CogVideo](https://github.com/THUDM/CogVideo) | [Multi-license](https://huggingface.co/THUDM) |

### Large Language Models & Multimodal Models

| Brief Description                                           | Multimodal | Link (Click to Visit)                      | License                                                                             |
|-------------------------------------------------------------|------------|--------------------------------------------|-------------------------------------------------------------------------------------|
| DeepSeek: Exceptional LLM with multimodal versions.         | Yes        | [deepseek](https://github.com/deepseek-ai) | [MIT](#protocol-document-links)                                                     |
| Llama by Meta: Rich ecosystem but limited language support. | Partial    | [Llama](https://www.llama.com/)            | [Custom](https://www.llama.com/docs/how-to-guides/responsible-use-guide-resources/) |
| Qwen by Alibaba: Includes image/audio/math/code versions.   | Yes        | [QwenLM](https://github.com/QwenLM)        | [Multi-license](https://huggingface.co/Qwen)                                        |
| GLM by Tsinghua University: Supports image/audio/code.      | Yes        | [GLM4](https://github.com/THUDM/GLM-4)     | [Multi-license](https://huggingface.co/THUDM)                                       |

## Utility Libraries

| Brief Description                                                       | Language | Link (Click to Visit)                                  | License                                |
|-------------------------------------------------------------------------|----------|--------------------------------------------------------|----------------------------------------|
| Huggingface's Diffusers: State-of-the-art library for diffusion models. | Python   | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#protocol-document-links) |
| Langchain: Python-based LLM application framework (widely recognized).  | Python   | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#protocol-document-links)        |

## Algorithm Frameworks

| Brief Description                                   | Link (Click to Visit)                                  | License                                                        |
|-----------------------------------------------------|--------------------------------------------------------|----------------------------------------------------------------|
| PyTorch: Beginner-friendly, maintained by Meta.     | [pytorch](https://github.com/pytorch/pytorch)          | [Custom](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow: Google's production-grade AI framework. | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#protocol-document-links)                         |
| JAX: High-performance framework by Google.          | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#protocol-document-links)                         |

# DEV

## Protocols

### RPC

| Brief Description                                                                   | Link (Click to Visit)                      | License                                |
|-------------------------------------------------------------------------------------|--------------------------------------------|----------------------------------------|
| gRPC: Google's cross-language RPC with HTTP/2 and predefined protocols.             | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#protocol-document-links) |
| Thrift: Meta's cross-language RPC with customizable protocols. No native streaming. | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#protocol-document-links) |

## Databases

| Brief Description                                                                                            | Link (Click to Visit)                               | License                                   |
|--------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|-------------------------------------------|
| TiDB: Distributed SQL database compatible with MySQL, supporting OLAP/OLTP. Better ecosystem than OceanBase. | [tidb](https://github.com/pingcap/tidb)             | [Apache 2.0](#protocol-document-links)    |
| OceanBase: Distributed relational DB by Ant Group with Paxos protocol.                                       | [oceanbase](https://github.com/oceanbase/oceanbase) | [Mulan PubL v2](#protocol-document-links) |

## Golang

### Core Utilities

| Brief Description                 | Link (Click to Visit)                                     | License                                |
|-----------------------------------|-----------------------------------------------------------|----------------------------------------|
| High-performance goroutine pool.  | [ants](https://github.com/panjf2000/ants)                 | [MIT](#protocol-document-links)        |   
| Map ↔ struct conversion library.  | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#protocol-document-links)        |
| In-memory cache with size limits. | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#protocol-document-links) |
| Simplified in-memory cache.       | [freecache](https://github.com/coocood/freecache)         | [MIT](#protocol-document-links)        |
| Lock-free concurrent-safe Map.    | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#protocol-document-links)        |

### Utility Libraries

| Brief Description                                            | Link (Click to Visit)                             | License                                |
|--------------------------------------------------------------|---------------------------------------------------|----------------------------------------|
| Smarter UUID alternative for unique string keys.             | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#protocol-document-links)        |   
| Go implementation of FFmpeg (C-based multimedia processing). | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#protocol-document-links) |

### HTTP

| Brief Description                                                | Link (Click to Visit)                       | License                                |
|------------------------------------------------------------------|---------------------------------------------|----------------------------------------|
| ByteDance's high-performance HTTP framework surpassing fasthttp. | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#protocol-document-links) |   
| Popular HTTP client library.                                     | [resty](https://github.com/go-resty/resty)  | [MIT](#protocol-document-links)        |

### Container Capabilities

| Brief Description                                                      | Link (Click to Visit)                                  | License                                |
|------------------------------------------------------------------------|--------------------------------------------------------|----------------------------------------|
| Container runtime for managing containers, often used with Kubernetes. | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#protocol-document-links) |   

### GUI

| Brief Description                                                 | Link (Click to Visit)                   | License                           |
|-------------------------------------------------------------------|-----------------------------------------|-----------------------------------|
| Fyne: Cross-platform GUI framework for desktop/mobile (uses CGO). | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#protocol-document-links) |   

### OS Interfaces

| Brief Description                                                               | Link (Click to Visit)                          | License                           |
|---------------------------------------------------------------------------------|------------------------------------------------|-----------------------------------|
| Go psutil: System monitoring and process management (Go port of Python psutil). | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#protocol-document-links) |   

### Out-of-the-Box Solutions

| Brief Description                                             | Type           | Link (Click to Visit)                         | License                                |
|---------------------------------------------------------------|----------------|-----------------------------------------------|----------------------------------------|
| Casbin: Powerful access control library supporting RBAC/ABAC. | Authorization  | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#protocol-document-links) |
| Casdoor: Identity and Access Management (IAM/SSO) solution.   | Authentication | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#protocol-document-links) |
| NPS: Intranet penetration proxy with web-based management.    | Proxy          | [nps](https://github.com/ehang-io/nps)        | [GPL 3.0](#protocol-document-links)    |

### Development Tools

| Brief Description                    | Link (Click to Visit)                                             | License                         |
|--------------------------------------|-------------------------------------------------------------------|---------------------------------|
| Goimports-reviser: Import formatter. | [goimports-reviser](https://github.com/incu6us/goimports-reviser) | [MIT](#protocol-document-links) |

## Web Scraping

### Targeted Scraping

| Brief Description                     | Link (Click to Visit)                          | License                         |
|---------------------------------------|------------------------------------------------|---------------------------------|
| Bilibili live stream danmaku scraper. | [blivedm](https://github.com/xfgryujk/blivedm) | [MIT](#protocol-document-links) |   

## Android

### Utility Libraries

| Brief Description                    | Link (Click to Visit)                                         | License                                |
|--------------------------------------|---------------------------------------------------------------|----------------------------------------|
| Android runtime permissions library. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#protocol-document-links) |   

# Font

| Project       | Languages | Commercial Use | Link                                                 | License                                                  |
|---------------|-----------|----------------|------------------------------------------------------|----------------------------------------------------------|
| Google Fonts  | Multiple  | Mostly Allowed | [fonts.google.com](https://fonts.google.com)         | [Multi-license](https://developers.google.com/fonts/faq) |
| Alibaba Fonts | Chinese   | Mostly Allowed | [www.alibabafonts.com](https://www.alibabafonts.com) | [Custom](https://www.alibabafonts.com/#/more)            |

# Protocol Document Links

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
| Mulan PubL v2            | http://license.coscl.org.cn/MulanPubL-2.0                                            |
