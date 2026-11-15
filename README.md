# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库提供安装包、签名更新包和更新清单；应用源码保存在私人开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.19](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.19)。Windows x64 仍提供现有 0.1.11 测试安装包。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.19 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.19/MochiBot_0.1.19_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，验证范围见对应发行说明 |

0.1.19 增加当前聊天技能 ZIP 检查、向真实机器人安装／分配技能，以及主助手部门和群聊管理；审批后保存真实结果和收据，支持符合条件的撤回。修复 Codex MCP 单次工具审批和轮次归属。创建、安装不会自动执行技能脚本，也不代表视频任务已完成。完整变化与验收范围见[发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.19)。

升级前请导出备份。本版在主库 schema 13、扩展库 schema 3 下增加组织状态、收据表和触发器；schema 版本不变不代表旧应用可直接读取。回退须恢复升级前备份，勿让旧版本直接打开升级后的数据库。

macOS 应用内更新使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)，当前提供 Mac 制品。旧版若持续显示“更新连接失败”，请手动下载本页 DMG，退出应用后替换完整 MochiBot.app 一次。保留 0.1.18 的 macOS 静态 HTTPS 系统代理支持、超时与来源分类；PAC、自动发现和仅 SOCKS 系统配置未新增支持。

首次安装请把完整 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 证书，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制仍需辅助功能、屏幕录制权限及应用内本机访问开关。稳定签名不等于系统权限延续已验收。

Windows 新包须完成独立构建与验收，现有 0.1.11 不改标。Windows 0.1.11 尚无 Authenticode 签名。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。

安装前请完成或停止任务与排队工作。真实模型账号、用户技能 ZIP、视频渲染／发布、安装升级及系统权限需独立验收，不由隔离测试或制品验签推定。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。Homebrew tap 尚未发布，目前请使用上述安装包。

官网：https://www.zhonghedingfu.com
