# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.14](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.14)。Windows x64 目前仍提供现有 0.1.11 测试安装包，0.1.14 安装包尚待构建验收。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.14 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.14/MochiBot_0.1.14_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，实机验证范围见对应发行说明 |

0.1.14 修复聊天框视频与普通文件的拖放、选择、发送关联、重启恢复和中文文件名下载；支持 MP4／MOV／M4V／WebM，以及 ZIP 等普通文件附件。视频目前只保存原文件并提供文件信息，尚未解析画面与音轨；非图片文件单个上限为 25 MiB。本版还包含浏览器控制权交接、已保存步骤、草稿恢复和 Codex／Claude 配置复用改进。完整变化和限制见 [发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.14)。

升级前请在应用中保存数据备份。主数据库仍为 schema 12；从 0.1.13 升级不新增数据库版本迁移。退回 0.1.11 需要恢复升级前备份，不能直接让旧版读取 schema 12 数据目录。

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

macOS 可通过应用内“检查更新”获取 0.1.14，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)。本次清单仅提供 Mac 制品；Windows 0.1.14 尚未提供应用内更新，请使用上面的 0.1.11 安装器。

Windows 0.1.11 尚无 Authenticode 签名。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。真实系统权限延续、网站与模型账号、Windows 实体设备及跨版本升级验收范围见各版发行说明。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
