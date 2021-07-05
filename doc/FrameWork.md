# APP启动流程
应用进程不存在的情况下，从点击桌面应用图标，到应用启动（冷启动），大概会经历以下流程：

Launcher startActivity
AMS startActivity
Zygote fork 进程
ActivityThread main()
4.1.  ActivityThread attach
4.2. handleBindApplication
4.3  attachBaseContext
4.4. installContentProviders
4.5. Application onCreate
ActivityThread 进入loop循环
Activity生命周期回调，onCreate、onStart、onResume...

整个启动流程我们能干预的主要是 4.3、4.5 和6，应用启动优化主要从这三个地方入手。理想状况下，这三个地方如果不做任何耗时操作，那么应用启动速度就是最快的，但是现实很骨感，很多开源库接入第一步一般都是在Application onCreate方法初始化，有的甚至直接内置ContentProvider，直接在ContentProvider中初始化框架，不给你优化的机会。