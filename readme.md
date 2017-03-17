[TOC]



# 流式图计算

## 项目内容

​    本项目研究的核心问题是流式场景下的图计算问题。希望能够建立流式图计算模型，并且在现有的流计算引擎上得以实现模型，构建系统原型。结合毕业论文要求，主要分为以下两个部分：论文和系统。

+ 论文：论文分为1绪论（4页）、2相关工作（14页）、3计算模型（13页）、4. 算法设计（9页）、5系统设计与实现（10页）、6实验（6页）、7总结（2页）六个部分。 4+14+13+9+10+6+2= 58页

  + 第一章 绪论（4页）


+   第二章 图计算相关工作（14页）

    + 2.1 问题定义[1页]  

    + 2.2 关键技术[7页=1+2+2+2]

    + 2.3 常见系统[5页] 

    + 2.4 存在问题[2/3页] 

    + 2.5 本章小结[1/3页]）

      {绪论和相关工作这一块是最花时间也是最难写的，可以先写一个初版本，后续再修改}

+ 第三章 流式图计算模型 （13页）

    + 3.1 图算法特征分析（5页）
    + 3.2 模型定义（2页）
    + 3.3 状态存储和更新（4页）
    + 3.4 模型应用举例（1页）
    + 3.5 本章小结（1页）

+ 第四章 算法设计（9页）

    + 4.1 DD （1页）
    + 4.2 TC（2页）
    + 4.3 SSSP（3页）
    + 4.4 PR（3页）
    + 4.5 本章小结（0页）

+ 第5章 系统实现（10页）

    + 5.1 系统架构（2页）
    + 5.2 模型实现（4页）
    + 5.3 算法实现（4页）
    + 5.4 本章小结（0页）

+ 系统：第一版在Hazelcast上已经构建完成，但Hazelcast不是标准的流就算系统，后续有3种方案：a. Hazelcast提供了流式计算框架，可以集成进去；2. 将Hazelcast集成进Flink；3. 仅适用Flink原生API。系统实现分为 1.core、2.basic API、3.components、4.library、5.application五个模块。

## 工作计划

|          时间点          |    论文     |          系统           |
| :-------------------: | :-------: | :-------------------: |
| 2017.03.08-2017.03.12 |  完成1-2部分  | 确定3种技术路线中的一种，并且开始搭建项目 |
| 2017.03.13-2017.03.19 |  完成3-5部分  |        实现1-2部分        |
| 2017.03.20-2017.03.26 |  完成6-7部分  |        实现3-4部分        |
| 2017.03.27-2017.03.31 | 论文修缮、PPT等 |        系统维护测试等        |

## 工作进度

### 2017.03.08

+ 论文
  + 13:00-16:30 完成1绪论，2相关工作的2.1-2.2.1，共4页。
+ 系统
  + 16:50-17:30 学习Flink Streaming State。
  + 19:00-20:00 学习Flink Keyed Stream,写demo。
  + 22:00-24:50 系统学习Flink的State接口，撰写Streaming State文档。

### 2017.03.09

+ 论文
  + 15:30-17:30 完成 2相关工作2.2.1-2.2.2
  + 24:00-02:00 完成 2.3部分


### 2017.03.10

+ 论文
  + 13:40-17:30 完成第二章节

### 2017.03.13

+ 论文
  + 14:00-17:30 完成论文3.1部分（共5页）
  + 19:00-20:30 听报告
  + 21:00-22:00 完成论文3.2部分（共2页）
  + 22:30-23:45 完成论文3.3,3.4,3.5部分（共6页）

### 2017.03.14

+ 论文
  + 13:00-17:30 完成论文第四章 流式算法设计 4.1DD,4.2TC,4.3SSSP（共7页）
  + 20:30-21:40 完成论文第四章 4.4 节（共2页） 

### 2017.03.15

+ 论文
  + 13:30-17:00 完成论文第5章 系统实现章节的 5.1 架构实现（2页）5.2 模型实现（4页）
  + 20:00-21:00 完成论文第5章 系统实现章节的5.3算法实现（4页）5.4 本章小结（0页）

### 2017.03.16

+ 论文
  + 13:40-14:30 学习Flink Streaming Iterator => 权衡了下在Flink上做难度大，不确定性因素多，在Hz上完善。
+ 系统
  + 15:00-17:00 设计GraphBenchmark。
  + 23:50-02:00 完成GraphBenchmark.

### 2017.03.17

+ 系统
  + 13:30-14:45 完成MergeDriver工具。
  + 15:00-18:30 完成GraphBenchmark batch 测试脚本，完善MergeDriver和DataDriver，三个工具通过测试，可以使用。
  + 22:40-01:30 HzGraphFlow系统的RESTful模块设计实现完毕，现在可以通过外部服务器访问内存数据。
  + 01:30-02:00 HzGraphFlow系统的测试脚本编写完毕。

## 工作心得

[我没有偷懒=。=](https://github.com/DuanSky22/GraduationThesis/blob/master/notes/insight/Winterfell.md)

