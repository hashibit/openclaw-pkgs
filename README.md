# OpenClaw Packages

<p align="center">
  <img src="https://raw.githubusercontent.com/openclaw/openclaw/main/docs/assets/openclaw-logo-text.png" alt="OpenClaw" width="400">
</p>

<p align="center">
  <strong>完全离线运行 · 零依赖下载 · 多平台支持</strong>
</p>

<p align="center">
  <a href="https://github.com/openclaw/openclaw/releases">
    <img src="https://img.shields.io/github/v/release/openclaw/openclaw?label=Official&color=blue" alt="Official Version">
  </a>
  <a href="https://github.com/StanleyChanH/openclaw-offline-package/releases">
    <img src="https://img.shields.io/github/v/release/StanleyChanH/openclaw-offline-package?label=Offline%20Package&color=green" alt="Offline Package Version">
  </a>
</p>

---

## 支持平台

| 平台 | 架构 | 文件格式 |
|------|------|----------|
| Windows | x64 (amd64) | `.zip` |
| Windows | arm64 | `.zip` |
| macOS | x64 (amd64) | `.tar.gz` |
| macOS | arm64 (M1/M2/M3) | `.tar.gz` |
| Linux | x64 (amd64) | `.tar.gz` |
| Linux | arm64 | `.tar.gz` |

---

## 下载

前往 [**Releases**](https://github.com/StanleyChanH/openclaw-offline-package/releases) 页面下载对应平台的离线包。

---

## 使用方法

### 1. 解压离线包

```bash
# macOS/Linux
tar -xzf openclaw-pkgs-vX.X.X-PLATFORM-ARCH.tar.gz

# Windows
# 直接解压 ZIP 文件
```

### 2. 运行 OpenClaw

```bash
# macOS/Linux
./nodejs/bin/node ./node_modules/.bin/openclaw

# Windows
nodejs\node.exe node_modules\.bin\openclaw
```

### 常用命令

```bash
# 查看帮助
./nodejs/bin/node ./node_modules/.bin/openclaw --help

# 运行诊断
./nodejs/bin/node ./node_modules/.bin/openclaw doctor

# 配置 AI 模型
./nodejs/bin/node ./node_modules/.bin/openclaw onboard
```

> ⚠️ **注意**：首次配置需要联网进行 OAuth 认证。

---

## 包内容

```
openclaw-pkgs/
├── nodejs/            # Node.js 运行时
├── node_modules/      # OpenClaw 及所有依赖
├── package.json       # 依赖声明
├── package-lock.json  # 依赖锁定
└── README.md          # 说明文档
```

**包含完整运行环境，无需任何额外下载！**

---

## 系统要求

| 项目 | 要求 |
|------|------|
| 操作系统 | Windows 10/11、macOS 11+、Linux (glibc 2.17+) |
| 架构 | 选择与系统匹配的版本 |
| 网络 | 仅首次 OAuth 认证需要联网 |

---

## 自动版本同步

本仓库通过 GitHub Actions **自动检测并同步** [OpenClaw 官方版本](https://github.com/openclaw/openclaw)：

- ⏰ **每小时检查** - 自动检测 npm 上的最新版本
- 🤖 **自动构建** - 检测到新版本时自动打包所有平台
- 📦 **自动发布** - Release 与官方版本号保持一致
- 🔒 **SHA256 校验** - 每个包都提供完整性校验

---

## 更多资源

- [OpenClaw 官方文档](https://docs.openclaw.ai)
- [入门指南](https://docs.openclaw.ai/start/getting-started)
- [GitHub 仓库](https://github.com/openclaw/openclaw)
- [Discord 社区](https://discord.gg/clawd)

---

## 许可证

OpenClaw 采用 [MIT 许可证](https://github.com/openclaw/openclaw/blob/main/LICENSE)。

---

<p align="center">
  <strong>EXFOLIATE! EXFOLIATE!</strong>
</p>