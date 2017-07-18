标题只要在这段文字前加 # 号即可
# 一级标题
## 二级标题
### 三级标题

列表的显示只需要在文字前加上 +, - 或 * 即可变为无序列表，有序列表则直接在文字前加1. 2. 3. 符号要和文字之间加上一个字符的空格
* item 1
* item 2
1. item 1
2. item 2

引用只需要在文本前加入 > 这种尖括号（大于号）即可
> 这里是引用  

*注意尖括号和引用内容之间以有空格*

插入链接与插入图片的语法很像，区别在一个 !号  
[BAIDU](https://www.baidu.com)  
[Google](https://www.google.com)  
![mark_icon](http://img0.imgtn.bdimg.com/it/u=288426133,3294142091&fm=26&gp=0.jpg)  


用两个 * 包含一段文本就是粗体的语法  
 **这是粗体显示**  
 __这是粗体显示__

用两个 * 包含一段文本就是斜体的语法  
*这是斜体显示*  
_这是斜体显示_

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

原始MarkDown语法不支持，仅扩展支持如下表格，故此处可能显示有误
| 省名          | 省会         | 区号 |
| ------------- | -------------| -----|
| 陕西          | 西安         | 029|
| 湖北          | 武汉         | 027|


引用代码只需要用两个 ` 把中间的代码包裹起来  

`@Override
    protected void onResume() {
        super.onResume();
        mHandler.postDelayed(mElectronicUpdate, 500);
    }`
    
还有块代码(block code)的写法：代码每一行的前面都加4个空格或一个tab  
    private Handler mHandler;
    private Runnable mR = new Runnable() {
    public void run() {                       showResultDialog(getString(R.string.charger_info));
        }
    };

还有一种Fenced Code Block，写法是：第一行和最后一行都是3个 " ` "，中间的行是代码，

```
    @Override
    protected void onPause() {
        super.onPause();
        mHandler.removeCallbacks(mElectronicUpdate);
    }
```