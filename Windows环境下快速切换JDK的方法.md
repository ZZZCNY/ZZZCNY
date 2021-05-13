目前还不太清楚JAVA_HOME和用户变量中Path的影响，只发现系统变量中Path对JDK版本有影响。

![image-20210513165330113](image-20210513165330113.png)

在系统变量的Path中新建另一个版本的JDK，上下移动，哪个版本在上，WindowsPowerShell就会调用哪个版本的JDK。