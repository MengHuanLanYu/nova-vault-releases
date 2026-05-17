# Vaultic

**你的数据，只属于你。**

🌐 官网：https://vaultic.dpdns.org

Vaultic 是一款零信任架构的跨平台密码管理器，所有数据本地加密存储，绝不经过任何第三方服务器。配合 WebDAV 可实现多设备同步，但你的密钥永远不会离开你的设备。

## 为什么选择 Vaultic

**绝对数据自持**
- 本地 SQLite 加密存储，数据不离开你的设备
- WebDAV 同步，远端只存密文，无法被解读
- 不依赖任何云服务，你掌控一切

**零信任安全架构**
- 主密码 + Secret Key 双密钥保护
- AES-256-GCM 加密，Argon2id 密钥派生
- 即使设备丢失，没有双密钥也无法解密

**密码管理**
- 密码分组与标签管理
- 全局搜索、收藏常用条目
- 历史版本记录，误操作可回溯
- 平台图标自动抓取
- 一键复制，剪贴板 30 秒自动清空
- 密码生成器

**WebDAV 多设备同步**
- 连接你自己的 WebDAV 服务器
- 增量同步，仅传输变化部分
- 冲突自动归档，数据不丢失

**开发者工具箱（附赠）**
- JSON 格式化 / JSONPath 查询
- 文本 Diff 对比
- 时间戳转换、单位换算、Base64 编解码
- 纯本地运行，断网可用

## 下载

### macOS

| 文件 | 说明 |
|------|------|
| `Vaultic_aarch64.dmg` | Apple Silicon (M1/M2/M3/M4) |
| `Vaultic_x64.dmg` | Intel |

### Windows

| 文件 | 说明 |
|------|------|
| `Vaultic_x64-setup.exe` | 安装程序 |
| `Vaultic_x64-setup.msi` | MSI 安装包（企业部署） |

### Linux

| 文件 | 说明 |
|------|------|
| `Vaultic_amd64.AppImage` | 通用安装包 |
| `Vaultic_amd64.deb` | Debian / Ubuntu |
| `Vaultic_x86_64.rpm` | Fedora / RHEL |

## macOS 安装说明

首次打开可能提示 **"Vaultic" 已损坏**，这是因为应用未经过 Apple 公证。

**解决方法（任选其一）：**

**方法一：终端命令**
```bash
sudo xattr -rd com.apple.quarantine "/Applications/Vaultic.app"
```

**方法二：系统设置**
1. 打开 **系统设置** → **隐私与安全性**
2. 找到底部安全提示，点击 **"仍要打开"**

此操作只需执行一次，后续更新不受影响。
