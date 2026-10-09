# FocusFeed 0.2.0：界面小更新与个人离线许可

发布日期：2026-10-09（香港时间）

[官网原文](https://darastas.github.io/announcements/release-0-2-0.html)

> 界面与已有功能的交互可通过小更新改善；个人离线许可可在自己的设备间携带，无需登录和设备码。Windows、Android 与 Linux 同步更新。

Windows、Android 和 Linux 使用统一版本号 **0.2.0**。本次加入界面小更新与可携带的个人离线许可，订阅、文章和笔记继续保存在本机。

## 界面小更新

- 入口为「设置 → 关于 → 界面小更新」。检查和下载由你主动发起，也可以导入开发者提供的 `.ffupdate` 文件。
- 小更新可以调整界面、阅读排版、菜单、浮窗与使用已有本地功能的操作流程。需要新增核心能力、数据库迁移或系统权限时，仍通过安装包更新。
- 下载后在本地验证签名，下次启动加载；无需中断当前阅读。Android 请结束应用后重新打开。
- 可以关闭小更新、取消待更新包或恢复上一界面；新界面启动未确认时自动恢复上一可用界面或内置界面。
- 界面资源在本机加载。检查和下载不会向更新服务发送授权码、设备身份、订阅、文章或 API 密钥；更新服务不可用时仍可阅读本地内容。

从 0.1.8 或更早版本升级，请先安装 0.2.0。界面小更新只能使用当前安装包已有的本地能力，也需要匹配安装包版本。

## 个人离线许可

- Pro 授权无需新增账号或登录系统。
- 已有有效的 RSSC1 / RSSC2 授权码可以在自己的设备上直接使用，无需重新提供设备码；签名与权益仍会在本地验证。
- 「设置 → Pro」支持粘贴授权码、复制原码以及导入、导出 `.fflicense` 许可证文件，方便备份和换机。
- 许可证文件仅包含签名授权码，不包含阅读数据库和 AI 密钥。请自行保管，不要公开分享。
- 许可证遗失后可凭购买记录联系开发者重发；本版本不提供在线找回或即时撤销。

## AI 配置

已保存的 API 密钥由本地核心管理，设置页只显示是否已保存。编辑 API 配置时留空会保留原密钥；需要移除时使用明确的清除操作。AI 请求仍只发送到你配置的服务商。

## 三端下载

- [Windows 安装版](https://focusfeed-site.pages.dev/download/FocusFeed_0.2.0_x64-setup.exe)
- [Windows 便携版](https://focusfeed-site.pages.dev/download/FocusFeed_v0.2.0.exe)
- [Android ARM64 APK](https://focusfeed-site.pages.dev/download/FocusFeed_v0.2.0_arm64.apk)
- [Linux Beta DEB](https://focusfeed-site.pages.dev/download/FocusFeed_0.2.0_amd64.deb)
- [Linux Beta RPM](https://focusfeed-site.pages.dev/download/FocusFeed-0.2.0-1.x86_64.rpm)

官网[下载区](https://darastas.github.io/#download)提供真实安装包的 SHA-256。Android 沿用旧版签名，可覆盖安装；安装前请备份重要阅读数据。

Linux 继续标注 **Beta 测试版**，需要 x86_64、glibc 2.34 或更新版本及 WebKitGTK 4.1。可使用终端安装：`curl -fsSL https://focusfeed-site.pages.dev/install.sh | sh`。安装前关闭应用；脚本校验下载包后调用 apt 或 dnf，仅安装步骤需要 sudo。实体桌面的动画、稳定性与高刷新率表现仍需用户反馈。
