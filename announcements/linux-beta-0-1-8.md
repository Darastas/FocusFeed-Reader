# FocusFeed Linux 0.1.8 Beta：AI 接入修复

发布日期：2026-10-09（香港时间）

[官网原文](https://darastas.github.io/announcements/linux-beta-0-1-8.html)

> Linux Beta 同步修复 OpenAI 兼容服务的地址拼接与模型拉取错误显示，提供 x86_64 的 DEB 和 RPM 安装包。

Linux 0.1.8 Beta 与 Windows、Android 同步更新。此次修复 AI 接口地址的重复版本路径问题，并改善模型拉取失败时的错误提示。具体配置方法见[完整更新公告](https://darastas.github.io/announcements/release-0-1-8.html)。

## 下载与安装

- Linux Mint、Ubuntu、Debian：[DEB 安装包](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.8_amd64.deb)。
- Fedora 与支持 RPM 的发行版：[RPM 安装包](https://focusfeed-site.pages.dev/download/FocusFeed-0.1.8-1.x86_64.rpm)。
- [官网下载区](https://darastas.github.io/#download)提供对应的 SHA-256、可复制的手动安装命令及终端安装入口。

终端安装：`curl -fsSL https://focusfeed-site.pages.dev/install.sh | sh`。

需要 x86_64、glibc 2.34 或更新版本及 WebKitGTK 4.1。安装前请关闭 FocusFeed；脚本会校验安装包，再调用 apt 或 dnf，仅安装步骤需要 sudo。

## Beta 范围

Linux 继续作为 Beta 测试版提供。实体桌面的动画、字体切换、稳定性与高刷新率表现仍需用户反馈。阅读数据保存在本地，AI 请求发往你配置的服务商。
