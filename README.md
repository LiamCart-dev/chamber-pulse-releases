# Chamber Pulse · 会话脉动

macOS 会话悬浮窗，汇总本机及远程 OpenChamber、DeepSeek Harness 的进行中会话和完成待查看结果。

## 下载与安装

前往 [最新版本](https://github.com/LiamCart-dev/chamber-pulse-releases/releases/latest)，下载与你的 Mac 对应的 DMG：Apple Silicon 选择 `arm64`，Intel 选择 `x64`。要求 macOS 13 或更新版本。

打开 DMG，将 **Chamber Pulse.app** 拖入 **Applications**，再从应用程序打开。独立应用已内置 Node.js。当前版本尚未进行 Apple Developer ID 签名和公证；如被 macOS 阻止，请按「系统设置 → 隐私与安全性」中的提示允许打开。

## 更新

0.5.0 起，独立应用支持菜单栏「检查更新…」和「自动检查更新」。更新包通过 Sparkle 签名验证，用户确认后安装并重新启动，保留已配置实例和窗口位置。0.4.0 及更早版本需先手动安装新版。

## 扩展与插件

- `openchamber-arm64.zip` / `openchamber-x64.zip`：在 OpenChamber 2.6.0+ 的「设置 → 扩展」导入对应架构的 ZIP，并允许本地服务。
- `dsh-plugin.zip`：解压后在插件目录执行 `dsh plugin --profile desktop add "file:$(pwd)"`，然后重启 DSH Host 并重新加载客户端。详细说明随插件提供。

扩展和插件通过各自宿主安装新版，不由桌面应用的自动更新替换。Release 中的 `update-*.zip` 和 `appcast-*.xml` 供应用自动更新使用，手动安装请选择 DMG。
