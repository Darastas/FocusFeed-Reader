# FocusFeed 0.1.8：修复 AI 接口地址与错误提示

发布日期：2026-10-09（香港时间）

[官网原文](https://darastas.github.io/announcements/release-0-1-8.html)

> 修复 OpenAI 兼容服务的重复版本路径问题，模型拉取错误现在持续显示并支持复制。Windows、Android 与 Linux 同步更新。

本次更新修复 AI 服务接入中的地址兼容问题，Windows、Android 和 Linux 使用统一版本号 **0.1.8**。

## AI 接口地址

- OpenAI 兼容接入按你填写的 API 根地址发送请求，不再自动添加 `/v1`。
- 保留服务商要求的版本路径。例如，硅基流动填写 `https://api.siliconflow.cn/v1`；OpenAI 填写 `https://api.openai.com/v1`。
- 支持粘贴完整的 Chat Completions 或 Responses 接口地址；拉取模型时会使用同一 API 根地址下的模型列表接口。
- 摘要、翻译、解读和共用 OpenAI 接入配置的朗读同步采用这一地址规则。

升级后请检查「设置 → AI」中的 Base URL。如果旧配置只填了域名，且服务商要求 `/v1` 等版本路径，请把相应路径补入地址。已填写完整根地址的配置可以继续使用。

## 错误提示

- 模型拉取失败的原因持续显示在对应 API 卡片中，支持选中复制和自动换行。
- 重新拉取模型或保存配置会清除旧提示；连接测试成功仍显示「连接正常」。
- 修正窄屏下全局提示被设置面板遮挡或超出屏幕的问题。

## 三端下载

- [Windows 安装版](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.8_x64-setup.exe)
- [Windows 便携版](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.8.exe)
- [Android ARM64 APK](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.8_arm64.apk)
- [Linux Beta DEB](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.8_amd64.deb)
- [Linux Beta RPM](https://focusfeed-site.pages.dev/download/FocusFeed-0.1.8-1.x86_64.rpm)

Linux 继续标注 **Beta 测试版**，需要 x86_64、glibc 2.34 或更新版本及 WebKitGTK 4.1。官网[下载区](https://darastas.github.io/#download)提供 SHA-256 和终端安装说明。

终端安装：`curl -fsSL https://focusfeed-site.pages.dev/install.sh | sh`。安装前请关闭 FocusFeed；脚本校验安装包后调用 apt 或 dnf，仅安装步骤需要 sudo。实体桌面的动画、字体切换、稳定性与高刷新率表现仍需用户反馈。

## 本地数据与隐私

订阅、阅读记录、笔记与接入配置仍保存在本机。AI 请求只发送到你配置的服务商；本次更新不增加阅读数据上传或云端同步。
