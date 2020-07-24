## OpenWrt for K2P

## 介绍

基于最新的 Lean 的 OpenWrt 源码编译，编译时间为`2020-07-24`。

此为斐讯 K2P 专用固件，只加入了常用功能，比较精简。

**下载地址：https://github.com/hmsjy2017/openwrt-k2p/releases/tag/v19.07.3**

## 关于固件的刷写

`breed`直接刷`squashfs-sysupgrade`

`opboot`先刷`initramfs-kernel`，开机后再从系统里刷`squashfs-sysupgrade`。

注：上面的`squashfs-sysupgrade`是指`openwrt-ramips-mt7621-phicomm_k2p-squashfs-sysupgrade.bin`，`initramfs-kernel`是指`openwrt-ramips-mt7621-phicomm_k2p-initramfs-kernel.bin`。
