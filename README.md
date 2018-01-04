# Open Duo iOS for Objective C

*Read this in other languages: [English](README.en.md)*

- **本示例项目中动态密钥的计算在移动设备上执行，为了安全和避免出错，建议正式环境中在自己的业务服务器计算，参考 [动态密钥鉴权](https://docs.agora.io/cn/2.0.2/product/Voice/Product%20Overview/key) **

这个开源示例项目演示了如何快速集成 Agora 视频 SDK 和信令 SDK，实现1对1视频通话。

在这个示例项目中包含了以下功能：

- 登录信令；
- 拨号和呼叫；
- 接听和挂断；
- 静音和解除静音；
- 切换前置摄像头和后置摄像头；

Agora 视频 SDK 和信令 SDK 支持 iOS / Android / Web 等多个平台，你可以查看对应各平台的示例项目：

- [OpenDuo-Android](https://github.com/AgoraIO/OpenDuo-Android)
- [OpenDuo-Web](https://github.com/AgoraIO/OpenDuo-Web)

## 运行示例程序
- 首先在 [Agora.io 注册](https://dashboard.agora.io/cn/signup/) 注册账号，并创建自己的测试项目，获取到 AppID。
- 将 AppID  和 AppCertificate 填写进 KeyCenter.mm。

```
static NSString * const kAppID = @"Your App ID"
static NSString * const kAppCertificate = @"Your App Certificate";
```

然后在 [Agora.io SDK](https://www.agora.io/cn/download/)
- 下载 **视频通话 + 直播 SDK**，解压后将其中的 **libs/AgoraRtcEngineKit.framework** 复制到本项目的 “OpenDuo” 文件夹下。
- 下载 **信令SDK**，解压后将其中的 **libs/AgoraSignalKit.framework** 复制到本项目的 “OpenDuo” 文件夹下。

最后使用 XCode 打开 OpenDuo.xcodeproj，连接 iPhone／iPad 测试设备，设置有效的开发者签名后即可运行。

## 运行环境
* XCode 9.0 +
* iOS 真机设备
* 不支持模拟器

## 联系我们

- 完整的 API 文档见 [文档中心](https://docs.agora.io/cn/)
- 如果在集成中遇到问题，你可以到 [开发者社区](https://dev.agora.io/cn/) 提问
- 如果有售前咨询问题，可以拨打 400 632 6626，或加入官方Q群 12742516 提问
- 如果需要售后技术支持，你可以在 [Agora Dashboard](https://dashboard.agora.io) 提交工单
- 如果发现了示例代码的bug，欢迎提交 [issue](https://github.com/AgoraIO/OpenDuo-iOS-Objective-C/issues)

## 代码许可

The MIT License (MIT).
