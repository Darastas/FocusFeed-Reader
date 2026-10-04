# FocusFeed 阅读器

把注意力还给阅读。FocusFeed 是一款本地优先的 RSS 与电子书阅读器，提供 Windows 和 Android 版本，支持高光批注、RSS 账户同步，以及使用自己的 AI 接口进行摘要、翻译、解读和朗读。

**官网与界面演示：** [darastas.github.io](https://darastas.github.io/)

**更新公告：** [0.1.6 更新说明](https://darastas.github.io/announcements/release-0-1-6.html) · [全部公告](https://darastas.github.io/announcements/) · [订阅公告 RSS](https://darastas.github.io/announcements.xml)

## 下载 · v0.1.6

| 平台 | 版本 | 安装包 | 大小 |
| --- | --- | --- | --- |
| Windows x64 | 安装版 | [下载 EXE](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.6_x64-setup.exe?rev=1065B7B3E74C1078) | 10.2 MiB |
| Windows x64 | 便携版 | [下载 EXE](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.6.exe?rev=98485C7F5ECBEA1D) | 34.0 MiB |
| Android ARM64 | 安装包 | [下载 APK](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.6_arm64.apk?rev=68653228D9586408) | 43.8 MiB |

安装包由 Cloudflare 提供下载。这个仓库用于发布软件介绍、下载入口与使用说明。

### 文件校验（SHA-256）

```text
FocusFeed_0.1.6_x64-setup.exe  1065B7B3E74C107828E119D435FD033B05FBABE3568DBC41963496F1C331202C
FocusFeed_v0.1.6.exe          98485C7F5ECBEA1D795575FCE46660A7DAE1A85F43616A386ECB0F437317A809
FocusFeed_v0.1.6_arm64.apk    68653228D95864089E69939665453D0E8FF4E8EA4CD8050943E1D3593D8880C8
```

Windows 安装包尚未进行代码签名，系统可能提示“未知发布者”。Android 版仅适用于 ARM64 设备。

## 0.1.6 更新

0.1.6 修正版已修复 Tiny Tiny RSS 正文与订阅失败提示，以及 Miniflux Fever 的订阅和分组同步。已连接真实服务验证文章分页、已读 / 收藏回传和断网补传；下载与校验值对应修正版。

- **RSS 账户同步**：接入 FreshRSS、Miniflux、Tiny Tiny RSS、Google Reader 兼容 API 和 Fever API，支持订阅、分组、文章与已读 / 收藏状态同步。
- **离线操作补传**：离线时的已读与收藏变更保存在本机，联网同步时自动补传，失败后可重试。
- **AI 朗读**：独立选择语音模型、音色与速度，支持试听，以及文章、电子书章节和选中文字朗读。播放器支持暂停、继续、停止与进度显示。
- **检查更新**：在设置的关于页面点击“检查更新”，查看版本状态并前往公告或下载页面。
- **官方公告订阅**：侧栏固定置顶官网公告源，支持在阅读器内查看全文公告。
- **阅读与官网排版**：划词工具条渐显动画与软件其他动画保持一致；官网缩小截图，采用左右图文布局，补充功能说明和原图入口。

Fever 的订阅管理在服务网页中完成。Feedly、Folo、Feedbin、BazQux 和 The Old Reader 目前提供服务入口与接入说明。

## 开始使用

1. **订阅与账户**：在设置 → RSS 账户中添加服务，按提示填写服务器地址与 API 凭据。账户切换器可查看全部账户、本地订阅或单个账户；服务器分组在对应服务网页管理。
2. **AI 与朗读**：在设置 → AI 接入中配置自己的服务，再为朗读分配支持音频输出的模型。支持 OpenAI 兼容语音接口及 Gemini AUDIO 输出，费用由对应服务商收取。
3. **获取后续更新**：在设置 → 关于中检查版本，也可以订阅上方公告 RSS。
