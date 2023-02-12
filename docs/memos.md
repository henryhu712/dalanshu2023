---
sidebar_position: 5
---

# 备忘录

网摘笔记

## ts-node

每周下周量高达2千万：
[npm ts-node](https://www.npmjs.com/package/ts-node)

## SketchUp 插件开发

发布路径：

    [废弃]  /mnt/d/projects/sketchup-plugins77-for-release/sketchup-plugins
            /mnt/d/projects/sketchup-plugins88-for-release/sketchup-plugins

删除了 google, sqlite3 目录。


## git：按照代码查找提交

1. git-log

按照代码内容查找 commit，例如，有一行代码为：foo = foo + bar

    git log -S "foo = foo + bar"

上述命令将给出该行代码创建的 commit。

2. git-blame

按照行号查询提交。例如，查找第 110 行代码是谁写的：

    git blame -L 100,100

上面的命令将给出该行的最后提交，也就可以找到该行的最后一个作者。


## 日本新干线

最近发现了一个问题。
很多人刚来日本的时候，不会买新干线的票。
最大的问题还是弄不清楚日本这种乘车券和特急券甚至指定券这种多元的制度。
就出现只买了特急券，结果单凭特急券无法进站的状况。

就说JR
首先你要使用铁道，最基础的就是要购买乘车券（乗車券）
这个是按照里程计算的基础票价（不坐什么特急新干线，而是坐普通车到一个地方的票价）
这个乘车券可以是纸质票，也可以是suica等交通卡。

在这个基础上，如果你要享受诸如特急或者新干线等更高的服务，就要购买特急券，或者也有线路叫做green券（特急券、グリーン券）
有些公司还会再细分出一个指定券（指定券），也就是可以选座的服务。
所以单买这种券的话，因为没有付乘车券的费用，所以会有不能进站的情况。

新干线有三个等级，自由席（3等），指定席（2等）和green席（1等）特急券也是有对应这三个等级的价格。
自由席就是上了车随便坐，反而也意味着有座没座靠运气。
指定席开始是有指定座位号。
green席就是座位稍微高级点

source: [tweet](https://twitter.com/yuebanzhu/status/1622961425739313153)


## Ruby: require vs include

The require method does what include does in most other programming languages: run another file. It also tracks what you've required in the past and won't require the same file twice. To run another file without this added functionality, you can use the load method.

The include method takes all the methods from another module and includes them into the current module. This is a language-level thing as opposed to a file-level thing as with require. The include method is the primary way to "extend" classes with other modules (usually referred to as mix-ins). For example, if your class defines the method "each", you can include the mixin module Enumerable and it can act as a collection. This can be confusing as the include verb is used very differently in other languages.

source: [A Quick Peek at Ruby: 'Include' vs. 'Require'](http://ruby.about.com/b/2008/10/23/a-quick-peek-at-ruby-include-vs-require.htm)

