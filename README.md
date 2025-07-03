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

# Table of Contents

<!-- TOC -->
* [open-power](#open-power)
* [Table of Contents](#table-of-contents)
* [Projects](#projects)
  * [AI](#ai)
    * [AI Middle Platform](#ai-middle-platform)
    * [AI Tools](#ai-tools)
      * [General Tools](#general-tools)
      * [Graphics & Images](#graphics--images)
      * [Audio Processing](#audio-processing)
      * [Others](#others)
  * [Access Control](#access-control)
  * [Network Control](#network-control)
  * [Message Middleware](#message-middleware)
  * [OPS](#ops)
  * [CI/CD](#cicd)
    * [CD](#cd)
    * [Container Capabilities](#container-capabilities)
* [AI Models](#ai-models)
  * [Generative AI Models](#generative-ai-models)
    * [Diffusion Models](#diffusion-models)
      * [Image Generation](#image-generation)
      * [Video Generation](#video-generation)
  * [Large Language Models & Multimodal Understanding Models & Autoregressive Multimodal Models](#large-language-models--multimodal-understanding-models--autoregressive-multimodal-models)
* [Language Capabilities](#language-capabilities)
  * [Cross-Language Frameworks](#cross-language-frameworks)
    * [RPC](#rpc)
  * [Python](#python)
    * [AI Capabilities](#ai-capabilities)
      * [AI Toolkits](#ai-toolkits)
      * [Algorithm Frameworks](#algorithm-frameworks)
  * [Golang](#golang)
    * [AI Capabilities](#ai-capabilities-1)
      * [AI Toolkits](#ai-toolkits-1)
    * [Basic Capabilities](#basic-capabilities)
    * [Toolkits](#toolkits)
    * [HTTP](#http)
      * [Server](#server)
      * [Client](#client)
    * [GUI](#gui)
    * [OS Interfaces](#os-interfaces)
* [Java](#java)
  * [Android](#android)
    * [Permission Management](#permission-management)
* [Font](#font)
* [Protocol Document Links](#protocol-document-links)
<!-- TOC -->

# Projects

## AI

### AI Middle Platform

| Project Summary                                                                                                                                                                                                                                    | Main Features      | Link (Click to Visit)                      | License                                                 |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------|--------------------------------------------|---------------------------------------------------------|
| Dify is currently the most powerful (as of 20250309) open-source large language model middle platform, capable of defining workflows, Agent templates, etc. The project is not entirely based on Apache 2.0 and has restrictions on multi-tenancy. | AI Middle Platform | [dify](https://github.com/langgenius/dify) | [Multiple Licenses](https://github.com/langgenius/dify) |

### AI Tools

#### General Tools

| Project Summary                                                                                                                            | Main Features | Link (Click to Visit)                                | License                             |
|--------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------------------------------------|-------------------------------------|
| This is a production-level low-code node-editing AI workflow software. The community has a large number of workflow templates and plugins. | AI Workflow   | [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | [GPL 3.0](#protocol-document-links) |

#### Graphics & Images

| Project Summary                                                                                                                                                                                                                                   | Main Features    | Link (Click to Visit)                                                             | License                              |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------|-----------------------------------------------------------------------------------|--------------------------------------|
| Stable-diffusion-webui allows one-click setup of a web page for AI drawing, making AI drawing simple. With plugins, it also supports video generation. The ecosystem is now very rich, with a large number of excellent plugins in the community. | Image Generation | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#protocol-document-links) |
| A classic face-swapping project. Please be aware of legal risks.                                                                                                                                                                                  | Image Processing | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                            | [GPL 3.0](#protocol-document-links)  |

#### Audio Processing

| Project Summary                                                                                                                                                                                            | Main Features                    | Link (Click to Visit)                                                              | License                                |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------|------------------------------------------------------------------------------------|----------------------------------------|
| A more powerful audio processing integration project than UVR5-UI, with the author still active (as of 20250222).                                                                                          | Audio Separation/Noise Reduction | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#protocol-document-links)   |
| Compared to most discontinued SVC projects, the author of RVC is still active (as of 20250222), and it is ready to use out of the box.                                                                     | Voice Conversion                 | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#protocol-document-links)        |
| One of the best text-to-speech systems still being updated, with an active community (as of 20250309).                                                                                                     | Text-to-Speech                   | [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)                               | [MIT](#protocol-document-links)        |
| CosyVoice, an open-source TTS system by Alibaba, performs better than GPT-SoVITS in some scenarios. Unfortunately, the community is still not active, relying mainly on official support (as of 20250309). | Text-to-Speech                   | [CosyVoice](https://github.com/FunAudioLLM/CosyVoice)                              | [Apache 2.0](#protocol-document-links) |

#### Others

| Project Summary                                                                                                                                                       | Main Features | Link (Click to Visit)                                                      | License                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------------------------------------------------------------------|----------------------------------------|
| A large language model (LLM) project based on Langchain, supporting RAG and Agent-related features (an improved version of Langchain-ChatGLM).                        | ChatGPT-like  | [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) | [Apache 2.0](#protocol-document-links) |
| A ready-to-use ChatGPT-like project (API-based) with extensive feature support. If you want to quickly deploy a ChatGPT-like project, this might be the first choice. | ChatGPT-like  | [open-webui](https://github.com/open-webui/open-webui)                     | [MIT](#protocol-document-links)        |

## Access Control

| Project Summary                                                                                                                                                                                                            | Type                    | Link (Click to Visit)                         | License                                |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------|-----------------------------------------------|----------------------------------------|
| Casbin is a powerful and efficient open-source access control library that supports RBAC, ABAC, etc. However, we believe that complex permission management, obscure jargon, and low-code solutions may not suit everyone. | Permission Management   | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#protocol-document-links) |
| An identity authentication project (IAM/SSO) from the same creators as Casbin.                                                                                                                                             | Identity Authentication | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#protocol-document-links) |

## Network Control

| Project Summary                                                        | Type                 | Link (Click to Visit)                  | License                             |
|------------------------------------------------------------------------|----------------------|----------------------------------------|-------------------------------------|
| NPS can set up an intranet penetration proxy with a web-based backend. | Intranet Penetration | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#protocol-document-links) |

## Message Middleware

| Project Summary                                                                                                                                                                                                  | Link (Click to Visit)                               | Type       | License                                               |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|------------|-------------------------------------------------------|
| TiDB is a financial-grade distributed database compatible with MySQL API, supporting both OLAP and OLTP. Compared to OceanBase, TiDB has a better open-source atmosphere.                                        | [tidb](https://github.com/pingcap/tidb)             | New-SQL-DB | [Apache 2.0](#protocol-document-links)                |
| OceanBase Database is a distributed relational database entirely developed by Ant Group. OceanBase, based on the Paxos protocol and distributed architecture, achieves high availability and linear scalability. | [oceanbase](https://github.com/oceanbase/oceanbase) | New-SQL-DB | [Mulan PubL v2](#protocol-document-links)             |
| Qdrant is a vector database written in Rust, capable of distributed production.                                                                                                                                  | [qdrant](https://github.com/qdrant/qdrant)          | Vector-DB  | [Apache 2.0](#protocol-document-links)                |
| Milvus is a vector database written in Go and C++, capable of distributed production.                                                                                                                            | [milvus](https://github.com/milvus-io/milvus)       | Vector-DB  | [Apache 2.0](#protocol-document-links)                |
| A shared KV memory cache project. To date, I have not found a replacement for Redis.                                                                                                                             | [redis](https://github.com/redis/redis)             | KV-Cache   | [Proprietary License](https://github.com/redis/redis) |

## OPS

## CI/CD

### CD

| Project Summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | Link (Click to Visit)                           | License                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|----------------------------------------|
| K8S is a standard process orchestration CD system that has been hailed by some as a distributed operating system. In essence, it's just a CD system (I'm referring to K8S core functionality, not the K8S/cloud-native ecosystem), and I don't understand why it receives such high praise. Business applications in modern medium to large enterprises are basically all managed by K8S, and currently the K8S ecosystem is beginning to develop toward stateful application and GPU application management. | [k8s](https://github.com/kubernetes/kubernetes) | [Apache 2.0](#protocol-document-links) |   

### Container Capabilities

| Project Summary                                                                                                                                                                                                                           | Link (Click to Visit)                                  | License                                |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|----------------------------------------|
| A container runtime tool responsible for starting, stopping, pausing, and deleting containers, typically used in combination with K8S-like projects for deployment, not usually for single-node or personal use, and cannot build images. | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#protocol-document-links) |   
| Kaniko is no longer maintained. If you need to build images, choose a suitable tool.                                                                                                                                                      | [buildkit](https://github.com/moby/buildkit)           | [Apache 2.0](#protocol-document-links) |

# AI Models

## Generative AI Models

### Diffusion Models

#### Image Generation

| Project Summary                                                                                                                                                                                                                          | Link (Click to Visit)                                                                           | License                                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|------------------------------------------------------|
| Stable Diffusion v1-5 is an improved version of the original CompVis model and remains the most well-supported image base model to date (as of 20250222).                                                                                | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#protocol-document-links)   |
| Stable-diffusion-xl-base-1.0 is a high-definition version of SD developed by Stability AI. Although newer technologies have emerged, the completeness of related toolchains (e.g., ControlNet) is second only to SD1.5 (as of 20250222). | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#protocol-document-links) |

#### Video Generation

| Project Summary                                                                                                                                                                                       | Link (Click to Visit)                                       | License                                                            |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------|--------------------------------------------------------------------|
| Hunyuan Video Generation Model, developed by Tencent, includes versions for image-to-video and text-to-video generation.                                                                              | [HunyuanVideo](https://huggingface.co/tencent/HunyuanVideo) | [Proprietary License](https://huggingface.co/tencent/HunyuanVideo) |
| An open-source video generation model by Alibaba with multiple versions, performing well among open-source models. The license on the GitHub page is Apache 2.0, but the model page does not specify. | [Wan-Video](https://github.com/Wan-Video)                   | [Apache 2.0](#protocol-document-links)                             |

## Large Language Models & Multimodal Understanding Models & Autoregressive Multimodal Models

Multimodal models are usually modified versions based on large language models.

| Project Summary                                                                                                                                                                                                                                                                                              | Multimodal                    | Link (Click to Visit)                      | License                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------|--------------------------------------------|--------------------------------------------------------------------------------------------------|
| Deepseek, which made a splash in early 2025, is now slightly behind top models like Claude and Qwen in some scenarios (as of 20250703).                                                                                                                                                                      | Multimodal Versions Available | [deepseek](https://github.com/deepseek-ai) | [MIT](#protocol-document-links)                                                                  |
| Llama, a large language model released by Meta, has a rich open-source ecosystem but supports fewer languages.                                                                                                                                                                                               | Some Versions                 | [Llama](https://www.llama.com/)            | [Proprietary License](https://www.llama.com/docs/how-to-guides/responsible-use-guide-resources/) |
| Qwen, a large language model released by Alibaba, includes versions for image understanding, audio understanding, mathematics, and code optimization.                                                                                                                                                        | Multimodal Versions Available | [QwenLM](https://github.com/QwenLM)        | [Multiple Licenses](https://huggingface.co/Qwen)                                                 |
| GLM, a large language model released by Tsinghua University, had a strong advantage in the open-source field before Q4 2024 (excluding Q4), with versions for image understanding, audio dialogue, and code optimization. Currently, it lags behind and may be removed from the collection (as of 20250703). | Multimodal Versions Available | [GLM4](https://github.com/THUDM/GLM-4)     | [Multiple Licenses](https://huggingface.co/THUDM)                                                |

# Language Capabilities

## Cross-Language Frameworks

### RPC

| Project Summary                                                                                                                                                 | Link (Click to Visit)                      | License                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|----------------------------------------|
| GRPC is a cross-language RPC protocol developed by Google, using HTTP/2 and predefined field protocols to enhance performance. It is less flexible than Thrift. | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#protocol-document-links) |
| Thrift is a cross-language RPC protocol developed by Meta, allowing custom protocols but natively lacking streaming support. It is less performant than GRPC.   | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#protocol-document-links) |

## Python

### AI Capabilities

#### AI Toolkits

| Project Summary                                                                                                                                                                                                                              | Link (Click to Visit)                                  | License                                |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|----------------------------------------|
| Huggingface's open-source Diffusers is the go-to library for state-of-the-art pre-trained diffusion models for generating images, audio, and even 3D structures of molecules.                                                                | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#protocol-document-links) |
| Langchain is a framework for developing and managing applications based on large language models. It provides standardized interfaces and toolchains, simplifying interactions with AI models, data processing, and application development. | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#protocol-document-links)        |

#### Algorithm Frameworks

| Project Summary                                                                                                                        | Link (Click to Visit)                                  | License                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|-----------------------------------------------------------------------------|
| PyTorch is easy to use and the first choice for beginners, currently maintained by Meta.                                               | [pytorch](https://github.com/pytorch/pytorch)          | [Proprietary License](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow is Google's engineered AI framework solution.                                                                               | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#protocol-document-links)                                      |
| An AI framework that Google has invested significant effort in recently, known for higher performance but with a steep learning curve. | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#protocol-document-links)                                      |

## Golang

### AI Capabilities

#### AI Toolkits

| Project Summary                                                                                           | Link (Click to Visit)                     | License                                |
|-----------------------------------------------------------------------------------------------------------|-------------------------------------------|----------------------------------------|
| Eino is a Go language large model toolchain framework open-sourced by ByteDance, comparable to Langchain. | [eino](https://github.com/cloudwego/eino) | [Apache 2.0](#protocol-document-links) |

### Basic Capabilities

| Project Summary                                                                               | Link (Click to Visit)                                     | License                                |
|-----------------------------------------------------------------------------------------------|-----------------------------------------------------------|----------------------------------------|
| This is a Go language coroutine pool library, stably used in production.                      | [ants](https://github.com/panjf2000/ants)                 | [MIT](#protocol-document-links)        |   
| A Go language library for parsing between maps and structs.                                   | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#protocol-document-links)        |
| A ready-to-use in-memory cache library that can also be configured with a maximum cache size. | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#protocol-document-links) |
| An in-memory cache library with simpler configuration than Bigcache.                          | [freecache](https://github.com/coocood/freecache)         | [MIT](#protocol-document-links)        |
| A lock-free and concurrency-safe Map.                                                         | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#protocol-document-links)        |

### Toolkits

| Project Summary                                                                                                                                                             | Link (Click to Visit)                             | License                                |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|----------------------------------------|
| A smarter approach than standard RFC document UUIDs, suitable for distributed IDs or string unique keys, with ordered prefixes.                                             | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#protocol-document-links)        |   
| A Go language implementation of ffmpeg-python. [FFmpeg](https://github.com/FFmpeg/FFmpeg) is a well-known open-source audio and video data processing library written in C. | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#protocol-document-links) |

### HTTP

#### Server

| Project Summary                                                                                                                                               | Link (Click to Visit)                       | License                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|----------------------------------------|
| An HTTP framework open-sourced by ByteDance. According to benchmark tests in the documentation, its performance and stability surpass the fasthttp framework. | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#protocol-document-links) |   

#### Client

| Project Summary                      | Link (Click to Visit)                      | License                         |
|--------------------------------------|--------------------------------------------|---------------------------------|
| A commonly used HTTP client library. | [resty](https://github.com/go-resty/resty) | [MIT](#protocol-document-links) |

### GUI

| Project Summary                                                                                                                                                             | Link (Click to Visit)                   | License                           |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|-----------------------------------|
| Fyne is a Go language GUI framework that can create desktop applications and package mobile applications. Although I dislike CGO, there are currently no good alternatives. | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#protocol-document-links) |   

### OS Interfaces

| Project Summary                                                                                                                                                                                                    | Link (Click to Visit)                          | License                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|-----------------------------------|
| Gopsutil is a library for system monitoring, analysis, limiting process resources, and managing processes. It is a Go language implementation of the Python project [psutil](https://github.com/giampaolo/psutil). | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#protocol-document-links) |   

# Java

## Android

### Permission Management

| Project Summary                              | Link (Click to Visit)                                         | License                                |
|----------------------------------------------|---------------------------------------------------------------|----------------------------------------|
| A useful Android permission request library. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#protocol-document-links) |   

# Font

| Project Summary    | Language     | Commercial Use | Link                                        | License                                                      |
|--------------------|--------------|----------------|---------------------------------------------|--------------------------------------------------------------|
| Google Free Fonts  | Multilingual | Mostly Allowed | [fonts.google.com](fonts.google.com)        | [Multiple Licenses](https://developers.google.com/fonts/faq) |
| Alibaba Free Fonts | Chinese      | Mostly Allowed | [www.alibabafonts.co](www.alibabafonts.com) | [Proprietary License](https://www.alibabafonts.com/#/more)   |

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