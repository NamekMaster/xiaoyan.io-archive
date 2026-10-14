# 小燕科技（Terncy / 小燕）官网资料存档

[xiaoyan.io](https://www.xiaoyan.io) 官网的完整镜像备份，抓取时间 **2023-12-28**。

## 背景

上海小燕科技有限公司（品牌 Terncy / 小燕）成立于 2015 年，是国内最早通过 Apple HomeKit 认证的智能家居品牌之一，产品线覆盖 ZigBee 网关（家庭中心）、墙壁开关、筒灯/吸顶灯/灯带驱动、窗帘电机、传感器等。

大陆主体已停止运营，官网无法访问，安卓 App 亦无法从常规渠道获取。本仓库保存其公开资料，供仍在使用小燕设备的用户查阅——**重置方法、双模切换（ZigBee ↔ 蓝牙 HomeKit 直连）、固件发布历史、故障排查**等文档如今只存在于这类存档中。

## 仓库内容

| 位置 | 内容 |
|---|---|
| `manuals/` | **68 份官方产品说明书 PDF**（中文/英文，覆盖全产品线：网关 GW01/GW02、墙壁开关 WS 系列、调光器 DIM/ST 系列、筒灯 DL/CL、窗帘电机 CM/RM 系列、传感器、门锁等） |
| Release: `xiaoyan.io_2023-12-28.zip` | 官网整站镜像（886MB，含全部网页、产品页、博客教程、图片视频） |
| Release: `xiaoyan-app-android-latest.apk` | 官网 `/android/latest` 提供的安卓安装包（146MB，抓取于 2023-12-28）。注意：App 真实版本线为 3.0.x（APKPure 末版 3.0.35，2023-07；有用户实机持有更新的 3.0.60 build 823——**如你手机装有更新版本，建议用 APK 提取工具导出存档并联系仓库所有者补充上传**，那可能是全网仅存的末代新版） |

## 值得知道的几件事（写给小燕设备存量用户）

- **灯与开关多为蓝牙/ZigBee 双模**：墙壁开关全系（青鸾/朱雀/白鹭/知更/蓝鹊）、DIM001、ST01、CL001、CM02 窗帘电机等支持切换为蓝牙模式后**直连 Apple HomeKit，完全不需要网关**（切换入口在小燕 App 设备详情页，通过刷入另一版固件实现）。DL001 支持双模；DL002（防眩筒灯）博客仅见 ZigBee 版固件记录。具体以各说明书为准。
- **Zigbee2MQTT 官方支持 16 款小燕设备**（含全部 WS01 系列开关、DL001、CL001、DIM003 等），详见 [zigbee2mqtt.io 支持列表](https://www.zigbee2mqtt.io/supported-devices)（搜 TERNCY）。
- **Home Assistant 集成（仍在维护）**：[rxwen/homeassistant-terncy-component](https://github.com/rxwen/homeassistant-terncy-component)，走家庭中心的本地 TCP 协议，无需云端账号。
- 台湾代理站 [terncy.com.tw](https://www.terncy.com.tw) 截至 2026 年仍在线，含 HA 整合等教程。
- 官方 GitHub：[xiaoyantech](https://github.com/xiaoyantech)。

## 版权

本仓库所有内容版权归**上海小燕科技有限公司**所有，仅作资料存档与非商业参考用途，不用于任何商业目的。若权利方对内容有异议，请提交 Issue 或联系仓库所有者，将及时处理。
