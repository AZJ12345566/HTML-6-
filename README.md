# HTML-6-
HTML CSS，链接，图像
//HTML CSS
    //如何使用样式
    //1.外部样式表：当样式需要被引用到很多页面的时候，则使用外部样式表，通过更改一个文件来改变整个站点的外观
    <head>
    <link rel="stylesheet"type="text/css"href="mystyle.css">
    </head>
    //2.内部样式表：当单个文件需要特别样式是。就可以使用内部样式表
    <head>

    <style type="text/css">
    body{background-color:red}
    p{margin-left:20px}
    </style>
    </head>
    //3.当特殊样式需要应用到个别元素时，可以用到内联样式，使用内联样式的方法是在相关的标签中使用样式属性，样式属性可以包含任何css属性
    <p style="color:red;margin-left:20px">
    This is a paragraph
    </p>
    //标签积累：
        //<style>:定义样式定义
        //<link>:定义资源引用
        //<div>:定义文档中的节或区域(块级）
        //<span>:定义文档中的行内的小块或区域
        //<font>:规定文本的字体、字体尺寸、字体颜色。不赞成使用，请使用样式
        //<basefont>:定义基准字体。不赞成使用/请使用样式
        //<center>:对文本进行水平居中。不赞成使用。请使用样式

//HTML链接
        //HTML使用超级链接与网络上的另一个文档相连
        //几乎可以在所有网页中找到链接。点击链接可以从一张页面跳转到另一张页面
        //创建超级链接：
        <html>

        <body>

        <p>
        <a href="/index.html">本文本</a>是一个指向本网站中的一个页面的链接
        </p>

        <p><a href="http://www.microsoft.com/">本文本</a>是一个指向万维网上的页面的链接</p>

        </body>
        </html>
        //将图像转化为链接：
        <html>

        <body>
        <p>
        您也可以使用图像来做链接：
        <a href="/example/html/lastpage.html">
        <img border="0"src="/i/eg_buttonnext.gift"/>
        </a>
        </p>

        </body>
        </html>

        //HTML超链接(链接)
        //超链接可以是一个字，一个词，或者一组词，也可以是一副画像，您可以点这些内容跳转到新的文档或着当前文档的某个部分
        //通过<a>标签在HTML中创建链接，有两种方式：
        //1.通过使用href属性-创建指向另一个文档的链接
        //2.通过使用name属性-创建文档内的书签

        //HTML的链接语法
        //类似：<a href="url">Link text</a>
        //href属性规定链接的目标
        //开始标签和结束标签之间的文字被作为超级链接来显示
        <a href="http://www.w3school.com.cn/">Visit W3School</a>//这行代码显示为Visit W3School
        //注：“链接文本”不必是文本。图片或其他HTML元素都可以称为链接

        //HTML链接-target属性
        //使用Target属性，你可以定义被链接的文档在何处显示
        //下面这行代码会在新窗口打开文档
        <a href="http://www.w3school.com.cn/"target="_black">Visit W3School!</a>

        //HTML链接- name属性
        //name属性规定anchor的名称
        //你可以使用name属性创建HTML页面中的书签
        //书签不会以任何方式显示，他对读者是不可见的
        //当使用命名anchor时，我们可以创建直接跳至该命名anchor(比如页面中某个小节)的链接
        //命名锚的语法：
        <a name="label">锚(显示在页面上的文本)</a>
        //注：锚的名称可以是任何你喜欢的名字，效果相同
        //例：
        //1.首先·在HTML文档中对锚进行一个命名(创建一个书签)
        <a name="tips">基本的注意事项-有用的提示</a>
        //2.我们在同一个文档中创建指向该锚的链接
        <a href="#tips">有用的提示</a>
        //也可在其他页面中创建指向该锚的链接
        <a href="http://www.w3school.com.cn/html/html_linksasp#tips">有用的提示</a>

        //基本的注意事项-有用的提示：
        //命名锚经常用于大型文档开始位置上创建目录。可以为每个章节赋予一个命名锚，然后把链接到这些链接的锚放在文档上部，百度百科就是这样导航的
        //加入浏览器找不到已定义的命名锚，那么就会定义到文档的顶端，不会有错误发生

        //跳出框架
        <html>

        <body>

        <p>被所在框架中了吗？</p>

        <a href="/index.html"
        target="_top">请点击这里！</a>

        <?body>
        </html>

        //创建电子邮件链接
        <html>

        <body>

        <p>
        这是邮件链接：
        <a href="maito:someone@microsoft.com?subject=Heloo%20again">发送邮件</a>
        </p>

        <p>
        <b>注意：</b>应该使用%20来替换单词之间的空格，这样浏览器就可以准确的显示文本了
        </p>

        </body>
        </html>
        //标签积累：
        //<a>：定义锚

//HTML图像
    //实例1:插入图像
    <html>

    <body>

    <p>
    一副图像：
    <img src="/i/eg_mouse.jpg"width="128"height="128"/>
    </p>

    <p>
    一副动画图像：
    <img src="/i/eg_cute.gif"width="50"height="50"/>
    </p>

    <p>请注意，插入动画图像的语法与插入普通图像的语法没有区别。</P>

    </body>
    </html>

    //实例2:
    <html>

    <body>

    <p>
    来自另一个文件夹的图像:
    <img src="/i/ct_netscape.jpg"/>
    </p>

    <p>
    来自W3School.com.cn的图像：
    <img
    src="http://www.w3school.com.cn/i/w3school_logo_white.gif"/>
    </p>

    </body>
    </html>

    //图像标签(<img>)和源属性(Src)
    //在HTML中，图像由<img>标签来定义
    //<img>是空标签，意思是，它只包括属性，并且没有闭合标签
    //要在页面上显示图像，你需要使用源属性(src).src指"source".源属性的值是图像的URL地址
    //定义图像的语法是：
    <img src="url"/>
    //URL指存储图像的位置。如果名为"boat.gif"的图像位于www.w3school.com.cn的image目录中，那么其URL为http://www.w3school.com.cn/images/boat.gif
    //浏览器将图像显示在文档中图像标签出现的地方

    //替换文本属性(Alt)
    //alt属性用来为图像定义一串预备的可替换的文本。替换文本的值是用户定义的
    <img src="boat.gif"alt="Big Boat">
    //当浏览器无法载入图像时，替换文本属性可告诉读者他们失去的信息。此时浏览器将显示替代性的文本而不是图像，添加替换文本属性是一个好习惯

    //基本注意事项-有用的提:
    //若HTML文件包含十个图片，那么为了正确显示这个页面，需要加载11个文件，加载需要时间，所以慎用图像
    //gif和jpg都可以做HTML的背景

    //标签积累：
    //<img>:定义图像
    //<map>:定义图像地图
    //<area>:定义图像地图的可以点击的区域


        
