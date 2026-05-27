# FocusTomato

简体中文 | [English](README.md)

FocusTomato 是一款原生 macOS 网站与应用拦截器。启动专注会话、设置重复保护时间，在工作期间把分心内容挡在外面。

![FocusTomato Blue theme interface](https://alexab612.github.io/FocusTomatoDoc/img/screenshot.png)

- [网站](https://alexab612.github.io/FocusTomatoDoc/)
- [下载 v1.0.3](https://github.com/alexab612/FocusTomato/releases/tag/v1.0.3)
- [隐私政策](https://alexab612.github.io/FocusTomatoDoc/privacy/)
- [使用条款](https://alexab612.github.io/FocusTomatoDoc/terms/)
- [反馈与支持](https://github.com/alexab612/FocusTomato/issues)

### 下载

当前稳定版本：**v1.0.3**

- [下载 FocusTomato-1.0.3.dmg](https://github.com/alexab612/FocusTomato/releases/download/v1.0.3/FocusTomato-1.0.3.dmg)
- [查看 v1.0.3 发布说明](https://github.com/alexab612/FocusTomato/releases/tag/v1.0.3)
- [查看所有 Releases](https://github.com/alexab612/FocusTomato/releases)

### macOS 安装说明

1. 下载并打开 DMG，将 `FocusTomato` 拖入 `Applications` 文件夹。
2. 当前安装包尚未使用 Developer ID 签名与 Apple 公证。首次打开时，macOS 可能提示无法验证开发者并阻止启动。
3. 如果启动被阻止，请打开 `系统设置 -> 隐私与安全性 -> 安全性`，在 FocusTomato 的提示旁点击“仍要打开”。
4. 在随后的系统确认窗口中再次选择“打开”，之后即可正常启动应用。

网站拦截需要 macOS 自动化权限。首次对浏览器执行网站拦截时，请按系统提示允许 FocusTomato 控制对应浏览器；也可以在 `系统设置 -> 隐私与安全性 -> 自动化` 中查看授权状态。

### 核心功能

- 网站与应用规则：每个预设分别管理网站和应用的黑名单或白名单。
- 临时启停条目：用列表中的勾选框停用某个条目，无需将其删除。
- 专注与休息：启动定时专注，支持暂停、继续及专注结束后的休息流程。
- 重复计划：按星期和时间段自动启动预设的拦截规则。
- 统计记录：查看专注时长、会话次数和被拦截最多的网站或应用。
- 菜单栏操作：从菜单栏快速查看状态和控制当前会话。
- 更新检测：在应用中手动检查 GitHub Releases 上的新版本。
- 外观模式：提供跟随系统、浅色、深色和 `Blue` 四个外观选项。

### 支持的浏览器

网站拦截目前支持 `Safari`、`Google Chrome`、`Microsoft Edge`、`Brave`、`Opera` 与 `Arc`。应用拦截针对你添加到预设中的 macOS App 生效。

### 隐私

FocusTomato 当前版本是本地优先的 macOS 应用。设置、预设、专注记录和统计信息保存在本机；应用不包含账号系统、远程分析服务或广告追踪 SDK。MVP 版本暂不提供云同步功能。

[查看完整隐私政策](https://alexab612.github.io/FocusTomatoDoc/privacy/)

### 使用条款

FocusTomato 的使用条款基于 Apple 标准最终用户许可协议，并包含简短的应用补充条款。

[查看完整使用条款](https://alexab612.github.io/FocusTomatoDoc/terms/)

### 反馈与支持

遇到问题或希望提出改进建议，请在 [GitHub Issues](https://github.com/alexab612/FocusTomato/issues) 中提交反馈。

### 本地开发

构建 macOS App：

```bash
xcodebuild -project FocusTomato.xcodeproj -scheme FocusTomato -configuration Debug -destination 'platform=macOS' build
```

构建文档站：

```bash
cd FocusTomatoDoc
npm install
npm run build
```
