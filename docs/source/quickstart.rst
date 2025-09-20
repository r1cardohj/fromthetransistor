QuickStart
==========


现在社会上招人很难，很多现在计算机科学教育真的很糟糕，很难找到一个从头开始了解现代计算机堆栈的人。

.. note::

   这个页面翻译自George Hotz原仓库中的README部分


intro:在晶体管问题上“作弊”
--------------------------


关于 **Transistors(晶体管)** ，我们需要了解一些概念:


* 我们需要描述如何用晶体管构建 `FPGA <https://zh.wikipedia.org/wiki/%E7%8E%B0%E5%9C%BA%E5%8F%AF%E7%BC%96%E7%A8%8B%E9%80%BB%E8%BE%91%E9%97%A8%E9%98%B5%E5%88%97>`_
* `IC(集成电路) <https://zh.wikipedia.org/wiki/%E9%9B%86%E6%88%90%E7%94%B5%E8%B7%AF>`_ 只是晶体管的集合，他们在一个美丽且可靠的包裹当中
* 了解 `LUT(查找表) <https://en.wikipedia.org/wiki/Lookup_table>`_ 之类的东西


实践性的项目是一个按顺序严格依赖的序列，而这个序列的起点和根基是理论知识本身。在打好理论基础之前，任何实践项目（即使是第一个）都无法真正有效地进行
。因此，当前的首要任务不是急着做项目，而是必须先“谈谈晶体管的理论”。


还有 **Emulation(仿真)** :


在真实的硬件上构建这些东西会限制这个课程的覆盖范围，所以咱们使用 `Verilator <https://verilator.org/guide/latest/>`_ 这种工具让任何人都能在电脑上去玩耍。


Bringup:硬件用什么来编程
--------------------------


这一章节我们将学习使用 Verilog :


* 闪烁 LED (Verilog, 10) -- 这是你第一个小程序！让模拟器运行起来，并且乘机学习 Verilog 。
* 构建 `UART(通用异步收发传输器) <https://zh.wikipedia.org/zh-cn/UART>`_ -- 这是 Verilog 的一个入门章节，复现一个真实的 UART ，
  介绍 `MMIO(内存映射IO) <https://zh.wikipedia.org/wiki/%E5%AD%98%E5%82%A8%E5%99%A8%E6%98%A0%E5%B0%84%E8%BE%93%E5%85%A5%E8%BE%93%E5%87%BA>`_ 的概念，
  尽管串口可能是 semihosting（半主机，串行测试回显程序和LED控制。
