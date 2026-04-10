# OpenClaw Packages

<p align="center">
  <img src="https://github.com/openclaw/openclaw/raw/refs/heads/main/docs/assets/openclaw-logo-text-dark.svg" alt="OpenClaw" width="400">
</p>

<p align="center">
  <strong>Fully Offline · Zero Dependencies · Multi-Platform</strong>
</p>

<p align="center">
  <a href="https://github.com/openclaw/openclaw/releases">
    <img src="https://img.shields.io/github/v/release/openclaw/openclaw?label=Official&color=blue" alt="Official Version">
  </a>
  <a href="https://github.com/StanleyChanH/openclaw-pkgs/releases">
    <img src="https://img.shields.io/github/v/release/StanleyChanH/openclaw-pkgs?label=Packages&color=green" alt="Packages Version">
  </a>
</p>

---

## Supported Platforms

| Platform | Architecture | Format |
|----------|--------------|--------|
| Windows | x64 (amd64) | `.zip` |
| Windows | arm64 | `.zip` |
| macOS | x64 (amd64) | `.tar.gz` |
| macOS | arm64 (M1/M2/M3) | `.tar.gz` |
| Linux | x64 (amd64) | `.tar.gz` |
| Linux | arm64 | `.tar.gz` |

---

## Download

Visit the [**Releases**](https://github.com/StanleyChanH/openclaw-pkgs/releases) page to download the package for your platform.

---

## Usage

### 1. Extract the package

```bash
# macOS/Linux
tar -xzf openclaw-pkgs-vX.X.X-PLATFORM-ARCH.tar.gz

# Windows
# Extract the ZIP file directly
```

### 2. Run OpenClaw

```bash
# macOS/Linux
./nodejs/bin/node ./node_modules/.bin/openclaw

# Windows
nodejs\node.exe node_modules\.bin\openclaw
```

### Common commands

```bash
# Show help
./nodejs/bin/node ./node_modules/.bin/openclaw --help

# Run diagnostics
./nodejs/bin/node ./node_modules/.bin/openclaw doctor

# Configure AI model
./nodejs/bin/node ./node_modules/.bin/openclaw onboard
```

> ⚠️ **Note**: Initial configuration requires internet connection for OAuth authentication.

---

## Package Contents

```
openclaw-pkgs/
├── nodejs/            # Node.js runtime
├── node_modules/      # OpenClaw and all dependencies
├── package.json       # Dependency declaration
├── package-lock.json  # Dependency lock
└── README.md          # Documentation
```

**Complete runtime environment included, no additional downloads required!**

---

## System Requirements

| Requirement | Details |
|-------------|---------|
| OS | Windows 10/11, macOS 11+, Linux (glibc 2.17+) |
| Architecture | Select the version matching your system |
| Network | Only needed for initial OAuth authentication |

---

## Automatic Version Sync

This repository automatically detects and syncs with [OpenClaw official releases](https://github.com/openclaw/openclaw) via GitHub Actions:

- ⏰ **Hourly check** - Automatically detects latest version on npm
- 🤖 **Auto build** - Packages all platforms when new version detected
- 📦 **Auto release** - Release version matches official version
- 🔒 **SHA256 checksum** - Integrity verification for each package

---

## Resources

- [OpenClaw Documentation](https://docs.openclaw.ai)
- [Getting Started Guide](https://docs.openclaw.ai/start/getting-started)
- [GitHub Repository](https://github.com/openclaw/openclaw)
- [Discord Community](https://discord.gg/clawd)

---

## License

OpenClaw uses the [MIT License](https://github.com/openclaw/openclaw/blob/main/LICENSE).

---

<p align="center">
  <strong>EXFOLIATE! EXFOLIATE!</strong>
</p>