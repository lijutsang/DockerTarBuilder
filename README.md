[![GitHub](https://img.shields.io/github/license/wukongdaily/DockerTarBuilder.svg?label=LICENSE&logo=github&logoColor=%20)](https://github.com/wukongdaily/DockerTarBuilder/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/wukongdaily/DockerTarBuilder.svg?style=flat&logo=appveyor&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/wukongdaily/DockerTarBuilder.svg?style=flat&logo=appveyor&label=Forks&logo=github) [![Github](https://img.shields.io/badge/RELEASE:DockerTarBuilder-123456?logo=github&logoColor=fff&labelColor=green&style=flat)](https://github.com/wukongdaily/DockerTarBuilder/releases) [![Bilibili](https://img.shields.io/badge/Bilibili-123456?logo=bilibili&logoColor=fff&labelColor=fb7299)](https://www.bilibili.com/video/BV1yyq6YREdF) 

## 🤔 这是什么？
[操作步骤](README_CN.md) | 简介 <br>
它是一个工作流。可快速构建指定架构/平台的单个或多个docker镜像 并存储在Artifact文件或Release文件

## 使用说明
https://wkdaily.cpolar.top/archives/gc
> 如果你的docker镜像小于2GB 你可以使用红色框框这三种Release工作流<br> 
> 如果你的docker镜像大于2GB且小于5GB 你可以使用蓝色框框的这三种Artifact工作流<br>
> 如果你的docker镜像大于5GB 比如 `vllm/vllm-openai:v0.6.4.post1` 抱歉了 只能自己解决网络问题直接pull了 本项目爱莫能助啦！

<img src="https://github.com/user-attachments/assets/e537c746-ec4f-4588-9315-ecf73a05b8d0" width="40%" />

## 2024-12-09 新增功能：
> 增加了新的工作流<br>
> 可以将docker镜像转存到自己项目的Github Release文件里<br>
## 2025-5月 新增下载提醒
对于Release文件，可以尝试直接使用“迅雷下载”，有一定概率加速。比如我这个项目里的Release 由于很多人下载过了，所以用迅雷下载很快。
如果迅雷速度是0 就把地址套用一下 下面的这些国内加速站的前缀 然后在复制到迅雷吧 这样下载大文件很快。

> [![Github](https://img.shields.io/badge/国内加速站下载-FC7C0D?logo=github&logoColor=fff&labelColor=000&style=for-the-badge)](https://wkdaily.cpolar.top/archives/1)

> [![Github](https://img.shields.io/badge/RELEASE:DockerTarBuilder-123456?logo=github&logoColor=fff&labelColor=green&style=for-the-badge)](https://github.com/wukongdaily/DockerTarBuilder/releases)<br>

> 如果Github Release文件下载缓慢 你可以在<br>         

> [![Github](https://img.shields.io/badge/国内加速站前缀套用点此处查看网址列表-FC7C0D?logo=github&logoColor=fff&labelColor=000&style=for-the-badge)](https://wkdaily.cpolar.top/archives/1)

## 2026-06-24 更新日志
> 适配 GitHub Actions Runner 的 Node 20 退役计划，升级工作流依赖：`actions/checkout@v5`、`actions/upload-artifact@v6`、`softprops/action-gh-release@v3`。<br>
> 优化 ARM64 工作流：部分镜像的 Docker Hub 标签显示为 `linux/arm64`，但 manifest list 的平台描述可能异常，导致 `docker pull --platform linux/arm64` 报错 `no matching manifest for linux/arm64 in the manifest list entries`。现在 ARM64 工作流会在严格拉取失败后自动重试普通拉取，并检查镜像实际架构必须是 `linux/arm64`，确认无误后才继续打包。<br>
> 例如：`amilys/embyserver_arm64v8:latest` 曾出现 Docker Hub 显示 ARM64，但 manifest list 平台描述异常的情况。
 
## 教学视频
https://www.bilibili.com/video/BV1EZ421M7mL<br>
https://www.bilibili.com/video/BV1yyq6YREdF
## 新手常见问题必看
https://github.com/wukongdaily/DockerTarBuilder/wiki
## 解压工具
> Windows 上推荐使用7zip<br>
> macOS 推荐使用MacZip<br>
> Linux上推荐直接用tar 命令

## ❤️其它GitHub Action项目推荐🌟 （建议收藏）⬇️
- ### [一键生成run插件] 🆕
- https://github.com/wukongdaily/RunFilesBuilder<br>
- ### [一键构建自定义软件包大小的Immortalwrt] 🆕
- https://github.com/wukongdaily/AutoBuildImmortalWrt
- ### [OpenWrt/Armbian 安装器ISO] 🆕
- https://github.com/wukongdaily/armbian-installer
## 在哪里可以搜索或查询docker镜像的详细信息
### [查询镜像的详细信息 点击这里直达](https://docker.fxxk.dedyn.io/)

