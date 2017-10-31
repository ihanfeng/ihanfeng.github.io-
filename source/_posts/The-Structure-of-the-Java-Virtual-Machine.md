---
title: JAVA虚拟机结构
date: 2017-10-11 21:30:00
tags:
  - JAVA
  - 虚拟机
  - JVM
  - JAVA8
categories:
  - JAVA
---
## class文件格式

class文件是一种8位字节的二进制流文件，各个数据项按顺序紧密的从前向后排列，相邻的项之间没有间隙，使得class文件非常紧凑，体积轻巧，可以被JVM快速加载到内存，并且占据较少的内存空间。JAVA源文件被编译后，每个类或者接口都单独占据1个class文件，并且类中的所有信息都会在class文件中有相应的描述。

class文件中的信息是一项一项排列的，每项数据都有它的固定长度，或占1个字节，或2个字节，或4个字节，或8个字节。数据项的长度分别用u1，u2，u4，u8表。

详细介绍:(后面补充)

## 数据类型

Java虚拟机可以操作的数据类型分为2类，原始类型和引用类型。也存在原始值和引用值，用于变量赋值，参数传递，方法方法和运算操作。

JAVA虚拟机希望尽可能多的类型检查在程序运行前完成，即编译器在编译期间就要尽最大努力完成可能的类型检查，使虚拟机在运行期间无需这些操作。

### 原始类型：primitive type

数值类型

  * 整型类型
    * byte类型： 值为8位有符号二进制补码整数，默认值0，取值范围 -128 ~ 127
    * short类型：值为16位有符号二进制补码整数，默认值0，取值范围 -32768 ~ 32767
    * int类型：  值为32位有符号二进制补码整数，默认值0，取值范围 -2147483648 ~ 2147483647
    * long类型： 值为64位有符号二进制补码整数，默认值0，取值范围 -9223372036854775808 ~ 9223372036854775808
    * char类型： 值为用16位无符号整数表示，，取值范围 0 ~ 65535

  * 浮点类型
    * float类型； 值为单精度浮点数集合中的元素，默认值为正数0.
    * double类型：值为双精度浮点数集合中的元素，默认值为正数0.

布尔类型

值为true和false，默认值false。

returnAddress类型

### 引用类型：reference type


## 运行时数据区

## 栈帧

## 对象的表示

## 浮点算法

## 特殊方法

## 异常

## 字节码指令集简介

## 类库

## 共有设计、私有实现