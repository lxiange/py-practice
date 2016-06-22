# 生成器

### 【解决思路】

1. 所谓生成器，核心就是那个“生成器函数”，生成器函数的原理也很简单，就是把原本应该写`return`的地方写成`yield`，然后每次执行到yield时，就会返回，但是下一次再执行时，从yield的地方继续向后执行，而不是从头开始重新执行函数。因此此函数返回后，函数的上下文依然没有释放（是不是有点类似于闭包？）。

2. 所以你只要考虑每次yield返回的结果是什么，这将是你每次迭代此生成器后获得的值。

3. 注意到，生成器函数依然是函数，函数是不可以迭代的。此函数返回的对象才是一个可以迭代的对象。所以记得先调用函数获取它返回的生成器。

4. 你可以再实现一个普通的计算斐波拉契数列的函数，对比下与生成器函数之间的区别。然后再对比一下之前迭代器实现的代码，这时候你就会发现用生成器是多么方便直观了。

   ​
