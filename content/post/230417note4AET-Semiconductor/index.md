---
title: 常用半导体器件——模电学习笔记 part1
date: 2023-04-17
slug: note4AET-Semiconductor
tags: 
- 模拟电子技术基础
categories:
- note4study
# link_refer:
#   -
#     url: https://book.douban.com/subject/26973602/
#     title: 《模拟电子技术基础（第五版）》- 童诗白
#   -
#     url: https://book.douban.com/subject/31158898/
#     title: 《电子技术基础模拟部分（第六版）》- 康华光
---

> 模电基础薄弱，需要从头学习一遍。借助[费曼学习法](https://zhuanlan.zhihu.com/p/88209825)原理，以输出倒逼输入。
> 若有不正确的地方，欢迎在评论区指出，感激不尽！

## 1 BJT 相关

### **1.1 判断 BJT 引脚的方法**

* 根据所给**两个引脚的电流**判断

&emsp;&emsp;*注：这里一般题设为“已知**放大电路**中管子**两个电极的电流**”，所以默认管子处于放大状态。*

&emsp;&emsp;① 由 Ie=Ic+Ib=(β+1)*Ib，假设 β>>1，则 Ie≈Ic，故电流量微弱侧为 Ib；

&emsp;&emsp;② 根据 Ib 电流流向判断 BJT 类型为 NPN 或 PNP；

&emsp;&emsp;③ 通过题设条件中另一个引脚的电流方向区分集电极 c 与发射极 e。

* 根据所给**三个引脚的直流电位**判断

&emsp;&emsp;*注：这里一般题设为“已知**放大电路**中管子的**直流电位**”，所以默认管子处于放大状态。*

&emsp;&emsp;① 因为管子工作在放大状态，所以发射极 e 与基极 b 的直流电位相近，剩下的就是集电极 c；

&emsp;&emsp;② 若集电极 c 的电位最高，则为 NPN 型管，电位最低的为发射极 e，电位居中的基极 b；否则为 PNP 管，电位最高的为发射极 e，电位居中的为基极 b；

&emsp;&emsp;③ 一般默认硅管的导通电压 Uce 为 0.6\~0.8V，锗管的导通电压 Uce 为 0.1\~0.3V。
