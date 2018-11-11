### Q：什么是Web？
网站访问的大概过程： 
![网站访问过程](https://pic4.zhimg.com/80/528560fb56581ae59a16e48309835003_hd.jpg)
浏览器和服务器交流，服务器和数据库交流  

服务器HTTP响应之后，浏览器会得到html文件，并进行解析渲染  
HTML是一种标记语言  

浏览器按默认样式渲染html，简洁但是难看  
CSS是一种样式设计语言，自定义浏览器渲染html的样式

HTML5是一种新的标准，新加了很多可以用的标签和属性  
XHTML是html按照xml的严格化，标签必须封闭……

html+css, 是静态的页面  
JavaScript给页面添加动态效果，鼠标弹窗  

用 JS 向服务器发送一个请求，得到这个小窗口应该显示的数据，放在这个小窗口里（这就是所谓的AJAX，不用刷新就能与服务器进行交互，更新页面的一小部分~）

浏览器脚本，可以理解成为了实现某些功能，用JS编写的代码

### Q:什么是CSS
Cascading Style Sheets (CSS) 是一门指定文档该如何呈现给用户的语言

CSS使用一门标记语言作为结构

CSS 并非仅仅用于浏览器，也不仅限于视觉展现。按照 CSS 的正式术语来讲，将文档呈现给用户的程序称为用户代理(UA)。浏览器只是用户代理的其中之一。

### Q:为什么使用CSS
样式是文档展现的细节，CSS将样式从内容分离
+ 避免重复
+ 容易维护
+ 可以对同样的内容，应用不同的样式

### CSS如何工作
浏览器展现一个文档，要把内容和样式结合起来，两个阶段：
+ 浏览器将标记语言和CSS转换成DOM（文本对象模型），DOM是内存中相应的融合了内容和样式的文档
+ 浏览器最终把DOM的内容展示出来

### DOM
DOM是一种树形结构，每个元素和非空文本都可以看做是树形结构上的一个节点

DOM 结构就是CSS和文档内容融合而成的
![DOM](https://mdn.mozillademos.org/files/11781/rendering.svg)

### line-height
"段落的行距至少要1.5倍"  

4种boxes
+ containing boxes
+ inline boxes、匿名inline boxes
+ line boxes
+ content area

行高应用在 inline boxes上  
line box 的高度取决内部最高的inline box  
inline box 最初取决于 font-size  
行高可以增加 inline box 的高度  
上下标（垂直对齐）也会增加 inline box 的高度  
替换元素（如图像）也会影响 inline box 的高度  