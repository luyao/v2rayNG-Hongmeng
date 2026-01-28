# v2rayH (HarmonyOS Next v2ray Client)

### 🚀 项目愿景
为 HarmonyOS NEXT (纯血鸿蒙) 提供原生、高效、安全的网络隧道工具。

### 🛠️ 技术栈
- **UI:** ArkUI (ArkTS)
- **Core:** Xray-core (Go via NAPI)
- **Network:** Network Extension Kit (Packet Tunnel Provider)

### 📈 开发计划 (Roadmap)
- [ ] UI 框架搭建 (Current)
- [ ] Xray-core 交叉编译 (ohos-arm64)
- [ ] NAPI 接口封装 (TS <=> C++)
- [ ] 申请 Network Extension 特许权限
- [ ] 订阅解析与节点管理

### 项目结构

```
/v2rayH
  ├── entry/               # 你的 ArkUI 主工程 (ArkTS)
  ├── library/             # 逻辑模块 (HAR/HSP)
  ├── native/              # 这是大工程的核心！
  │    ├── cpp/            # NAPI 桥接代码 (C++)
  │    └── xray/           # 存放编译好的 Xray-core (.so 文件)
  ├── scripts/             # 存放利用 setup-ohos-sdk 逻辑编写的编译脚本
  └── README.md
```
