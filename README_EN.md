# WePadBridge

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Android](https://img.shields.io/badge/Android-5.0%2B-green.svg)](https://android.com)
[![Xposed](https://img.shields.io/badge/Xposed-LSPosed-blue.svg)](https://github.com/LSPosed/LSPosed)

[中文文档](README.md) | English

An Xposed module that enables tablet interface and features in WeChat Work mobile app.

## 📱 Features

- **Device Type Spoofing**: Modifies device type detection to tablet
- **Tablet Interface**: Enables tablet-optimized UI layout in WeChat Work
- **Multi-Class Support**: Hooks multiple detection methods for comprehensive coverage
- **Debug Logging**: Built-in logging for troubleshooting
- **Lightweight**: Minimal performance impact

## 🛠️ Requirements

- Rooted Android device (Android 5.0+)
- Xposed Framework (LSPosed recommended)
- WeChat Work app installed

## 📦 Installation

1. Download the latest APK from [Releases](../../releases)
2. Install the APK on your device
3. Activate the module in LSPosed Manager
4. Enable the module scope for WeChat Work
5. Restart WeChat Work

## 🎯 Usage

Once activated, WeChat Work will automatically display the tablet interface with:
- Optimized layout for larger screens
- Tablet-specific UI elements
- Enhanced navigation experience

## 🔧 Technical Details

### Hooked Methods
- `getDeviceTypeFromLocal()` - Device type detection
- `isAndroidPad()` - Tablet mode verification

### Supported Classes
- Application class tablet detection
- WeworkServiceImpl class tablet detection

### Built With
- [YukiHookAPI](https://github.com/HighCapable/YukiHookAPI) - Modern Xposed API
- [KavaRef](https://github.com/HighCapable/KavaRef) - Reflection library
- Kotlin - Primary development language

## 📱 Compatibility

| Android Version | WeChat Work | Status |
|----------------|-------------|--------|
| 5.0 - 6.0      | 4.0.0+     | ✅ Tested |
| 7.0 - 10.0     | 4.0.0+     | ✅ Tested |
| 11.0 - 14.0    | 4.0.0+     | ✅ Tested |

## 🐛 Troubleshooting

### Module Not Working
1. Ensure LSPosed is properly installed
2. Check if the module is activated
3. Verify WeChat Work is in the module scope
4. Restart WeChat Work after activation

### Interface Issues
1. Clear WeChat Work app data
2. Reinstall the module
3. Check logs in LSPosed Manager

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## ⚠️ Disclaimer

This module is for educational and research purposes only. Use at your own risk. The developer is not responsible for any damage or issues caused by using this module.

## 📞 Support

- Create an [Issue](../../issues) for bug reports
- Star ⭐ this repository if you find it useful
- Follow for updates

---

**Note**: This module only works with WeChat Work (Enterprise WeChat), not the regular WeChat app.
