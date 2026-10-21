# Listening Lab

A standalone browser-based listening practice tool inspired by the publicly documented Harman “How to Listen” exercises. It is an independent implementation and is not affiliated with or endorsed by Harman.

**Live demo / 在线体验：** [Open Listening Lab](https://ivalynifmuse.github.io/ZhenEarTrain/)

[简体中文说明](#简体中文)

## Features

- Band identification with peak, dip, low-pass, and high-pass filters
- Attribute, spectral profile, spatial mapping, and preference exercises
- Practice and session modes, adaptive task difficulty, local history
- Pink noise, white noise, and user-selected local audio
- Simplified Chinese and English interface
- No build step, backend, account, or upload required

## Publish with GitHub Pages

The included GitHub Actions workflow deploys the root `index.html` after pushes to `main`. GitHub Pages is enabled for this repository and the current site is available at <https://ivalynifmuse.github.io/ZhenEarTrain/>. For a fork, enable GitHub Pages in **Settings → Pages** and select **GitHub Actions** as the build and deployment source.

## Run locally

Open `index.html` in a current Safari, Chrome, Firefox, or Edge browser. Start playback from a page control so the browser can enable audio. Audio files selected by the user are decoded locally. Progress is stored in that browser’s local storage.

For local web-server testing, run:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Privacy and audio

The app has no analytics, network calls, or backend. Imported audio is not uploaded. Playback depends on the browser, operating system, output device, and listening level; this tool does not calibrate sound pressure or certify hearing ability.

## Project status

This is a single-file prototype. Its task levels and adaptive rules are original approximations and do not reproduce Harman’s internal algorithms or constitute Harman certification. The original Harman music tracks and installer contents are not included. Use audio you have permission to use.

## Acknowledgements, inspiration, and rights

This project was independently developed with AI-assisted “vibe coding” after the author found that the Harman “How to Listen” desktop application would no longer run on their Mac after upgrading to macOS Tahoe. Its exercise ideas, task flow, and training approach draw substantially on Harman “How to Listen”; this project is an unofficial, independent web implementation. It does not include Harman’s source code, installer, original music tracks, or other proprietary assets, and it is not affiliated with, endorsed by, or certified by Harman. “Harman” and “How to Listen” are used only to identify the source of inspiration and remain the property of their respective owners.

Listening Lab also includes independent spatial-audio exercises beyond the original project scope, including front/back sound-image localization and discrimination. Those exercises are this project’s own implementation and do not imply equivalence to Harman’s tests.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE). The license applies to this project’s original code, not to Harman trademarks, installers, or third-party audio.

## 简体中文

Listening Lab 是一个独立的浏览器听音训练工具，参考了 Harman 公开介绍的听音训练任务。它不是 Harman 官方产品，也未获其背书。

### 功能

- 频段辨识：峰值、凹陷、低通与高通
- 属性判断、频谱曲线、空间定位与偏好练习
- Practice / Session 模式、自适应任务难度、本地历史记录
- 粉噪、白噪，以及用户从本机选择的音频
- 简体中文与 English 界面
- 无需构建工具、后端、账号或上传音频

### 使用 GitHub Pages 发布

仓库中的 GitHub Actions 工作流会在推送到 `main` 后发布根目录的 `index.html`。本仓库已启用 GitHub Pages，可直接访问 <https://ivalynifmuse.github.io/ZhenEarTrain/>。复制仓库后，请在 **Settings → Pages** 中将构建与部署来源设为 **GitHub Actions**。

### 本地运行

使用新版 Safari、Chrome、Firefox 或 Edge 打开 `index.html`。请点击页面中的播放控件以启用浏览器音频。导入的音频在本机解码；训练记录保存在当前浏览器。

如需通过本地服务器运行，可执行：

```sh
python3 -m http.server 8000
```

然后访问 <http://localhost:8000>。

### 隐私与音频

本工具不包含分析追踪、网络请求或后端。导入的音频不会上传。播放效果受浏览器、操作系统、输出设备和音量影响；本工具不校准声压，也不认证听力能力。

### 项目状态

这是一个单文件原型。任务等级和自适应规则是本项目的近似实现，不复刻 Harman 内部算法，也不构成 Harman 认证。项目不包含 Harman 原版曲目或安装包内容。请使用你有权使用的音频素材。

### 致谢、灵感来源与权利说明

作者在升级到 macOS Tahoe 后发现 Harman「How to Listen」桌面软件无法在自己的 Mac 上运行，于是通过 AI 辅助的 vibe coding 独立开发了本网页工具。项目的练习思路、任务流程和训练方式大量参考了 Harman「How to Listen」，但这是非官方、独立实现；项目没有包含 Harman 源代码、安装包、原版音乐曲目或其他专有素材，也未获 Harman 认可、背书或认证。「Harman」和「How to Listen」仅用于说明灵感来源，相关名称及权利仍归其各自权利人所有。

本项目还加入了原版项目范围之外的独立空间声练习，包括前后声像定位与辨别。这些练习由本项目自行实现，不代表与 Harman 测试等同。

### 许可证

本项目原创代码采用 MIT 许可证，详见 [LICENSE](LICENSE)。该许可证不涵盖 Harman 商标、安装包或第三方音频素材。
