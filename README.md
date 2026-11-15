# MochiBot 发行下载

众合桌面 AI 助手的公开制品仓库。此仓库只提供安装包、签名更新包和更新清单；应用源码保留在私有开发仓库。

macOS Apple Silicon 当前测试版为 [0.1.17](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.17)。Windows x64 目前仍提供现有 0.1.11 测试安装包，0.1.17 安装包尚待构建验收。

| 平台 | 安装包 | 安装要求 |
| --- | --- | --- |
| macOS Apple Silicon | [下载 0.1.17 ARM64 DMG](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.17/MochiBot_0.1.17_aarch64.dmg) | Apple Silicon Mac，macOS 12 或更高版本 |
| Windows x64 | [下载 0.1.11 NSIS 安装器](https://github.com/asd8237731/zhonghebot-releases/releases/download/v0.1.11/MochiBot_0.1.11_x64-setup.exe) | Windows x64，实机验证范围见对应发行说明 |

0.1.17 增加 Codex 原聊天核查与恢复回执，修正引擎／CLI 配置模型展示，完善同轮有效配置及最终诊断。浏览器可等待准确子框架的加载与换文档；桌面支持指定窗口标题、菜单与焦点事件等待。工作区视频／PDF 改用磁盘分块快照上传，HTTP MCP 目录发现与连接复用、浏览器预览重复查询得到改进。视频仍不解析画面或音轨，网页文件赋值不代表网站发布成功；ego 中由助手接收网页下载文件仍待官方桥支持。完整变化和验收范围见 [发行说明](https://github.com/asd8237731/zhonghebot-releases/releases/tag/v0.1.17)。

升级前请在应用中保存数据备份。主数据库从 schema 12 迁移到 13，扩展库仍为 schema 3；首次启动完成数据库迁移后，0.1.16 不能直接打开该数据库，回退须恢复升级前备份。

macOS 首次安装请退出旧版，把完整的 MochiBot.app 拖入“应用程序”。沿用原 Apple Development 身份签名，尚未经过 Apple 公证；首次打开可能需要在“系统设置 → 隐私与安全性”中允许。电脑控制需另授予辅助功能和屏幕录制权限，并在应用中启用本机访问。

macOS 可通过应用内“检查更新”获取 0.1.17，使用[固定更新清单](https://github.com/asd8237731/zhonghebot-releases/releases/latest/download/latest.json)。本次清单仅提供 Mac 制品；Windows 0.1.17 尚未提供应用内更新，请使用上面的 0.1.11 安装器。

Windows 0.1.11 尚无 Authenticode 签名。Tauri 更新签名、Apple 代码签名／公证和 Windows Authenticode 是不同机制。安装前请完成或停止任务与排队工作。真实系统权限延续、网站与模型账号、Windows 实体设备及跨版本升级验收范围见各版发行说明。

安装包保留上游 LICENSE、NOTICE 和第三方许可资源。此仓库不保存用户聊天、账号或密钥。

官网：https://www.zhonghedingfu.com

Homebrew tap 尚未发布，目前请使用上述安装包。
