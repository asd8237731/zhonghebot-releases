# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.12](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.12)。Windows x64 目前仍提供已验证的 0.1.11，0.1.12 安装包尚待构建验收。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.12 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.12/MochiBot_0.1.12_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，实机验证范围见对应发行说明 |

0.1.12 改进长任务与中断恢复、浏览器断线及控件识别、窗口局部观察、机器人委派、MCP Schema 校验和技能发现，并更新附件解析与 SQLite 依赖。旧式 OLE／XLS 暂不支持文本提取，可转换为 XLSX；XLSX／ODS 继续支持。完整变化和限制见 [发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.12)。

升级前请在应用中保存数据备份。本版首次启动会将主数据库迁移到 schema 12；退回 0.1.11 需要恢复升级前备份，不能直接让旧版读取迁移后的数据目录。

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

macOS 可通过应用内“检查更新”获取 0.1.12，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)。本次清单仅提供 Mac 制品；Windows 0.1.12 尚未提供应用内更新，请使用上面的 0.1.11 安装器。

Windows 0.1.11 尚无 Authenticode 签名。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。真实系统权限延续、网站与模型账号、Windows 实体设备及跨版本升级验收范围见各版发行说明。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
