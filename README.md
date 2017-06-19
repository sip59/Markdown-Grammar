
## 1. Markdown是什么？
+ Markdown 是一个 Web 上使用的文本到HTML的转换工具，可以通过简单、易读易写的文本格式生成结构化的HTML文档。目前 github、Stackoverflow 等网站均支持这种格式。

## 2. Markdown的一些优点
+ **纯文本，所以兼容性极强，可以用所有文本编辑器打开。**
+ **让你专注于文字而不是排版。**
+ **格式转换方便，Markdown 的文本你可以轻松转换为 html、电子书等。**
+ **Markdown 的标记语法有极好的可读性。**

## 3. 常用的语法及例子
### 3.1 标题
Markdown 支持两种标题的语法，类 Setext 和类 atx 形式。
  
类 Setext 形式是用底线的形式，利用 = （最高阶标题）和 - （第二阶标题），例如：

    一级标题
    =============

    二级标题
    -------------
  
效果：
  
一级标题
=============

二级标题
-------------
  
任何数量的 = 和 - 都可以有效果。
  
<br>
  
类 Atx 形式则是在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶，例如：
<p>## 一级标题</p>
<p>## 二级标题</p>
<p>### 三级标题</p>
<p>#### 四级标题</p>
<p>##### 五级标题</p>
<p>###### 六级标题</p>

效果：
## 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题


### 3.2 区块引用
+ Markdown 标记区块引用是使用类似 email 中用 > 的引用方式。如果你还熟悉在 email 信件中的引言部分，你就知道怎么在 Markdown 文件中建立一个区块引用，那会看起来像是你自己先断好行，然后在每行的最前面加上 > ：
<p>> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,</p>
<p>> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.<p/>
<p>> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.</p>
<p>></p>
<p>> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse</p>
<p>> id sem consectetuer libero luctus adipiscing.</p>
  
效果：
  
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
  <br>
Markdown 也允许你偷懒只在整个段落的第一行最前面加上 > ：
<p>> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,</p>
<p>consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.<p/>
<p>Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.</p>
  
<p>> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse</p>
<p>id sem consectetuer libero luctus adipiscing.</p>
  
效果：
  
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
  
  <br>
区块引用可以嵌套（例如：引用内的引用），只要根据层次加上不同数量的 > ：
<p> This is the first level of quoting.</p>
<p>></p>
<p>> > This is nested blockquote.</p>
<p>></p>
<p>> Back to the first level.</p>
  
效果：
  
 This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.
  
<br>
引用的区块内也可以使用其他的 Markdown 语法，包括标题、列表、代码区块等：
<p>> ## 这是一个标题。</p>
<p>> </p>
<p>> 1.   这是第一行列表项。</p>
<p>> 2.   这是第二行列表项。</p>
<p>> </p>
<p>> 给出一些例子代码：</p>
<p>> </p>
<p>>     return shell_exec("echo $input | $markdown_script");</p>
  
效果：
  
> ## 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");
  
任何像样的文本编辑器都能轻松地建立 email 型的引用。例如在 BBEdit 中，你可以选取文字后然后从选单中选择增加引用阶层。
  
  
### 3.3 列表
Markdown 支持有序列表和无序列表。
  
无序列表使用星号（*）、加号（+）或是减号（-）作为列表标记：
> \* Big<br>
> \* Middle<br>
> \* Small<br>

等同于：
> \+ Big<br>
> \+ Middle<br>
> \+ Small<br>

也等同于：
> \- Big<br>
> \- Middle<br>
> \- Small<br>
  
效果：
* Big
* Middle
* Small
  
有序列表则使用数字接着一个英文句点：
<p> 1. Bird</p>
<p> 2. McHale</p>
<p> 3. Parish</p>
  
效果:
  
1. Bird
2. McHale
3. Parish
  
列表项目标记通常是放在最左边，但是其实也可以缩进，最多 3 个空格，项目标记后面则一定要接着至少一个空格或制表符。

要让列表看起来更漂亮，你可以把内容用固定的缩进整理好：
<p>*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.</p>
<p>    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,</p>
<p>    viverra nec, fringilla in, laoreet vitae, risus.</p>
<p>    > This is a blockquote</p>
<p>    ></p>
<p>    > inside a list item.</p>
<p>*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.</p>
<p>    Suspendisse id sem consectetuer libero luctus adipiscing.</p>
  
效果：
*   Lorem ipsum dolor sit amet, consectetuer adipiscing elit.
    Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi,
    viverra nec, fringilla in, laoreet vitae, risus.
    > This is a blockquote
    >
    > inside a list item.
*   Donec sit amet nisl. Aliquam semper ipsum sit amet velit.
    Suspendisse id sem consectetuer libero luctus adipiscing.

    
### 3.4 代码区块
和程序相关的写作或是标签语言原始码通常会有已经排版好的代码区块，通常这些区块我们并不希望它以一般段落文件的方式去排版，而是照原来的样子显示，Markdown 会用 \<pre> 和 \<code> 标签来把代码区块包起来。

