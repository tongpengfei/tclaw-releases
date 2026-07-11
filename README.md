# tclaw — 本地私人 AI 助手 · [English](README.en.md)

> 用 AI，做自己的应用

tclaw 是一款本地私人 AI 助手。下载解压即可运行，只需配置一下大模型的 API Key，几分钟内就能上手，无需安装额外环境。

tclaw 本身完全免费，使用成本取决于你选择的大模型服务，国内多家平台提供免费额度，零成本即可开始体验。

所有对话记录和文件都保存在你自己的电脑里，没有云端账号，没有数据上传。

**支持的模型服务**：
- 🔥 **火山引擎（豆包）** — 字节跳动旗下，国内访问速度快，新手首选
- ☁️ **阿里云百炼（通义千问）** — 阿里云旗下，有免费额度
- 🧠 **智谱 AI（GLM）** — 清华系，有免费额度
- 🌊 **DeepSeek** — 性价比极高，推理能力强
- 🌙 **Moonshot（Kimi）** — 长文本处理能力强
- 🤖 **Claude（Anthropic）** — 海外模型，综合能力强
- ⚙️ **自定义服务商** — 兼容 OpenAI 协议的任意服务均可接入

---

## 效果展示

### 演示

**tclaw 内置应用展示**（支持自定义开发应用）

![tclaw app showcase](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/showcase/tclaw_app_showcase_01.gif)

**由 tbrain + tclaw 开发的 Idle RPG 游戏**

![idle RPG built by tclaw](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/showcase/tbrain_game_01.gif)

### 截图

| CLI 启动 | 小红书内容生成 |
|---|---|
| ![CLI](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw01_cli01.png) | ![小红书](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw02_xhs01.png) |

| 股票分析 | 文件浏览器 |
|---|---|
| ![股票](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw03_stock01.png) | ![文件浏览器](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw04_file_browser01.png) |

| 调试日志 | 内置应用 |
|---|---|
| ![日志](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw05_log01.png) | ![内置应用](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw06_apps01.png) |

| 代码开发 1 | 代码开发 2 |
|---|---|
| ![代码1](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw07_code01.png) | ![代码2](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw08_code02.png) |

| AI 图片编辑（内置应用）| |
|---|---|
| ![AI图片编辑](https://github.com/tongpengfei/tclaw-releases/raw/main/docs/screenshots/tclaw09_app_show_01.png) | |

---

## 能做什么

### 自定义应用开发

tclaw 内置了一套应用框架，你可以用自然语言描述想要的工具，AI 帮你生成一个可以直接跑起来的应用。内置了图片编辑、视频处理、音频编辑、TTS、文件浏览器等应用，也支持随时自己扩展。用 tbrain + tclaw 甚至能开发出完整的游戏，上面的 Idle RPG 就是这么来的。

### 代码开发

内置多个软件开发 agent，覆盖日常开发的各个环节——写代码、调试、架构设计、代码审查、重构、生成测试、写文档。agent 可以直接读文件、跑命令、改代码，不只是给建议。

### 股票和投资研究

内置投资分析 agent，可以搜索财报、分析商业模式、做基本面诊断，最终给出买入/持有/卖出判断。多个 agent 协作完成，结果比单轮对话靠谱。

### 内容创作

内置社交媒体内容创作 agent，支持小红书、微信公众号，从选题到生成到配图一套走。

### 产品和设计

有产品经理、需求分析、头脑风暴、UX/UI 设计、设计评审等 agent，适合产品开发过程中各类场景。

### 查资料、整理内容

把文章、报告、对话直接粘进来，提炼重点、整理结构、翻译内容，不用每次都去开网页版 AI。

### 分析文件和数据

上传 CSV、Excel、PDF 或文本文件，直接问问题，找关键数据、生成分析报告。

### 飞书 / 微信直接对话

在飞书或微信里直接给 AI 发消息，随时提问、查资料、处理任务，不需要开电脑上的界面。

---

## 特点

- **自定义应用**：内置多款应用，支持自己开发扩展，告诉 AI 你想要什么就能生成
- **完全本地**：数据存在自己电脑里，不经过任何第三方服务器
- **多模型支持**：兼容 OpenAI 和 Anthropic 协议，支持的大模型服务随时切换
- **轻量无依赖**：单个可执行文件，解压即用，不需要装 Python / Node 等环境，CLI 约 8 MB，GUI 约 10 MB
- **跨平台**：macOS、Windows、Linux 均可用

---

## 下载安装

### macOS（推荐 GUI 版）
1. 下载 `tclaw-darwin-arm64-gui.dmg`（M 系列芯片）或 `tclaw-darwin-amd64-gui.dmg`（Intel）
2. 打开 DMG，将 `tclaw.app` 拖入 **Applications（应用程序）** 文件夹
3. 双击打开

> **提示**：首次打开如果提示"文件已损坏"或"无法验证开发者"，在终端执行：
> ```
> xattr -cr /Applications/tclaw.app
> ```
> 然后重新打开即可。这是 macOS 对未经苹果公证的应用的限制，不影响正常使用。

### Windows（GUI 版）
1. 下载 `tclaw-windows-amd64-gui.zip`，解压
2. 双击运行 `tclaw.exe`
3. 如弹出安全警告，点击**更多信息 → 仍要运行**

### 命令行版（CLI，适合所有平台）
下载对应平台的 ZIP，解压后：
1. 复制 `config.json.example` 为 `config.json`，填入你的 API Key
2. 运行 `./tclaw`，浏览器访问 `http://localhost:PORT`

---

## 快速上手

### 第一步：配置 API Key
打开设置（左下角齿轮图标），选择大模型服务商，填入 API Key。首次启动有引导向导，按提示操作即可。

### 第二步：开始对话
点击左上角「+」新建对话，直接开始提问。

### 第三步：上传文件
点击输入框旁的 📎 按钮，上传文档、图片或代码文件，让 AI 结合内容回答。

### 第四步：用应用或自己做一个
点击左侧应用图标，可以直接用内置工具，也可以告诉 AI 你想要什么，它帮你生成一个。

---

## 期待你的需求

你最希望 tclaw 帮你解决哪些场景？欢迎在 [Issues](../../issues) 告诉我，你的需求会直接影响开发方向。

---

## 反馈与支持

遇到问题或有功能建议，请在 [Issues](../../issues) 提交，我会持续改进。
