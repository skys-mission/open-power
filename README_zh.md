<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp?version=0.3" width="80" border="0" alt="open-power">
  </a>
</p>

其它语言：[English](README.md)

# open-power

> 开源技术选型索引，聚焦 AI 模型、MCP、编码代理、基础设施与语言生态能力。

覆盖常用开源项目、协议与工具链，便于快速调研、对比与选型。

本项目使用 AI 工具辅助编辑文档，但所有项目筛选与收录均为 100% 人工完成。

# 目录

<!-- TOC -->
* [open-power](#open-power)
* [目录](#目录)
* [AI](#ai)
  * [AI模型](#ai模型)
    * [大语言模型与多模态模型](#大语言模型与多模态模型)
    * [生成式AI模型](#生成式ai模型)
      * [图像生成模型](#图像生成模型)
        * [图片生成](#图片生成)
        * [视频生成](#视频生成)
  * [AI协议与标准](#ai协议与标准)
    * [协议](#协议)
  * [AI工作流](#ai工作流)
  * [AI工具](#ai工具)
    * [图像生成](#图像生成)
    * [音频处理](#音频处理)
      * [音频分离与降噪](#音频分离与降噪)
      * [音色转换](#音色转换)
      * [文字转语音](#文字转语音)
    * [编码代理](#编码代理)
    * [其它](#其它)
* [基础设施](#基础设施)
  * [权限控制](#权限控制)
  * [网络控制](#网络控制)
  * [数据存储与缓存](#数据存储与缓存)
  * [交付与镜像构建](#交付与镜像构建)
    * [CD](#cd)
    * [容器能力](#容器能力)
* [语言能力](#语言能力)
  * [跨语言框架](#跨语言框架)
    * [RPC](#rpc)
  * [Python](#python)
    * [AI能力](#ai能力)
      * [LLM应用框架](#llm应用框架)
      * [模型训练与推理工具](#模型训练与推理工具)
      * [算法框架](#算法框架)
  * [Golang](#golang)
    * [AI能力](#ai能力-1)
      * [LLM应用框架](#llm应用框架-1)
    * [基础能力](#基础能力)
    * [工具库](#工具库)
    * [HTTP](#http)
      * [Server](#server)
      * [Client](#client)
    * [RPC](#rpc-1)
      * [Server](#server-1)
    * [服务框架](#服务框架)
    * [GUI](#gui)
    * [操作系统接口](#操作系统接口)
* [Java](#java)
  * [Android](#android)
    * [权限管理](#权限管理)
* [字体](#字体)
* [许可证原文链接](#Protocol-document-link)
<!-- TOC -->

# AI

## AI模型

### 大语言模型与多模态模型

多模态模型通常是基于大语言模型的改造版本。

| 项目简要                                                                                                                                                              | 多模态                 | 地址（点击访问）                           | 协议情况       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ------------------------------------------ | -------------- |
| DeepSeek 是开源大模型系列，覆盖推理与多模态等方向。                                                                                                                | 多模态版本处于试验阶段 | [deepseek](https://github.com/deepseek-ai) | 按具体模型而定 |
| Qwen 是阿里开源的大模型系列，覆盖文本、图像理解、音频、数学与代码等多类能力。                                                                                      | 有多模态版本           | [QwenLM](https://github.com/QwenLM)        | 按具体模型而定 |
| GLM 是 zai-org 推出的开源大模型系列，覆盖通用、多模态与智能体相关能力。                                                                                             | 有多模态版本           | [GLM](https://huggingface.co/zai-org)      | 按具体模型而定 |
| Kimi 是 Moonshot AI 推出的开源模型系列，覆盖通用与推理能力方向。                                                                                                  | 有多模态版本           | [KIMI](https://github.com/MoonshotAI)      | 按具体模型而定 |
| Gemma 是 Google DeepMind 推出的开放权重大语言模型系列，基于 Gemini 研究和技术，提供用于推理与微调的 JAX 库。 | 有多模态版本           | [gemma](https://github.com/google-deepmind/gemma) | [Apache 2.0](#Protocol-document-link) |

### 生成式AI模型

#### 图像生成模型

##### 图片生成

| 项目简要                                                                                                                                                          | 地址（点击访问）                                                                                | 使用许可证                                          |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | --------------------------------------------------- |
| stable diffusion v1-5 是经典图像生成基座，具备成熟的 WebUI / ComfyUI / LoRA / ControlNet 生态支持。                                                              | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#Protocol-document-link)   |
| stable-diffusion-xl-base-1.0 是经典高清图像生成基座，在画质、分辨率与社区支持之间保持较好平衡。                                                                  | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#Protocol-document-link) |
| HunyuanImage-3.0 是原生多模态自回归图像生成模型，技术路线较新，部署资源需求较高。                                                                                 | [HunyuanImage-3.0](https://github.com/Tencent-Hunyuan/HunyuanImage-3.0)                         | [独立协议](https://github.com/Tencent-Hunyuan/HunyuanImage-3.0/blob/main/LICENSE) |
| HiDream-I1 是 17B 参数文生图基座模型，基于 Sparse DiT 架构，支持中英双语提示，提供 Full / Dev / Fast 多版本。                                                     | [HiDream-I1](https://github.com/HiDream-ai/HiDream-I1)                                          | [MIT](#Protocol-document-link)                       |

##### 视频生成

| 项目简要                                                                                                           | 地址（点击访问）                          | 使用许可证                            |
| ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------- | ------------------------------------- |
| 阿里开源的视频生成模型系列，提供多个版本。 | [Wan-Video](https://github.com/Wan-Video) | [Apache 2.0](#Protocol-document-link) |
| LTX-Video 是基于 DiT 架构的视频生成模型，支持图生视频、多关键帧、视频扩展与视频到视频转换，最高可达 4K 分辨率 50 FPS。 | [LTX-Video](https://github.com/Lightricks/ltx-video) | [Apache 2.0](#Protocol-document-link) |

## AI协议与标准

### 协议

| 项目简要                                                                                                                                           | 类型       | 地址（点击访问）                                                     | 使用许可证                            |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | -------------------------------------------------------------------- | ------------------------------------- |
| Model Context Protocol（MCP）是面向 LLM 应用与外部数据源、工具集成的开放协议，定义统一的上下文交换与客户端/服务端交互方式，并形成了规范、SDK 与服务端生态。 | AI协议标准 | [MCP](https://github.com/modelcontextprotocol/modelcontextprotocol) | [MIT](#Protocol-document-link)        |
| Agent2Agent（A2A）是面向智能体应用的开放通信协议，支持不同框架与厂商构建的 Agent 相互发现能力、协商交互方式并协作完成长期任务。 | AI协议标准 | [A2A](https://github.com/a2aproject/A2A) | [Apache 2.0](#Protocol-document-link) |
| Agent Client Protocol（ACP）是标准化代码编辑器与编码 Agent 之间通信的协议，提供 Kotlin、Java、Python、Rust、TypeScript 多语言 SDK。 | AI协议标准 | [ACP](https://github.com/agentclientprotocol/agent-client-protocol) | [Apache 2.0](#Protocol-document-link) |

## AI工作流

| 项目简要                                                                                                                                                          | 主要功能 | 地址（点击访问）                                     | 使用许可证                            |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ---------------------------------------------------- | ------------------------------------- |
| ComfyUI 是面向生成式 AI 的低代码节点式工作流工具，社区提供大量工作流模板与插件。                                                                                  | AI工作流 | [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | [GPL 3.0](#Protocol-document-link)    |

## AI工具

### 图像生成

| 项目简要                                                                                                                                      | 主要功能 | 地址（点击访问）                                                                  | 使用许可证                          |
| --------------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------------------------------------------------------------------- | ----------------------------------- |
| Stable Diffusion WebUI 是成熟的图像生成 Web 界面项目，插件生态丰富，并支持扩展到视频等相关工作流。 | 图像生成 | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#Protocol-document-link) |

### 音频处理

#### 音频分离与降噪

| 项目简要                                                                   | 主要功能      | 地址（点击访问）                                                                   | 使用许可证                            |
| -------------------------------------------------------------------------- | ------------- | ---------------------------------------------------------------------------------- | ------------------------------------- |
| 音频处理整合项目，覆盖分离、降噪等常见能力。                               | 音频分离/降噪 | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#Protocol-document-link)   |

#### 音色转换

| 项目简要                                     | 主要功能 | 地址（点击访问）                                                                   | 使用许可证                            |
| -------------------------------------------- | -------- | ---------------------------------------------------------------------------------- | ------------------------------------- |
| 开源音色转换项目，社区认知度较高。           | 音色转化 | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#Protocol-document-link)        |

#### 文字转语音

| 项目简要                                   | 主要功能   | 地址（点击访问）                                     | 使用许可证                            |
| ------------------------------------------ | ---------- | ---------------------------------------------------- | ------------------------------------- |
| 开源文字转语音项目，兼顾效果与生态。       | 文字转语音 | [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS) | [MIT](#Protocol-document-link)        |
| Voxtral-4B-TTS 是 Mistral 开源的多语言文字转语音模型，支持 9 种语言与 3 秒参考音频的零样本语音克隆，延迟约 70ms。 | 文字转语音 | [Voxtral-4B-TTS](https://huggingface.co/mistralai/Voxtral-4B-TTS-2603) | [CC BY-NC 4.0](#Protocol-document-link) |
| Fish Speech（Fish Audio S2 Pro）是基于 Dual-AR 架构与 RL 对齐的多语言文字转语音系统，支持自然语言语调控制与 80 余种语言的多说话人生成。 | 文字转语音 | [fish-speech](https://github.com/fishaudio/fish-speech) | [FISH AUDIO RESEARCH LICENSE](https://github.com/fishaudio/fish-speech/blob/main/LICENSE) |

### 编码代理

| 项目简要                                                                                                                                      | 主要功能 | 地址（点击访问）                                    | 使用许可证                            |
| --------------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------------------------------------- | ------------------------------------- |
| OpenCode 是开源 AI 编码代理，强调终端体验与客户端/服务端架构，适合在本地环境中进行交互式编码、执行与远程驱动。                                | AI编码代理 | [opencode](https://github.com/anomalyco/opencode)   | [MIT](#Protocol-document-link)        |

### 其它

| 项目简要                                                                                                  | 主要功能  | 地址（点击访问）                                                           | 使用许可证                            |
| --------------------------------------------------------------------------------------------------------- | --------- | -------------------------------------------------------------------------- | ------------------------------------- |
| light-ocr 是面向 Node.js 与 C++ 的快速离线 OCR 工具包，基于 PP-OCRv6 与 ONNX Runtime，并可选使用 CoreML 和 WebGPU 加速。 | OCR | [light-ocr](https://github.com/arcships/light-ocr) | [Apache 2.0](#Protocol-document-link) |
| 类 ChatGPT Web 应用项目，适合基于 API 快速搭建通用对话界面。 | 类ChatGPT | [open-webui](https://github.com/open-webui/open-webui)                     | [MIT](#Protocol-document-link)        |

# 基础设施

## 权限控制

| 项目简要                                                                                                                                | 类型     | 地址（点击访问）                              | 使用许可证                            |
| --------------------------------------------------------------------------------------------------------------------------------------- | -------- | --------------------------------------------- | ------------------------------------- |
| Casbin 是开源访问控制库，支持 RBAC、ABAC 等常见访问控制模型。 | 权限管理 | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#Protocol-document-link) |
| Casdoor 是同一生态中的身份验证项目（IAM/SSO）。                                                                                         | 身份验证 | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#Protocol-document-link) |

## 网络控制

| 项目简要                                             | 类型     | 地址（点击访问）                       | 使用许可证                         |
| ---------------------------------------------------- | -------- | -------------------------------------- | ---------------------------------- |
| NPS 可以搭建内网穿透代理，并提供 Web 管理界面。 | 内网穿透 | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#Protocol-document-link) |

## 数据存储与缓存

| 项目简要                                                                                                                                | 地址（点击访问）                                    | 类型       | 使用许可证                                 |
| --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------- | ---------- | ------------------------------------------ |
| TiDB 是金融级分布式数据库，兼容 MySQL API，同时支持 OLAP 与 OLTP。                                                                         | [tidb](https://github.com/pingcap/tidb)             | New-SQL-DB | [Apache 2.0](#Protocol-document-link)      |
| OceanBase Database 是一个分布式关系型数据库。完全由蚂蚁集团自主研发。 OceanBase 基于 Paxos 协议以及分布式架构，实现了高可用和线性扩展。 | [oceanbase](https://github.com/oceanbase/oceanbase) | New-SQL-DB | [Mulan PubL v2](#Protocol-document-link)   |
| Qdrant 是一个 Rust 编写的向量数据库，具备分布式生产能力。                                                                               | [qdrant](https://github.com/qdrant/qdrant)          | Vector-DB  | [Apache 2.0](#Protocol-document-link)      |
| Milvus 是一个由 Go 和 C++ 编写的向量数据库，具备分布式生产能力。                                                                        | [milvus](https://github.com/milvus-io/milvus)       | Vector-DB  | [Apache 2.0](#Protocol-document-link)      |
| 高性能内存 KV 数据库与缓存系统，广泛用于缓存、消息与数据结构场景。                                                                     | [redis](https://github.com/redis/redis)             | KV-Cache   | [独立协议](https://github.com/redis/redis) |

## 交付与镜像构建

### CD

| 项目简要                                                                                                                                                                                                                                              | 地址（点击访问）                                | 使用许可证                            |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- | ------------------------------------- |
| Kubernetes 是主流容器编排与集群管理平台，提供声明式部署、服务发现、扩缩容、自愈和滚动更新等能力。                                                          | [k8s](https://github.com/kubernetes/kubernetes) | [Apache 2.0](#Protocol-document-link) |

### 容器能力

| 项目简要                                                                                                                | 地址（点击访问）                                       | 使用许可证                            |
| ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------- |
| containerd 是容器运行时，负责镜像拉取、容器生命周期管理与执行，常作为 Kubernetes 节点运行时，也可独立用于本地或单机环境；本身不负责镜像构建。                   | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#Protocol-document-link) |
| BuildKit 是现代镜像构建工具链，支持高效缓存、并行构建、多平台构建和无 root 运行；Docker Engine 23.0 起，`docker build` 默认基于 Buildx/BuildKit。               | [buildkit](https://github.com/moby/buildkit)           | [Apache 2.0](#Protocol-document-link) |

# 语言能力

## 跨语言框架

### RPC

| 项目简要                                                                                           | 地址（点击访问）                           | 使用许可证                            |
| -------------------------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------- |
| gRPC 是 Google 开源的跨语言 RPC 框架，基于 HTTP/2，支持双向流、超时控制、认证与代码生成，广泛用于服务间通信。 | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#Protocol-document-link) |
| Thrift 最初由 Facebook 开发，现为 Apache 基金会项目，提供 IDL、代码生成以及可替换的传输层与协议层实现。     | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#Protocol-document-link) |

## Python

### AI能力

#### LLM应用框架

| 项目简要                                                                                                                              | 地址（点击访问）                                       | 使用许可证                            |
| ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ | ------------------------------------- |
| LangChain 是一个用于开发和管理基于大型语言模型应用程序的框架，提供标准化接口和工具链，简化与 AI 模型的交互、数据处理和应用开发流程。 | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#Protocol-document-link)        |

#### 模型训练与推理工具

| 项目简要                                                                                                               | 地址（点击访问）                                      | 使用许可证                            |
| ---------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------- |
| Huggingface 开源的 Diffusers 是扩散模型训练与推理工具库，覆盖图像、音频与 3D 等场景。                             | [diffusers](https://github.com/huggingface/diffusers) | [Apache 2.0](#Protocol-document-link) |
| Unsloth 是面向开源模型本地训练与推理的工具链，支持微调、强化学习、导出与统一本地界面，强调低显存占用与训练效率。   | [unsloth](https://github.com/unslothai/unsloth)        | [多种协议](https://github.com/unslothai/unsloth) |

#### 算法框架

| 项目简要                                                             | 地址（点击访问）                                       | 使用许可证                                                       |
| -------------------------------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------------- |
| PyTorch 是主流深度学习框架之一，易于上手、生态完整，由 PyTorch Foundation 推动开放治理。 | [pytorch](https://github.com/pytorch/pytorch)          | [独立协议](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow 是 Google 推动的工程化机器学习框架，覆盖训练、推理、部署与移动端等场景。               | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#Protocol-document-link)                            |
| JAX 是面向加速器的高性能数组计算与程序变换库，强调 JIT 编译、自动微分、向量化与并行化能力。       | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#Protocol-document-link)                            |

## Golang

### AI能力

#### LLM应用框架

| 项目简要                                                        | 地址（点击访问）                          | 使用许可证                            |
| --------------------------------------------------------------- | ----------------------------------------- | ------------------------------------- |
| Eino 是字节跳动开源的 Go 语言大模型工具链框架，对标产品是 LangChain。 | [eino](https://github.com/cloudwego/eino) | [Apache 2.0](#Protocol-document-link) |

### 基础能力

| 项目简要                                     | 地址（点击访问）                                          | 使用许可证                            |
| -------------------------------------------- | --------------------------------------------------------- | ------------------------------------- |
| Go 语言协程池库。                            | [ants](https://github.com/panjf2000/ants)                 | [MIT](#Protocol-document-link)        |
| Go 语言 map 与 struct 相互解析的库。         | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#Protocol-document-link)        |
| Sonic 是高性能 JSON 库，通过 JIT 与 SIMD 加速，在无需代码生成的前提下提供高效的序列化与反序列化能力。 | [sonic](https://github.com/bytedance/sonic)               | [Apache 2.0](#Protocol-document-link) |
| 内存缓存库，支持配置最大缓存大小。           | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#Protocol-document-link) |
| 内存缓存库，相较于 bigcache 配置更简单。     | [freecache](https://github.com/coocood/freecache)         | [MIT](#Protocol-document-link)        |
| 无锁且并发安全的Map                          | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#Protocol-document-link)        |

### 工具库

| 项目简要                                                                                                          | 地址（点击访问）                                  | 使用许可证                            |
| ----------------------------------------------------------------------------------------------------------------- | ------------------------------------------------- | ------------------------------------- |
| ffmpeg-python 的 Go 语言实现。[FFmpeg](https://github.com/FFmpeg/FFmpeg) 是一个 C 语言开发的知名开源音视频数据处理库。 | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#Protocol-document-link) |

### HTTP

#### Server

| 项目简要                                                                       | 地址（点击访问）                            | 使用许可证                            |
| ------------------------------------------------------------------------------ | ------------------------------------------- | ------------------------------------- |
| Hertz 是字节跳动开源的 Go 微服务 HTTP 框架，强调高性能、高易用性与可扩展性，适合对性能和工程化都有要求的场景。 | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#Protocol-document-link) |

#### Client

| 项目简要             | 地址（点击访问）                           | 使用许可证                     |
| -------------------- | ------------------------------------------ | ------------------------------ |
| HTTP客户端常用的库。 | [resty](https://github.com/go-resty/resty) | [MIT](#Protocol-document-link) |

### RPC

#### Server

| 项目简要                                                                                                                                                   | 地址（点击访问）                            | 使用许可证                            |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------- |
| Kitex 是字节跳动开源的 Go RPC 框架，支持 Thrift、Kitex Protobuf 与 gRPC，提供代码生成、治理扩展和流式通信能力。 | [kitex](https://github.com/cloudwego/kitex) | [Apache 2.0](#Protocol-document-link) |

### 服务框架

| 项目简要                                                                                                                                               | 地址（点击访问）                              | 使用许可证                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------- | ------------------------------ |
| Kratos 是面向微服务的 Go 框架，默认支持 HTTP 和 gRPC，提供工程化目录、配置、日志、注册发现与中间件等基础能力。 | [kratos](https://github.com/go-kratos/kratos) | [MIT](#Protocol-document-link) |

### GUI

| 项目简要                                                                                                   | 地址（点击访问）                        | 使用许可证                       |
| ---------------------------------------------------------------------------------------------------------- | --------------------------------------- | -------------------------------- |
| Fyne 是 Go 语言 GUI 框架，支持桌面与移动端应用开发，提供统一的组件、布局与打包能力。 | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#Protocol-document-link) |

### 操作系统接口

| 项目简要                                                                                                                                  | 地址（点击访问）                               | 使用许可证                       |
| ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------- | -------------------------------- |
| Gopsutil 是一个用于系统监控、分析和限制进程资源以及管理进程的库，它是 Python 项目 [psutil](https://github.com/giampaolo/psutil) 的 Go 语言实现。 | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#Protocol-document-link) |

# Java

## Android

### 权限管理

| 项目简要                      | 地址（点击访问）                                              | 使用许可证                            |
| ----------------------------- | ------------------------------------------------------------- | ------------------------------------- |
| 一个好用的Android权限申请库。 | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#Protocol-document-link) |

# 字体

| 项目简要     | 语种   | 可商用         | 地址                                        | 使用许可证                                          |
| ------------ | ------ | -------------- | ------------------------------------------- | --------------------------------------------------- |
| 谷歌免费字体 | 多语种 | 多数情况下可以 | [fonts.google.com](https://fonts.google.com)        | [多种协议](https://developers.google.com/fonts/faq) |
| 阿里免费字体 | 中文   | 多数情况下可以 | [www.alibabafonts.co](https://www.alibabafonts.com) | [独立协议](https://www.alibabafonts.com/#/more)     |

<a id="Protocol-document-link"></a>

# 许可证原文链接

| 许可证                   | 原文链接                                                                             |
| ------------------------ | ------------------------------------------------------------------------------------ |
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
