<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp" width="100" border="0" alt="open-power">
  </a>
</p>

Other languages: [简体中文](README_zh.md), (Currently unable to translate more)

# open-power

This repository is dedicated to documenting open-source projects that excel in one or more aspects such as productivity,
performance, stability, and design. Here, you can quickly find options suitable for production use. We advocate for
completing one’s work efficiently rather than getting bogged down in minute details.

For projects with overlapping functionalities, we generally only document 1-2 of them. We do not see the point of
listing all open-source projects of the same type.

Our evaluation principles are as follows: simplicity over complexity; ease of use over professionalism; stability over
performance.

The scope includes but is not limited to artificial intelligence, blockchain, graphics and imaging, algorithms,
development tools, operations tools, various protocols, fonts, and documentation collections.

# index

<!-- TOC -->
* [open-power](#open-power)
* [index](#index)
* [AI](#ai)
  * [out-of-the-box](#out-of-the-box)
  * [Generative AI Models](#generative-ai-models)
    * [Image Generation](#image-generation)
      * [Images](#images)
      * [Video](#video)
    * [Large Language Models & Multimodal Models](#large-language-models--multimodal-models)
  * [Tool Libraries](#tool-libraries)
  * [Algorithm Frameworks](#algorithm-frameworks)
* [DEV](#dev)
  * [Protocols](#protocols)
    * [RPC](#rpc)
  * [Database](#database)
  * [Golang](#golang)
    * [Core Capabilities](#core-capabilities)
    * [Utility Libraries](#utility-libraries)
    * [HTTP](#http)
    * [Container Capabilities](#container-capabilities)
    * [GUI](#gui)
    * [Operating System Interface](#operating-system-interface)
    * [out-of-the-box](#out-of-the-box-1)
    * [Development Tools](#development-tools)
  * [Web Crawling](#web-crawling)
    * [Targeted Crawlers](#targeted-crawlers)
  * [Android](#android)
    * [Utility Libraries](#utility-libraries-1)
* [Font](#font)
* [Protocol document link](#protocol-document-link)
<!-- TOC -->

# AI

## out-of-the-box

| Project Summary                                                                                                                                                                                                                                                         | Main Features              | Address (Click to Visit)                                                           | License                               |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|------------------------------------------------------------------------------------|---------------------------------------|
| Stable-diffusion-webui is a one-click solution to build AI image generation web interface, making AI image generation simple. With plugins, it also has video generation capabilities. Currently, the ecosystem is very rich with numerous excellent community plugins. | Image Generation           | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui)  | [AGPL 3.0](#Protocol-document-link)   |
| A production-grade low-code node editing AI workflow software. The community has numerous workflow templates and plugins.                                                                                                                                               | AI Workflow                | [ComfyUI](https://github.com/comfyanonymous/ComfyUI)                               | [GPL 3.0](#Protocol-document-link)    |
| A more powerful audio processing integration project than UVR5-UI, with the author still active (as of November 17, 2024).                                                                                                                                              | Audio Separation/Denoising | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#Protocol-document-link)   |
| A classic face replacement project, please be aware of legal risks.                                                                                                                                                                                                     | Image Processing           | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                             | [GPL 3.0](#Protocol-document-link)    |
| Compared to most discontinued SVC projects, RVC's author remains active, offering an out-of-the-box solution.                                                                                                                                                           | Voice Conversion           | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#Protocol-document-link)        |
| A langchain-based large language model project supporting RAG and Agent-related functions (an improved version of Langchain-ChatGLM).                                                                                                                                   | ChatGPT-like               | [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat)         | [Apache 2.0](#Protocol-document-link) |
| An out-of-the-box ChatGPT-like project (API-based) with extensive features. If you want to quickly deploy a ChatGPT-like project, this might be your first choice.                                                                                                      | ChatGPT-like               | [open-webui](https://github.com/open-webui/open-webui)                             | [MIT](#Protocol-document-link)        |

## Generative AI Models

### Image Generation

#### Images

| Brief Description                                                                                                                                                                                                        | Address (Click to Visit)                                                                        | License                                             |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| Stable Diffusion v1-5 is an improved version of CompVis's original version, currently remains the most complete image base model with the most comprehensive toolchain. (As of 20241117)                                 | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#Protocol-document-link)   |
| stable-diffusion-xl-base-1.0 is a HD version developed by stabilityai. Although some newer technologies have emerged, the completeness of related toolchains such as controlnet is second only to sd1.5 (As of 20241117) | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#Protocol-document-link) |

#### Video

Typically, video models generate videos from images, and the text-to-video process usually follows the path: text->
image->video.

### Large Language Models & Multimodal Models

Multimodal models are usually modified versions based on large language models

| Brief Description                                                                                                                                                        | Multimodal              | Address (Click to Visit)               | License                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|----------------------------------------|--------------------------------------------------------------------------------------------------|
| Llama is a large language model released by Meta, though supporting fewer languages, it's currently one of the most popular large language base models. (As of 20241117) | Some versions           | [Llama](https://www.llama.com/)        | [Independent License](https://www.llama.com/docs/how-to-guides/responsible-use-guide-resources/) |
| Qwen is a large language model released by Alibaba, including versions for image understanding, audio understanding, mathematics, and code optimization.                 | Has multimodal versions | [QwenLM](https://github.com/QwenLM)    | [Multiple Licenses](https://huggingface.co/Qwen)                                                 |
| GLM is a large language model released by Tsinghua University, with versions for image understanding, audio conversation, and code optimization.                         | Has multimodal versions | [GLM4](https://github.com/THUDM/GLM-4) | [Multiple Licenses](https://huggingface.co/THUDM)                                                |

## Tool Libraries

| Brief Description                                                                                                                                                                                                       | Development Language | Address (Click to Visit)                               | License                               |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------|--------------------------------------------------------|---------------------------------------|
| Huggingface's open-source Diffusers is the go-to library for the latest pre-trained diffusion models for generating images, audio, and even 3D molecular structures.                                                    | Python               | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#Protocol-document-link) |
| An application-oriented development framework for large language models based on Python. Honestly, I don't think Python-based application frameworks are competitive, but including this due to langchain's popularity. | Python               | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#Protocol-document-link)        |

## Algorithm Frameworks

| Brief Description                                                                                                                                 | Address (Click to Visit)                               | License                                                                     |
|---------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|-----------------------------------------------------------------------------|
| PyTorch is user-friendly, ideal for beginners, currently maintained by Meta.                                                                      | [pytorch](https://github.com/pytorch/pytorch)          | [Independent License](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow is Google's engineered AI framework solution.                                                                                          | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#Protocol-document-link)                                       |
| A Google AI framework that has received significant investment in recent years, characterized by higher performance but a steeper learning curve. | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#Protocol-document-link)                                       |

# DEV

## Protocols

### RPC

We don't believe there are meaningful fundamental advantages or disadvantages between different RPC protocols - perhaps
choosing any one would suffice.

| Project Description                                                                                                                      | Link (Click to Visit)                      | License                               |
|------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|---------------------------------------|
| GRPC is a cross-language RPC protocol from Google that uses HTTP/2 and predefined field protocols to increase performance.               | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#Protocol-document-link) |
| If you don't want to use GRPC, thrift is a good choice, though the current editors of this project are not familiar with this framework. | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#Protocol-document-link) |

## Database

| Project Description                                                                                                                                                                                       | Link (Click to Visit)                               | License                                  |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|------------------------------------------|
| OceanBase Database is a distributed relational database fully developed by Ant Group. OceanBase implements high availability and linear scaling based on the Paxos protocol and distributed architecture. | [oceanbase](https://github.com/oceanbase/oceanbase) | [Mulan PubL v2](#Protocol-document-link) |

## Golang

### Core Capabilities

| Project Description                                                                                                                                                         | Link (Click to Visit)                                     | License                               |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------|---------------------------------------|
| A Golang goroutine pool library that we use stably in production.                                                                                                           | [ants](https://github.com/panjf2000/ants)                 | [MIT](#Protocol-document-link)        |
| A library for parsing between Go maps and structs.                                                                                                                          | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#Protocol-document-link)        |
| Compared to native map, bigcache reduces GC overhead through some techniques and can set cache data expiration time, showing excellent performance among similar libraries. | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#Protocol-document-link) |
| A lock-free and concurrency-safe hashmap that performs worse than native map in serial scenarios.                                                                           | [hashmap](https://github.com/cornelk/hashmap)             | [Apache 2.0](#Protocol-document-link) |

### Utility Libraries

| Project Description                                                                                                                                                         | Link (Click to Visit)                             | License                               |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------|
| A smarter approach than standard RFC document UUID, suitable for unique string keys or snowflake algorithm.                                                                 | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#Protocol-document-link)        |
| Go language implementation of ffmpeg-python, [FFmpeg](https://github.com/FFmpeg/FFmpeg) is a well-known open-source audio and video data processing library developed in C. | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#Protocol-document-link) |

### HTTP

| Project Description                                                                                                                                                                       | Link (Click to Visit)                       | License                               |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------|
| An HTTP framework open-sourced by ByteDance, which according to benchmark tests in the documentation, surpasses the fasthttp framework in both performance and stability - we believe it. | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#Protocol-document-link) |
| A commonly used HTTP client library.                                                                                                                                                      | [resty](https://github.com/go-resty/resty)  | [MIT](#Protocol-document-link)        |

### Container Capabilities

| Project Description                                                                                                                                                                                          | Link (Click to Visit)                                  | License                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|---------------------------------------|
| A container runtime tool responsible for starting, stopping, pausing, and deleting containers, typically deployed with k8s-like projects, not intended for single-node or personal use, cannot build images. | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#Protocol-document-link) |

### GUI

| Project Description                                                                                                                                      | Link (Click to Visit)                   | License                          |
|----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|----------------------------------|
| Fyne is a Go GUI framework that can create both desktop and mobile applications. Although we dislike CGO, there aren't many good alternatives currently. | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#Protocol-document-link) |

### Operating System Interface

| Project Description                                                                                                                                                                                         | Link (Click to Visit)                          | License                          |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|----------------------------------|
| Gopsutil is a library for system monitoring, analysis, process resource limitation, and process management. It's the Go implementation of the Python project [psutil](https://github.com/giampaolo/psutil). | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#Protocol-document-link) |

### out-of-the-box

| Project Description                                                                                                                                                                                            | Type                  | Link (Click to Visit)                         | License                               |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------|-----------------------------------------------|---------------------------------------|
| Casbin is a powerful and efficient open-source access control library supporting RBAC, ABAC, though we believe complex permission management, technical jargon, and low-code may not be suitable for everyone. | Permission Management | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#Protocol-document-link) |
| An authentication project (IAM/SSO) from the same creators as casbin.                                                                                                                                          | Authentication        | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#Protocol-document-link) |
| NPS can set up an intranet penetration proxy with a web interface backend.                                                                                                                                     | Intranet Penetration  | [nps](https://github.com/ehang-io/nps)        | [GPL 3.0](#Protocol-document-link)    |

### Development Tools

| Project Description                                             | Link (Click to Visit)                                             | License                        |
|-----------------------------------------------------------------|-------------------------------------------------------------------|--------------------------------|
| A development plugin for organizing Go language import sorting. | [goimports-reviser](https://github.com/incu6us/goimports-reviser) | [MIT](#Protocol-document-link) |

## Web Crawling

### Targeted Crawlers

| Project Description                                                                                    | Link (Click to Visit)                          | License                        |
|--------------------------------------------------------------------------------------------------------|------------------------------------------------|--------------------------------|
| A lightweight Bilibili live streaming danmaku crawling script that's simple to use and easy to modify. | [blivedm](https://github.com/xfgryujk/blivedm) | [MIT](#Protocol-document-link) |

## Android

### Utility Libraries

| Project Description                          | Link (Click to Visit)                                         | License                               |
|----------------------------------------------|---------------------------------------------------------------|---------------------------------------|
| A useful Android permission request library. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#Protocol-document-link) |

# Font

| Project Brief      | Language     | Commercial Use | Address                                      | License                                                        |
|--------------------|--------------|----------------|----------------------------------------------|----------------------------------------------------------------|
| Google Free Fonts  | Multilingual | Mostly allowed | [fonts.google.com](fonts.google.com)         | [Multiple agreements](https://developers.google.com/fonts/faq) |
| Alibaba Free Fonts | Chinese      | Mostly allowed | [www.alibabafonts.com](www.alibabafonts.com) | [Independent agreement](https://www.alibabafonts.com/#/more)   |

# Protocol document link

| 许可证                      | 原文                                                                                   |
|--------------------------|--------------------------------------------------------------------------------------|
| MIT                      | https://opensource.org/license/mit                                                   |
| AGPL 3.0                 | https://www.gnu.org/licenses/agpl-3.0.txt                                            |
| GPL  3.0                 | https://www.gnu.org/licenses/gpl-3.0.txt                                             |
| Apache 2.0               | https://www.apache.org/licenses/LICENSE-2.0.txt                                      |
| BSD 3                    | https://opensource.org/license/bsd-3-clause                                          |
| CreativeML Open RAIL-M   | https://github.com/CompVis/stable-diffusion/blob/main/LICENSE                        |
| CreativeML Open RAIL++-M | https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/blob/main/LICENSE.md |
| OFL1.1 2007              | https://openfontlicense.org/documents/OFL.txt                                        |
| Mulan PubL v2            | http://license.coscl.org.cn/MulanPubL-2.0                                            |