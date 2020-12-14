
## 面试总结系列

https://juejin.im/post/5ea2ab266fb9a03c82234a9f#heading-1 
https://www.jianshu.com/p/ecbf69ee7641
https://juejin.im/post/5eb01866f265da7b9c24562c

## Mvvm Jetpack

1.Lifecycle
刘望舒的文章
http://liuwangshu.cn/application/jetpack/3-lifecycle-theory.html 
讲清楚了如何处理注解，生命周期event和state,反射回调observer的方法

2.viewmodel
ViewModel源码解析
这篇是基于目前最新源码的分析，讲清楚了viewmodel 何时viewmodel 被清除，以及存在哪的问题
https://www.jianshu.com/p/731ca42823ee
https://juejin.im/post/5e5bd0d2e51d4526e807f55f#heading-12 

3.LiveData
https://juejin.im/post/5ce54c2be51d45106343179d

4.Event .SingleLiveEevent  .之前一直收藏的meideum文章，有人翻译了.
https://juejin.im/post/5b2b1b2cf265da5952314b63

5.关注一下这个小伙儿的文章https://www.jianshu.com/u/ae6d42bbd950  主要跟我的目前的技术比较搭

6.https 看完彻底明白
https://www.jianshu.com/p/9038e6899d0f

7.Jvm 图不错，类加载子系统，运行时数据区，执行引擎 栈帧 对象头
https://mp.weixin.qq.com/s/S1Jcm1YOyEPRZpvB0DlPDQ

8.协程用法 中文官网 https://www.kotlincn.net/docs/reference/coroutines/basics.html
主要看秉心说的三篇文章以及escape自己写的demo
协程原理 https://blog.csdn.net/suyimin2010/article/details/91125803 涉及语言层面对supend关键字的优化，将挂起代码封装成类，并缓存，有状态机负责resume挂起点之后的代码，实在线程池上封装，续体拦截器负责指定恢复代码应该执行在哪个线程。

9.room 
https://www.jianshu.com/p/3e358eb9ac43

10.性能优化  jsonchao系列文章
https://juejin.im/post/5eb168e9f265da7bb65fb27a
https://mp.weixin.qq.com/s/3QhMGVIcR1yW3xweJCa-9Q
极客时间android开发高手课

11.Windows 和 view 添加流程
https://blog.csdn.net/freekiteyu/article/details/79408969


5.Anroid进阶解密结合Gityuan的文章看 Android系统启动，activity 启动，ams相关，
6.艺术探索 补缺 aidl binder
7.java并发编程的艺术 
8.Jvm 相关的carson_ho 进阶解密，webview相关 recycler view相关
9.设计模式和算法
10.kotlin 协程
11.flutter 官网，flutter原理Gityuan
12.面试总结
13.性能优化


## 程序员的修养

1.<<代码整洁之道>> 读后感 

https://mp.weixin.qq.com/s/7ADpdhK6AJ5dkmGp0wXTtA https://blog.csdn.net/AlpinistWang 

2.阿里巴巴 Java 编程规范 阿里巴巴Java开发手册  

https://www.cnblogs.com/han-1034683568/p/7682594.html 

3.谷歌面试大学jwasham/coding-interview-university  
https://github.com/jwasham/coding-interview-university/blob/master/translations/README-cn.md 

4.成为android专家
https://www.zhihu.com/question/37549641/answer/83217748
https://zhuanlan.zhihu.com/p/20708611


## Android  

0.官方开发指南
https://developer.android.google.cn/guide
http://hukai.me/android-training-course-in-chinese/index.html 官方教程翻译版本

1.android常用utils 

https://blankj.com/ 

2..Jni 加密存储相关 

https://github.com/dfqin/AndroidNativeEncryption

3..方舟编译器相关

https://juejin.im/post/5d4bdb23e51d453c2577b747

4.Jetpack MVVM 架构相关
ViewModel源码解析
这篇是基于目前最新源码的分析，讲清楚了viewmodel 何时viewmodel 被清除，以及存在哪的问题
https://juejin.im/post/5e5bd0d2e51d4526e807f55f#heading-12 

这篇有点过时了,不过思路可以参考
https://juejin.im/post/5c047fd3e51d45666017ff86   
作者 ：却把青梅嗅  
基于lifecycle1.1  但是2.0版本已经没有文中的holderfragment了 

databinding 
https://juejin.im/post/5d5663f7f265da03bf0f3e3c 
https://www.jianshu.com/p/c4f5411cb0ae 源码解析

https://blog.csdn.net/xfhy_/article/details/88703853  
作者： 潇风寒月 
基于 androidx.lifecycle:lifecycle-extensions:2.0.0 的源码进行分析 

