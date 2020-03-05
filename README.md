# Thinkpad T450s Catalina
## 简介 Introduction
- 这是一个完整的Thinkpad T450s macOS Catalina配置 （基于 @jsassu20 的T450配置）
- This is a complete Thinkpad T450s macOS Catalina configuration (T450 configuration based on @ jsassu20)
- 由于T450s只有一条内存插槽（使用8GB以上内存时板载内存识别不正常）您需要注入内存信息
- Since the T450s has only one memory slot (the onboard memory is not recognized properly when using more than 8GB of memory) 
  you need to inject memory information
- 使用DW1820A时只需将驱动复制到kext 安装系统时无需在BIOS中禁用WIFI
- When using DW1820A, you only need to copy the driver to kext. You do not need to disable WIFI in the BIOS when installing     the system.
- 音频问题请执行alc_fix脚本 或者把CodecCommander.kext复制到 L / E 目录重建缓存修复权限
-Audio issue, please execute alc_fix script or copy CodecCommander.kext to L / E directory to rebuild cache repair permissions

## 硬件信息 Device Information

```  
- Intel Core i7-5600U 2.6GHz (Boots 3.2GHz)or Intel Core i5-5300U

- Intel HD 5500 Graphics 

- 声卡：ALC292 or HD Audio, Realtek ALC3232 codec

- 无线网卡：DW1820A CN-08PKF4 CN-0VW3T3 CN-00JT494（感谢 @Axelpop ）
```

## BIOS (1.37)
-  Security -> Security Chip`: **Disabled**;
-  Memory Protection -> Execution Prevention`: **Enabled**;
-  Virtualization -> Intel Virtualization Technology`: **Enabled**;
-  Internal Device Access -> Bottom Cover Tamper Detection`: must be **Disabled**;
-  Anti-Theft -> Current Setting`: **Disabled**;
-  Anti-Theft -> Computrace -> Current Setting`: **Disabled**;
-  Secure Boot -> Secure Boot`: **Disabled**;
-  UEFI/Legacy Boot`: **UEFI Only**;
-  CSM Support`: **Yes**.

## 有效 Work

- 睡眠/唤醒 Sleep / Wake
- Wifi
- 蓝牙 Bluetooth
- Handoff, Continuity, AirDrop 
- iMessage, FaceTime, App Store, iTunes Store
- 以太网卡 Ethernet card
- 板载音频 (使用alc_fix或CodecCommander.kext修复音频问题) Onboard audio (use alc_fix or CodecCommander.kext to fix audio issues)
- USB
- 电池 Battery
- 触摸屏 (10.14) Touch screen (10.14)
- 触摸板 Touchpad
- 小红点 Red dot
- miniDP
- SD卡读卡器 SD card reader

## 无效 Not work

- VGA
- 触摸屏 (10.15) Touch screen (10.15)
