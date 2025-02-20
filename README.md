#  android_samsung_a12_kernel
The Samsung A12s (codename _"a12s"_) have following parameters:

Basic                   | Spec Sheet
-----------------------:|:-------------------------
Chipset					| Exynos 850 (8nm)
CPU                     | Octa-core (4x2.0 GHz Cortex-A53 & 4x2.0GHz Cortex-A53)
GPU                     | Mali-G52
Shipped OS				| Android 11
Memory                  | 32GB 2GB RAM or 32GB 3GB RAM or 64GB 4GB RAM or 128GB 3GB RAM or 128GB 4GB RAM or 128GB 6GB RAM, eMMC 5.1
MicroSD                 | microSDXC (dedicated slot)
Network                 | GSM / HSPA / LTE
Video                   | 1080p@30fps
USB                     | USB Type-C 2.0
Battery 				| Li-Po 5000 mAh, non-removable
Power                   | 15W


<img src="device.png" alt="Samsung A12" style="height: 500px; width:500px;"/>

# Build
1. clone repo
```
git clone https://github.com/foxiyofox/kernel-a12s-modded.git
```
2. clone toolchain
```
git clone https://github.com/theshoqanebi/aarch64-linux-android-4.9.git android_samsung_a12_kernel/toolchain/gcc/linux-x86/aarch64/aarch64-linux-android-4.9
git clone https://github.com/theshoqanebi/clang-r353983c.git android_samsung_a12_kernel/toolchain/clang/host/linux-x86/clang-r353983c
```
3. build kernel (output path = `out/arch/arm64/boot/Image`)
```
bash build_kernel.sh
```
