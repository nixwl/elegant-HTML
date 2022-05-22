## **二、HTML基础**

1. <font color="Aqua"><stong>HTML的基本标签有哪些</stong></font>
   一个网页中必定包括以下标签
   - `<html> and </html>`:中间的文本用于描述网页。
   - `<head> and </head>`:在`<html>` 和 `</html>`间，不出现在网页上，代码段用于浏览器内核解析。
   - `<body> and </body>`:在`<html>` 和 `</html>`间，出现在网页上，是网页的主体。
   - `<title> and </title>`:在`<title>` 和 `</title>`间，表示<font color="yellow">网页名</font>
   
2. <font color="Aqua"><stong>HTML的标题如何指定？</stong></font><br>
   - 标题级别分为：`<h1></h1> ~ <h6></h6>,`
共6个级别，h1等级最高，字号最大;h6等级最低，字号最小。</br>
   - 示例：   
    `<h1>hello world i am h1</h1>`<br>
    `<h2>hello world i am h2</h2>`<br>
    `<h3>hello world i am h3</h3>`<br>
3. <font color="Aqua"><stong>HTML的段落是什么？</stong></font><br>
   使用`<p> and </p>`来分割段落
   > <font size="3">示例: 
   `<p>hello world i am p</p>`
   </fnot>
4. <font color="Aqua"><stong>HTML如何设置链接？</stong></font><br>
   HTML的标签由`<a> and </a>`定义
   > <font size="3">示例:
   `<a href="https://github.com/">there is a link</a>`  
   href属性用于指定URL</font>
5. <font color="Aqua"><stong>HTML中如何放置图像？</stong></font><br>
   HTML的图像是通过`<img>`指定的
   > `<img src="hello.jpg" width="104" height="142">`
6. <font color="Aqua"><stong>什么是HTML的元素？</stong></font><br>
   所谓HTML元素，指的就是开始标签和结束标签中间的代码
   > - HTML元素可以有也、也可以没有<br>
   > - HTML元素中也可以嵌套其他元素
    >>- 例如：<br>
      >>>  ```
      >>>      <html>
      >>>         <body>
      >>>            <p> hello world</p> 
      >>>         </body>
      >>>     </html>
      >>>   ```
   就是一种嵌套结构
7. <font color="Aqua"><stong>何谓HTML的属性 ?</stong></font><br>
   我们知道，HTMl的标签用于指定某种操作，但同一标签想要达成的结果不完全相同，所以，必须要有一个设置对标签进行参数调整，即我们所说的HTML属性。
   > - <font size="3">例如：前面我们举过的例子
      ` <a href="https://github.com/">there is a link</a>" `
      <br>href即一个属性，在这里用于指定链接URL  
   > - 此外：HTML对大小写不敏感，但推荐使用小写属性，始终为属性值加引号</font>
8. <font color="Aqua"><stong>HTML的样式设定</stong></font><br>
   通过使用style属性，设置网页背景，文字字体大小、对齐方式、颜色等属性
9. <font color="Aqua"><stong>HTML如何格式化？</stong></font><br>
   HTML的格式化是通过各种标签设置的
   - 文本格式化标签  
      ```
      <b>:定义粗体文本
      <em>: 定义着重文字
      <strong>: 定义加重语气
      <i>: 定义斜体字
      <sub>:定义下标字
      <sup>:定义上标字
      <ins>:定义插入字
      <del>:定义删除字
      <big>:定义大号文本 
      <small>:定义小号文本
      ```
   - “计算机输出”标签
      ```
      <code>:定义计算机代码
      <kdd>: 定义键盘码
      <samp>: 定义计算机代码样本
      <tt>: 定义打字机代码
      <var>:定义变量
      <pre>:定义预格式文本
      ```
10. <font color="Aqua"><stong>什么是HTML引用</stong></font><br>
   HTML引用类似于编辑自己的文本时引用了其他人的文本，需要将被引用文本与其他文本区分开。HTML引用就是完成这样的功能
       - 10.1 HTML的短引用：通过 `<q> </q>`标记被引用文本  
         > 例如:`<p>it is a：<q>构建人与自然和谐共存的世界。</q></p>`
       - 10.2 HTML的长引用：通过`<blockquote>`定义被引用文本
         > 例如：
         ```
         <p>以下内容引用自 WWF 的网站：</p>
            <blockquote cite="http://www.worldwildlife.org/who/index.html">
            五十年来，WWF 一直致力于保护自然界的未来。
            世界领先的环保组织，WWF 工作于 100 个国家，
            并得到美国一百二十万会员及全球近五百万会员的支持。
            </blockquote>
         ```
