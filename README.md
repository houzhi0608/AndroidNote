计算机网络

    http/https
    tcp/upd/ip

计算机组成原理

    cpu相关
        MESI/伪共享/缓存行

操作系统

    进程、线程
    内存
    I/O

设计模式

    创建
    结构
    行为

数据结构&算法

    排序、查找
    数组、链表
    栈、队列
    树、图
    贪心、分治、动态规划
    HashMap、SparseArray、ArrayMap、LinkedHashMap、ConcurrentHashMap、CopyOnWriteArrayList、LRU、红黑树

C语言

    指针、函数指针
    静动态开辟内存
    结构体

C++

JNI

Linux

NDK

Java

    OOP/AOP
    反射、泛型、注解
    JVM
    class结构、字节码指令（操作码+操作数）
    类加载机制 Bootstrap->Extension->Application
    执行子系统 解释执行、JIT、AOT（ART）
    JMM 
        运行时数据区、栈帧（操作数栈、局部变量表、动态链接、方法返回）
        内存屏障
        有序性----虚拟机级别内存屏障（loadBarrier、storeBarrier）不一定通过CPU级别内存屏障（lFence、sFence、mFence）实现 也可以通过lock指令（full barrier）
        as-serial、happens-before原则
    GC 可达性分析、finalize(两次标记)、回收算法(标清、复制、标整/压)、回收器（六+G1+ZGC）
    JVM参数 标准- 非标准 -X 不稳定 -XX
    对象分配过程 栈上分配（逃逸分析、标量替换）->TLAB(thread local alloc buffer)->HEAP
    并发
        原子性、可见性、有序性
        Thread/Runnable/Callable/Future/FutureTask
        线程池 （Executor ExecutorService AbstractExecutor ThreadPoolExecutor）、阻塞队列
        wait、notify、notifyAll、sleep、join、interrupt
        synchronized（1.6之后优化）/volatile
        对象内存布局  对象头（MarkWord，类型指针）、实例数据、padding
        CAS（耗CPU、ABA、只能用于一个共享变量）、AQS、Unsafe
        Queue、Lock、Atomic
        ThreadLocal、强/软/弱/虚引用    

Kotlin
    
    语法糖
    泛型
    协程
    
JS
    
    函数一等公民

ReactNative
    
    Redux
    性能问题
    代码规范

Flutter
    
    Dart

KMM

gradle

    生命周期
    语法
    transform

android
    
    View体系
    Compose
    NestedScrollView、RecyclerView、ViewPager、Fragment
    动画
    四大组件
    webview
    bitmap、drawable
    IO/Nio/Okio
    framework（AMS/PMS/WPS/Input）
    binder、mmap

    插件化、组件化、热修复
    AspectJ、ASM
    dex结构、apk加固
    构建打包流程
    gradle插件
    dalvik/art虚拟机

    jetpack组件
    MVVM/MVI
    DI:Hilt、Dagger2

    性能优化：内存、启动、卡顿、IO、电量、包体、ANR、Crash方案、屏幕适配
    APM平台

    开源库：okhttp、retrofit、rxjava、eventbus、glide
    LeakCanary、BlockCanary、Matrix、Booster、MMKV

    
