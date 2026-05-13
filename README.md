# NovaVault

NovaVault 是一款主打**绝对数据自持**的跨平台密码管理与开发者工具箱。

## 核心特性

**密码管理器**
- 密码分组、条目管理、搜索、收藏
- 历史版本记录、平台图标自动抓取
- 一键复制、剪贴板自动清空
- MFA 两步验证码实时读秒

**开发者工具箱**
- JSON 格式化 / 压缩
- 文本 Diff 对比
- 时间戳转换
- Base64 编解码
- 纯本地运行，断网可用

**零信任安全架构**
- 主密码 + Secret Key 双密钥保护
- AES-256-GCM 加密，Argon2 密钥派生
- 本地 SQLite 存储，数据不离开你的设备
- WebDAV 加密同步，远端只存密文

**跨平台**
- macOS (Apple Silicon / Intel)
- Windows
- Linux

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