5.AOP android最佳用法 

https://www.jianshu.com/p/85678f228712  

https://www.jianshu.com/p/2779e3bb1f14  

https://blog.csdn.net/eclipsexys/article/details/54425414 

6.RecyclerView 回收复用原理 
https://www.jianshu.com/p/2b19e9bcda84

7.插件化 腾讯Shadow 
https://juejin.im/post/5d331fa8f265da1bba593ff6 

8.volitale 
https://www.cnblogs.com/xrq730/p/7048693.html 

9.RxJava 
玉刚说: 
https://juejin.im/post/5b17560e6fb9a01e2862246f 
抛物线:
https://gank.io/post/560e15be2dca930e00da1083  
Carson_Ho:背压策略
https://www.jianshu.com/p/ceb48ed8719d  
却把青梅嗅 autodisposable 
https://blog.csdn.net/mq2553299/article/details/79418068 

10.Android 性能优化
https://juejin.im/post/5d95f4a4f265da5b8f10714b 

11.Dragger 
https://www.jianshu.com/p/1d84ba23f4d2  很好理解的文章
https://mp.weixin.qq.com/s/fatc5Q8z68p6ZOV70-OBQg 


12.内存优化 
https://www.2cto.com/kf/201510/445485.html 

13. App架构开发指南(翻译) 
http://www.jcodecraeer.com/a/anzhuokaifa/androidkaifa/2017/0523/7963.html 

14. 代替drager2的依赖注入框架 Koin 
https://www.jianshu.com/p/80c4852cbd95   koin 关于viewmodel 
https://blog.csdn.net/u012122009/article/details/88364848  
目前koin的原理文章不多，官网没有很好的介绍，这篇文章段尾，说明了大概方向是函数拓展，但是还不尽然 

我理解是这个框架 存了一个全局的并且知道如何创建所依赖注入类的方法实例的仓库，当需要注入时，就去这个仓库去查怎么创建实例并注入 
除了Koin 还有Kodein 类似的框架


15.Jni
https://www.jianshu.com/p/87ce6f565d37 (错别字比较多，但是适合入门)

16.UI控件
//To do 
NestedScrolling
materialviewpager

17.viewpager
https://juejin.im/post/5a4c2f496fb9a044fd122631 用法
https://juejin.im/post/5df4aabe6fb9a0161104c8eb viewpager2 新特性介绍
https://github.com/android/views-widgets-samples 谷歌官方的例子
https://github.com/youth5201314/banner 基于viewpager2的开源框架9.4K star

18. 插件化
https://github.com/tiann/understand-plugin-framework

https://blog.csdn.net/lmj623565791/article/details/75000580

19.热更新
book <<深入探索Android热修复技术原理>> https://github.com/feelschaotic/AndroidKnowledgeSystem/blob/master/7.%20%E8%BF%9B%E9%98%B6/%E5%8A%A8%E6%80%81%E5%8C%96/%E6%B7%B1%E5%85%A5%E6%8E%A2%E7%B4%A2Android%E7%83%AD%E4%BF%AE%E5%A4%8D%E6%8A%80%E6%9C%AF%E5%8E%9F%E7%90%86.pdf

https://www.jianshu.com/p/19d92329d9f2

20 Binder
http://weishu.me/2016/01/12/binder-index-for-newer/

21. 如何调试Android fw
http://weishu.me/2017/01/14/how-to-debug-android-native-framework-source/

22.Arouter 原理
https://www.jianshu.com/p/857aea5b54a8
通过注解处理器apt技术编译时生成路由映射表

23.自定义view
https://www.jianshu.com/p/760374ece737 
https://www.jianshu.com/p/9862cddca1b3 双缓冲机制一定要知道
https://www.jianshu.com/nb/9976005  carson_ho

24.gradle
http://liuwangshu.cn/application/gradle/1-study-gradle.html 刘望舒

关于gradle还是看那两本书吧.

25.安全 TEE
https://www.freebuf.com/author/%E5%AE%89%E5%B0%8F%E7%99%BD 

26.android领域的一些新动态 秉心说
https://juejin.im/search?query=%E7%A7%89%E5%BF%83%E8%AF%B4&type=all 

28.捕获andorid异常，上报的实现
https://www.jianshu.com/p/457a4783fe6f

29.性能优化 付费课程
https://time.geekbang.org/column/intro/100021101

30.android fw
1.gityuan
2.https://blog.csdn.net/freekiteyu/article/details/79408969 总结的简洁
3.https://blog.csdn.net/Innost 阿拉神灯

31.hutool
https://www.hutool.cn/

## Kotlin 

1.协程 
https://www.jianshu.com/p/2979732fb6fb 原理有点难

