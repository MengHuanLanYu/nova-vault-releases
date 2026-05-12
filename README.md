# NovaVault Releases

NovaVault 官方发布仓库。

## 下载

### macOS

| 文件 | 说明 |
|------|------|
| `NovaVault_aarch64.dmg` | Apple Silicon (M1/M2/M3/M4) |
| `NovaVault_x64.dmg` | Intel |

### Windows

| 文件 | 说明 |
|------|------|
| `NovaVault_x64-setup.exe` | 安装程序 |
| `NovaVault_x64-setup.msi` | MSI 安装包（企业部署） |

### Linux

| 文件 | 说明 |
|------|------|
| `NovaVault_amd64.AppImage` | 通用安装包 |
| `NovaVault_amd64.deb` | Debian / Ubuntu |
| `NovaVault_x86_64.rpm` | Fedora / RHEL |

## macOS 安装说明

首次打开可能提示 **"NovaVault" 已损坏**，这是因为应用未经过 Apple 公证。

**解决方法（任选其一）：**

**方法一：终端命令**
```bash
sudo xattr -rd com.apple.quarantine "/Applications/NovaVault.app"
```

**方法二：系统设置**
1. 打开 **系统设置** → **隐私与安全性**
2. 找到底部安全提示，点击 **"仍要打开"**

此操作只需执行一次，后续更新不受影响。
