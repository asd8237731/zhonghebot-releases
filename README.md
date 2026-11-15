# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.18](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.18)。Windows x64 目前仍提供现有 0.1.11 测试安装包。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.18 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.18/MochiBot_0.1.18_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，实机验证范围见对应发行说明 |

0.1.18 修复 Mac 应用内更新未读取系统 HTTPS 代理的问题，保留代理环境配置优先及 NO_PROXY 排除，改进超时与来源错误分类。没有关闭 TLS、签名、签名版本或下载来源核验。系统代理兼容仅覆盖 macOS 静态 HTTPS 配置，不包含 PAC、自动发现或仅 SOCKS 系统配置。

旧版若始终显示“更新连接失败”，请手动下载本页 DMG，退出应用后替换完整 MochiBot.app 一次；旧客户端的代理读取逻辑无法由线上清单直接修复。网络恢复时也可再次检查更新。

本版保留 0.1.17 的 Codex 原聊天核查与恢复、浏览器／桌面等待、媒体磁盘快照与 HTTP MCP 改进。完整变化和验收范围见 [发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.18)。

升级前请在应用中保存数据备份。与 0.1.17 相同，主库为 schema 13，扩展库为 schema 3；从 0.1.16 或更早版本首次完成迁移后，0.1.16 不能直接打开该数据库，回退须恢复升级前备份。

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

macOS 应用内更新使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)。本次清单仅提供 Mac 制品；Windows 新版尚待独立构建与验收，现有 0.1.11 安装器不改标。

Windows 0.1.11 尚无 Authenticode 签名。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。真实系统权限延续、网站与模型账号、Windows 实体设备及跨版本升级验收范围见各版发行说明。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
