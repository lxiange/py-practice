# 函数式编程

### 【解决思路】

1. 首先是读取文件，这应该不是什么大问题吧！

2. 然后按行进行处理，在进行函数式编程时，就要尽可能地尝试以函数式的思想去解决问题，尽量不要用过程式的方法。虽然目前冯诺依曼体系的计算机最终一定是过程式的，但是很多时候你自己实现的过程效率反而不如编译器的实现。

3. 假设你已经了解`map`, `reduce`, `filter`的用法，那么你想想哪些步骤可以用它们来实现？而不是用普通的循环？

4. Python中函数作为“一等公民”的体现就在于，函数可以当成参数自由传递，你会发现很多地方函数的参数也是函数。

5. 最后，有关柯里化，这是函数式编程里的一个重要概念，虽然实际用的时候不多，但是还是了解一下比较好。所谓柯里化，其实道理很好理解，就是将多参数函数的参数固化，变成单参数函数。

   ​
