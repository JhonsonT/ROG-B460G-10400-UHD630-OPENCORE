# ROG-B460G-10400-UHD630-OPENCORE
黑苹果oc配置文件分享

## EFI
```text
引导 : opencore(我有时间就会更新)
系统版本 : MacOS13 Ventura(我有时间就会更新)
```

## BIOS设置

```text
仅针对当前主板,主板有搜索功能,直接搜英文即可,例如EHCI/XHCI Hand-off,直接搜索hand
```

### 1. Disable(禁用)
```text
Fast Boot(快速启动)
Secure Boot(安全启动)
Serial/COM Port(串口)
CSM
Intel SGX
CFG Lock(主板bios中无设置,默认关闭)
```

### 2. Enable(启用)
```text
Above 4G decoding(4G解码)
Hyper-Threading(超线程)
EHCI/XHCI Hand-off(接管EHCI/XHCI)
SATA Mode: AHCI(SATA硬盘模式)
```

## 注意事项

1. 非相同主板请勿抄作业
2. 纯核显EFI是UHD630核显 dp口输出4k60hz + HDMI口输出4k30hz(板子限制只能30hz)，如果使用dvi接口，请自行修改，vga用户"建议"洗洗睡吧
3. 独显EFI是UHD630加速,6650xt独显输出（理论上6650xt和6950xt都可以用）
4. 使用免驱博通无线网卡94360cd , 使用其他网卡请自行添加网卡驱动,eg: [intel无线网卡驱动链接](https://openintelwireless.github.io/itlwm/)
5. efi内放入的是通用usb驱动，11.2及以下系统可以直接使用，升级系统前请自行定制usb驱动后再升级
6. 请使用与当前oc版本相同的Opencore configuration进行修改配置，否则造成的文件结构错误会让你明白什么叫做残忍，当然你也可以使用其他工具: xcode，[ProperTree](https://github.com/corpnewt/ProperTree)，推荐[OCAT](https://github.com/ic005k/QtOpenCoreConfig)
7. 关于HEVC硬件，BIGSUR(即macos 11)之后版本系统,见下图
![avatar](https://github.com/JhonsonT/ROG-B460G-10400-UHD630-OPENCORE/blob/main/images/HEVC.jpg)
8. 纯核显可选择机型有Macmini8,1 和 iMac19,1 和 iMac20,1 ，建议使用iMac19,1，其他两个机型有T2锁
