# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

当前测试版为 [0.1.10](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.10)。也可从 [最新发行](https://github.com/asd8237731/zhonghebot-releases/releases/latest) 查看后续版本与已知限制。

| 平台 | 0.1.10 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.10/MochiBot_0.1.10_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。0.1.10 使用 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。使用电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

Windows x64 安装包仍在原生验收中，尚未发布。真实网站与账号、系统授权继承和跨版本升级仍需分别验证；隔离夹具不代表这些项目均已通过。

macOS 0.1.2 及后续版本提供应用内“检查更新”，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)；应用会按平台选择制品，并核验独立的 Tauri 更新签名和版本。更新签名与 Apple 签名／公证、Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。请阅读每次 Release 的已知限制；此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
