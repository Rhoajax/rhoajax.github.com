---
layout: post
title: "Kaggle : Python, R, Matlab and Julia"
description: "Comparing 4 languages widely used in Kaggle"
---

来自Quora的[一篇帖子](http://www.quora.com/Kaggle/How-useful-is-Matlab-for-Kaggle-as-compared-with-R-and-Python)对比了这几种语言在Kaggle上使用时的特色。

Python

    - 琐碎但是齐全的各色装备：Pandas, scikit.learn, numpy, scipy, ipython, matplotlib，不同情况下按需组装使用。
    - IPyhton极佳的交互体验
    - 作为一门通用编程语言的所有优势
    - 慢！
    - 因为琐碎，所以也有相应的缺点。比如有些工具仍然只支持2.7版本。
    - 开源的生态环境

R

    - 一般来说，如果这个问题对统计学家来说比较有趣，那么它就适于R
    - 高质量的库，且专注于Unit Test
    - 在数据分析时RStudio 提供优秀的交互体验
    - 慢，各种占内存。
    - 语言本身长得难看（仅代表作者观点，我就不这么认为嘛……R自有它自己的一套哲学）

Matlab

    - 信号分析的无价之宝
    - 对于任何涉及到矩阵运算的过程，都是最简洁漂亮的语言。处理矩阵得心应手，相对的，处理其他东西就不那么利索。
    - 非开源，无法和其他系统整合

Julia

    - 单听名字就能判定性别的语言……开个玩笑……
    - 新生语言（2012年），在扩展库支持方面还很弱。
    - 努力把Matlab、Python等的高等语言的特性和C的速度结合起来。
    - 语法和Matlab很相似。但拥有高效的for loop，因此避免了不必要的Vectorization。
    - 我个人看好这种语言，以后后机会一定要试用一下。

    另外，关于Julia，其主要开发者之一“在 Strata 站点上[撰文阐释](http://strata.oreilly.com/2013/10/julias-role-in-data-science.html)了 Julia 在数据科学中的定位： 文章娓娓道来，解释了 Julia 语言的设计、与 R 和  Python 的关系，综述了生态系统的现状，以及对未来的展望~”（以上文字来自“统计之都”）在对于未来的展望这方面，作者提到了三点：一是完善Julia的图形工具，二是提高其与Python的整合能力，三是提升建模工具质量，继续引入R的各种统计功能。当然，除此之外，Julia自身也还在持续进化中。
