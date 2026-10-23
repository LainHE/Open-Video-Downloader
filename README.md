<img src="https://raw.githubusercontent.com/jely2002/youtube-dl-gui/v2.0.0/renderer/img/icon.png" alt="logo" align="left" height="100"/>

# Open Video Downloader (youtube-dl-gui) <br> ![version badge](https://img.shields.io/github/v/release/jely2002/youtube-dl-gui?label=latest-release) ![GitHub](https://img.shields.io/github/license/jely2002/youtube-dl-gui) ![downloads](https://img.shields.io/github/downloads/jely2002/youtube-dl-gui/total) 
[https://jely2002.github.io/youtube-dl-gui](https://jely2002.github.io/youtube-dl-gui)

> [English version](./README.en.md) | 简体中文

Open Video Downloader 是一款简洁的跨平台桌面应用，支持从数百个网站下载视频、音频、字幕和元数据，不仅限于 YouTube。  
它基于 [yt-dlp](https://github.com/yt-dlp/yt-dlp) 提供了易用的图形界面，无需触碰命令行。


## 功能特性

- **跨平台：** 支持 Windows、macOS 和 Linux。
- **音频或视频下载：** 下载完整视频或仅提取音轨。
- **字幕和元数据：** 自动保存可用的字幕和视频信息。
- **画质控制：** 选择你偏好的分辨率、帧率和输出格式（如 MP4 或 MKV）。
- **播放列表：** 一键下载整个播放列表。
- **自定义输出：** 设置下载位置，使用预设或自定义模板控制文件名。
- **智能队列：** OVD 自动平衡多个下载任务，避免电脑变慢。
- **身份验证：** 支持浏览器 Cookie 文件、基本认证和视频密码。
- **自动更新：** 应用和 yt-dlp 均会自动更新到最新版本。
- **明暗模式：** 跟随系统主题，进度和错误提示清晰可见。
- **快捷键：** 使用快捷键排队和下载视频，通过通知随时掌握进度。

## 下载

**Windows**、**macOS** 和 **Linux** 的最新版本可在  
[GitHub Releases 页面](https://github.com/LainHE/Open-Video-Downloader/releases)获取。

下载对应平台的安装包或压缩包，按常规步骤安装即可。  
无需命令行配置。

#### 我该下载哪个文件？
| 你的系统                         | 下载文件                                       |
|---------------------------------------|------------------------------------------------|
| **Windows**                           | `Open.Video.Downloader_x.x.x_x64-setup.exe`    |
| **Mac (Intel)**                       | `Open.Video.Downloader_x.x.x_x64.dmg`          |
| **Mac (Apple Silicon – M1, M2 … M5)** | `Open.Video.Downloader_x.x.x_aarch64.dmg`      |
| **Linux generic (x64)**               | `Open.Video.Downloader_x.x.x_amd64.AppImage`   |
| **Linux generic (aarch64)**           | `Open.Video.Downloader_x.x.x_aarch64.AppImage` |
| **Linux Debian/Ubuntu (x64)**         | `Open.Video.Downloader_x.x.x_amd64.deb`        |
| **Linux Debian/Ubuntu (aarch64)**     | `Open.Video.Downloader_x.x.x_arm64.deb`        |
| **Linux Fedora/RHEL (x64)**           | `Open.Video.Downloader_x.x.x-x_amd64.rpm`      |
| **Linux Fedora/RHEL (aarch64)**       | `Open.Video.Downloader_x.x.x-x_aarch64.rpm`    |

#### 命令行下载
Open Video Downloader 可通过命令行工具下载，如 Mac 上的 [Homebrew](https://brew.sh/) 或 Windows 上的 [WinGet](https://github.com/microsoft/winget-cli)。

```shell
brew install --cask open-video-downloader
```

```shell
winget install -e --id jely2002.youtube-dl-gui
```

## 工作原理

Open Video Downloader 前端基于 Vue 3 构建，后端由 [Tauri](https://tauri.app/) 驱动的 Rust 提供动力。  
添加视频或播放列表后，应用会与 yt-dlp 通信以获取信息、处理选项并启动下载。  
下载进度和任何错误都会在应用中显示。

## 本地化

简体中文（zh-CN）与繁体中文（zh-TW）和英文同时可用。  
原始 `zh-TW` 语言文件位于 [src/locales/zh-TW.original.json](./src/locales/zh-TW.original.json)。

## 贡献指南

欢迎开发者参与贡献。  
你需要安装 Node.js（v24+）和 Rust。

```
npm install
npm run tauri dev
```

更多详情，请参阅 [CONTRIBUTING.md](./CONTRIBUTING.md)。

## 许可证与免责声明

Open Video Downloader 在 [AGPL-3.0 许可证](./LICENSE)下分发。

#### 负责任地使用本应用
正如 AGPL-3.0 许可证第 16 条所述，Open Video Downloader 的维护者不对本应用的滥用承担责任。  
我们不鼓励使用此软件违反当地法律或平台服务条款（包括 DMCA）。  
用户需自行确保公平合法地使用本软件。
