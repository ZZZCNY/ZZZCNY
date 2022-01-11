# Python

> 以下所有 numpy 均用 np 代替

1. 
   ```python
   np.arange(0,50,3)
   ```

   arange 中的第一个参数表示起始值，第二个参数表示终止值，是一个左闭右开的区间。第三个参数表示步长。

2. 
   ```python
   list(filter(odd,arr))
   ```

   odd 是用来判断该数字是否为奇数。filter 用于过滤序列，把 arr 的值放入 odd 函数运算，返回值为 true 的保留。因为 filter 只是一个容器，所以需要 list 将其转换为列表。

3. ```python
   np.where(odd(arr),-1,arr)
   ```

   这是将奇数全部替换为-1。当 where 有三个参数时，第一个参数获取 bool 类型的值，若为 true，则使用第二个参数的值，若为 false，则使用第三个参数的值。  
   若只有一个参数，则是返回结果为 True 的坐标。例如：

   ```python
   where(isnan())
   ```

   

4. ```python
   split()
   ```

   这是一个很常见的分割字符串的函数，当括号内的参数为空时，默认分割所有的空字符。

5. ```python
   arr.resize()
   ```

   这个函数用于调整 ndarray 的形状，如果只有一个参数，需要将那个参数用括号再括起来，因为它可以拥有第二个参数，而第二个参数拥有默认值，一般情况下不进行传递。

6. ```python
   np.random.choice()
   ```

   可以用来指定随机数的范围和个数。

7. ```python
   np.nan
   ```

   这是一个 float64 的空值，不能用 None 进行判断，只能用 isnan() 来判断。

> 这就是今天的学习日记了，第一次总结一日所学，感觉很像写实验报告。  
> 既然开了这个坑，就要坚持写下去！