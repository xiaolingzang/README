MY Test
===========================
该文件用来测试和展示书写README的各种markdown语法。GitHub的markdown语法在标准的markdown语法基础上做了扩充，称之为`GitHub Flavored Markdown`。简称`GFM`，GFM在GitHub上有广泛应用，除了README文件外，issues和wiki均支持markdown语法。

#### Author:zangxiaoling
#### Email:1550539332@qq.com

##目录
* [横线](#横线)
* [标题](#标题)
* [文本](#文本)
    * 普通文本
    * 单行文本
    * 多行文本
    * 文字高亮
    * 换行
    * 斜体
    * 粗体
    * 删除线
 * [图片](#图片)
    * 来源于网络的图片
    * GitHub仓库中的图片
 * [链接](#链接)
     * 文字超链接
        * 链接本库中的URL
       * 链接外部的URL
    * 描点
		* [图片链接](#图片链接)
* [列表](#列表)
    * 无序列表
    * 有序列表
    * 复选框列表
* [块引用](#块引用)
* [代码高亮](#代码高亮)
* [表格](#表格) 
* [表情](#表情)
* [diff语法](#diff语法)

### 横线
-----------
***、---、___可以显示横线效果
***
---
____

标题
---------
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题

文本
-----
### 普通文本
这是一段普通文本
### 单行文本
    Hello，大家好。
### 文本块
#### 语法1
	欢迎到访
	很高心见到你
	祝您，身体健康，往事如意。
#### 语法二
使用一对各三个的反引号：
```
欢迎到访
我是学生
正在学习github的使用
```
该语法也可以实现代码高亮，见[代码高亮](#代码高亮)
### 文字高亮
文字高亮功能能使行内部分文字高亮，使用一对反引号。
语法：
```
`linux` `网络编程`
```
### 换行
直接回车不能换行，
可以在上一行文本后面补两个空格，  
这样下一行的文本就换行了。

或者就是在两行文本直接加一个空行。

也能能够实现换行，不过这个行间距有点大。*联系*
### 斜体、粗体、删除线
|语法|效果|
|----|----|
|`*斜体1*`|*斜体*|
|`_斜体2_`|_斜体_|
|`**粗体1**`|**粗体1**|
|`__粗体2__`|__粗体__|
|`这是一个 ~~删除线~~`|这是一个~~删除线~~|
|`***斜粗体1***`|***斜粗体1***|
|`___斜粗体2___`|___斜粗体2___|
|`***~~斜粗体删除线1~~***`|***~~斜粗体删除线1~~***|
|`~~***斜粗体删除线2***~~`|~~***斜粗体删除线2***~~|

图片
-----
基本格式：
```
![alt](URL title)
```
![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo")
![foryou](https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif)

链接
### 链接外部URL
|#|语法|效果|
|---|----|-----|
|1|`[我的博客](http://blog.csdn.net/guodongxiaren "悬停显示")`|[我的博客](http://blog.csdn.net/guodongxiaren "悬停显示")|
|2|`[我的知乎][zhihu] `|[我的知乎][zhihu] |

语法2由两部分组成：  
第一部分使用两个中括号，[ ]里的标识符（本例中zhihu），可以是数字，字母等的组合，标识符上下对应就行了（**姑且称之为URL标识符**）
第二部分标记实际URL。

### 链接本库中的URL
|语法|效果|
|----|-----|
|`[我的简介](/example/profile.md)`|[我的简介](/example/profile.md)|
|`[Book](./Book)`|[Book](/Book)|


### 图片链接
给图片加链接的本质是混合图片显示语法和普通的链接语法。普通的链接中[ ]内部是链接要显示的文本，而图片链接[ ]里面则是要显示的图片。  
直接混合两种语法当然可以，但是十分啰嗦，为此我们可以使用URL标识符的形式。

|#|语法|效果|
|---|----|:---:|
|1|`[![weibo-logo]](http://weibo.com/linpiaochen)`|[![weibo-logo]](http://weibo.com/linpiaochen)|
|2|`[![](/img/zhihu.png "我的知乎，欢迎关注")][zhihu]`|[![](/img/zhihu.png "我的知乎，欢迎关注")][zhihu]|
|3|`[![csdn-logo]][csdn]`|[![csdn-logo]][csdn]|


##列表
### 无序列表
* 昵称：lingling
- 别名：Markov
* 英文名：Jelly

### 多级无序列表
* 编程语言
    * 脚本语言
        * python
	
### 有序列表
面向对象的三个基本特性：  
1. 封装
2. 继承
3. 多态

### 有序列表自动排序
面向对象的七大原则：  
1. 开闭原则
2. 里氏转换原则
* 依赖倒转原则
* 接口隔离原则
* 组合/聚合复用原则
* “迪米特”法则

### 多级有序列表
1. 这是一级有序列表
    1. 这是二级有序列表
        1. 这是三级有序列表
	
### 复选框列表
- [x] 需求分析
- [x] 系统设计
- [x] 详细设计
- [ ] 编码
- [ ] 测试
- [ ] 交付

您可以使用这个功能来标注某个项目各项任务的完成情况。
> Tip:
>> 在GitHub的**issue**中使用该语法是可以实时点击复选框来勾选或解除勾选的，而无需修改issue原文。


### 块引用
#### 文本摘自《深入理解计算机系统》P27
　令人吃惊的是，在哪种字节顺序是合适的这个问题上，人们表现得非常情绪化。实际上术语“little endian”（小端）和“big endian”（大端）出自Jonathan Swift的《格利佛游记》一书，其中交战的两个派别无法就应该从哪一端打开一个半熟的鸡蛋达成一致。因此，争论沦为关于社会政治的争论。只要选择了一种规则并且始终如一的坚持，其实对于哪种字节排序的选择都是任意的。
> **“端”（endian）的起源**  
以下是Jonathan Swift在1726年关于大小端之争历史的描述：  
“……下面我要告诉你的是，Lilliput和Blefuscu这两大强国在过去36个月里一直在苦战。战争开始是由于以下的原因：我们大家都认为，吃鸡蛋前，原始的方法是打破鸡蛋较大的一端，可是当今的皇帝的祖父小时候吃鸡蛋，一次按古法打鸡蛋时碰巧将一个手指弄破了，因此他的父亲，当时的皇帝，就下了一道敕令，命令全体臣民吃鸡蛋时打破较小的一端，违令者重罚。”

### 块引用有多级结构
> 数据结构
>> 树
>>> 二叉树
>>>> 平衡二叉树
>>>>> 满二叉树


代码高亮
----------
在三个反引号后面加上编程语言的名字，另起一行开始写代码，最后一行再加上三个反引号。
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "hello GitHub" #Bash
```
```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; //javascipt
```
```cpp
string &operator+(const string& A,const string& B) //cpp
```

表格
--------

表头1  | 表头2|
--------- | --------|
表格单元  | 表格单元 |
表格单元  | 表格单元 |

| 表头1  | 表头2|
| ---------- | -----------|
| 表格单元   | 表格单元   |
| 表格单元   | 表格单元   |

### 对齐
表格可以指定对齐方式

| 左对齐 | 居中  | 右对齐 |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
### 混合其他语法
表格单元中的内容可以和其他大多数GFM语法配合使用，如：  
#### 使用普通文本的删除线，斜体等效果

| 名字 | 描述          |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |
#### 表格中嵌入图片（链接）
其实前面介绍图片显示、图片链接的时候为了清晰就是放在在表格中显示的。

| 图片 | 描述 |
| ---- | ---- |
|![baidu][baidu-logo] | 百度|

diff语法
---------
版本控制的系统中都少不了diff的功能，即展示一个文件内容的增加与删除。
GFM中可以显示的展示diff效果。使用绿色表示新增，红色表示删除。

其语法与代码高亮类似，只是在三个反引号后面写diff，
并且其内容中，以 `+ `开头表示新增，`- `开头表示删除。

效果如下：

```diff
+ 鸟宿池边树，僧敲月下门
- 鸟宿池边树，僧推月下门
```



--------------------------------
[csdn]:http://blog.csdn.net/guodongxiaren "我的博客"
[zhihu]:https://www.zhihu.com/people/jellywong "我的知乎，欢迎关注"
[weibo]:http://weibo.com/linpiaochen
[baidu-logo]:http://www.baidu.com/img/bdlogo.gif "百度logo"
[weibo-logo]:/img/weibo.png "点击图片进入我的微博"
[csdn-logo]:/img/csdn.png "我的CSDN博客"
[foryou]:https://github.com/guodongxiaren/ImageCache/raw/master/Logo/foryou.gif
