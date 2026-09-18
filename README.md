<div align="center">

# TopSSH

**为认真管理服务器的人打造的跨平台 SSH 工作台**

一个快速、安全、安静的现代 SSH 客户端。连接 Windows 桌面与 iOS 移动端，随时随地掌控生产环境。

[下载客户端](#下载与获取) · [功能亮点](#核心亮点) · [跨端同步](#跨平台互通与同步) · [定价与订阅](#定价说明) · [常见问题](#常见问题)

</div>

---

## 为什么选择 TopSSH？

作为运维工程师与开发者，我们常常在工位使用 **Windows 电脑**高频操作终端与传输文件，而在通勤、会议或突发故障时，需要立刻掏出 **iPhone 或 iPad** 查看服务状态、重启进程。

TopSSH 打破了桌面与移动端的割裂体验：**在 Windows 上规划好的主机列表、命令片段与备忘录，无缝漫游到 iOS 设备上**，随时保持专注，从容应急。

---

## 核心亮点

### 1. 跨平台互通，一个工作流
* **Windows 与 iOS 无缝协同**：主机配置、自定义分组、快捷命令与运维备忘录在各端之间完全兼容、自由同步。
* **桌面端强大完整**：基于高性能核心构建，支持多标签终端、SFTP 双向文件管理与在线代码编辑、端口转发与 SOCKS5 代理隧道。
* **iOS 原生精悍**：专为 iPhone 与 iPadOS 适配的原生界面，支持真 PTY 交互式全屏终端（完整 ANSI 颜色、支持 `vim`/`htop` 全屏程序）、键盘辅助条与快捷命令抽屉。

### 2. 本地优先，坚固的安全基石
* **系统级钥匙串保护**：敏感凭据绝不存入未加密的明文文本。Windows 凭据存入系统 **Credential Manager**，iOS/macOS 凭据严格存入 **系统 Keychain**。
* **生物识别加锁**：iOS 端支持连接前调用 **Face ID / Touch ID / 设备密码** 鉴权，避免手机借出时服务器被未授权访问。
* **零遥测与隐私保护**：无中心化账号体系，无广告，无数据追踪分析 SDK，终端敲击流完全点对点直连服务器，绝不记录任何击键数据。

### 3. 灵活自主的端到端加密同步
TopSSH 不强制绑定任何第三方中心化云服务，所有同步均在客户端本地进行高强度加密（PBKDF2 派生密钥 + AES-GCM-256），云端仅保存密文快照：
* **WebDAV 同步**：支持自建 NAS（群晖/威联通）、Nextcloud、坚果云等私有云。
* **S3 兼容对象存储**：支持 Cloudflare R2、AWS S3、阿里云 OSS、MinIO 等。
* **iCloud 自动同步（开发中 🚀）**：即将支持 Apple 原生 iCloud 云端无感自动同步，体验更加丝滑。

---

## 平台支持矩阵

| 功能 / 特性 | Windows 桌面端 | iOS / iPadOS 移动端 |
| :--- | :---: | :---: |
| **交互式终端** | 多标签页 / xterm.js | 原生全屏 PTY / SwiftTerm |
| **认证方式** | 密码 / 私钥（Ed25519, RSA） | 密码 / 私钥（支持口令解锁） |
| **跳板机（Bastion）** | 多跳代理 | 单跳跳板机 |
| **快捷命令片段** | 分组管理 / 一键执行 | 侧栏抽屉 / 终端实时注入 |
| **文件管理 (SFTP)** | 目录树 / 断点续传 / 在线编辑 | — |
| **端口转发与隧道** | 本地 / 远程 / SOCKS5 | — |
| **凭据存储** | Windows Credential Manager | iOS Keychain (`ThisDeviceOnly`) |
| **生物识别验证** | Windows Hello | Face ID / Touch ID |
| **同步协议** | WebDAV / S3 | WebDAV / S3 / iCloud (开发中) |

---

## 定价说明

TopSSH 采用透明、简单的订阅策略，无任何隐藏收费：

* **桌面端（Windows / macOS）**：**免费使用**，提供完整的本地连接、SFTP 与终端能力。
* **iOS / iPadOS 专业版**：**$3.99 / 年（订阅）**
  * 包含所有平台功能更新；
  * 解锁移动端完整的 WebDAV 与 S3 跨端端到端加密同步；
  * 未来享有即将推出的 iCloud 无感多端同步支持；
  * 专为移动运维打造的极致轻量与安全体验，极具性价比。

---

## 下载与获取

* **iOS / iPadOS**：即将上架 [Apple App Store](#)（或加入 TestFlight 尝鲜）
* **Windows / macOS**：前往本仓库的 [Releases 页面](https://github.com/cnliucheng/TopSSH/releases) 直接下载最新安装包（`.exe` / `.dmg`）。

---

## 隐私与服务协议

* [隐私政策 (Privacy Policy)](https://cnliucheng.github.io/TopSSH_iOS/privacy.html)
* [服务条款 (Terms of Service)](https://cnliucheng.github.io/TopSSH_iOS/terms.html)

---

## 问题反馈与支持

如果你在日常使用中遇到问题、发现 Bug 或有新功能构想，欢迎通过以下渠道交流：

* 提交问题反馈：[GitHub Issues](https://github.com/cnliucheng/TopSSH_iOS/issues)
* 联系开发者：[wusky1988@gmail.com](mailto:wusky1988@gmail.com)

---

<div align="center">
<small>© 2026 TopSSH. Made for engineers who take server management seriously.</small>
</div>
