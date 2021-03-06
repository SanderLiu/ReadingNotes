# 《鸟哥的Linux私房菜》读书笔记

> 我为什么要读这本书？
>
> 第一次听Linux的时候，那还是我在大一的时候，当时有个老师给我们推荐Linux，推荐我们学习并使用Linux，并给我们说了各种学习Linux的好处。我是在大学二年级买了自己的第一台电脑，那时还是Windows盛行的时代，当时我自己不愿意舍弃自己笔记本上面的Windows系统，因为当时太习惯Windows了。因为当时笔记本性能的局限和安装虚拟机的麻烦，也不愿意在自己电脑上安装虚拟机。安装双系统也是一件麻烦的事情，还有风险会丢掉自己本有的Windows系统，也放弃了。
>
> 后面也尝试过Linux系统几次，但对于一个习惯了Windows的人，Linux确实是难用的。
>
> 工作之后，在Windows上工作的很少，更多的用到的是Linux，开发、编译、运行、测试都要在Linux系统上进行，在这个过程中发现因为自己不会Linux而导致了工作上不方便。并且当前主流的开源软件也都是基于Linux系统开发的，想要学习开源项目，也需要会Linux。基于这一切，我决定好好学习Linux，而《鸟哥的Linux私房菜》是一本非常经典的Linux入门书籍，因此我选中了这本书来作为自己学习Linux系统的第一本书。

[TOC]



## 第0章 计算机概论

> 在学习Linux之前，首先要对计算机有一个大致的了解，本章主要对计算机做了一个简单的介绍

### 0.1 计算机：辅助人脑的好工具

计算机：接收用户输入指令与数据，经过中央处理器的数据与逻辑单元运算处理后，以产生或存储成有用的信息。

> 从上面的概念可以看出来，计算机对信息的处理有以下三个步骤：
>
> 1. 接收信息：计算机通过输入设备来获取用户想要处理的信息，是信息的入口
> 2. 处理信息：计算机按照用户的要求对输入的信息进行处理，诸如，求和、排版等活动
> 3. 输出信息：计算机通过输出设备将处理完的信息呈现给用户，诸如，显示器、音响、打印机等设备

#### 0.1.1 计算机硬件的五大单元

计算机硬件由以下几个单元组成：输入单元、输出单元、CPU内部的控制单元、算术逻辑单元与内存

> 输入输出单元是分别接收信息和输出信息的。
>
> 这里需要重点理解一下CPU内部的控制单元、算术逻辑单元与内存：
>
> 控制单元：顾名思义，就是执行控制动作的单元，这个单元执行计算机中所有的控制动作，诸如将从输入单元输入的数据写入存储中，从存储单元中将数据输出给算术逻辑单元进行运算等。控制单元的主要作用是协调各组件与各单元间的工作。
>
> 算术逻辑单元：主要负责程序运算与逻辑判断。运算包括加减乘除等运算，逻辑判断包括与或非异或运算。
>
> 内存：书中的原话写的是内存，但我理解这里可能更好的用词应该是存储单元，计算机有存储体系，内存只是存储体系中的一个，计算机中的所有数据都会存放在存储单元的中。

#### 0.1.2 CPU的种类

根据CPU所使用的指令集的不同，CPU可分为精简指令集（RISC）和复杂指令集（RISC）