https://me.csdn.net/NJP_NJP  看下怎么用协程处理网络请求

https://www.jianshu.com/p/76d2f47b900d 

https://juejin.im/post/5d5d5aac51882549be53b75b  关注一下这个作者的几篇文章 

https://www.bennyhuo.com/  应该也不错

2.Kotlin的单例模式
https://www.jianshu.com/p/5797b3d0ebd0


## C++
https://pan.baidu.com/s/1BwAPeBCRJ0BPvXfJHVtfZg?errno=0&errmsg=Auth%20Login%20Sucess&&bduss=&ssnerror=0&traceid=#list/path=%2Fsharelink812091596-211960096844187%2FAndroid%E8%BF%9B%E9%98%B6%E4%B9%8B%E6%97%85%EF%BC%88NDK%E5%AE%9E%E6%88%98%E7%AF%87%EF%BC%89&parentPath=%2Fsharelink812091596-211960096844187

xdps

## Java

1.线程
https://www.cnblogs.com/wxd0108/p/5479442.html
https://www.jianshu.com/p/f65ea68a4a7f  关注此人的其他文章

https://juejin.im/post/5d45a75de51d4561ee1bdf10#heading-30  比较全面的线程知识 

2.volatile
https://www.infoq.cn/article/ftf-java-volatile 

3.java并发
CAS
https://www.jianshu.com/p/ab2c8fce878b

4.动态代理
https://www.jianshu.com/p/5dc416ea58a2

5.生产者消费者的几种模式
https://www.jianshu.com/p/ab013a4d5878

6.static
https://github.com/Snailclimb/JavaGuide/blob/master/docs/java/basic/final,static,this,super.md

7 hashmap 扩容问题
https://blog.csdn.net/qq_36071795/article/details/83655055
2的n次方-1，二进制是111111.按位与之后，正好等于去模运算。  尽量避免了hash碰撞

## flutter
https://juejin.im/post/5dac91296fb9a04e270fb204 

flutter 实战
https://book.flutterchina.club/chapter1/dart.html 

flutter 原理分析 gityuan  
http://gityuan.com/flutter/

flutter 异步
https://juejin.im/post/5c898b4af265da2de25bcc2d

flutter 另外一本电子书
https://www.kancloud.cn/alex_wsc/flutter_demo/1563027

flutter 实践
https://www.jianshu.com/u/cbf2ad25d33a

flutter 布局教程
http://laomengit.com/

Dart
https://www.dartcn.com/guides/language/effective-dart/
https://www.jianshu.com/p/9e5f4c81cc7d

flutter Mvvm
https://www.jianshu.com/p/ce011acad64e
https://www.jianshu.com/p/43eb17163468

## uni-app
https://uniapp.dcloud.io/

## mPaas 支付宝架构
https://blog.csdn.net/weixin_44326589/article/details/92773742
https://help.aliyun.com/document_detail/49549.html

蚂蚁金服 mPaaS、Google Firebase、AWS Mobile Hub 等

## 容器化架构
1.android app bundle https://www.jianshu.com/p/0c551eaa2020
2.支付宝客户端架构解析 https://www.jianshu.com/p/b7ee3538936d
3.美团外卖容器化 https://mp.weixin.qq.com/s/kW5wu7GM7pMRRvN-dQvE2g 

##Liunx 
http://akaedu.github.io/book/  Liunx C 编程来源于Gityuan的博客


## 后端开发
https://www.bilibili.com/video/av47952931?p=27  spring 黑马视频教程


## 开发常见的坑
https://www.jianshu.com/p/ec09dc60061e  组件化后，尽量不用Databinding.


## 设计模式 

待更新

## 算法
自己的总结
https://github.com/RenHongshuang/arithmetic

## 英语学习
https://www.jianshu.com/p/a4d031ee3f55 

## 工具
1.在线画图工具
https://www.processon.com/
https://www.draw.io/
https://www.zenflowchart.com/?ref=appin


2.任务管理工具
worklite
后端托管
bmob
https://www.bmob.cn/
## 其他
1.Android 大佬的blog 汇总
https://juejin.im/post/5e0389ec5188251281602a2e


2.小程序框架
https://baijiahao.baidu.com/s?id=1603297934363840853&wfr=spider&for=pc

3.Android开发工具大全
https://www.androiddevtools.cn/

4.大厂分享 
https://www.wanandroid.com/article/list_by_chapter/1?cid=510

5.下载电子书
别:
https://www.yunpanjingling.com/

6.面试总结
https://www.jianshu.com/p/c70989bd5f29
https://www.jianshu.com/p/a2b3831fbf2e
https://www.jianshu.com/p/b3c1b9c6dd40  看看这个..

