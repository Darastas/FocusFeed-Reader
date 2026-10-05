# FocusFeed Linux 0.1.7 Beta 已上线

发布日期：2026-10-05（香港时间）

[官网原文](https://darastas.github.io/announcements/linux-beta-0-1-7.html)

> Linux Beta 现已提供原生 x86_64 的 DEB 与 RPM 安装包，欢迎下载体验并反馈。

FocusFeed 的 **Linux 0.1.7 Beta 测试版已上线**。现在可以在 Linux 上阅读订阅与电子书，使用账户同步、批注和自己的 AI 接口。

## 下载与安装

- Linux Mint、Ubuntu、Debian：下载 [DEB 安装包](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.7_amd64.deb)。
- Fedora 与支持 RPM 的发行版：下载 [RPM 安装包](https://focusfeed-site.pages.dev/download/FocusFeed-0.1.7-1.x86_64.rpm)。
- [官网下载区](https://darastas.github.io/#download)提供两种安装包的 SHA-256 校验值。

当前支持 **x86_64**，需要 glibc 2.34 或更新版本及 WebKitGTK 4.1。建议使用系统的 apt 或 dnf 安装下载的文件，由包管理器解析依赖。

## 本次 Beta 调整

三端 0.1.7 更新现已加入高亮与批注导出，可在设置中批量保存 ZIP，或在阅读页导出本篇 Markdown / HTML 笔记。
详见[本次更新内容](https://darastas.github.io/announcements/release-0-1-7.html)。此前已安装的早期 Linux Beta 请下载当前安装包覆盖安装。

- 调整设置卡片层级与背景效果，减少设置页面的重绘负担。
- 优化字体设置应用时机和羽化滑块的拖动释放处理。
- 关闭 WebKit 偏向 60 FPS 的设置，让高刷新率显示器有机会使用系统显示时钟；实际效果取决于桌面环境和显卡驱动。
- 新增运行与崩溃诊断；渲染进程意外退出后最多自动重载一次。
- 接入独立的 Linux 更新清单和 DEB/RPM 下载入口。

## 测试版与反馈

**这是 Beta 测试版。** 动画、字体切换、高刷新率和不同 Linux 桌面环境的稳定性仍需实际使用验证；目前不承诺所有设备都能达到显示器的最高刷新率。

遇到闪退、卡死或显示异常时，请提供发行版版本、桌面环境、显卡驱动和复现步骤。运行日志位于 `~/.local/share/com.rsscross.app/logs/linux-runtime.log`；设置了 XDG_DATA_HOME 时，请在对应的数据目录中查找。

渲染进程重载可能丢失未保存的界面状态，不能处理主进程崩溃或显卡驱动卡死。感谢参与测试并帮助我们完善 Linux 体验。
