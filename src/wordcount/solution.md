# 单词统计

### 【解决思路】

1. 标准的wc工具，有一些附加选项，可以单独统计单词数、行数等，我们简化起见，采用了wc的默认行为，即统计全部内容并输出。

2. 首先是统计功能，统计行数很简单，我们直接按行读取即可得到行数。统计字节数就更简单了，要学会变通，没有必要将文件遍历一遍再统计字节数。注意到字节数即文件的大小，我们直接通过`os.path.getsize`命令得到文件大小即可。

3. 需要注意的是统计单词数，对于单词的定义有多种，这里我们保持和`wc`的行为一致：即被` \t\n\r\x0b\x0c`这些空白符分割的部分即可认为是一个单词。

4. 最后需要注意的是命令行参数，python提供了`sys.argv`存储命令行参数，我们直接读取它即可，需要注意的是，和Java等语言不通，这里的第一个参数是文件名，而不是真正的的第一次参数。

   ​

   最后更进一步，作为思考题，你能让这个程序支持管道功能么？毕竟管道是Unix最值得骄傲的功能之一。（tips: stdin/stdout）

   ​
