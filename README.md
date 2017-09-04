Markdown 是一种用来写作的轻量级「标记语言」，它用简洁的语法代替排版，而不像一般我们用的字处理软件 Word 或 Pages 有大量的排版、字体设置。它使我们专心于码字，用「标记」语法，来代替常见的排版格式，优点如下

* 专注你的文字内容而不是排版样式，安心写作。
* 轻松的导出 HTML、PDF 和本身的 .md 文件。
* 纯文本内容，兼容所有的文本编辑器与字处理软件。
* 随时修改你的文章版本，不必像字处理软件生成若干文件版本导致混乱。
* 可读、直观、学习成本低。

标题只要在这段文字前加 # 号即可
# 一级标题
## 二级标题
### 三级标题

列表的显示只需要在文字前加上 +, - 或 * 即可变为无序列表，有序列表则直接在文字前加1. 2. 3. 符号要和文字之间加上一个字符的空格
* item 1
* item 2
1. item 1
2. item 2

引用只需要在文本前加入 > 这种尖括号即可
>这里是引用  
*注意尖括号和引用内容之间以有空格*

缩进用多个>尖括号：  
>数据结构
>>线性表
>>>链表
>>>>单链表


插入链接  
[BAIDU](https://www.baidu.com)  
[Google](https://www.google.com)  

插入图片的语法和链接很像，多了一个 !号  
![mark_icon](https://timgsa.baidu.com/timg?image&quality=80&size=b10000_10000&sec=1504491447&di=a212e399c6a3c35d2c71352c83f8651d&src=http://img.phperz.com/data/icon/14166289897448.jpg)  
![baidu](http://www.baidu.com/img/bdlogo.gif)

用两个 * 或 _ 包含一段文本就是粗体的语法   
 **这是粗体显示**
 __这是粗体显示__

用一个 * 或 _ 包含一段文本就是斜体的语法  
*这是斜体显示*  
_这是斜体显示_

文本划线用两个\~\~包裹文本    
~~绕树三匝，何枝可依~~

分割线的语法只需要三个 *, -, _ 号
***   
-----
_____

反斜杠和转义字符  
\\   反斜线  
`   反引号  
\*   星号  
_   底线  
{}  花括号  
[]  方括号  
()  括弧  
\#   井字号  
\+   加号  
\-   减号  
.   英文句点  
!   惊叹号  

>原始MarkDown语法不支持，仅扩展支持如下表格，故此处可能显示有误  

| 省名          | 省会         | 区号 |  
| 陕西          | 西安         | 029|  
| 湖北          | 武汉         | 027|  


引用代码只需要用两个 ` 把中间的代码包裹起来  

`@Override
    protected void onResume() {
        super.onResume();
        mHandler.postDelayed(mElectronicUpdate, 500);
    }`


Fenced Code Block，写法是：第一行和最后一行都是3个 \`，中间的行是代码  
```
    @Override
    protected void onPause() {
        super.onPause();
        mHandler.removeCallbacks(mElectronicUpdate);
    }
```

代码差异可以用在三个\`\`\`后加diff，并且内容中每行加+或-：  
``` diff
-       mCallBacks = (Callbacks)getActivity();
+       mCallBacks = (Callbacks)context;
```

锚点：  
[回到顶部](#readme)
