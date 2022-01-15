目前还不太清楚 JAVA_HOME 和用户变量中 Path 的影响，只发现系统变量中 Path 对 JDK 版本有影响。

![image-20210513165330113](image-20210513165330113.png)

在系统变量的 Path 中新建另一个版本的 JDK，上下移动，哪个版本在上，WindowsPowerShell 就会调用哪个版本的 JDK。
