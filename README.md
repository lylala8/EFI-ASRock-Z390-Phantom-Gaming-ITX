# Mini ITX 4k 视频剪辑黑苹果 macOS 13 Ventura EFI

Geekbench 5 [CPU 测试报告](https://browser.geekbench.com/v5/cpu/12662933) | [OpenCL 独显测试报告](https://browser.geekbench.com/v5/compute/5789051)

## 装机清单

| 名称 | 品牌型号 | 备注 |
| --- | --- | --- |
| CPU | 英特尔 i7 8700 |  |
| 主板 | 华擎 Z390 Phantom Gaming itx/ac |  |
| 散热器 | 利民axp90-47 |   |
| 内存 | 海盗船 Vengeance LPX DDR4 3000 16G x 2 |  |
| 硬盘 | 三星 970evo 500g<br /> 东芝机械 2T |  |
| 显卡 | AMD 6900xt | 非矿 |
| 无线网卡/蓝牙 | 博通 BCM94360CS2 | 需转接卡[替换主板原有模块 M.2 Key E 口](https://icyleaf.com/uploads/2019/03/28/install-boardcom-module-to-motherboard.jpg) |
| 显示器 | LG 27UL600 4k HDR400 IPS<br>LG LM270WR5-SSB1 27 4k 背板 DIY 显示器<br>NV140QUM-N61 背板 15.6 4k 便携显示器 | (Mini)DisplayPort 接入 |
| 机箱 | 机甲A4 ITX |  |
| 电源 | 银欣sfx600 |  |

## 兼容情况

从 2021 年 3 月 25 开始升级使用 OpenCore 方案。

### 完美

- [x] BIOS 版本
    - [x] 4.40
    - [x] 1.5
- [x] macOS 版本
    - [x] [13.0.1](https://github.com/icyleaf/EFI-ASRock-Z390-Phantom-Gaming-ITX/issues/65) - OpenCore
- [x] 显卡
    - [x] 单/[双](https://github.com/icyleaf/EFI-ASRock-Z390-Phantom-Gaming-ITX/issues/36)/[三](https://github.com/icyleaf/EFI-ASRock-Z390-Phantom-Gaming-ITX/issues/65#issuecomment-1321711241) 4k 显示器（DisplayPort）
    - [x] [AMD RX5600XT](https://github.com/icyleaf/EFI-ASRock-Z390-Phantom-Gaming-ITX/issues/66)
    - [x] [AMD RX580](https://github.com/icyleaf/EFI-ASRock-Z390-Phantom-Gaming-ITX/issues/67) - macOS Monterey 12
- [x] 声卡(Realtek ALC1220)
    - [x] 主板后置
    - [x] 机箱前置
    - [x] DisplayPort 声音输出
- [x] 睡眠/唤醒
- [x] 有线网卡
- [x] 无线 WiFi
- [x] 蓝牙
    - [x] Handoff
    - [x] Airdrop
- [x] 所有 USB 插口
    - [ ] 前置 USB 外接麦克风无法识别

### 未知

- Intel UHD630 核显 (使用独显后没测试)

## 安装教程

### 前期准备

开机 F2 进入 BIOS 再按 F6 切换高级模式，至少需要做如下修改具体情况还需要看硬件情况：

- 高级（Advanced） > 芯片配置（Chipset Configuration） > VT-d -> Disabled
- 高级（Advanced） > USB 配置（USB Configuration） > XHCI Hand-off -> Enabled


## 教科书版黑苹果教程

- https://www.tonymacx86.com/threads/guide-asrock-z390-phantom-gaming-itx-ac-i9-9900k-rx-580.268992/
- https://www.tonymacx86.com/threads/success-asrock-z390-phantom-gaming-itx-tb3-igpu-mojave-sff-build.277418/
- https://www.tonymacx86.com/threads/success-gigabyte-designare-z390-thunderbolt-3-i7-9700k-amd-rx-580.267551/
- https://apple.sqlsec.com/
