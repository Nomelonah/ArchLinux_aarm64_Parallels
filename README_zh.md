# ArchLinux_aarm64_Parallels

<p align="left">
  <a href="./README.md"><b>📄 English README (切换至英文版)</b></a>
</p>

---

## 📌 项目描述
专为 **Apple Silicon Mac** (M系芯片) 上的 **Parallels Desktop** 深度定制、纯手工肉身调优的纯净 Arch Linux ARM64 完全体虚拟机镜像。

本镜像彻底终结了在 ARM64 架构下手动折腾 Arch Linux 的痛苦。

## 🔐 账户、用户与密码凭据
为了彻底避免权限死锁或家目录残缺的悲剧，系统底层的账户经脉已全部理顺。请使用以下凭据进行登录或执行高级特权命令：

| 账户类型 | 用户名 (Username) | 密码 (Password) | 底层权限 / 附加组 |
| :--- | :--- | :--- | :--- |
| **日常主账户** | `watermelon` | *1234* | 已绑定 `wheel`, `storage`, `power` (完美 `sudo`) |
| **最高超级管理员** | `root` | *1234* | 至高无上全系统主权 (`#`) |

> ⚠️ **注意**：以上密码均为初始密码，你进入系统后可以随时根据个人喜好进行修改喵！

## 🚀 怎么用 / 华丽部署指南

得益于 Mac Parallels Desktop 完美的胶囊封装机制，你不需要任何复杂的命令导出，它天生就是一个独立的文件。

### 第一步：下载虚拟机胶囊文件
直接从本仓库（或 Release 页面）下载独立的 `ArchLinux_aarm64_Parallels.pvm` 文件，并将其保存到你 Mac 本地的日常目录中（例如 `~/Documents/Parallels/`）。

### 第二步：无脑肉身强灌 Parallels
1. 在 Mac 访达中找到下载好的 **`ArchLinux_aarm64_Parallels.pvm`** 文件（带有红蓝色小杠图标的虚拟机大胶囊）。
2. 鼠标双击这个 `.pvm` 文件，Parallels Desktop 会自动被唤醒并加载它。
3. **【最关键的一步】**：当软件弹询问 **“此虚拟机是由复制还是移动而来的？”** 时，请务必果断点击 **`已复制` (Copied)**！


---
*一些问题由AI修复，有问题请联系我谢谢。*
