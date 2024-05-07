<p align="center">
  <a href="https://github.com/skys-mission/open-power">
    <img  src="./.images/LOGO.png" width="350" border="0" alt="open-power">
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

- [Index](#index)
- [AI](#ai)
- [DEV](#dev)

# AI

## Production-ready-tools

| Project Summary                                                                                                                                                                                                                                                                                   | Address (click to visit)                                                          | License                           |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------|-----------------------------------|
| Stable-diffusion-webui can build a web page for AI drawing with one click, making AI drawing simple. Currently, the ecosystem is very rich, and there are a large number of excellent plugins in the community.                                                                                   | [stable-diffusion-webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) | [AGPL 3.0](#quoting-license-text) |
| This is a production-level, low-code node editing mode Web project that operates the Diffusers library. Similarly, the community has a large number of workflow templates and plugins available.                                                                                                  | [ComfyUI](https://github.com/comfyanonymous/ComfyUI)                              | [GPL 3.0](#quoting-license-text)  |
| A tool for separating vocals from audio, where the developer has trained most of the models included in the software package. Although the project’s README mentions that it is licensed under MIT, the MIT license file has been removed from the project, and the reason for this is not known. | [UVR](https://github.com/Anjok07/ultimatevocalremovergui)                         | [MIT](#quoting-license-text)      |
| A classic face swapping project, where the owner of this project believes that such projects have no value beyond academic significance and only serve to subject vulnerable groups to online fraud.                                                                                              | [DeepFaceLive](https://github.com/iperov/DeepFaceLive)                            | [GPL 3.0](#quoting-license-text)  |

## Utility library

| Project Summary                                                                                                                                                           | Address (click to visit)                              | License                             |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------|-------------------------------------|
| Huggingface’s open-source Diffusers is the go-to library for generating images, audio, and even 3D structures of molecules using the latest pre-trained diffusion models. | [diffusers](https://github.com/huggingface/diffusers) | [Apache 2.0](#quoting-license-text) |

## Artificial Intelligence models

| Project Summary                                                                                                                                                                                                                                                                                | Address (click to visit)                                                        | License                                         |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------|-------------------------------------------------|
| Stable-diffusion is currently the most well-known open-source text-to-image model. Due to reasons that are not entirely clear, as of May 7, 2024, the owner of this project believes that the subsequent versions released by Stability.ai are not as active in the community as this version. | [stable-diffusion](https://github.com/CompVis/stable-diffusion)                 | [CreativeML Open RAIL-M](#quoting-license-text) |
| Stable Diffusion v1-5 is, in fact, the most active model in the community based on stable-diffusion as of now. However, the related technology has not been updated for a year (as of May 7, 2024).                                                                                            | [stable-diffusion v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5n) | [CreativeML Open RAIL-M](#quoting-license-text) |

## Algorithm frameworks

| Project Summary                                                                                 | Address (click to visit)                      | License                                                         |
|-------------------------------------------------------------------------------------------------|-----------------------------------------------|-----------------------------------------------------------------|
| If you don't know Pytorch, it means you know nothing about artificial intelligence development. | [pytorch](https://github.com/pytorch/pytorch) | [pytorch](https://github.com/pytorch/pytorch/blob/main/LICENSE) |

# DEV

## Cross-language

### RPC

We don’t believe that the pros and cons of various RPC protocols are fundamentally meaningful. Perhaps, it’s sufficient
to just pick one and use it.

| Project Summary                                                                                                                                             | Address (click to visit)                   | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------|-------------------------------------|
| gRPC is a language-agnostic RPC protocol introduced by Google, which uses HTTP/2 and increases performance through the use of a predefined fields protocol. | [grpc](https://github.com/grpc/grpc)       | [Apache 2.0](#quoting-license-text) |
| If you don’t want to use gRPC, Thrift is a good alternative, but currently, the editors of this project are not familiar with this framework.               | [thrift](https://github.com/apache/thrift) | [Apache 2.0](#quoting-license-text) |

## Database

| Project Summary                                                                                                                                                                                               | Address (click to visit)                            | License                                |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------|----------------------------------------|
| OceanBase Database is a distributed relational database, fully developed by Ant Group. Based on the Paxos protocol and distributed architecture, OceanBase achieves high availability and linear scalability. | [oceanbase](https://github.com/oceanbase/oceanbase) | [Mulan PubL v2](#quoting-license-text) |

## Golang

### Basic capabilities

| Project Summary                                                                                                                                                                                                     | Address (click to visit)                                  | License                             |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------|-------------------------------------|
| This is a goroutine pool library for the Go language that we reliably use in production.                                                                                                                            | [ants](https://github.com/panjf2000/ants)                 | [MIT](#quoting-license-text)        |   
| A library for converting between Go language maps and structs.                                                                                                                                                      | [mapstructure](https://github.com/mitchellh/mapstructure) | [MIT](#quoting-license-text)        |
| Relative to native maps, bigcache reduces GC overhead through various techniques and allows setting an expiration time for cached data, performing exceptionally well compared to similar libraries in all aspects. | [bigcache](https://github.com/allegro/bigcache)           | [Apache 2.0](#quoting-license-text) |
| A lock-free and concurrent-safe hashmap that performs less efficiently than the native map in serial scenarios.                                                                                                     | [hashmap](https://github.com/cornelk/hashmap)             | [Apache 2.0](#quoting-license-text) |

### Toolkit

| Project Summary                                                                                                                                                               | Address (click to visit)                          | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|-------------------------------------|
| I believe it is a smarter approach than the standard RFC UUID, suitable for unique string keys or the snowflake algorithm.                                                    | [ksuid](https://github.com/segmentio/ksuid)       | [MIT](#quoting-license-text)        |   
| A Go language implementation of ffmpeg-python, [FFmpeg](https://github.com/FFmpeg/FFmpeg) is a well-known open-source audio and video data processing library developed in C. | [ffmpeg-go](https://github.com/u2takey/ffmpeg-go) | [Apache 2.0](#quoting-license-text) |

### HTTP

| Project Summary                                                                                                                                                                                                   | Address (click to visit)                    | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------|-------------------------------------|
| The HTTP framework open-sourced by Douyin Group (TikTok's parent company), according to the benchmarks in the documentation, outperforms the fasthttp framework in both performance and stability. I'm convinced. | [hertz](https://github.com/cloudwego/hertz) | [Apache 2.0](#quoting-license-text) |   
| Commonly used HTTP client libraries.                                                                                                                                                                              | [resty](https://github.com/go-resty/resty)  | [MIT](#quoting-license-text)        |

### Container capabilities

| Project Summary                                                                                                                                                                                                                                             | Address (click to visit)                               | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------|-------------------------------------|
| A container runtime tool responsible for starting, stopping, pausing, and deleting containers. It is typically deployed in conjunction with Kubernetes-like projects and is generally not used for single nodes or personal use, as it cannot build images. | [containerd](https://github.com/containerd/containerd) | [Apache 2.0](#quoting-license-text) |   

### Production projects

| Project Summary                                                                                                                                                                                                                                             | Address (click to visit)                      | License                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------|-------------------------------------|
| Casbin is a powerful and efficient open-source access control library that supports RBAC, ABAC, and more. However, we believe that complex permission management, arcane professional terminology, and low-code solutions may not be suitable for everyone. | [casbin](https://github.com/casbin/casbin)    | [Apache 2.0](#quoting-license-text) |
| An identity authentication project (IAM/SSO) from the same organization as Casbin.                                                                                                                                                                          | [casdoor](https://github.com/casdoor/casdoor) | [Apache 2.0](#quoting-license-text) |

### Development tools

| Project Summary                                       | Address (click to visit)                                          | License                      |
|-------------------------------------------------------|-------------------------------------------------------------------|------------------------------|
| A development plugin for sorting Go language imports. | [goimports-reviser](https://github.com/incu6us/goimports-reviser) | [MIT](#quoting-license-text) |   

### Gui

| Project Summary                                                                                                                                                                           | Address (click to visit)                | License                        |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|--------------------------------|
| Fyne is a GUI framework for the Go language that enables the creation of both desktop and mobile applications. Although I dislike CGO, there aren’t many good alternatives at the moment. | [fyne](https://github.com/fyne-io/fyne) | [BSD 3](#quoting-license-text) |   

### Network processing

| Project Summary                                                                                                                                                                                            | Address (click to visit)               | License                          |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------|----------------------------------|
| nps can set up an intranet penetration proxy with a web interface for the backend. We don’t believe that using a self-built solution for small projects is cost-effective compared to commercial products. | [nps](https://github.com/ehang-io/nps) | [GPL 3.0](#quoting-license-text) |   

### Operating system interface

| Project Summary                                                                                                                                                                                                         | Address (click to visit)                       | License                        |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|--------------------------------|
| gopsutil is a library used for system monitoring, analysis, limiting process resources, and managing processes. It is a Go language implementation of the Python project [psutil](https://github.com/giampaolo/psutil). | [gopsutil](https://github.com/shirou/gopsutil) | [BSD 3](#quoting-license-text) |   

### Python

## Script

| Project Summary                                                                                                                         | Address (click to visit)                       | License                      |
|-----------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------|------------------------------|
| A simple and easy-to-use script for crawling Bilibili live chat with minimal features, and it’s easy to modify for further development. | [blivedm](https://github.com/xfgryujk/blivedm) | [MIT](#quoting-license-text) |   

## Android

### Toolkit

| Project Summary                                          | Address (click to visit)                                      | License                             |
|----------------------------------------------------------|---------------------------------------------------------------|-------------------------------------|
| A user-friendly Android library for permission requests. | [XXPermissions](https://github.com/getActivity/XXPermissions) | [Apache 2.0](#quoting-license-text) |   

# quoting-license-text

| License                | Original Text                                                 |
|------------------------|---------------------------------------------------------------|
| MIT                    | https://opensource.org/license/mit                            |
| AGPL 3.0               | https://www.gnu.org/licenses/agpl-3.0.txt                     |
| GPL  3.0               | https://www.gnu.org/licenses/gpl-3.0.txt                      |
| Apache 2.0             | https://www.apache.org/licenses/LICENSE-2.0.txt               |
| BSD 3                  | https://opensource.org/license/bsd-3-clause                   |
| CreativeML Open RAIL-M | https://github.com/CompVis/stable-diffusion/blob/main/LICENSE |
| OFL1.1 2007            | https://openfontlicense.org/documents/OFL.txt                 |
| Mulan PubL v2          | http://license.coscl.org.cn/MulanPubL-2.0                     |
