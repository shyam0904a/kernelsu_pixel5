# KernelSU on redbull  
Base on [Building Kernels](https://source.android.com/docs/setup/build/building-kernels) and [KernelSU](https://github.com/tiann/KernelSU)  
Support Pixel 5 (redfin)  
It should also support Pixel 5a (barbet) and Pixel 4a (5G) (bramble) because they are using the same kernel. You only need to replace boot.img and ramdisk.cpio. I dont have these devices so i cannot test it.  
I will provide the boot.img but i cannot make sure it can run.  
You can download it from release and then flash it.  
Or you can build it yourself by following the workflow file.  
## Something may important  
exec.c open.c read_write.c stat.c are from kernel source and modded to work with ksu(because kprobe seems doesnt work)  
magiskboot is from [topjohnwu](https://github.com/topjohnwu)/[Magisk](https://github.com/topjohnwu/Magisk) [Releases](https://github.com/topjohnwu/Magisk/releases)v25.2  
boot.img and ramdisk.cpio is from "redfin" for Pixel 5 [Factory Images for Nexus and Pixel Devices](https://developers.google.com/android/images) and use magiskboot to extract ramdisk.cpio  
ksu.c is from KernelSU and remove kprobe check  
