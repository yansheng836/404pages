## 404pages

![404pages](https://s2.ax1x.com/2019/07/17/ZLQV0g.jpg)



### ﻿介绍：

​	1. 该项目收集了几个404的页面模板，可用于替换原生的404页面。我这里只是进行整理，部分来自网络，部分来自其他项目。

​	2. 自定义一个404页面好像并不难，难的是如何让”状态码为404的请求“都转向我们自定义的404页面，关于这个问题可参考我转发的一篇博客：[三种思路实现自定义404页面](https://blog.csdn.net/weixin_41287260/article/details/96030104)，我这里用的是第三种:利用web容器提供的error-page标签，在`web.xml`中添加<error-page>标签即可实现，如下所示：

```html
<error-page>
    <error-code>404</error-code>
    <location>/resource/view/404.html</location>
</error-page>
```



### 404页面分类：

（注：该分类主要是以页面是否有大量js交互为依据）

1. 静态404页面：HTML+简单CSS+简单的js交互。
   - 404页面1:透明404
   - 404页面2:暗黑主题
   - 404页面3:飞机404
   - 404页面4:哭脸404
   - 404页面5:蓝色，纯文字

2. 动态404页面：HTML+CSS动画+简单的js交互。（浏览器加载时，会比较耗内存。）
   - 404动态页面1:纯css3海面上404页面动画特效
   - 404动态页面2:（暂未添加）
   
3. 404小游戏：
   
   - 404小游戏1: 吾爱破解社区--404游戏《圈小猫》](https://www.52pojie.cn/12)
   
   - 404小游戏2：google-酷跑（暂未添加）
   
     

### 致谢：

1. i7素材网：http://www.17sucai.com，部分404页面来自此网站。
2. 吾爱破解社区：https://www.52pojie.cn，一开始想起自定义404页面就是受《圈小猫》游戏的影响，该项目中的此部分内容转载自：吾爱破解社区在github上的开源项目：<https://github.com/ganlvtech/phaser-catch-the-cat>，游戏试玩地址：<https://ganlvtech.github.io/phaser-catch-the-cat/>。



### 补充内容：

1. 应用js的三种方式。
2. 使超链接失效的方法。
3. 实现跳转到上一页的方法。



### 我的环境：

myeclipse10.7
jdk1.8
Tomcat7.0




### 构建：

1.克隆项目到本地：git clone https://github.com/yansheng836/404pages.git

2.1利用IDE（因为后期考虑添加另外两种访问404的方法）：导入(my)eclipse，调整相关环境，部署到Tomcat，访问`index.html`。

2.2不利用IDE（只能查看404页面，不能实现让”状态码为404的请求“都转向我们自定义的404页面）：直接用浏览器打开`index.html`。



## 总结

我会持续改进，希望 `watch` 、 `star`或者`fork`，以便下次访问。





## License

![GitHub](https://img.shields.io/github/license/yansheng836/404pages.svg)

