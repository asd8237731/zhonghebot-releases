# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库提供安装包、签名更新包和更新清单；应用源码保存在私人开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.27](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.27)。Windows x64 仍提供现有 0.1.11 测试安装包。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.27 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.27/MochiBot_0.1.27_aarch64.dmg) | Apple Silicon Mac，macOS 13 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，验证范围见对应发行说明 |

0.1.27 增加 Codex 初始化分段诊断，改进 FFmpeg 发现、浏览器满槽回收、群派工回报、MCP 应用核查和大素材目录处理。完整变化与验证范围见[发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.27)。

升级前请导出备份。本版主库 schema 19、扩展主库 schema 3；旧版不能直接打开升级后的主库，回退须恢复升级前备份，不要手工修改数据库版本。恢复备份保留历史和来源证据，但不会继承待执行授权或自动重放未确认的操作。

macOS 应用内更新使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)，当前提供 Mac 制品。旧版若持续显示“更新连接失败”，可手动下载本页 DMG，退出应用后替换完整 MochiBot.app 一次。保留 macOS 静态 HTTPS 系统代理支持、超时与来源分类；PAC、自动发现和仅 SOCKS 系统配置未新增支持。

首次安装请把完整 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 证书，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制仍需辅助功能、屏幕录制权限及应用内本机访问开关。稳定签名不等于系统权限延续已验收。

Windows 新包须完成独立构建与验收，现有 0.1.11 不改标。Windows 0.1.11 尚无 Authenticode 签名，也不包含本次 Mac 0.1.27 修复。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。

安装前请完成或停止任务与排队工作。首次历史构建、来源认证和部分发送／分支／回应仍有完整读取成本。真实模型账号、网站上传与发布、实际安装升级及系统权限需独立验收，不由隔离测试或制品验签推定。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。Homebrew tap 尚未发布，目前请使用上述安装包。

官网：https://www.zhonghedingfu.com
