# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

macOS 当前测试版为 [0.1.11](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.11)，Windows x64 当前公开测试版仍为 [0.1.10](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.10)。也可从 [最新发行](https://github.com/asd8237731/zhonghebot-releases/releases/latest) 查看后续版本与已知限制。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.11 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.10 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.10/MochiBot_0.1.10_x64-setup.exe) | Windows x64，实机验证范围见发行说明 |

macOS 0.1.11 新增与改进：

- 后台技能回顾、同部门手动／自动共享及准确撤销，保留助手自己的同名技能；修复同时关联多个技能目录时的同名技能优先级。
- 补齐快速创建与完整日程表单的中文显示。
- 电脑工具准备失败时明确操作是否执行、是否创建审批卡，并给出对应恢复提示。
- 首次欢迎页与无 AI 主页面可直接配置众合AI Key；清理无效安装指南及尚未接入的 VPS／Podman 部署步骤。

后台技能回顾默认关闭，目前支持普通 HTTP 对话，会使用对应模型额度；Codex／Claude 等 CLI 后台回顾及群聊、目标、日程会话暂不支持。电脑恢复提示不代表系统权限已自动修复；Codex 桌面应用包扫描尚未实现，已有配置继续通过 CLI 复用。详情见 [0.1.11 发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.11)。

Windows 0.1.11 仍在构建与验收中，尚未公开；当前请使用表中的 0.1.10 安装器。本次先上线 Mac 更新项，Windows 更新项待 0.1.11 验收完成后加入。

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。0.1.11 沿用原 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。使用电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

Windows x64 0.1.10 为测试安装器，已在 GitHub Windows Server 2022 完成完整 Rust、WebView2 隔离界面及临时安装／同版重装／卸载／数据保留验收。安装器尚无 Authenticode 签名，Tauri 更新签名使用原密钥。Windows 10／11 实际设备、混合 DPI、旧版本跨版本升级、真实网站与账号及系统授权继承仍需分别验证。

macOS 0.1.2 及后续版本、Windows 当前测试版提供应用内“检查更新”，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)；应用会按平台选择制品，并核验独立的 Tauri 更新签名和版本。更新签名与 Apple 签名／公证、Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。请阅读每次 Release 的已知限制；此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
