# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

当前测试版为 [0.1.10](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.10)。也可从 [最新发行](https://github.com/asd8237731/zhonghebot-releases/releases/latest) 查看后续版本与已知限制。

| 平台 | 0.1.10 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.10/MochiBot_0.1.10_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.10/MochiBot_0.1.10_x64-setup.exe) | Windows x64，实机验证范围见发行说明 |

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。0.1.10 使用 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。使用电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

Windows x64 为测试安装器，已在 GitHub Windows Server 2022 完成完整 Rust、WebView2 隔离界面及临时安装／同版重装／卸载／数据保留验收。安装器尚无 Authenticode 签名，Tauri 更新签名使用原密钥。Windows 10／11 实际设备、混合 DPI、旧版本跨版本升级、真实网站与账号及系统授权继承仍需分别验证。

macOS 0.1.2 及后续版本、Windows 当前测试版提供应用内“检查更新”，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)；应用会按平台选择制品，并核验独立的 Tauri 更新签名和版本。更新签名与 Apple 签名／公证、Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。请阅读每次 Release 的已知限制；此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
