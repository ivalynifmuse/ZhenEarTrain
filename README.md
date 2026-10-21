# Listening Lab

A standalone browser-based listening practice tool inspired by the publicly documented Harman “How to Listen” exercises. It is an independent implementation and is not affiliated with or endorsed by Harman.

[简体中文说明](#简体中文)

## Features

- Band identification with peak, dip, low-pass, and high-pass filters
- Attribute, spectral profile, spatial mapping, and preference exercises
- Practice and session modes, adaptive task difficulty, local history
- Pink noise, white noise, and user-selected local audio
- Simplified Chinese and English interface
- No build step, backend, account, or upload required

## Publish with GitHub Pages

The included GitHub Actions workflow deploys the root `index.html` after pushes to `main`. After creating the repository, enable GitHub Pages in **Settings → Pages** and select **GitHub Actions** as the build and deployment source. The first successful workflow run publishes the site at `https://<owner>.github.io/<repository>/`.

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

仓库中的 GitHub Actions 工作流会在推送到 `main` 后发布根目录的 `index.html`。创建仓库后，在 **Settings → Pages** 中将构建与部署来源设为 **GitHub Actions**。首次工作流成功后，可通过 `https://<owner>.github.io/<repository>/` 访问。

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

### 许可证

本项目原创代码采用 MIT 许可证，详见 [LICENSE](LICENSE)。该许可证不涵盖 Harman 商标、安装包或第三方音频素材。
