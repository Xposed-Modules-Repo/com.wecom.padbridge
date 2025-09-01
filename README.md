# 手机企业微信平板登录/WePadBridge

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Android](https://img.shields.io/badge/Android-5.0%2B-green.svg)](https://android.com)
[![Xposed](https://img.shields.io/badge/Xposed-LSPosed-blue.svg)](https://github.com/LSPosed/LSPosed)

中文文档 | [English](README_EN.md)

一个让企业微信手机版伪装成平板进行扫码登录的 Xposed 模块。新增对企业微信 5.0+ 版本的支持。

## 📱 功能特性

- **设备类型伪装**: 修改设备类型检测为平板设备
- **平板界面**: 启用企业微信的平板优化UI布局
- **多类支持**: Hook多个检测方法，确保全面覆盖
- **调试日志**: 内置日志功能，便于问题排查
- **轻量级**: 对性能影响极小

## 🛠️ 使用要求

- 已Root的Android设备 (Android 5.0+)
- Xposed框架 (推荐使用LSPosed)
- 已安装企业微信应用

## 📦 安装方法

1. 从 [Releases](../../releases) 下载最新APK文件
2. 在设备上安装APK
3. 在LSPosed管理器中激活模块
4. 为企业微信启用模块作用域
5. 重启企业微信

## 🎯 使用说明

激活后，企业微信将自动显示平板登录界面，可以使用另外一个企业微信扫码登录。

## 🔧 技术细节

### Hook的方法
- `getDeviceTypeFromLocal()` - 设备类型检测
- `isAndroidPad()` - 平板模式验证

### 支持的类
- Application类平板检测
- WeworkServiceImpl类平板检测

### 技术栈
- [YukiHookAPI](https://github.com/HighCapable/YukiHookAPI) - 现代化Xposed API
- [KavaRef](https://github.com/HighCapable/KavaRef) - 反射库
- Kotlin - 主要开发语言

## 📱 兼容性

| Android版本 | 企业微信版本 | 状态 |
|------------|------------|------|
| 7.0 - 10.0 | 4.0.0 - 5.0.0+     | ✅ 已测试 |
| 11.0 - 14.0| 4.0.0 - 5.0.0+     | ✅ 已测试 |

## 🐛 问题排查

### 模块不生效
1. 确保LSPosed正确安装
2. 检查模块是否已激活
3. 验证企业微信是否在模块作用域内
4. 激活后重启企业微信

### 界面问题
1. 清除企业微信应用数据
2. 重新安装模块
3. 在LSPosed管理器中查看日志

## 📄 开源协议

本项目采用 MIT 协议 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🤝 贡献代码

欢迎贡献代码！请随时提交 Pull Request。

## ⚠️ 免责声明

本模块仅供教育和研究目的使用，使用风险自负。开发者不对使用本模块造成的任何损害或问题负责。

## 📞 支持

- 创建 [Issue](../../issues) 报告bug
- 如果觉得有用请给个 ⭐ Star
- 关注获取更新

---


**注意**: 本模块仅适用于企业微信，不支持个人微信。



