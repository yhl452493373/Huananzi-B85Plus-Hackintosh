# 华南B85 PLUS + RX 580 macOS Tahoe 黑苹果

## 硬件
+ 主板：华南B85 PLUS
+ CPU：E3-1271 v3
+ 显卡：RX 580 4G （怀疑是480刷的BIOS，不过能正常用）
+ 内存：DDR3 16G
+ 有线网卡：RTL 8111
+ 无线网卡：Intel AX200
  + 由于主板的9针USB接口不够，因此加了个`主板USB2.0 9PIN转双9PIN接口9针转双9针一分二扩展HUB集线器`
+ 声卡：ALC 887

## 黑苹果情况

+ macOS 26 Tahoe （其他未测试）
+ 有线网卡正常
+ 无线网卡正常
+ 蓝牙正常
+ 定位正常
+ 独显正常
+ 声卡正常（后置粉色插口没反应，不知道是不是我主板坏了，Windows也没法用）

## 主板设置

+ Advanced -> CPU Configuration -> CFG Lock : Disabled
+ Advanced -> CSM Configuration -> CSM Support ：Disabled
+ Advanced -> USB Configuration
  + Legacy USB Support : Enabled
  + XHCI Hand-off : Enabled
  + EHCI Hand-off : Enabled
+ Chipset
  + DVMT Pre-Allocated : 128M
  + DVMT Total Gfx Mem : Max
  + VT-d : Enabled

## COLP补丁说明
 
请参考 https://bbs.pcbeta.com/viewthread-2058963-1-1.html ，最好先下KDK