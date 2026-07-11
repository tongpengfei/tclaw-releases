# tclaw — 本地私人 AI 助手 · [English](README.en.md)

> 用 AI，做自己的应用

tclaw 是一款**开箱即用**的本地私人 AI 助手。下载解压即可运行，只需配置一下大模型的 API Key，几分钟内就能上手——无需安装额外环境。

tclaw 本身**完全免费**，使用成本取决于你选择的大模型服务，国内多家平台提供免费额度，零成本即可开始体验。

所有对话记录和文件都保存在你自己的电脑里，没有云端账号，没有数据上传，完全属于你自己。

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

### 演示视频

https://mjgc.oss-cn-qingdao.aliyuncs.com/dafei_blog/tclaw/res/tclaw_app_showcase_01.mp4

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

---

## 能做什么

### 📋 查询与整理资料
粘贴一篇文章、一份报告、一段对话，让 AI 帮你提炼重点、整理结构、翻译内容。  
不用再来回复制粘贴到网页版 AI，直接在本地完成。

### 📊 分析文档与数据
上传 CSV、Excel、PDF 或文本文件，让 AI 读懂内容，回答你的问题，生成分析报告，或者帮你找出关键数据。

### 🛠️ 打造专属提效工具
tclaw 内置了多款实用应用，也支持你自己定制 AI 工作流。  
比如：一键整理会议记录、批量处理文件命名、自动生成周报……  
告诉 AI 你想要什么，它帮你做出来。

### 🌐 生成网页原型
描述你想要的页面效果，AI 直接生成可预览的 HTML 原型，方便沟通需求或快速验证想法。

### 📁 管理本地文件
内置文件浏览器，可以直接浏览、预览、整理本地文件，结合 AI 能力批量处理文档。

### 💬 飞书 / 微信直接对话
在飞书或微信里直接给 AI 发消息，随时随地提问、查资料、处理任务，不需要打开电脑上的界面。

---

## 特点

- **完全本地**：对话记录存在你的电脑里，不经过任何第三方服务器
- **多模型支持**：兼容 OpenAI 和 Anthropic 两种主流协议，凡是实现了这两种协议的大模型服务均可接入，自由切换
- **轻量无依赖**：单个可执行文件，解压即用，不需要安装 Python / Node 等环境。CLI 包体积约 8 MB，GUI 包约 10 MB
- **跨平台**：提供 macOS、Windows、Linux 版本

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
打开设置（左下角齿轮图标），选择你的大模型服务商，填入对应的 API Key。  
首次启动会有引导向导，按提示操作即可。

### 第二步：开始对话
点击左上角「+」新建一个对话，直接开始提问。

### 第三步：上传文件
点击输入框旁边的 📎 按钮，上传文档、图片或代码文件，让 AI 结合文件内容回答问题。

### 第四步：使用内置应用
点击左侧应用图标，探索内置工具，或者自己创建一个专属工作流。

---

## 期待你的需求

你最希望 tclaw 帮你解决哪些工作场景？欢迎在 [Issues](../../issues) 告诉我，你的需求会直接影响开发方向。

---

## 反馈与支持

遇到问题或有功能建议，请在 [Issues](../../issues) 页面提交，我会持续改进。
