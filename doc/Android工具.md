# SDK工具
> TraceView性能损耗太大，得到的结果不真实。 Systrace 可以方便追踪关键系统调用的耗时情况
> 
> http://gityuan.com/2016/01/17/systrace/


# Dex相关

- 4.1.dx 和 dexdump工具
> 在sdk目录：~/Android/Sdk/build-tools/ 下有dex 打包工具:dx
> 解析dex的工具：dexdump;
> 源码目录下prebuilts下也有该工具;
> 手机中也有该工具： system/bin/dexdump

- 4.2. oatdump工具
> 在手机中有该工具： /system/bin/oatdump，可以解析oat文件。

- 4.3.objdump工具
> 对于android开发是源码下对应的arm-linux-androideabi-objdump而非电脑系统的objdump：
> ./prebuilts/gcc/linux-x86/arm/arm-linux-androideabi-4.9/bin/arm-linux-androideabi-objdump -S ~/Documents/f3b/symbol/out/target/product/pyxis/symbols/vendor/lib/hw/camera.qcom.so | tee camera.qcom.asm
用来反编译symbol文件为汇编指令用于问题定位。

- 4.4. Vdex Extractor工具
> Vdex Extractor：从Vdex文件反编译和提取Android Dex字节码的工具：[https://www.freebuf.com/sectool/185881.html]