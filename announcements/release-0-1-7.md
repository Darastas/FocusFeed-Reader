# FocusFeed 0.1.7：高亮与批注导出，Linux 继续 Beta

发布日期：2026-10-05（香港时间）

[官网原文](https://darastas.github.io/announcements/release-0-1-7.html)

> Windows、Android 与 Linux 新增阅读笔记导出，支持 Markdown、HTML 和批量 ZIP。Linux 版本继续标记 Beta。

这次更新让你把阅读时保存的高亮和批注带到应用之外。Windows、Android 和 Linux 使用统一版本号 **0.1.7**。

> 将摘录和自己的想法整理成可保存、可阅读的笔记。

## 如何导出

- **导出本篇笔记**：打开文章或书本章节，点击阅读工具栏的下载图标，选择 Markdown 或 HTML。
- **批量导出**：设置 → 导出 → 选择「高亮与批注」，选全部文章或仅收藏，保存 ZIP。每篇有笔记的文章或章节是一份文件。
- **保留阅读信息**：文件包含标题、作者、来源链接、摘录、批注、标记颜色、笔型及创建和更新时间。HTML 显示标记颜色与样式；Markdown 使用引用块和文字描述。
- **离线可用**：导出本机已经保存的笔记，无需联网。安卓使用系统文档保存界面选择位置。

升级后新建的标记会保存完整摘录。旧版已截断的长摘录无法补回未保存的文字；批注编辑仍最多 2000 个字符。
导出文件用于阅读和整理，暂不支持导入还原。

## 三端下载

- [Windows 安装版](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.7_x64-setup.exe)
- [Windows 便携版](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.7.exe)
- [Android ARM64 APK](https://focusfeed-site.pages.dev/download/FocusFeed_v0.1.7_arm64.apk)
- [Linux Beta DEB](https://focusfeed-site.pages.dev/download/FocusFeed_0.1.7_amd64.deb)
- [Linux Beta RPM](https://focusfeed-site.pages.dev/download/FocusFeed-0.1.7-1.x86_64.rpm)

## Linux Beta

Linux 0.1.7 继续作为 **Beta 测试版** 提供。需要 x86_64、glibc 2.34 或更新版本及 WebKitGTK 4.1。
DEB 适用于 Linux Mint、Ubuntu、Debian 等发行版；RPM 适用于 Fedora 等发行版。

现在可以直接在终端安装：`curl -fsSL https://focusfeed-site.pages.dev/install.sh | sh`。
脚本自动选择 DEB / RPM、校验 SHA-256，再通过 apt 或 dnf 安装；也会处理同版本早期 Beta 重装及误标版本降级。
安装前请关闭 FocusFeed；需要 x86_64、curl、sha256sum 和可提供 WebKitGTK 4.1 的软件源。官网[下载区](https://darastas.github.io/#download)也提供可复制的手动下载与安装命令。
使用 apt 或 dnf 安装可自动解析依赖。

笔记导出的后端与三端构建已验证，前端交互由用户验收。实体桌面的动画、字体切换、稳定性与高刷新率表现仍需反馈。

## 版本号更正

本次三端更新的正确版本号为 **0.1.7**，现已统一更正。已经安装误标版本的用户，请下载本页对应平台的安装包覆盖安装；安卓保留较高的内部构建编号，以允许覆盖升级。
