练习 demo

# NodeJS 一个调试技巧

node --inspect -brk dir

# NodeJS 是什么

构建在 Chorme V8 引擎上的 JS 语言的运行时（runtime）。

# NodeJS 两大特性：

非阻塞（异步） I/O
事件驱动

# I O 密集（在处理高并发、I/O 密集场景性能优势明显）

存取设备、网络设施的读取操作
文件操作|网络操作|数据库

# CPU 密集

一个程序大部分事件是做计算，逻辑判断
压缩|解压|加密|解密

# 进程

计算机中的程序关于某数据集合上的一次运行活动，是系统进行资源分配和调度的基本单位。

# 多进程

启动多个进程，多个进程可以一块执行多个任务。

# 线程

进程内一个相对独立的、可调度的执行单元，与同属一个进程的线程共享的资源。

# 多线程

启动一个进程，在一个进程内启动多个线程，这样，多个线程也可以执行多个任务。

# NodeJS 的单线程

一个 CPU 上只开一个进程，一个进程也只开一个线程（原理）。

# NodeJS 模型

主进程发起一个请求，交给 I/O 之后，他只负责接收，至于怎么处理由操作系统底层去实现。
