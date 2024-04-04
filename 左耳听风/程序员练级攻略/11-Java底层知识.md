# Java底层知识

## Java字节码相关

* [Java Zone: Introduction to Java Bytecode](https://dzone.com/articles/introduction-to-java-bytecode) 是一篇很不错的入门讲述java字节码的文章
* [IBM DeveloperWorks: Java bytecode](https://www.ibm.com/developerworks/library/it-haggar_bytecode/index.html) 是一篇非常好的讲 Java 字节码的文章。 【没跳转到相关文章】
* [Java Bytecode and JVMTI Examples](https://github.com/jon-bell/bytecode-examples) 使用[JVM Tool Interface](https://docs.oracle.com/javase/7/docs/platform/jvmti/jvmti.html)操作字节码的使用案例

三个比较好用的库
* [asmtools](https://wiki.openjdk.java.net/display/CodeTools/asmtools) 用于生产环境的 Java .class 文件开发工具。
* [byte buddy](http://bytebuddy.net/) 代码生成库：运行时创建 Class 文件而不需要编译器帮助。【作者更喜欢】
* [jitescript](https://github.com/qmx/jitescript) 和[bitescript](https://github.com/headius/bitescript)类似的字节码生成库。


Java Agent：使用 [Java Instrumentation API](https://stackoverflow.com/questions/11898566/tutorials-about-javaagents) 主要方法是实现一个叫 premain() 的方法，（一个比 main() 函数还要超前执行的 main 函数），然后把你的代码编译成一个 jar 文件。


如何用 Java Agent 做监控，你可以看一下这个项目 [Stage Monitor](http://www.stagemonitor.org/)