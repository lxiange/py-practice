# Python操作Spark
### 【问题描述】

如今大数据是越来越火了。以谷歌的三篇论文作为转折点，大数据处理也一下子变得简单起来。处理海量数据，再也不是那些科学家们的特权，你只需要很少的工作，就可以在个人电脑上去处理大数据。目前有很多大数据处理系统可供选择，其中最火的，一定是Spark了。

Spark是用Scala编写的，原生API自然是Scala（相信我，这是一门比C++还要复杂的语言）。不过好在即使你不会Scala也没关系，它也提供了Python的接口，并且自1.4版本之后，就同时兼容Python2/3了。可见Python用户是一个非常值得重视的群体啊！

关于Spark的安装，你可以参考[官网文档](https://spark.apache.org/docs/latest/)，建议你**不要**使用源码编译的方式安装，而是直接下载预编译的程序，然后只要配置环境变量就可以运行了。

我们假设你已经安装好了Spark，并大体了解了Spark的工作流程以及启动方式。下面你要做的是：

* 在交互式命令行下，实现WordCount，统计给定文件中每个单词出现的次数
* 编写一个`.py`文件，实现上述功能，毕竟我们不可能所有任务都在交互式命令行下完成吧？






### 【[解决思路](solution.md)】
