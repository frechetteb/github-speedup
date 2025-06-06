# GitHub 加速站免费开源项目

![GitHub Release](https://img.shields.io/github/v/release/WJQSERVER-STUDIO/ghproxy)
![Go Version](https://img.shields.io/github/go-mod/go-version/WJQSERVER-STUDIO/ghproxy)
![Go Report Card](https://goreportcard.com/badge/github.com/WJQSERVER-STUDIO/ghproxy)
## 目录

- [项目简介](#项目简介)
- [项目特点](#项目特点)
- [快速开始](#快速开始)
  - [Git clone 仓库加速](#Git-clone-仓库加速)
  - [Raw 加速](#Raw-加速)
  - [Release 文件加速](#Release-文件加速)
  - [Docker(OCI) 代理加速（Beta）](#DockerOCI-代理加速Beta)
- [项目相关](#项目相关)
  - [演示站](#演示站)
  - [TG 讨论群组](#tg-讨论群组)
  - [项目文档](#项目文档)
- [致谢](#致谢)

## 项目简介
GitHub 加速站开源项目是一个专为开发者打造的高性能GitHub加速项目，公益性质、100%永久免费使用，提供全方位GitHub加速服务，包括 Git clone 克隆加速、Raw 文件实时加速、Release 文件高速下载以及 Docker 镜像代理加速（Beta），旨在解决 GitHub 资源访问慢、下载失败等问题。基于 Go 语言开发，性能卓越且资源占用极低，支持便捷自托管部署。作为国内领先的 GitHub 访问解决方案，已帮助数千开发者提升工作效率，彻底告别网络限制带来的开发困扰。

本项目后端基于 [ghproxy](https://github.com/WJQSERVER-STUDIO/ghproxy) 开发，特别鸣谢 @WJQSERVER-STUDIO 的开源贡献。

若您喜欢这个开源项目提供的免费 GitHub 加速服务，请给予点赞（Star）。

## 项目特点

- ⚡ **高性能**：基于 Go 语言实现，跨平台，提供高并发性能。
- 🌐 **现代框架**：使用字节旗下的 HertZ 作为 Web 框架。
- 📡 **高效客户端**：采用 Touka-HTTPC 作为 HTTP 客户端。
- 📥 **多种文件拉取支持**：支持 Git clone、raw、Release 等多种文件拉取方式。
- 🐳 **镜像仓库支持**：支持反代 Docker、GHCR 等镜像仓库。
- 🎨 **多主题支持**：提供多个前端主题，满足不同用户需求。
- 🚫 **灵活的访问控制**：支持自定义黑名单和白名单。
- 🗄️ **高效缓存**：支持 Git Clone 缓存，配合 Smart-Git 使用效果更佳。
- 🐳 **多种部署方式**：支持自托管和 Docker 容器化部署。
- 🐚 **脚本加速**：支持 shell 脚本多层嵌套加速，提高下载效率。

## 快速开始
### Git clone 仓库加速

> **提示**：只需在原始 GitHub 链接前添加 `github-speedup.com/` 即可实现加速克隆。支持 HTTPS 协议，需要 SSH 协议请前往演示站查看解决方法。

**使用方法**：
1. 复制您需要克隆的 GitHub 仓库地址
2. 在地址前添加 `github-speedup.com/`
3. 使用修改后的地址执行 git clone 命令

**示例对比**：

git clone 原始链接（未加速）
```shell
git clone https://github.com/git/git.git
```
git clone 加速链接
```shell
git clone https://github-speedup.com/github.com/git/git.git
```

### Raw 加速

> **提示**：只需在原始 Raw 链接前添加 `github-speedup.com/` 即可实现 Raw 加速。

**使用方法**：
1. 复制您需要加速的 Raw 地址
2. 在地址前添加 `github-speedup.com/`
3. 使用修改后的地址查看 Raw 内容

**示例对比**：

raw 原始链接（未加速）
```shell
https://raw.githubusercontent.com/git/git/refs/tags/v2.48.1/README.md
```
raw 加速链接
```shell
https://github-speedup.com/raw.githubusercontent.com/git/git/refs/tags/v2.48.1/README.md
```

### Release 文件加速

> **提示**：只需在原始 Release 文件链接前添加 `github-speedup.com/` 即可实现 Release 文件加速。

**使用方法**：
1. 复制您需要加速的 Release 文件链接
2. 在地址前添加 `github-speedup.com/`
3. 使用修改后的地址加速下载 Release 文件

**示例对比**：

Release 原始链接（未加速）
```shell
wget https://github.com/git/git/archive/refs/tags/v2.49.0.zip
```
Release 加速链接
```shell
wget https://github-speedup.com/github.com/git/git/archive/refs/tags/v2.49.0.zip
```

### Docker(OCI) 代理加速(Beta)
```shell
docker pull alpine/git:v2.36.1
docker pull github-speedup.com/alpine/git:v2.36.1

docker pull gcr.io/google-containers/coredns:1.3.0
docker pull github-speedup.com/gcr.io/google-containers/coredns:1.3.0
```
## 项目相关

### 演示站

访问 [演示站](https://github-speedup.com/)， 体验加速效果。

### TG 讨论群组

加入 [Telegram 讨论群组](https://t.me/jindcloud_cc) 与社区成员交流。

### 项目文档

详细的项目文档请参考 [GitHub加速项目文档](https://github-speedup.com/docs.html)。

## 致谢

本项目后端基于 [ghproxy](https://github.com/WJQSERVER-STUDIO/ghproxy) 开发，特别鸣谢 @WJQSERVER-STUDIO 的开源贡献。

© 2025 GitHub 加速站免费公益项目. 保留所有权利。
