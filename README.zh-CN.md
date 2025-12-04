# LSPosed框架

[![Build](https://img.shields.io/github/actions/workflow/status/re-zero001/LSPosed-Irena/core.yml?branch=dev&event=push&logo=github&label=Build)](https://github.com/re-zero001/LSPosed-Irena/actions/workflows/core.yml?query=event%3Apush+branch%3Adev+is%3Acompleted) [![Channel](https://img.shields.io/badge/Follow-Telegram-blue.svg?logo=telegram)](https://t.me/lsposed-irena) [![Download](https://img.shields.io/github/v/release/LSPosed/LSPosed?color=orange&logoColor=orange&label=Download&logo=DocuSign)](https://github.com/re-zero001/LSPosed-Irena/releases/latest) [![Total](https://shields.io/github/downloads/LSPosed/LSPosed/total?logo=Bookmeter&label=Counts&logoColor=yellow&color=yellow)](https://github.com/LSPosed/LSPosed/releases)

* [English](README.md)
* [简体中文](README.zh-CN.md)

## 简介

这是一个 Zygisk 模块，旨在提供一个与原版 Xposed 框架保持一致的 ART hook 框架，并利用 LSPlant hook 框架。

> Xposed 是一个模块框架，它允许模块在不修改任何 APK 的情况下改变系统和应用程序的行为。这非常棒，因为这意味着模块可以兼容不同的系统版本甚至 ROM，而无需任何修改（只要原始代码没有被大幅改动）。而且，撤销也很容易。由于所有更改都在内存中进行，您只需停用模块并重启即可恢复原始系统。Xposed 还有许多其他优势，这里再举一个例子：多个模块可以同时修改系统或应用程序的同一部分。而使用修改过的 APK，您只能选择其中一个。除非作者构建了多个包含不同组合的 APK，否则无法将它们组合起来使用。

## 支持的版本

Android 8.1 ~ 16

## 安装

1. 安装 Magisk v26+

2. 安装 [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext/releases)

> 或者在 Magisk 中启用 Zygisk，我们推荐使用 ZygiskNext。

3. [下载](#download) 并在 Magisk 应用中安装 LSPosed

4. 重启

5. 从通知栏打开 LSPosed 管理器

> 或者安装压缩包中的 manager.apk 文件。

6. 尽情享受吧 :)

＃＃ 下载

- 转到电报：[@lspose-irena](https://t.me/s/lsposed_irena)
- 对于金丝雀构建，请检查 [Github Actions](https://github.com/re-zero001/LSPosed-Irena/actions/workflows/core.yml?query=branch%3Adev)

## 获取帮助

**仅接受来自**最新调试版本**的错误报告。**
- GitHub 问题：[问题](https://github.com/re-zero001/LSPosed-Irena/issues/)
-（针对中文人士）本项目仅接受英语**标题**的问题。如果您不懂英语，请使用[翻译工具](https://www.deepl.com/zh/translator)

## 致开发者

欢迎开发者使用基于 LSPosed 框架的钩子编写 Xposed 模块。基于 LSPosed 框架的模块与原始 Xposed 框架完全兼容，反之亦然，基于 Xposed 框架的模块也能与 LSPosed 框架良好配合。

- [Xposed 框架 API](https://api.xposed.info/)
- 我们使用自己的模块仓库。我们欢迎开发者向我们的仓库提交模块，之后即可在 LSPosed 中下载这些模块。

- [LSPosed 模块仓库](https://github.com/Xposed-Modules-Repo)

## 社区讨论

此分支将不包含以下内容。

## 致谢

- [Magisk](https://github.com/topjohnwu/Magisk/): 使这一切成为可能

- [ZygiskNext](https://github.com/Dr-TSNG/ZygiskNext): 提供了一种将代码注入 Zygote 进程的方法

- [XposedBridge](https://github.com/rovo89/XposedBridge): 原始的 Xposed 框架 API

- [Dobby](https://github.com/re-zero001/Dobby): 用于内联 hook

- [LSPlant](https://github.com/LSPosed/LSPlant): 核心 ART hook 框架

- [LSPosed](https://github.com/LSPosed/LSPosed): 分支源代码

- [EdXposed](https://github.com/ElderDrivers/EdXposed): LSPosed 分支源代码

- [xz_embedded](https://github.com/tukaani-project/xz-embedded): 将 debug_info 部分解压缩为剥离后的库

- [system_properties](https://github.com/topjohnwu/system_properties): 在 LSPosed 中切换属性访问

- ~[SandHook](https://github.com/ganyao114/SandHook/): SandHook 变体的 ART hooking 框架~

- ~[YAHFA](https://github.com/rk700/YAHFA): 之前的 ART hooker 框架~

- ~[dexmaker](https://github.com/linkedin/dexmaker) 和 [dalvikdx](https://github.com/JakeWharton/dalvik-dx): 用于动态生成 YAHFA hooker 类~

- ~[DexBuilder](https://github.com/LSPosed/DexBuilder): 用于动态生成 YAHFA hooker 类~

## 许可

LSPosed 采用 **GNU 通用公共许可证 v3 (GPL-3)** 授权 (http://www.gnu.org/copyleft/gpl.html)。

