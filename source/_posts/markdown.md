---
title: Markdown 语法手册
categories: 文档知识
tags: markdown
---

# 斜体和粗体 
```
*斜体*或_斜体_
**粗体**
***加粗斜体***
~~删除线~~
```
*斜体*或_斜体_
**粗体**
***加粗斜体***
~~删除线~~
*****

# 分级标题
```
# 分级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
*****

# 超链接
## 行内式
```
[我的博客](http://hedonglin.com)
[我的博客](http://hedonglin.com "标题提示")
```
[我的博客](http://hedonglin.com)
[我的博客](http://hedonglin.com "标题提示")
## 参考式
```
我的网站[博客][1]、[博客2][2]、[笔记][3]还有个特殊的描述[百度][];
[1]:http:hedonglin.com "hedonglin博客"
[2]:http:w3c0929.com "资源博客"
[3]:http:www.w3c0929.com "www资源博客"
[百度]:htttp://www.baidu.com "百度"
```
我的网站[博客][1]、[博客2][2]、[笔记][3]还有个特殊的描述[百度][];
[1]:http://hedonglin.com "hedonglin博客"
[2]:http://w3c0929.com "资源博客"
[3]:http://www.w3c0929.com "www资源博客"
[百度]:https://www.baidu.com "百度"
*****

# 自动连接
```
<http://www.youku.com>
<http://hedonglin.com>
<w3c0929@163.com>
```
<http://www.youku.com>
<http://hedonglin.com>
<w3c0929@163.com>
*****

# 锚点
```
[锚点](#jump)
<span id = "jump">跳转到这里</span>
```
[锚点](#jump)
<span id = "jump">跳转到这里</span>
*****

# 列表
## 无序列表
```
注意：*号后面带一个空格
* 无序列表1
* 无序列表2
* 无序列表3
- 列表1
- 列表2
- 列表3
+ 列表1111
+ 列表2222
+ 列表3333
```
* 无序列表1
* 无序列表2
* 无序列表3
- 列表1
- 列表2
- 列表3
+ 列表1111
+ 列表2222
+ 列表3333

## 有序列表
```
注意：.号后面带一个空格
1. 列表1
2. 列表2
3. 列表3
```
1. 列表1
2. 列表2
3. 列表3
*****

# 列表缩进
```
注意：*号后面至少一个空格
* 窗前明月光，疑是地上霜。
举头望明月，低头思故乡。
```
* 窗前明月光，疑是地上霜。
举头望明月，低头思故乡。
*****

# 包含段落的列表
```
注意：分段之后也就是（"举"的前面至少要一个空格）
* 窗前明月光，疑是地上霜。

 举头望明月，低头思故乡。
```
* 窗前明月光，疑是地上霜。

 举头望明月，低头思故乡。
*****

# 包含引用的列表
```
注意：*号和>后面都带空格
* 阅读的方法:
> 打开书本。
> 打开电灯。
```
* 阅读的方法:
> 打开书本。
> 打开电灯。
*****

# 包含代码区块的引用
```
注意：缩进了2个制表符8个空格
        <代码写在这>
```
        <代码写在这>
*****

# 一个特殊情况
```
注意：数字后面如果带.那么就要跟一个\进行转义否则1986.就不会显示
1986\. What a great season.
```
1986\. What a great season.
*****

# 引用
```
注意：在开头添加>就变成引用了，最好在>后加一个空格
> 这就是引用
这就是引用

>这就是引用
这就是引用
```
> 这就是引用
这就是引用

>这就是引用
这就是引用
*****

# 引用的多层嵌套
```
注意：每段都隔一行，并且符号逐个减少
>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白
```
>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白
*****

# 引用其它要素
```
> 1.   这是第一行列表项。
2.   这是第二行列表项。

> 给出一些例子代码：

>     return shell_exec("echo $input | $markdown_script");
```
> 1.   这是第一行列表项。
2.   这是第二行列表项。

> 给出一些例子代码：

>       return shell_exec("echo $input | $markdown_script");

*****

# 插入图像
## 行内式
```
注意：文章多的时候一般图片采用绝对路径，查找方便不易丢失,第三种方式可以改变大小
![图片alt内容](/images/avatar.png)
![图片alt内容](/images/avatar.png "图片title")
<img src="/images/avatar.png" alt="图片" />
```
![图片alt内容](/images/avatar.png)
![图片alt内容](/images/avatar.png "图片title")
<img src="/images/avatar.png" alt="图片" width="100" height="100"/>
## 参考式
```
![图片alt内容][flower]
[flower]:/images/avatar.png "图片title"
```
![图片alt内容][flower]
[flower]:/images/avatar.png "图片title"
*****
# 注脚
```
注意都需要脚注之间都要隔一行，此在next的markdown下没效果
今天[^1]的日子[^2]很灿烂[^Le]

[^1]:你是谁

[^2]:我是谁

[^Le]:到底是谁
```
今天[^1]的日子[^2]很灿烂[^Le]

[^1]:你是谁

[^2]:我是谁

[^Le]:到底是谁
*****

# LaTeX 公式
```
注意:此在next的markdown下没效果
$$\sum_{i=1}^n a_i=0$$

$$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$

$$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$
```
$$\sum_{i=1}^n a_i=0$$

$$f(x_1,x_x,\ldots,x_n) = x_1^2 + x_2^2 + \cdots + x_n^2 $$

$$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$
*****

# 流程图
```
flow
st=>start: Start:>https://www.zybuluo.com
io=>inputoutput: verification
op=>operation: Your Operation
cond=>condition: Yes or No?
sub=>subroutine: Your Subroutine
e=>end
st->io->op->cond
cond(yes)->e
cond(no)->sub->io
```
flow
st=>start: Start:>https://www.zybuluo.com
io=>inputoutput: verification
op=>operation: Your Operation
cond=>condition: Yes or No?
sub=>subroutine: Your Subroutine
e=>end
st->io->op->cond
cond(yes)->e
cond(no)->sub->io
*****

# 表格
```
注意：第二行为不同的列指定对齐方向。默认为左对齐，在-右边加上:就右对齐。-的两边都加:那么就是居中对齐
学号|姓名|分数
-|-|-
小明|男|75
小红|女|79
小陆|男|92

学号|姓名|分数
-:|-:|-:
小明|男|75
小红|女|79
小陆|男|92

学号|姓名|分数
:-:|:-:|:-:
小明|男|75
小红|女|79
小陆|男|92
```
学号|姓名|分数
-|-|-
小明|男|75
小红|女|79
小陆|男|92

学号|姓名|分数
-:|-:|-:
小明|男|75
小红|女|79
小陆|男|92

学号|姓名|分数
:-:|:-:|:-:
小明|男|75
小红|女|79
小陆|男|92
*****
# 分隔线
```
*****

* * * 

- - - 

-----
```
*****

* * * 

- - - 

-----

*****

# 代码块
```
注意：有三种方式
        两个制表符8个空格
我是一个`行内式`的代码
6个`包裹多行代码
```
        两个制表符8个空格
我是一个`行内式`的代码
6个`包裹多行代码

*****

# 内容目录
```
在段落中填写 [TOC] 以显示全文内容的目录结构，但此处没效果！
```
[TOC]
