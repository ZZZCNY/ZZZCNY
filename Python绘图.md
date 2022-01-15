# Python

1. Matplotlib 绘图时显示中文

   ```python
   from pylab import mpl
   mpl.rcParams['font.sans-serif']=['simhei']
   ```

2. '//'表示整除

3. 曼哈顿距离：直角距离。$|x_1-x_2|+|y_1-y_2|$

   ```python
   def manhattan(rating1,rating2):
       return sum(abs(rating1-rating2))
   ```

4. 欧氏距离：直线距离。$\sqrt{(x_1-x_2)^2+(y_1-y_2)^2}$

   ```python
   def distEclud(vecA,vecB):
       return numpy.sqrt(sum(pow(vecA-vecB,2)))
   ```

5. 判断数字

   ```python
   Isnumeric()
   ```

6. 判断小写字母

   ```python
   Islower()
   ```

7. 判断大写字母

   ```python
   Isupper()
   ```

8. 日期转换

   ```python
   df_dt=to_datetime(df.date,format="%Y/%/m/%d")
   ```

9. 日期格式化

   ```python
   df_dt.apply(lambda x:datetime.strftime(x,"%Y/%m/%d"))
   ```

10. 箱式图删除异常值数据

    ```python
    def box_plot_outliers(data_ser, box_scale):
        # IQR即尺度*（上四分位点-下四分位点）
        IQR = box_scale * (data_ser.quantile(0.75) - data_ser.quantile(0.25))
        val_low = data_ser.quantile(0.25) - IQR # 计算下边缘
        val_up = data_ser.quantile(0.75) + IQR # 计算上边缘
        rule_low = (data_ser < val_low) # 小于下边缘的值
        rule_up = (data_ser > val_up) # 大于上边缘的值
        return (rule_low, rule_up), (val_low, val_up)

    scale = 3
    rule, value = box_plot_outliers(kobe['shot_distance'], box_scale = scale)
    kobe = kobe.reset_index(drop = True)
    index = arange(kobe['shot_distance'].shape[0])[rule[0] | rule[1]]
    kobe = kobe.drop(index)
    ```
