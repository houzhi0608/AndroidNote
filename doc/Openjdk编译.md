环境配置
> brew install ccache  //加速编译
> 
> brew install freetype //字体引擎，编译过程中会被依赖到
> 
> brew install autoconf

编译
> bash configure --with-debug-level=slowdebug --with-jvm-variants=server --enable-ccache --with-freetype=bundled  --with-boot-jdk=/Library/Java/JavaVirtualMachines/adoptopenjdk-16.jdk/Contents/Home --disable-warnings-as-errors
> 
> make images 2>&1 | tee make_mac_x64.log

清除
> make clean
> 
> make print-configuration > current-configuration 
> 
> make dist-clean 
> 
> bash configure $(cat current-configuration)

验证
> cd /Users/houzhi/openjdk/openjdk-16/build/macosx-x86_64-server-slowdebug/jdk/bin
> 
> java -version
