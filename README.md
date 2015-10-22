<img src=./doc/images/redhat.png style="width: 300px;"/>

RHEL OSP Director 入门培训
==================================

注意：只用于内部培训,文档中的内容非官方正试支持,仅供参考。

## 简介

首先，欢迎来到 **OSP Director** 培训课程。它的时间是我们的荣幸，欢迎您的光临
，希望它将实用。本课程旨在让你与我们新的 OpenStack 部署工具，使您自信地与客户交>谈有关的功能，并能够部署和疑难解答 OpenStack Director的相关问题。

课程设计适用教练带领和自学，您可以自定进度阅读本文，参加基于课堂课程时，你将会参
与主题幻灯演示的分组讨论，你也可以与经验丰富的工程师和架构师进行交流。如果您有任
何疑问，请不要犹豫，问问他们。


你需要以下准备条件以便您能进行此培训

1. 40GB 以上内存、 8 核的服务器。
   或
   3台16GB内存、4核的笔记本脑（笔记本需要有 **两个网卡**，可以是RHEL支持USB网卡）。
2. 有效的OSP红帽订阅
   或
   提前提供一套机器给老师，以便为您准备安装源。

## 课程安排

我们有一个严格的课程，我们需要遵循你就读的讲师指导的培训，下面是课程日程:

### 第一天

时间          | 内容
------------- | -----------------
**1030-1100** | 欢迎, 介绍和组织
**1100-1230** | [现有的OpenStack安装机制的总结分析 (好处与制约)] (./doc/existing-tools.md)
**1230-1330** | 午餐
**1300-1500** | 介绍 [Director工具] (./doc/contents.md); 组成, [特性] (./doc/contents.md), 集成
**1500-1520** | 中间休息 
**1520-1700** | 继续介绍 [Director工具] (./doc/contents.md)

### 第二天

时间          | 内容
------------- | -----------------
**0900-1045** | 动手操作及硬件安装的介绍
**1045-1100** | 中间休息
**1100-1230** | **实验一**: [安装的种子主机] (./doc/lab01.md)
              | **实验二**: Undercloud 的配置
**1230-1330** | 午餐
**1330-1530** | **实验三**: 安装并测试Undercloud
              | **实验四**: 创建和配置的基本节点镜像
**1530-1550** | 中间休息
**1550-1730** | **实验五**: 注册/发现 Overcloud 节点
              | **实验六**: 部署 Overcloud

### 第三天

时间          | 内容
------------- | -----------------
**0900-1045** | **实验七**: Overcloud 的测试部署
              | **实验八**: 拆解现有的环境和重新安装
**1045-1100** | 中间休息
**1100-1230** | **实验九**: 高级的配置和部署的新 Overcloud
              | - 味道匹配
              | - 自定义的网络配置
              | - 添加自定义的软件包到overcloud 节点
              | - 特定更改 overcloud 配置
**1230-1330** | 午餐
**1330-1600** | 实验九 (继续)
              | **实验十**: 部署后配置更改
**1600-1615** | 中间休息
**1600-1730** | **实验十一**: 彻底的测试 overcloud，包括高可用测试

### 第四天

时间          | 内容
------------- | -----------------
**0900-1030** | **实验十二**: 实例 HA 配置和测试
**1030-1200** | **实验十三**: 实验故障排除
**1200-1300** | 午餐
**1300-1430** | 实验十三 (继续)
**1430-1500** | 闭幕辞


## 实验流程

动手实验的 **工作流程** 将如下:

## 实验的原则和公约

整个实验室，我们会给明确说明有关如何部署环境中使用OSP-director（OSP-导演）。任课教师将指导您部署到虚拟机中; 不要 修改实验的环境。我们将会有非常有限的时间来完成必要的实验室，不能由个人偏离任课。

实验说明虽然已经过端到端测试，但可能基于不断变化的代码仍然有问题，所以如果有任何问题请提醒我们注意。请注意，这绝对**不**是 复制和粘贴练习。实验说明省略某些指令故意强迫你自己照顾自己。跳过前面和盲目复制和粘贴指令，您将不理解为什么做它，和不可避免地陷入浪费**您**和**我们**的时间。

### 代码的键入

许多实验室会期望你将命令键入 CLI 通过安全壳连接到主机。命令的每个条目将突出显示，并且在必要时将确定我们期待您要使用特定的用户。然而，为了清楚起见下文列出约定。

这命令输入框:

~~~
# uname -a
Linux s01.lab.redhat.com 2.6.32-504.16.2.el6.x86_64 #1 SMP Tue Mar 10 17:01:00 EDT 2015 x86_64 x86_64 x86_64 GNU/Linux
~~~

任何命令要求您以 **root** 身份运行的将以 (**#**) 开头, 例如:

~~~
# whoami
root
~~~

否则, 将以 (**$**), 开头, 例如:

~~~
$ whoami
stack

$ sudo su -
# whoami
root
~~~

## 内容

内容由多个章节，引入概念与相关实验室 (如有必要) 您可在任何时间导航到 [内容](./doc/contents.md) 页面，但最好在我们开始之前是回顾一下 [现有的部署工具] (./doc/existing-tools.md)

[现有的部署工具](./doc/existing-tools.md)

[内容](./doc/contents.md)
