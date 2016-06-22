# 函数式编程
### 【问题描述】

Python是一门支持多范式的编程语言，你可以按照C语言那样的面向过程式来编写程序，也可以像Java一样面向对象。当然Python对函数式编程也提供了一定的支持。

在Python里，函数是“一等公民”，并且在之前的题目里面我们有了解到，Python支持“闭包”等特性。不过，Python并不完美地支持函数式编程，譬如默认的CPython解释器就不支持尾递归优化。当然，这已经超出我们的讨论范围了，如果你对函数式编程比较感兴趣的话，可以参考[这篇文章](http://www.ruanyifeng.com/blog/2012/04/functional_programming.html)的介绍。

今天，我们只要了解Python中几个最基本的函数式编程特性即可，具体点，你需要：

* 尝试使用匿名函数。
  * 给定一个输入文件，每行是一个向量坐标。
  * 将模小于1的向量按照向量模大小逆序排序。
  * 计算上述排序后，前十个向量的和
* 尝试使用`map`, `reduce`, `filter`函数
* 尝试对函数进行'[柯里化](https://zh.wikipedia.org/wiki/%E6%9F%AF%E9%87%8C%E5%8C%96)'，只要实现最简单的例子即可。

### 【[解决思路](solution.md)】
