# ROG-B460G-10400-UHD630-OPENCORE-BIGSUR
黑苹果oc配置文件分享

## 一、系统截图
![avatar](https://github.com/JhonsonT/ROG-B460G-10400-UHD630-OPENCORE-BIGSUR/blob/main/images/system.png)

## 二、EFI
```text
引导 : opencore(我有时间就会更新)
系统版本 : BigSur(强迫症,逢新beta版必更)
```

## 三、BIOS设置

```text
仅针对当前主板,主板有搜索功能,直接搜英文即可,例如EHCI/XHCI Hand-off,直接搜索hand
```

### 3.1 Disable(禁用)
```text
Fast Boot(快速启动)
Secure Boot(安全启动)
Serial/COM Port(串口)
CSM
Intel SGX
CFG Lock(主板bios中无设置,默认关闭)
```

### 3.2 Enable(启用)
```text
Above 4G decoding(4G解码)
Hyper-Threading(超线程)
EHCI/XHCI Hand-off(接管EHCI/XHCI)
SATA Mode: AHCI(SATA硬盘模式)
```

## 四、注意事项
```text
1. SSDT用的不是通用版本，非相同主板请勿抄作业
2. 我用的是4k60hz的高分屏 + UHD630 dp口输出，如果使用hdmi/dvi接口，请自行打补丁，vga用户"建议"洗洗睡，别折腾了
```

## 五、联系方式
```text
QQ 194500975
注:  咱也不是专业的(能力有限)
    有自己的工作(有时候会很忙,没时间回你信息)
    不是那些某宝某黄鱼上收费给人装黑果的(不会提供售后啥的,想玩黑果就必须得学会自己折腾)
    so 喷子勿扰,伸手党勿扰
```
