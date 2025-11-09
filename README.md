# EFramework XHR for Unite

[![NPM](https://img.shields.io/npm/v/io.eframework.unite.xhr?label=NPM&logo=npm)](https://www.npmjs.com/package/io.eframework.unite.xhr)
[![DeepWiki](https://img.shields.io/badge/DeepWiki-Explore-blue)](https://deepwiki.com/eframework-io/Unite.XHR)
[![Discord](https://img.shields.io/discord/1422114598835851286?label=Discord&logo=discord)](https://discord.gg/XMPx2wXSz3)

基于 PuerTS 的 XMLHttpRequest 标准实现，可运行于 Unity、Unreal 等多个引擎环境中。

## 功能特性

- 🚀 跨平台：可运行于 Unity、Unreal 等多个引擎环境中
- 📦 标准兼容：完整实现 XMLHttpRequest Level 2 标准

### 核心功能

- Unity XMLHttpRequest：基于 UnityWebRequest 的 XMLHttpRequest 标准实现。
- Unreal XMLHttpRequest：基于 Unreal HTTP 的 XMLHttpRequest 标准实现。

### 平台支持

| Runtime/Platform | Windows | Linux | macOS | Android | iOS | Browser |
| :-: | :-: | :-: | :-: | :-: | :-: | :-: |
| Node | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Code | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Cocos | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Unity | ✅ | ✅ | ✅ | ✅ | ✅ | ➖ |
| Unreal | ❓ | ❓ | ❓ | ❓ | ❓ | ➖ |
| Electron | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
| Dom | ➖ | ➖ | ➖ | ➖ | ➖ | ➖ |
- ✅已支持  ❓开发中  ❌未支持  ➖不适用

### 使用示例

```typescript
// Unity 环境
import { XMLHttpRequest } from "io.eframework.unite.xhr/unity"

const xhr = new XMLHttpRequest()
xhr.open("GET", "https://api.example.com/data")
xhr.onload = () => {
    console.log(xhr.response)
}
xhr.send()
```

## 常见问题

更多问题，请查阅[问题反馈](CONTRIBUTING.md#问题反馈)。

### 1. TypeScript 导入报错？
问题：Cannot find module 'io.eframework.unite.xhr/unity'
解决：将 tsconfig.json 的 moduleResolution 修改为 bundler 或 node16

## 项目信息

- [更新记录](CHANGELOG.md)
- [贡献指南](CONTRIBUTING.md)
- [许可协议](LICENSE)
