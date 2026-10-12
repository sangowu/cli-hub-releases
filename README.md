# CLI Hub

![CLI Hub — 多个 CLI，一个工作台。Windows 桌面工作台，展示使用虚拟路径的示例会话。](docs/images/cli-hub-banner.png)

**少切窗口，多做事情。｜Fewer windows. More focus.**

[下载 Windows 版本 / Download for Windows](https://github.com/sangowu/cli-hub-releases/releases/latest) · [历史版本 / All releases](https://github.com/sangowu/cli-hub-releases/releases)

### 动态演示 / Animated demo

![CLI Hub demo — session grouping, sidebar collapse/expand, and launch templates](docs/images/cli-hub-demo-en.gif)

[下载高清 MP4 / Download HD MP4](docs/videos/cli-hub-demo-en.mp4) · English · 43s · 1080p

展示 CLI 分组排列、会话栏收起与展开，以及启动模板设置，含鼠标与键盘操作效果。使用示例会话和虚拟路径。

See session grouping, sidebar collapse/expand, and launch template configuration, with visible mouse and keyboard actions. Uses demo sessions and fictional paths.

## 中文

同时使用多个 Codex、Claude Code 或终端，却被满屏窗口困扰，找不到对应的项目？

CLI Hub 是一款基于 Rust 与 Tauri 构建的 Windows 桌面工作台，让你在一个界面中启动、查看和使用多个命令行工具。

- **按项目管理**：多工作区标签页，支持按工作目录、按 CLI 类型和不分组三种视图。每个工作区最多 8 个活动会话，全局最多同时运行 24 个。
- **高效交互**：实时输出预览、完整交互终端，为任意 CLI 提供统一的多行输入区，支持 Shift+Enter 换行。
- **后台继续运行**：关闭、重启或更新界面时，已运行的 CLI 可继续在后台工作；重新打开即可连接原有会话。
- **启动更省心**：保存多套启动配置，保留会话卡片，并可选择在后台进程停止后，下次启动时重新启动此前运行的 CLI。
- **兼容多种工具**：提供 Codex、Claude Code、Pi、Hermes Agent、OpenCode、PowerShell 和 CMD 启动模板，也可自定义可执行文件、参数与工作目录，保存为常用启动配置。提供中英文界面与明暗主题。

### 下载与使用

**前置准备**

- [ ] 使用 **Windows 10/11 x64** 系统。
- [ ] 安装 **Microsoft Edge WebView2 Runtime**；已安装可跳过。
- [ ] 安装需要使用的 **CLI 工具**（例如 Codex、Claude Code 或 PowerShell），并完成该工具要求的配置或登录。
- [ ] 确保 CLI 命令可从系统 `PATH` 找到，或在 CLI Hub 的自定义启动配置中指定可执行文件路径。

CLI Hub 安装版无需 Node.js 或 Rust；所选 CLI 工具的额外依赖请按其官方安装说明准备。

**安装与启动**

1. 前往[最新版本](https://github.com/sangowu/cli-hub-releases/releases/latest)，下载 `.exe` 或 `.msi` 安装包。
2. 安装并打开 CLI Hub，创建工作区，点击 **New session / 新建会话**，选择 CLI 和项目目录。
3. 运行多个会话，通过会话卡片查看输出、切换终端。

重新启动 CLI 不会恢复工具内部的对话状态。电脑重启或后台进程退出会结束原有任务；如需主动停止全部任务，请使用 **Stop all and exit / 停止全部并退出**。

## English

Running several Codex, Claude Code, or terminal sessions and losing track of which window belongs to which project?

CLI Hub is a Windows desktop workspace built with Rust and Tauri. Launch, monitor, and interact with multiple command-line tools from one interface.

- **Organize by project**: workspace tabs with directory grouping, CLI-type grouping, or an ungrouped view. Run up to 8 active sessions per workspace and 24 across the app.
- **Work comfortably**: live output previews, fully interactive terminals, and a shared multiline composer for any CLI, with Shift+Enter to insert a new line.
- **Keep tasks running**: active CLIs can continue in the background when you close, restart, or update the interface. Reopen CLI Hub to reconnect.
- **Start faster**: save multiple launch profiles, retain session cards, and optionally relaunch previously running CLIs on startup after the background host has stopped.
- **Use your tools**: launch templates for Codex, Claude Code, Pi, Hermes Agent, OpenCode, PowerShell, and CMD. Customize executables, arguments, and working directories, then save them as reusable launch profiles. English and Simplified Chinese interfaces, with light and dark themes.

### Get started

**Prerequisites**

- [ ] Use **Windows 10/11 x64**.
- [ ] Install **Microsoft Edge WebView2 Runtime**, unless it is already installed.
- [ ] Install the **CLI tools** you want to use (such as Codex, Claude Code, or PowerShell), and complete any required configuration or sign-in.
- [ ] Make the CLI commands available on the system `PATH`, or specify the executable path in a custom CLI Hub launch profile.

The installed CLI Hub app does not require Node.js or Rust. Follow each CLI tool's official installation instructions for any additional dependencies.

**Install and launch**

1. Open the [latest release](https://github.com/sangowu/cli-hub-releases/releases/latest) and download the `.exe` or `.msi` installer.
2. Install and open CLI Hub, create a workspace, and choose **New session** to select a CLI and project directory.
3. Run your sessions, preview their output, and switch terminals through the session cards.

Relaunching a CLI does not restore its internal conversation state. A computer restart or background-host exit ends the original tasks. Use **Stop all and exit** when you want to stop every task explicitly.

---

本仓库提供 CLI Hub 安装包、版本说明及更新清单。应用内更新使用 Tauri 更新签名；Windows 安装包尚未使用 Authenticode 签名。

This repository hosts CLI Hub installers, release notes, and update manifests. In-app updates use Tauri updater signatures; Windows installers are not Authenticode-signed.