要在 Markdown 中建立代码区块很简单，只要简单地缩进 4 个空格或是 1 个制表符就可以，例如，下面的输入：

    <pre><code>
    public static String logTimeOfDay(long millis) {
        Calendar c = Calendar.getInstance();
        if (millis >= 0) {
            c.setTimeInMillis(millis);
            return String.format("%tm-%td %tH:%tM:%tS.%tL", c, c, c, c, c, c);
        } else {
            return Long.toString(millis);
        }
    }
    </code></pre>

效果：
<pre><code>public static String logTimeOfDay(long millis) {
    Calendar c = Calendar.getInstance();
    if (millis >= 0) {
        c.setTimeInMillis(millis);
        return String.format("%tm-%td %tH:%tM:%tS.%tL", c, c, c, c, c, c);
    } else {
        return Long.toString(millis);
    }
}
</code></pre>
  
### 3.5 分隔线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：

    ***
    * * *
    ******
    - - - -
    -------------
    _ _ _ _
    _______

效果：
***
* * *
******
- - - -
-----------
_ _ _ _
_______

  
### 3.6 链接
Markdown 支持两种形式的链接语法： 行内式和参考式两种形式。
不管是哪一种，链接文字都是用 [方括号] 来标记。
行内式链接，只要在方块括号后面紧接着圆括号并插入网址链接即可，如果你还想要加上链接的 title 文字，只要在网址后面，用双引号把 title 文字包起来即可，例如：
  
<p>This is [an example](http://example.com/ "Title") inline link.</p>
  
效果：
This is [an example](http://example.com/ "Title") inline link.

  
参考式链接，是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记：
  
    This is [an example][id] reference-style link.
  
你也可以选择性地在两个方括号中间加上一个空格：
  
    This is [an example] [id] reference-style link.
  
接着，在文件的任意处，你可以把这个标记的链接内容定义出来：

    [id]: http://example.com/  "Optional Title Here"
  
  
例子：
  
    [lugl1]:http://www.google.com/ "Google"
    This is [Google site][lugl1].
  
效果：
  
[lugl1]:http://www.google.com/ "Google"
This is [Google site][lugl1].

  
### 3.7 代码
  
如果要标记一小段行内代码，你可以用反引号把它包起来（`），例如：
  
    Use the `printf()` function.
  
效果：
  
Use the `printf()` function.
  
如果要在代码区段内插入反引号，你可以用多个反引号来开启和结束代码区段：
  
    ``There is a literal backtick (`) here.``
  
效果：
  
``There is a literal backtick (`) here.``
  

### 3.8 图片
很明显地，要在纯文字应用中设计一个「自然」的语法来插入图片是有一定难度的。

Markdown 使用一种和链接很相似的语法来标记图片，同样也允许两种样式： 行内式和参考式。
  
行内式的图片语法看起来像是：

    ![小猪佩奇](https://github.com/sip59/Markdown-Grammar/blob/master/peppa_pig2.jpg)
![小猪佩奇](https://github.com/sip59/Markdown-Grammar/blob/master/peppa_pig2.jpg)

    ![小猪佩奇](/peppa_pig.jpg "peppa pig")
![小猪佩奇](/peppa_pig.jpg "peppa pig")
  

参考式的图片语法则长得像这样：
  
> ![Alt text][id]
>
> 「id」是图片参考的名称，图片参考的定义方式则和链接参考一样：
>
> \[id]: url/to/image  "Optional title attribute"

例子：
>    \[pig4]: https://github.com/sip59/Markdown-Grammar/blob/master/peppa_pig3.jpg "peppa=pig"
>
>    \![小猪佩奇]\[pig4]

[pig4]: https://github.com/sip59/Markdown-Grammar/blob/master/peppa_pig3.jpg "peppa=pig"
![小猪佩奇][pig4]
  
  
### 3.9 其他
反斜杠
Markdown 可以利用反斜杠来插入一些在语法中有其它意义的符号，例如：如果你想要用星号加在文字旁边的方式来做出强调效果，你可以在星号的前面加上反斜杠：
  
  
例子：
  
\\\*I like star.\\\*
  
效果：
  
\*I like star.\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：
  
    \   反斜线
    `   反引号
    *   星号
    _   底线
    {}  花括号
    []  方括号
    ()  括弧
    #   井字号
    +   加号
    -   减号
    .   英文句点
    !   惊叹号


自动链接
Markdown 支持以比较简短的自动链接形式来处理网址和电子邮件信箱，只要是用方括号包起来， Markdown 就会自动把它转成链接。一般网址的链接文字就和链接地址一样.
  
例如：
  
    <http://www.google.com>
  
    <lugl1@motorola.com>
  
效果：
  
<http://www.google.com>
  
<lugl1@motorola.com>



