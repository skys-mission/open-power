<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/logo.webp?version=0.1" width="400" border="0" alt="open-power">
  </a>
</p>

其它语言：[English](README.md), (Currently unable to translate more)

# open-power

本仓库用于记录在生产力/性能/稳定/设计等因素中，有某一方面处于优良水平的开源项目。

你可以在这里最快速得到自己需要的技术选型。

欢迎讨论与贡献。

# 目录

<!-- TOC -->
* [open-power](#open-power)
* [目录](#目录)
* [项目](#项目)
  * [AI](#ai)
    * [AI中台](#ai中台)
    * [AI工具](#ai工具)
      * [通用工具](#通用工具)
      * [图形图像](#图形图像)
      * [音频处理](#音频处理)
      * [其它](#其它)
  * [权限控制](#权限控制)
  * [网络控制](#网络控制)
  * [消息中间件](#消息中间件)
  * [OPS](#ops)
  * [CI/CD](#cicd)
    * [CD](#cd)
    * [容器能力](#容器能力)
* [AI模型](#ai模型)
  * [生成式AI模型](#生成式ai模型)
    * [扩散模型](#扩散模型)
      * [图片生成](#图片生成)
      * [视频生成](#视频生成)
  * [大语言模型&多模态理解模型&自回归多模态模型](#大语言模型多模态理解模型自回归多模态模型)
* [语言能力](#语言能力)
  * [跨语言框架](#跨语言框架)
    * [RPC](#rpc)
  * [Python](#python)
    * [AI能力](#ai能力)
      * [AI工具库](#ai工具库)
      * [算法框架](#算法框架)
  * [Golang](#golang)
    * [AI能力](#ai能力-1)
      * [AI工具库](#ai工具库-1)
    * [基础能力](#基础能力)
    * [工具库](#工具库)
    * [HTTP](#http)
      * [Server](#server)
      * [Client](#client)
    * [RPC](#rpc-1)
      * [Server](#server-1)
    * [Server-frame](#server-frame)
    * [Gui](#gui)
    * [操作系统接口](#操作系统接口)
* [Java](#java)
  * [Android](#android)
    * [权限管理](#权限管理)
* [Font](#font)
* [Protocol document link](#protocol-document-link)
<!-- TOC -->

# 项目

## AI

### AI中台

| 项目简要                                                                             | 主要功能 | 地址（点击访问）                                   | 使用许可证                                      |
|----------------------------------------------------------------------------------|------|--------------------------------------------|--------------------------------------------|
| Dify是目前最强大的（截止到20250309）开源大语言模型中台，可以定义工作流，Agent等模版。项目不是完全基于Apache 2.0的，再多租户上有限制。 | AI中台 | [dify](https://github.com/langgenius/dify) | [多种协议](https://github.com/langgenius/dify) |

### AI工具

#### 通用工具

| 项目简要                                     | 主要功能  | 地址（点击访问）                                             | 使用许可证                              |
|------------------------------------------|-------|------------------------------------------------------|------------------------------------|
| 这是一个生产级别低代码节点编辑的AI流程编辑软件。社区存在大量的流程模版与插件。 | AI工作流 | [ComfyUI](https://github.com/comfyanonymous/ComfyUI) | [GPL 3.0](#Protocol-document-link) |

#### 图形图像

| 项目简要                                                                                  | 主要功能 | 地址（点击访问）                                                                          | 使用许可证                               |
|---------------------------------------------------------------------------------------|------|-----------------------------------------------------------------------------------|-------------------------------------|
| Stable-diffusion-webui可以一键构建AI画图的web页面，让AI画图变得简单，使用插件也具备视频生成功能，目前生态已经非常丰富，社区存在大量优秀插件。 | 图像生成 | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#Protocol-document-link) |
| 一个经典的脸部替换项目，请注意法律风险。                                                                  | 图像处理 | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                            | [GPL 3.0](#Protocol-document-link)  |

#### 音频处理

| 项目简要                                                                       | 主要功能    | 地址（点击访问）                                                                           | 使用许可证                                 |
|----------------------------------------------------------------------------|---------|------------------------------------------------------------------------------------|---------------------------------------|
| 比UVR5-UI更强大的音频处理整合项目，作者目前仍在活跃（截止到20250222）。                                | 音频分离/降噪 | [MSST-WebUI](https://github.com/SUC-DriverOld/MSST-WebUI)                          | [AGPL 3.0](#Protocol-document-link)   |
| 相对于大多数停更的SVC项目，RVC的作者仍在活跃（截止到20250222），开箱即用。                               | 音色转化    | [RVC-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI) | [MIT](#Protocol-document-link)        |
| 目前仍在更新的效果最好的文字转语音体系之一，社区活跃（截止到20250309）                                    | 文字转语音   | [GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)                               | [MIT](#Protocol-document-link)        |
| CosyVoice阿里开源的TTS体系，在一些场景下表现比GPT-SoVITS好，可惜目前社区仍不活跃，主要依靠官方支持。（截止到20250309） | 文字转语音   | [CosyVoice](https://github.com/FunAudioLLM/CosyVoice)                              | [Apache 2.0](#Protocol-document-link) |

#### 其它

| 项目简要                                                            | 主要功能     | 地址（点击访问）                                                                   | 使用许可证                                 |
|-----------------------------------------------------------------|----------|----------------------------------------------------------------------------|---------------------------------------|
| 基于langchain的大语言模型llm项目，支持RAG和Agent相关功能（Langchain-ChatGLM的改进项目）。 | 类ChatGPT | [Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat) | [Apache 2.0](#Protocol-document-link) |
| 一个开箱即用的仿ChatGPT项目（基于API的），功能支持较多，如果你想快速落地一个类ChatGPT项目，或许这是首选。   | 类ChatGPT | [open-webui](https://github.com/open-webui/open-webui)                     | [MIT](#Protocol-document-link)        |

## 权限控制

| 项目简要                                                                        | 类型   | 地址（点击访问）                                      | 使用许可证                                 |
|-----------------------------------------------------------------------------|------|-----------------------------------------------|---------------------------------------|
| casbin 是一个强大而高效的开源访问控制库，可以支持RBAC，ABAC，当然我们认为复杂的权限管理和绕口的专业名词，以及低代码可能并不适合所有人。 | 权限管理 | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#Protocol-document-link) |
| 和casbin同出一家的身份验证项目（IAM/SSO）。                                                | 身份验证 | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#Protocol-document-link) |

## 网络控制

| 项目简要                          | 类型   | 地址（点击访问）                               | 使用许可证                              |
|-------------------------------|------|----------------------------------------|------------------------------------|
| nps可以搭建起一个内网穿透代理，并拥有web界面的后台。 | 内网穿透 | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#Protocol-document-link) |

## 消息中间件

| 项目简要                                                                                   | 地址（点击访问）                                            | 类型         | 使用许可证                                    |
|----------------------------------------------------------------------------------------|-----------------------------------------------------|------------|------------------------------------------|
| TIDB金融级分布式数据库，兼容MysqlAPI，同时支持OLAP和OLTP。相较于OceanBase，TIDB的开源氛围更好。                       | [tidb](https://github.com/pingcap/tidb)             | New-SQL-DB | [Apache 2.0](#Protocol-document-link)    |
| OceanBase Database 是一个分布式关系型数据库。完全由蚂蚁集团自主研发。 OceanBase 基于 Paxos 协议以及分布式架构，实现了高可用和线性扩展。 | [oceanbase](https://github.com/oceanbase/oceanbase) | New-SQL-DB | [Mulan PubL v2](#Protocol-document-link) |
| qdrant是一个rust编写的向量数据库，具备分布式生产能力                                                        | [qdrant](https://github.com/qdrant/qdrant)          | Vector-DB  | [Apache 2.0](#Protocol-document-link)    |
| milvus是一个go和c++编写的向量数据库，具备分布式生产能力                                                      | [milvus](https://github.com/milvus-io/milvus)       | Vector-DB  | [Apache 2.0](#Protocol-document-link)    |
| 共享KV内存缓存项目，至今我没有发现redis的替代品                                                            | [redis](https://github.com/redis/redis)             | KV-Cache   | [独立协议](https://github.com/redis/redis)   |

## OPS

## CI/CD

### CD

| 项目简要                                                                                                                                   | 地址（点击访问）                                        | 使用许可证                                 |
|----------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------|---------------------------------------|
| K8S是一个标准的流程编排CD系统，已经被一些人誉为分布式操作系统。其实就是一个CD系统（我指的K8S核心功能，而非K8S/云原生生态），我不明白为什么有这么高的评价。现代中大型企业的业务应用基本都被K8S管控，目前K8S生态已经开始向有状态应用和GPU应用管控发展。 | [k8s](https://github.com/kubernetes/kubernetes) | [Apache 2.0](#Protocol-document-link) |   

### 容器能力

| 项目简要                                                          | 地址（点击访问）                                               | 使用许可证                                 |
|---------------------------------------------------------------|--------------------------------------------------------|---------------------------------------|
| 一个容器运行时工具，负责启动、停止、暂停、删除容器，通常和k8s类项目组合部署，一般不用做单节点或个人使用，无法构建镜像。 | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#Protocol-document-link) |   
| Kaniko不再维护，你总是要构建镜像，选一个合适的工具                                  | [buildkit](https://github.com/moby/buildkit)           | [Apache 2.0](#Protocol-document-link) |

# AI模型

## 生成式AI模型

### 扩散模型

#### 图片生成

| 项目简要                                                                                                              | 地址（点击访问）                                                                                        | 使用许可证                                               |
|-------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|-----------------------------------------------------|
| stable diffusion v1-5 是CompVis原始版本的改进版本，目前仍是工具链最完善的图像底座模型没有之一。（截止到20250222）                                       | [stable-diffusion v1-5](https://huggingface.co/stable-diffusion-v1-5/stable-diffusion-v1-5)     | [CreativeML Open RAIL-M](#Protocol-document-link)   |
| stable-diffusion-xl-base-1.0 由stabilityai开发的sd高清版本，虽然出现了一些比较新的技术，但关于相关工具链，例如controlnet等的完善程度仅次于sd1.5（截止到20250222） | [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) | [CreativeML Open RAIL++-M](#Protocol-document-link) |

#### 视频生成

| 项目简要                                                             | 地址（点击访问）                                                    | 使用许可证                                               |
|------------------------------------------------------------------|-------------------------------------------------------------|-----------------------------------------------------|
| 混元视频生成模型，由腾讯开发有图生视频，文生视频等多个版本                                    | [HunyuanVideo](https://huggingface.co/tencent/HunyuanVideo) | [独立协议](https://huggingface.co/tencent/HunyuanVideo) |
| 阿里系开源的视频生成模型，有众多版本，开源模型中表现良好。使用协议从github页面上看是apche2.0，但模型页面没有标注。 | [Wan-Video](https://github.com/Wan-Video)                   | [Apache 2.0](#Protocol-document-link)               |

## 大语言模型&多模态理解模型&自回归多模态模型

多模态模型通常是基于大语言模型的改造版本

| 项目简要                                                                                  | 多模态    | 地址（点击访问）                                   | 使用许可证                                                                             |
|---------------------------------------------------------------------------------------|--------|--------------------------------------------|-----------------------------------------------------------------------------------|
| 25年初一鸣惊人的deepseek，目前相较于claude，qwen的顶级模型在一些场景下已经略显落后，截止到20250703                       | 有多模态版本 | [deepseek](https://github.com/deepseek-ai) | [MIT](#Protocol-document-link)                                                    |
| llama由meta发布的大语言模型，开源生态链比较丰富，但支持的语种较少。                                                | 部分版本   | [Llama](https://www.llama.com/)            | [独立协议](https://www.llama.com/docs/how-to-guides/responsible-use-guide-resources/) |
| qwen由阿里发布的大语言模型，包含图片理解，音频理解，数学，代码优化版本。                                                | 有多模态版本 | [QwenLM](https://github.com/QwenLM)        | [多种协议](https://huggingface.co/Qwen)                                               |
| glm由清华大学发布的大语言模型，在24年Q4前（不包括Q4）开源领域具有强大优势，有图片理解和音频对话，代码优化版本。目前落后偏多，考虑移除收藏，截止到20250703 | 有多模态版本 | [GLM4](https://github.com/THUDM/GLM-4)     | [多种协议](https://huggingface.co/THUDM)                                              |

# 语言能力

## 跨语言框架

### RPC

| 项目简要                                                           | 地址（点击访问）                                   | 使用许可证                                 |
|----------------------------------------------------------------|--------------------------------------------|---------------------------------------|
| GRPC是Google推出的跨语言RPC协议，使用HTTP/2并通过预先定义字段协议从而增加性能。 灵活性不如thrift。 | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#Protocol-document-link) |
| thrift是meta推出的跨语言RPC协议，可以自定义协议，原生不支持流式传输。性能不如GRPC。             | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#Protocol-document-link) |

## Python

### AI能力

#### AI工具库

| 项目简要                                                                     | 地址（点击访问）                                               | 使用许可证                                 |
|--------------------------------------------------------------------------|--------------------------------------------------------|---------------------------------------|
| Huggingface开源的Diffusers是用于生成图像、音频甚至分子3D结构的最新预训练扩散模型的首选库。                 | [diffusers](https://github.com/huggingface/diffusers)  | [Apache 2.0](#Protocol-document-link) |
| langchain是一个用于开发和管理基于大型语言模型应用程序的框架，它提供标准化接口和工具链，简化了与AI模型的交互、数据处理和应用开发流程。 | [langchain](https://github.com/langchain-ai/langchain) | [MIT](#Protocol-document-link)        |

#### 算法框架

| 项目简要                                   | 地址（点击访问）                                               | 使用许可证                                                        |
|----------------------------------------|--------------------------------------------------------|--------------------------------------------------------------|
| PyTorch简单易用，初学者首选，目前由Meta牵头维护。         | [pytorch](https://github.com/pytorch/pytorch)          | [独立协议](https://github.com/pytorch/pytorch/blob/main/LICENSE) |
| TensorFlow是Google的工程化AI框架解决方案。         | [tensorflow](https://github.com/tensorflow/tensorflow) | [Apache 2.0](#Protocol-document-link)                        |
| Google近年来投入了较大精力的AI框架，特点是性能更高，但学习曲线陡峭。 | [jax](https://github.com/jax-ml/jax)                   | [Apache 2.0](#Protocol-document-link)                        |

## Golang

### AI能力

#### AI工具库

| 项目简要                                    | 地址（点击访问）                                  | 使用许可证                                 |
|-----------------------------------------|-------------------------------------------|---------------------------------------|
| eino字节跳动开源的go语言大模型工具链框架，对标产品是langchain。 | [eino](https://github.com/cloudwego/eino) | [Apache 2.0](#Protocol-document-link) |

### 基础能力

| 项目简要                   | 地址（点击访问）                                                  | 使用许可证                                 |
|------------------------|-----------------------------------------------------------|---------------------------------------|
| 这是一个GO语言协程池库，我们稳定用于生产。 | [ants](https://github.com/panjf2000/ants)                 | [MIT](#Protocol-document-link)        |   
| go语言map和struct互相解析的库。  | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#Protocol-document-link)        |
| 开箱即用的内存缓存库，也可以配置最大缓存大小 | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#Protocol-document-link) |
| 内存缓存库，相较于bigcache配置更简单 | [freecache](https://github.com/coocood/freecache)         | [MIT](#Protocol-document-link)        |
| 无锁且并发安全的Map            | [haxmap](https://github.com/alphadose/haxmap)             | [MIT](#Protocol-document-link)        |

### 工具库

| 项目简要                                                                                   | 地址（点击访问）                                          | 使用许可证                                 |
|----------------------------------------------------------------------------------------|---------------------------------------------------|---------------------------------------|
| 我认为比标准RFC文档UUID更聪明的做法，适用于分布式ID或字符串唯一键，前缀是有序的。                                          | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#Protocol-document-link)        |   
| ffmpeg-python的Go语言实现，[FFmpeg](https://github.com/FFmpeg/FFmpeg) 是一个C语言开发的知名开源音视频数据处理库。 | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#Protocol-document-link) |

### HTTP

#### Server

| 项目简要                                          | 地址（点击访问）                                    | 使用许可证                                 |
|-----------------------------------------------|---------------------------------------------|---------------------------------------|
| 抖音集团开源的HTTP框架，根据文档中的基准测试，性能和稳定性均超过fasthttp框架。 | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#Protocol-document-link) |   

#### Client

| 项目简要         | 地址（点击访问）                                   | 使用许可证                          |
|--------------|--------------------------------------------|--------------------------------|
| HTTP客户端常用的库。 | [resty](https://github.com/go-resty/resty) | [MIT](#Protocol-document-link) |

### RPC

#### Server

| 项目简要                                                                                       | 地址（点击访问）                                    | 使用许可证                                 |
|--------------------------------------------------------------------------------------------|---------------------------------------------|---------------------------------------|
| 抖音集团开源的RPC Server框架，使用同为抖音开源的高性能网络库，目前主要支持为Thrift，虽然项目显示支持GRPC，但官方主要支持的协议是Thrift有自研高性能解析库。 | [kitex](https://github.com/cloudwego/kitex) | [Apache 2.0](#Protocol-document-link) |   

### Server-frame

| 项目简要                                                                                        | 地址（点击访问）                                      | 使用许可证                          |
|---------------------------------------------------------------------------------------------|-----------------------------------------------|--------------------------------|
| 由bilibili主导的go语言开源框架，中规中矩，简单易用，生态完善，如果你擅长使用GRPC生态可以使用该框架快速构建你的mvp，模版项目同时启动http和grpc server。 | [kratos](https://github.com/go-kratos/kratos) | [MIT](#Protocol-document-link) |   

https://github.com/go-kratos/kratos

### Gui

| 项目简要                                                        | 地址（点击访问）                                | 使用许可证                            |
|-------------------------------------------------------------|-----------------------------------------|----------------------------------|
| fyne是一个go语言的gui框架，它不仅能制作桌面程序还能打包移动程序。虽然我讨厌CGO，但目前实在没什么好的选择。 | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#Protocol-document-link) |   

### 操作系统接口

| 项目简要                                                                                                | 地址（点击访问）                                       | 使用许可证                            |
|-----------------------------------------------------------------------------------------------------|------------------------------------------------|----------------------------------|
| gopsutil是一个用于系统监控、分析和限制进程资源以及管理进程得库，它是python项目[psutil](https://github.com/giampaolo/psutil)的go语言实现。 | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#Protocol-document-link) |   

# Java

## Android

### 权限管理

| 项目简要               | 地址（点击访问）                                                      | 使用许可证                                 |
|--------------------|---------------------------------------------------------------|---------------------------------------|
| 一个好用的Android权限申请库。 | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#Protocol-document-link) |   

# Font

| 项目简要   | 语种  | 可商用     | 地址                                          | 使用许可证                                           |
|--------|-----|---------|---------------------------------------------|-------------------------------------------------|
| 谷歌免费字体 | 多语种 | 多数情况下可以 | [fonts.google.com](fonts.google.com)        | [多种协议](https://developers.google.com/fonts/faq) |
| 阿里免费字体 | 中文  | 多数情况下可以 | [www.alibabafonts.co](www.alibabafonts.com) | [独立协议](https://www.alibabafonts.com/#/more)     |

# Protocol document link

| 许可证                      | 原文链接                                                                                 |
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
