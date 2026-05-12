# NovaVault Releases

NovaVault 官方发布仓库，用于存放自动更新所需的安装包和签名文件。

## 📦 产物说明

### macOS

| 文件 | 说明 |
|------|------|
| `NovaVault_aarch64.app.tar.gz` | macOS Apple Silicon (M1/M2/M3/M4) 安装包，用于自动更新 |
| `NovaVault_aarch64.app.tar.gz.sig` | 对应的 minisign 签名文件，用于校验完整性 |
| `NovaVault_aarch64.dmg` | macOS Apple Silicon 磁盘镜像，手动安装用 |
| `NovaVault_x64.app.tar.gz` | macOS Intel 安装包，用于自动更新 |
| `NovaVault_x64.app.tar.gz.sig` | 对应的 minisign 签名文件 |
| `NovaVault_x64.dmg` | macOS Intel 磁盘镜像，手动安装用 |

### Windows

| 文件 | 说明 |
|------|------|
| `NovaVault_x64-setup.nsis.zip` | Windows 安装包 (NSIS)，用于自动更新 |
| `NovaVault_x64-setup.nsis.zip.sig` | 对应的 minisign 签名文件 |
| `NovaVault_x64-setup.exe` | Windows 安装程序，手动安装用 |
| `NovaVault_x64-setup.msi` | Windows MSI 安装包，企业部署用 |

### Linux

| 文件 | 说明 |
|------|------|
| `NovaVault_amd64.AppImage.tar.gz` | Linux AppImage，用于自动更新 |
| `NovaVault_amd64.AppImage.tar.gz.sig` | 对应的 minisign 签名文件 |
| `NovaVault_amd64.AppImage` | Linux 通用安装包，手动安装用 |
| `NovaVault_amd64.deb` | Debian/Ubuntu 安装包 |
| `NovaVault_x86_64.rpm` | Fedora/RHEL 安装包 |

### 更新清单

| 文件 | 说明 |
|------|------|
| `latest.json` | 自动更新清单，客户端通过此文件检查新版本 |

## 🔒 安全说明

所有自动更新包均使用 minisign 签名校验，确保下载文件未被篡改。

## 🍎 macOS 安装说明

macOS 用户首次打开应用时可能会提示 **"NovaVault" 已损坏，无法打开**，这是因为应用未经过 Apple 公证（Notarization）。

**解决方法：**

打开终端，执行以下命令后重新打开应用即可：

```bash
sudo xattr -rd com.apple.quarantine "/Applications/NovaVault.app"
```

**或者：**

1. 打开 **系统设置** → **隐私与安全性**
2. 滚动到底部，找到安全提示
3. 点击 **"仍要打开"**
4. 输入密码确认

此操作只需执行一次，后续更新不受影响。
