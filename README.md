# Z Router 客户端发布

本仓库用于发布 Z Router 桌面客户端的版本说明、安装包和更新检测清单。

## 下载安装

请从本仓库的 [Releases](https://github.com/aifeihu/z-router/releases) 页面选择适合当前系统与架构的版本。

| 系统 | 架构 | 人工安装包 |
| --- | --- | --- |
| macOS | Apple Silicon（arm64 / aarch64） | `.dmg` |
| macOS | Intel（x86_64） | `.dmg` |
| Windows | x64（x86_64） | `.exe` |

具体支持平台、最低系统和升级注意事项以对应版本说明为准。macOS 当前使用 Ad Hoc 签名，Windows 当前提供未签名安装包；系统可能提示手动放行，部分设备策略可能禁止运行。

## 版本与更新检测

- 正式版本使用 `v<版本号>` 标签，如 `v0.4.0`。
- 每个正式发行包含更新说明、已验收的平台安装包和 `client-update.json`。
- 客户端通过 GitHub 公开 API 匿名检测版本；当前阶段仅规划版本提示及人工下载，不代表已经实现自动安装。
- 已发布安装包和清单禁止覆盖，修复使用新版本。
- 本仓库初始化时不包含客户端发行；没有正式 Release 表示暂未提供可检测版本。

匿名版本查询接口：

```text
https://api.github.com/repos/aifeihu/z-router/releases
```

## 仓库范围

本仓库仅管理公开发行资料与二进制附件。源码在独立的内部仓库管理，不在此公开。

公开下载不代表授予源码或二进制的开源许可，使用与分发条件以随版本提供的许可说明为准。
