# 单线程

JS执行引擎、浏览器渲染引擎

同步任务 JS执行引擎执行的代码

异步任务 耗时过长 浏览器开启线程处理

宏队列 事件监听，setTimeout，setInterval
微队列 Promise（async、await）


0 -> 任务 -> 微队列遍历执行 -> 1 宏队列遍历执行（上一事件流程）

# Promise

