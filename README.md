
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

<p>一级标题</p>
=============

<p>二级标题</p>
-------------
  
效果：
  
一级标题
=============

二级标题
-------------
  
任何数量的 = 和 - 都可以有效果。
  
  
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

