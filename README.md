# github-speedup
GitHub 加速器 - 高性能 GitHub 资源访问解决方案


GitHub 加速器 - 高性能 GitHub 资源访问解决方案
<img src="https://img.shields.io/github/actions/workflow/status/WJQSERVER-STUDIO/ghproxy/build.yml?branch=main" alt="Build Status"></img> <img src="https://img.shields.io/github/v/release/WJQSERVER-STUDIO/ghproxy" alt="Release"></img> <img src="https://img.shields.io/badge/Go-1.24-blue" alt="Go Version"></img> <img src="https://img.shields.io/badge/license-WJQserver%20Studio%20License%202.0-blue" alt="License"></img>


极速访问 GitHub，畅享全球开源资源
GitHub 加速器是一款专为开发者打造的高性能 GitHub 资源访问解决方案。通过智能代理技术，显著提升 Git clone、Raw 文件、Releases 等资源的访问速度，解决网络限制问题，让您的开发效率立刻提升！
⚡ 核心特性
高性能架构：基于 Go 语言和 HertZ 框架构建，提供卓越的性能与极低的资源占用
全面资源支持：支持 Git clone、Raw 文件、Releases 下载和 Docker 镜像仓库
零门槛使用：无需复杂配置，一键转换链接即可使用
灵活部署选项：支持自托管和 Docker 容器化部署
多种高级功能：Git Clone 缓存、速率限制、用户鉴权等
🚀 使用示例
# 下载 Raw 文件
https://ghproxy.example.com/raw.githubusercontent.com/user/repo/branch/file.txt
https://ghproxy.example.com/https://raw.githubusercontent.com/user/repo/branch/file.txt

# 克隆仓库
git clone https://ghproxy.example.com/github.com/user/repo.git
git clone https://ghproxy.example.com/https://github.com/user/repo.git

# Docker(OCI) 代理
docker pull gh.example.com/user/image
docker pull gh.example.com/ghcr.io/user/image