11. <font color="Aqua"><stong>HTML的“定义”</stong></font><br>
      - 11.1 对缩写进行标记，为浏览器、翻译系统以及搜索引擎提供有用的信息：
         - a. 使用`<abbr>`元素定义
            > 例如:  
            >>```
            >>   <p>
            >>      <abbr title="World Health Organization">
            >>           WHO
            >>      </abbr> 
            >>         成立于 1948 年。
            >>   </p>
            >>```
         - b. 使用`<dfn>`元素定义
            - 如果`<dfn>`的title属性设置，则：
            > ```
            >  <p>
            >      <dfn title="World Health Organization">
            >         WHO
            >      </dfn>
            >      成立于 1948 年。
            >   </p>   
            > ```
            - 如果 `<dfn>`元素包含具有标题的`<abbr>`元素，则 title 定义项目
            >```
            >   <p>
            >      <dfn>
            >         <abbr title="World Health Organization">
            >            WHO
            >         </abbr>
            >      </dfn> 
            >      成立于 1948 年。
            >   </p>
            >```
         - c. a & b均不满足，`<dfn>`文本内容即是项目，并且父元素包含定义
            >```
            >   <p>
            >      <dfn>
            >            WHO
            >      </dfn> 
            >      World Health Organization 成立于 1948 年。
            >   </p>
            >```
      - 11.2 对联系信息进行定义：使用`<address>`
         > 示例：通常以斜体显示
            >```
            >   <address>
            >      Written by Donald Duck.<br> 
            >      Visit us at:<br>
            >      Example.com<br>
            >      Box 564, Disneyland<br>
            >      USA
            >   </address>
            >```
      - 11.3 对著作标题进行定义：使用`<cite>`
         > 示例：通常以斜体显示
            >```
            >  <p>
            >      <cite>
            >         The Scream
            >      </cite> 
            >      by Edward Munch. Painted in 1893.
            >   </p>      
            >```
      - 11.4 定义双向重写（即双流向覆盖）：使用`<bdo>`
         > 示例：即将逆向打印段落中的内容
            >```
            >  <bdo dir="rtl">
            >      This text will be written from right to left
            >   </bdo> 
            >```
12. <font color="Aqua"><stong>HTML如何添加注释？</stong></font><br>
   - 方法很简单，添加注释只需使用`<!-- -->`即可。  
      > 例如:
      > ```
      >   <!-- 这是一段注释 -->
      >    <p>这是一个段落。</p>
      >   <!-- 记得在此处添加信息 -->
      > ```
   - 我们在浏览其他网页代码时，也许会碰到这样的代码,。
      >``` 
      >   <!--[if IE 8]>
      >     .... some HTML here ....
      >   <![endif]-->
      >```
      > 我们称其为条件注释，条件注释定义只有 Internet Explorer 执行的 HTML 标签
   - 各种HTML软件程序也能够生成HTML注释,我们称其为软件程序注释    
13. <font color="Aqua"><stong>网页中如何灵活使用多种颜色？</stong></font><br>
       - 首先，我们知道，RGB通道颜色是由三原色组成，即红色(Red)、绿色(Green)、蓝色(Blue)  
       - 每个颜色都由一个16进制符号定义，这个符号是由红色、绿色、蓝色组成的  
       - 每种颜色的最小值为 0D(#00H),最大值为255(#FFH) 
          > 后缀-D 表示10进制数，后缀-H表示16进制数   
          > 下面我们给出一张普通的色卡 
          > ![色卡](https://github.com/nixwl/elegant-HTML/blob/master/img/color_page.jpg "color_page")
       - 颜色有多种多样，所以每种颜色都应当有颜色名(<font color="red"><stong>大多数的浏览器都支持颜色名集合</stong></font>)
          > - 如果你想查找HTMl中的颜色名，可以到该网站
          [HTML颜色名](https://www.w3school.com.cn/html/html_colornames.asp "HTML颜色名")
          > - 但是，仅有16中颜色名被W3C的 HTML4.0 标准支持，分别为：aqua, black, blue, fuchsia, gray, green, lime, maroon, navy, olive, purple, red, silver, teal, white, yellow
          > - 想要使用其他颜色，我们这是就需要用16进制的颜色值来精确地描述颜色了
       - 接下来，我们聊一聊Web安全色  
         Web安全色是什么呢？当初计算机使用256种颜色时，一系列216种Web 安全色作为 Web 标准被建议使用。其中的原因是，微软和 Mac 操作系统使用了 40 种不同的保留的固定系统颜色（双方大约各使用 20 种） 
           > 下面是这216跨平台色的色卡
           > ![色卡](https://github.com/nixwl/elegant-HTML/blob/master/img/color_page_216.jpg "color_page")

   


---------------



