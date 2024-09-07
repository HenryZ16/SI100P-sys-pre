---
marp: true
math: mathjax
paginate: true
style: |
  section::after {
    content: attr(data-marpit-pagination) '/' attr(data-marpit-pagination-total);
  }

---

# SI100+ 系统方向介绍
  by 张涵锐
  powered by Marp

---

# 我是谁？

<center>

<div style="display:flex">
  <div style="width:50%">
    <a align="center">
      <img src="img/生活照.jpg", height=500><br>
      <b>张涵锐</b><br>
      <font size=6> zhanghr2022@shanghaitech.edu.cn </font><br>
    </a>
</div>
  <div style="width:50%">
    <br>
      2022 级 CS 专业本科生
    </br>
    <br>
      曾担任 CS100 助教
    </br>
    <br>
      现任 Geekpie_HPC 超算队队长
    </br>
    <br>
      HPC 比赛教程主编之一：github.com/Ayanokoji-li/HPC-tutorial
    </br>
    <br>
      QQ: 1546169856
    </br>
    <br>
      常驻信院 1B205
    </br>
</div>
</div>

</center>

---

# 系统……操作系统！
<center>

<div style="display:flex">
  <div style="width:33%">
    <img src="img/windows11.jpg", height=300><br>
  </div>
  <div style="width:33%">
    <img src="img/linux.png", height=300><br>
  </div>
  <div style="width:33%">
    <img src="img/macos.jpg", height=300><br>
  </div>
</div>

</center>

### 这只是系统方向的冰山一角

---

# 计算机系统

> 现代计算机的组成要素

主要内容：
- 体系结构
- 操作系统
- 编译原理
- 计算机网络
- 高性能计算
- 嵌入式开发
- ……

---

# 体系结构 - 冯 · 诺依曼架构

> 从第一个计算尺的出现……到蒸汽时代的差分机……再到真空管电路第一次接通，你已经历许多。现在，开启你最伟大的探索吧：从早期计算机的摇篮到浩瀚星宇。

- 万物的源头，一切的开始！没有体系结构的研究，就没有计算机的迭代更新
- 万变不离其宗：沿用至今的冯 · 诺依曼架构（5个部分）
  - 控制单元：负责指示计算和其他任务
  - 处理器单元：负责执行计算任务
  - 内存：负责短期存储
  - 外存：负责长期存储
  - 输入 / 输出设备：负责跟你沟通

---

# 体系结构 - 硬件

- 能归类到以上5个部分的东西都是硬件：
  > 鼠标、键盘、显示器、音响：输入 / 输出设备
  > 机械硬盘、固态硬盘：外存
  > 内存条：内存
  > Intel CPU, AMD CPU：控制单元，处理器单元
  > 显卡：处理器单元
- 如何操控这些硬件？指令！

---

# 体系结构 - 指令

> 要让计算机工作，我们必须要念奇妙的咒语：
> 001, 110, 0011110

- 计算机只认识0和1，于是最早的指令的形式是一串0和1
- 你也不想在~~施法~~编写指令的时候查阅一大串容易混淆的01串吧？
- 于是我们有了汇编：不同指令的简写
  - 例如：000 -> add

---

# 体系结构 - 汇编

- 指令操控硬件，汇编简写指令
- 按照特定规则排布的汇编代码，构成了程序，也就是软件
- 因此，汇编沟通了计算机的软件与硬件

---

# 体系结构 - 指令集

- 硬件设计各有不同，操控不同硬件的指令也可能不同
- 由特定处理器执行的一套基本指令，称为指令集
- 由于一套指令集通常对应一种特定的处理器，所以也称指令集架构（ISA）
- 常见的：x86_64, arm64, RISC-V

---

# 体系结构 - 拓展

- 体系结构一方面研究硬件架构，另一方面也研究汇编代码的运行逻辑
- 想要探索更多？steam搜索Turing Complete
- 学了这个能做什么？
  - 反汇编：将exe等可执行文件翻译成汇编代码，研究执行逻辑
  - 架构设计：设计出更高效的硬件架构，并推出独特的指令集
  - 系统方向的研究几乎都需要体系结构的前置知识！

---

# 操作系统

- 汇编代码当然可以直接在硬件上运行