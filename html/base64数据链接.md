## 数据链接

在线搜索在线加密解密

该工具可以将图片进行base64解码

**书写 **
数据链接：将目标文件的数据直接书写到路径位置

语法：data:MIME,数据



**base64处理图片：**

优点：

1. 减少浏览器中的请求，减少请求中浪费的时间
2. 有篮球动态生成数据 

缺点：

1. 增加资源的体积(代码量增加)，导致传输内容增加，从而增加了单个资源的传输时间
2. 不利于浏览器缓存，浏览器通常会缓存图片文件，css文件，js文件(数据链接时浏览器不会缓存)
3. 会增加原资源的体积到原来的4/3（例如：图片大小为3kb,进行base64解码时变成4kb）

**应用场景： **

1. 请求单个图片体积小，并且该图片因为各种原因，不适合制作雪碧图，可以用数据链接

2. 图片由其他代码动态生成，并且图片较小，可以使用数据链接。



 **base64**
data:image/pang;base64,...
一种编码方式，图片是二进制数据。通常用于将一些二进制数据，用一个可书写的字符串表示 （不然会造成乱码）