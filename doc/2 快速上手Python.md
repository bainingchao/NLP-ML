# <center> 第 2 章 快速上手Python </center>


> **导读**：Python作为一门简洁优美且功能强大的语言，越来越受编程人员的喜欢。在工业界和学术界也是非常受欢迎的编程语言。本书的全部代码也都是python实现的，之所以选择python语言，因为其可以跨平台跨应用开发，因此本章旨在帮助读者快速领略python之概貌。如果读者具备python基础，可略过此章。本章首先介绍Python语言及其可以做什么事情。哪些人群适合学习python和python语法特点。其次介绍了Python进阶，以实际案例演示常用的语句和控制流、表达式、函数、数据结构、标准库等知识点。然后扩展介绍了python第三方库，使读者对python有个全面的理解和认识。最后一节，采用实际案例帮助读者综合运用python知识。 

## 2.1 初识Python编程语言
### 2.1.1 Python概述

> Python介绍

Python是一种面向对象、直译式的计算机程序语言。它包含了一组功能完备的标准库，能够轻松完成很多常见的任务。它的语法简单，与其它大多数程序设计语言使用大括号不一样，它使用缩进来定义语句块。Python同样是一种动态语言，具备垃圾回收功能，能够自动管理内存使用。它经常被当作脚本语言用于处理系统管理任务和网络程序编写，然而它也非常适合完成各种高级任务。Python支持命令式程序设计、面向对象程序设计、函数式编程、面向侧面的程序设计、泛型编程多种编程范式。Python是完全面向对象的语言。函数、模块、数字、字符串都是对象。并且完全支持继承、重载、派生、多重继承，有益于增强源代码的复用性。Python支持重载运算符，因此Python也支持泛型设计。

> Python发展历史

Python的创始人是Guido van Rossum。1989年的圣诞节期间，Guido van Rossum为了在阿姆斯特丹打发时间，决心开发一个新的脚本解释程序，作为ABC语言的一种继承。之所以选中Python作为程序的名字，是因为他是BBC电视剧——蒙提·派森的飞行马戏团（Monty Python's Flying Circus）的爱好者。ABC是由Guido参加设计的一种教学语言。就Guido本人看来，ABC这种语言非常优美和强大，是专门为非专业程序员设计的。但是ABC语言并没有成功，究其原因，Guido认为是非开放造成的。吉多决心在Python中避免这一错误，并获取了非常好的效果，完美结合了C和其他一些语言。就这样，Python在吉多手中诞生了。目前Guido仍然是Python的主要开发者，决定整个Python语言的发展方向。Python社区经常称呼他是仁慈的独裁者。

> Python标准库的主要功能

- 文本处理，包含文本格式化、正则表达式匹配、文本差异计算与合并、Unicode支持，二进制数据处理等功能。
- 文件处理，包含文件操作、创建临时文件、文件压缩与归档、操作配置文件等功能。
- 操作系统功能，包含线程与进程支持、IO复用、日期与时间处理、调用系统函数、日志（logging）等功能。
- 网络通信，包含网络套接字，SSL加密通信、异步网络通信等功能。
- 网络协议，支持HTTP，FTP，SMTP，POP，IMAP，NNTP，XMLRPC等多种网络协议，并提供了编写网络服务器的框架。
- W3C格式支持，包含HTML，SGML，XML的处理。
- 其它功能，包括国际化支持、数学运算、HASH、Tkinter等。

> Python优缺点

(1) 优点

- 简单、易学、免费、开源、高层语言（无需考虑如何管理你的程序使用的内存等细节。
- 可移植性（这些平台包括Linux、Windows、FreeBSD、Macintosh、Solaris、OS/2、Amiga、AROS、AS/400、BeOS、OS/390、z/OS、Palm OS、QNX、VMS、Psion、Acom RISC OS、VxWorks、PlayStation、Sharp Zaurus、Windows CE、PocketPC、Symbian以及Google基于linux开发的android平台
- 解释性、面向对象、可扩展性（可以部分程序用C或C++编写，然后在Python程序中使用它们。
- 可嵌入性（可以把Python嵌入C/C++程序，从而向程序用户提供脚本功能。）丰富的库、规范的代码。

(2) 缺点

- 单行语句和命令行输出问题、独特的语法、运行速度慢（与C和C++相比。

> Python开发环境

通用IDE / 文本编辑器，很多并非集成开发环境软件的文本编辑器，也对Python有不同程度的支持。本文默认开发环境均集成在Anaconda中，第1章已经详细介绍过。此外，还有如下开发环境：

- Eclipse + pydev插件，目前对Python 3.X只支持到3.0
- emacs +插件
- NetBeans +插件
- SlickEdit
- TextMate
- Python Tools for Visual Studio
- Vim +插件
- Sublime Text +插件
- EditPlus
- UltraEdit
- PSPad
- Editra由Python开发的程序编辑器。
- Notepad++  

### 2.1.2 Python能做什么？
> Python能做什么

1. 系统编程：提供API，能方便进行系统维护和管理，很多系统管理员理想的编程工具 。
1. 图形处理：有PIL、Tkinter等图形库支持，能方便进行图形处理。
1. 数学处理：NumPy扩展提供大量与许多标准数学库的接口。
1. 文本处理：python提供的re模块能支持正则表达式，还提供SGML，XML分析模块，许多程序员利用python进行XML程序的开发。
1. 数据库编程：程序员可通过遵循Python DB-API（数据库应用程序编程接口）规范的模块与Microsoft SQL Server，Oracle，Sybase，DB2，MySQL、SQLite等数据库通信。python自带有一个Gadfly模块，提供了一个完整的SQL环境。
1. 网络编程：提供丰富的模块支持sockets编程，能方便快速地开发分布式应用程序。
1. Web编程：应用的开发语言，支持最新的XML技术。
1. 多媒体应用：能进行二维和三维图像处理。PyGame模块可用于编写游戏软件。
1. 黑客编程：python有一个hack的库,内置你熟悉的或不熟悉的函数，但是缺少成就感。

> Python开发的应用案例

1. Reddit - 社交分享网站
1. Dropbox - 文件分享服务
1. 豆瓣网 - 图书、唱片、电影等文化产品的资料数据库网站
1. Django - 鼓励快速开发的Web应用框架
1. Pylons - Web应用框架
1. Zope - 应用服务器
1. Plone - 内容管理系统
1. TurboGears - 另一个Web应用快速开发框架
1. Twisted - Python的网络应用程序框架
1. Fabric - 用于管理成百上千台Linux主机的程序库
1. Python Wikipedia Robot Framework - MediaWiki的机器人程序
1. MoinMoinWiki - Python写成的Wiki程序
1. Trac - 使用Python编写的BUG管理系统
1. Mailman - 使用Python编写的邮件列表软件
1. Mezzanine - 基于Django编写的内容管理系统系统
1. flask - Python微Web框架
1. Webpy - Python微Web框架
1. Bottle - Python微Web框架
1. EVE - 网络游戏EVE大量使用Python进行开发
1. Blender - 使用Python作为建模工具与GUI语言的开源3D绘图软件
1. Inkscape - 一个开源的SVG矢量图形编辑器。
1. 知乎 - 一个问答网站
1. 果壳 - 一个泛科技主题网站

### 2.1.3 Python适合谁去学？

> 知乎精选：

于这个问题，我先带着大家去知乎看看，大家感兴趣可以去知乎搜索下，基本上语调是一致的。笔者本人而言，本科主要net技术研究，在C#学习上花费很多精力和时间。后来读研初期又开始java方面学习。虽说技不压身，但是总是因为研究方向的客观变化去转战于不同语言之间，外加语言环境平台还是浪费了不少时间的，且均没有深入下去。反之，python的跨平台性就优势凸显了，你习惯Linux命令行，完全可以适应。接近伪代码的操作为你节省不少时间，特别在文本处理，自然语言分析方面，笔者之前用java编写，耗费一番功夫。总而言之，园子里面，多数同学为本科在读生，在拥有一门入门语言的情况下，研究下python我觉得是值得的，也是大的趋势。无论你做运维或者web开发，亦或算法研究，大数据分析。前天与一家大数据公司技术负责人聊天，他们产品全是python，从文本处理到数据清洗分析，直到模型构建结果评价。读者也可以看看：我爱自然语言处理社区，里面无论求职数据挖掘、自然语言处理、机器学习等均要求python经验。
### 2.1.4 Python语法和特点
> Python基本语法

- 编码：默认情况下，Python 3 源码文件以 UTF-8 编码，所有字符串都是 unicode 字符串。 当然你也可以为源码文件指定不同的编码：
<pre>
# -*- coding: cp-1252 -*-
</pre>

- 标识符：
<pre>
在python里，标识符有字母、数字、下划线组成。
在python中，所有标识符可以包括英文、数字以及下划线（_），但不能以数字开头。
python中的标识符是区分大小写的。
以下划线开头的标识符是有特殊意义的。
以单下划线开头（_foo）的代表不能直接访问的类属性，需通过类提供的接口进行访问，不能用"from xxx import *"而导入.
以双下划线开头的（__foo）代表类的私有成员；以双下划线开头和结尾的（__foo__）代表python里特殊方法专用的标识。
</pre>

- python保留字：保留字即关键字，我们不能把它们用作任何标识符名称。
<pre>
>>> import keyword
>>> keyword.kwlist
['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue',
 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 
'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise',
 'return', 'try', 'while', 'with', 'yield']
</pre>

- 注释:Python中单行注释以 # 开头，实例如下：
<pre>
#!/usr/bin/python3

# 第一个注释
print ("Hello, Python!") # 第二个注释
</pre>

- 行与缩进:python最具特色的就是使用缩进来表示代码块，不需要使用大括号({})。四个空格或者Tab进行缩进。
<pre>
if True:
	print ("True")
else:
	print ("False")
</pre>

- 多行语句：Python 通常是一行写完一条语句，但如果语句很长，我们可以使用反斜杠(\)来实现多行语句，例如：
<pre>
total = item_one + \
        item_two + \
        item_three
</pre>

在 [], {}, 或 () 中的多行语句，不需要使用反斜杠(\)，例如：
<pre>
total = ['item_one', 'item_two', 'item_three',
        'item_four', 'item_five']
</pre>

- 引号:Python 接收单引号(' )，双引号(" )，三引号(''' """) 来表示字符串，引号的开始与结束必须的相同类型的。
<pre>
word = 'word'
sentence = "这是一个句子。"
paragraph = """这是一个段落。
包含了多个语句"""
</pre>
- 字符串
<pre>
python中单引号和双引号使用完全相同。
使用三引号('''或""")可以指定一个多行字符串。
转义符 '\'
自然字符串， 通过在字符串前加r或R。 如 r"this is a line with \n" 则\n会显示，并不是换行。
python允许处理unicode字符串，加前缀u或U， 如 u"this is an unicode string"。
字符串是不可变的。
按字面意义级联字符串，如"this " "is " "string"会被自动转换为this is string。
</pre>

- 空行
<pre>
函数之间或类的方法之间用空行分隔，表示一段新的代码的开始。类和函数入口之间也用一行空行分隔，以突出函数入口的开始。
</pre>

- Print 输出:print 默认输出是换行的，如果要实现不换行需要在变量末尾加上 end=""：
<pre>
#!/usr/bin/python3

x="a"
y="b"
# 换行输出
print( x )
print( y )

print('---------')
# 不换行输出
print( x, end=" " )
print( y, end=" " )
print()
</pre>
运行结果：

	a
	b
	---------
	a b


- import 与 from...import:在 python 用 import 或者 from...import 来导入相应的模块。


	(1) 将整个模块(somemodule)导入，格式为： import somemodule
	
	(2) 从某个模块中导入某个函数,格式为： from somemodule import somefunction
	
	(3) 从某个模块中导入多个函数,格式为： from somemodule import firstfunc, secondfunc, thirdfunc
	
	(4) 将某个模块中的全部函数导入，格式为： from somemodule import *
<pre>
导入 sys 模块
import sys
print('================Python import mode==========================');
print ('命令行参数为:')
for i in sys.argv:
    print (i)
print ('\n python 路径为',sys.path)
</pre>
<pre>
导入 sys 模块的 argv,path 成员
from sys import argv,path  #  导入特定的成员
 
print('================python from import===================================')
print('path:',path) # 因为已经导入path成员，所以此处引用时不需要加sys.path
</pre>

> 数据类型

<center>
表1-1 python数据类型
<table>
<tbody valign="top" style="color: black; font-family: 宋体; font-size: 10pt;">
	<tr style="background: #5b9bd5; text-align:center;vertical-align: middle;font-weight: bold;">
	<td >类型</td>
	<td >描述</td>
	<td >例子</td>
	</tr>

	<tr style=" background: #deeaf6;">
	<td>str</td>
	<td>一个由字符组成的不可更改的有序列。在Python 3.x里，字符串由Unicode字符组成。</td>
	<td>Wikipedia、Wikipedia、Spanning、multiple、lines</td>
	</tr>

	<tr >
	<td>bytes</td>
	<td >一个由字节组成的不可更改的有序列。</td>
	<td >b'Some ASCII' b"Some ASCII"</td>
	</tr>

	<tr style="background: #deeaf6;">
	<td >list</td>
	<td >可以包含多种类型的可改变的有序列</td>
	<td >[4.0, 'string', True]</td>
	</tr>
	
	<tr>
	<td >tuple</td>
	<td >可以包含多种类型的不可改变的有序列</td>
	<td>(4.0, 'string', True)</td>
	</tr>
	
	<tr style="background: #deeaf6;">
	<td >set/frozenset</td>
	<td >与数学中集合的概念类似。无序的、每个元素唯一。</td>
	<td >{4.0, 'string', True}/frozenset([4.0, 'string', True])</td>
	</tr>
	
	<tr style="">
	<td>dict或map</td>
	<td >一个可改变的由键值对组成的无序列。</td>
	<td >{'key1': 1.0, 3: False}</td>
	</tr>
	
	<tr style="background: #deeaf6;">
	<td >int</td>
	<td >精度不限的整数</td>
	<td >42</td>
	</tr>
	
	<tr ><td >float</td>
	<td >浮点数。精度与系统相关。</td>
	<td >3.1415927</td>
	</tr>
	
	<tr style="background: #deeaf6;">
	<td >complex</td>
	<td >复数</td>
	<td >3+2.7j</td>
	</tr>
	
	<tr>
	<td >bool</td>
	<td >逻辑值。只有两个值：真、假</td>
	<td>True   False</td>
	</tr>
</tbody>
</table>

</center>

## 2.2 Python进阶
### 2.2.1 Hello World

编程第一步，打印“Hello World”的输入结果：
<pre>
def callHello():
    print("hello world！")

callHello()
</pre>
运行结果：

	hello world！
### 2.2.2 语句和控制流

- if 语句::根据成绩评判等级
<pre>
# if 语句:根据成绩评判等级
def CallLevel(score):
    if score >= 90 :
        print("优秀")
    elif score >= 60:
        print("及格")
    else:
        print("不及格")
CallLevel(score=60)
</pre>
运行结果：

	及格

- for 语句:循环输出所有评分指标
<pre>
# for 语句:循环输出所有评分指标
def GetLevel(score):
    for lev in score:
        print(lev,end=" ") # 设置不换行
GetLevel(score=["优秀","及格","不及格"]) # 列表参数
</pre>
运行结果：

	优秀 及格 不及格

- while 语句:循环输出所有评分
<pre>
# while 语句:循环输出所有评分
def GetLevel2(score):
    countlen=len(score)
    while countlen > 0:
        print(score[countlen-1],end=" ") # 设置不换行
        countlen -= 1

GetLevel2(score=[90,30,100,98,60])
</pre>
运行结果：

	60 98 100 30 90 

- range() 函数:循环输出所有评分指标的下标
<pre>
# range() 函数:循环输出所有评分指标的下标
def GetValue(score):
    for lev in range(len(score)):
        print(lev,end=" ")
GetValue(score=["优秀","及格","不及格"])
</pre>
运行结果：

	0 1 2 

- break 语句：统计优秀学生的个数
<pre>
# break 语句:不及格的跳过
def GetHighLev(score):
    result=0
    for lev in score:
        if lev < 90:
            break
        else:
            result += 1
    print("成绩优秀的学生有："+str(result)+"位。")

GetHighLev(score=[90,30,100,98,60])
</pre>
运行结果：

	成绩优秀的学生有：1位。
	
	分析：实际优秀者个数是90,100,98共计3位，输出结果却是1位。造成这种结果的原因是，当循环输入列表90时候，满足条件自动加1.继续输入30，不满足条件，直接跳出整个程序，输出最后一条语句。



- continue 语句：统计优秀成绩的个数
<pre>
# continue 语句:统计优秀成绩的个数
def GetHighLev2(score):
    result=0
    for lev in score:
        if lev < 90:
            continue
        else:
            result += 1
    print("成绩优秀的学生有："+str(result)+"位。")

GetHighLev2(score=[90,30,100,98,60])
</pre>
运行结果：

	成绩优秀的学生有：3位。

- pass 语句：什么也不做，占位符
<pre>
# pass 语句：什么也不做，占位符
def callPass():
    pass
print(callPass())
</pre>
运行结果：

	None


### 2.2.3 函数
- 定义函数：斐波那契数列
<pre>
# 输出指定数的斐波那契数列
def fib(n):
    a, b = 0, 1
    while a < n:
        print(a, end=' ')
        a, b = b, a+b
    print()
fib(100)
</pre>
运行结果：

	 0 1 1 2 3 5 8 13 21 34 55 89 
结果分析：

关键字 def 引入了一个函数定义。在其后必须跟有函数名和包括形式参数的圆括号。函数体语句从下一行开始，必须是缩进的。一个函数定义会在当前符号表内引入函数名。函数名指代的值（即函数体）有一个被 Python 解释器认定为用户自定义函数的类型。

- 函数默认参数
<pre>
# 函数默认参数
def sayhello(name="Tom"):
    print("Hello,"+name)

sayhello()
</pre>
运行结果：

	Hello,Tom

- 关键字参数
<pre>
# 关键字参数
def person(name, age, **kw):  #前两个是必须参数，最后一个可选可变参数
    print('name:', name, 'age:', age, 'other:', kw)

person("Tome",30) # 只调用必须参数
person("Tom",30,city="ChengDu",sex="man") # 自定义关键字参数
</pre>
运行结果：

	name: Tome age: 30 other: {}
	name: Tom age: 30 other: {'sex': 'man', 'city': 'ChengDu'}

- 可变参数
<pre>
# 可变参数
def concat(*args, sep="/"):
    print(sep.join(args))
concat('我','是','可变','参数')
</pre>
运行结果：

	我/是/可变/参数

- Lambda 形式
<pre>
# Lambda 形式
def Lambda(nums):
    nums.sort(key=lambda num: num[0])
    print(nums)

Lambda(nums = [(1, 'one'), (2, 'two'), (3, 'three'), (4, 'four')])
</pre>
运行结果：

	[(1, 'one'), (2, 'two'), (3, 'three'), (4, 'four')]

### 2.2.4 List 列表
- list常用方法
<pre>
list.append(x)    添加元素到列表尾部。
list.extend(L)    列表合并。
list.insert(i, x) 在指定位置插入一个元素。
list.remove(x)    删除列表中值为 x 的第一个元素。
list.pop([i])     从列表的指定位置删除元素，并将其返回。
list.clear()      从列表中删除所有元素。相当于 del a[:]。
list.index(x)     返回列表中第一个值为 x 的元素的索引。
list.count(x)     返回 x 在列表中出现的次数。
list.sort()       对列表中的元素就地进行排序。
list.reverse()    就地倒排列表中的元素。
list.copy()       返回列表的一个浅拷贝。等同于 a[:]。
</pre>

- 列表的切分
<pre>
# 列表的切分
def calllist(names):
    print(names[-1:]) # 输出列表最后一个值
    print(names[:3])  # 输出列表前3个值
calllist(names=['this','is','a','list'])
</pre>

运行结果：

	['list'] 
	['this', 'is', 'a']

- List :列表作堆栈(先进先出)
<pre>
# 把列表当作堆栈使用
def SomeList(stack):
    print("原始列表（栈）：",end=' ')
    print(stack)
    stack.append('贺知章')
    stack.append('杜牧')
    print("追加后列表（栈）：",end=' ')
    print(stack)
    stack.pop()
    stack.pop()
    print("出栈后的数据：",end=' ')
    print(stack)

SomeList(stack=['李白','杜甫', '白居易'])
</pre>

运行结果：(先进先出)

	原始列表（栈）： ['李白', '杜甫', '白居易']
	追加后列表（栈）： ['李白', '杜甫', '白居易', '贺知章', '杜牧']
	出栈后的数据： ['李白', '杜甫', '白居易']

- List :列表作队列(先进后出)
<pre>
# 把列表当作队列使用：使用队列时调用collections.deque，它为在首尾两端快速插入和删除而设计。
from collections import deque
def SomeList2(queue):
    print("原始列表：",end=' ')
    print(queue)
    queue.append("李商隐")
    queue.append("杜牧")
    print("入队的列表：",end=' ')
    print(queue)
    queue.popleft()
    queue.popleft()
    print("出队后列表：",end=' ')
    print(queue)

SomeList2(queue = deque(['李白','杜甫', '白居易']))
</pre>

运行结果：(先进后出)

	原始列表： deque(['李白', '杜甫', '白居易'])
	入队的列表： deque(['李白', '杜甫', '白居易', '李商隐', '杜牧'])
	出队后列表： deque(['白居易', '李商隐', '杜牧'])

- 列表推导式
<pre>
# 列表推导式
def callList(nums):
    squares = [n**2 for n in nums]
    print(squares)
callList(nums=[2,4,6,8])
</pre>

运行结果：

	[4, 16, 36, 64]

- 列表的矩阵转秩
<pre>
# 矩阵转秩
def countList(matrix):
    result = [[row[i] for row in matrix] for i in range(4)]
    print(result)

matrix = [
     [1, 2, 3, 4],
     [5, 6, 7, 8],
     [9, 10, 11, 12],
]
countList(matrix)
</pre>

运行结果：

	[[1, 5, 9], [2, 6, 10], [3, 7, 11], [4, 8, 12]]

### 2.2.5 元组

虽然元组和列表很类似，它们经常被用来在不同的情况和不同的用途。元组有很多用途。例如 (x, y) 坐标对，数据库中的员工记录等等。元组就像字符串， 不可变的。列表是可变的 ，它们的元素通常是相同类型的并通过迭代访问。

- 操作元组
<pre>
def calltuple(tuples):
    for t in tuples:
        print(t+"\t",end=" ")
    print()
calltuple(tuples=('百度','阿里巴巴','腾讯')) # 元组参数
</pre>

运行结果：

	百度	 阿里巴巴	 腾讯	

### 2.2.6 set集合

集合是一个无序不重复元素的集。基本功能包括关系测试和消除重复元素。集合对象还支持 union（联合），intersection（交），difference（差）和 sysmmetric difference（对称差集）等数学运算。

- 操作set集合
<pre>
def callset(basket):
    result= set(basket)
    print(result)

callset(basket = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'})
</pre>

运行结果：

	{'pear', 'orange', 'apple', 'banana'}

### 2.2.7 字典

理解字典的最佳方式是把它看做无序的键：值对（key:value 对）集合，键必须是互不相同的（在同一个字典之内）。一对大括号创建一个空的字典： {} 。初始化列表时，在大括号内放置一组逗号分隔的键：值对，这也是字典输出的方式。

- 操作字典
<pre>
def calldict(dicts):
    print("原始字典",end=' ')
    print(dicts)   # 原始字典
    dicts['欧阳修'] = '宋朝' # 追加字典
    print("追加后的字典",end=' ')
    print(dicts)    # 追加后的字典
    print("字典键的集合",end=' ')
    print(list(dicts.keys())) # 字典键的集合
    print("字典键的排序",end=' ')
    print(sorted(dicts.keys())) # 字典键的排序
    print("字典值的集合",end=' ')
    print(list(dicts.values())) # 字典值的集合

calldict(dicts = {'李白': '唐朝', '杜甫': '唐朝'})
</pre>

运行结果：

	原始字典 {'杜甫': '唐朝', '李白': '唐朝'}
	追加后的字典 {'杜甫': '唐朝', '李白': '唐朝', '欧阳修': '宋朝'}
	字典键的集合 ['杜甫', '李白', '欧阳修']
	字典键的排序 ['李白', '杜甫', '欧阳修']
	字典值的集合 ['唐朝', '唐朝', '宋朝']

### 2.2.8 面向对象编程：类

- 通过案例理解python中的类：

父类是动物类，有初始化函数，且有动物讲话的方法，子类是一个狗类，继承父类所有属性，并扩展自己方法，调用子类讲话方法，并直接调用父类讲话方法。
<pre>
"""
# 欢迎进入我的主页：http://www.cnblogs.com/baiboy/.
"""
class BaseAnimal: # 父类：动物
    def __init__(self,name,age): # 初始化方法：括号里是形参
        self.name=name
        self.age=age
    def speak(self): # 父类的行为方法
        print("我的名字是[ %s ],今年[ %d ]岁" %(self.name,self.age))


class SubDog(BaseAnimal): # 子类：小狗
    def __init__(self,name,age,say): # 初始化方法：括号里是形参
        BaseAnimal.__init__(self,name,age)
        self.say=say
        print("这是子类[ %s ]."%(self.name))
        print('_'*20+'调用子函数方法'+'_'*20)
    def talk(self):      # 子类的行为方法
        # BaseAnimal.speak(self) # 调用父类的行为方法
        print("我的名字是[ %s ],今年[ %d ]岁,我想说： %s" %(self.name,self.age,self.say))


ani=SubDog('dog',12,'汪汪...')
print(ani.talk())
print('_'*20+'直接调用父函数方法'+'_'*20)
BaseAnimal('tom',13).speak()
</pre>

运行结果：

	这是子类[ dog ].
	 
	____________________调用子函数方法____________________
	
	我的名字是[ dog ],今年[ 12 ]岁,我想说： 汪汪...
	
	____________________直接调用父函数方法____________________
	
	我的名字是[ tom ],今年[ 13 ]岁

解析： __ init __ 方法（双下划线）：__ init __ 方法在类的一个对象被建立时，马上运行。这个方法可以用来对你的对象初始化。
注意，这个名称的开始和结尾都是双下划线。我们把__init__方法定义为取一个参数name（以及普通的参数self）。在__ init __ 方法里，我们只是创建一个新的域，也称为name。注意:它们是两个不同的变量，尽管它们有相同的名字。点号使我们能够区分它们。最重要的是，在创建一个类的新实例的时候，把参数包括在圆括号内跟在类名后面，从而传递给 __ init __ 方法。这是这种方法的重要之处。现在，我们能够在我们的方法中使用self.name域。给C++/Java/C#程序员的注释 __ init __ 方法类似于C++、C#和Java中的constructor 。


### 2.2.9 标准库

Python拥有一个强大的标准库。Python语言的核心只包含数字、字符串、列表、字典、文件等常见类型和函数，而由Python标准库提供了系统管理、网络通信、文本处理、数据库接口、图形系统、XML处理等额外的功能。
Python标准库的主要功能有：

1. 文本处理，包含文本格式化、正则表达式匹配、文本差异计算与合并、Unicode支持，二进制数据处理等功能
1. 文件处理，包含文件操作、创建临时文件、文件压缩与归档、操作配置文件等功能
1. 操作系统功能，包含线程与进程支持、IO复用、日期与时间处理、调用系统函数、日志（logging）等功能
1. 网络通信，包含网络套接字，SSL加密通信、异步网络通信等功能
1. 网络协议，支持HTTP，FTP，SMTP，POP，IMAP，NNTP，XMLRPC等多种网络协议，并提供了编写网络服务器的框架
1. W3C格式支持，包含HTML，SGML，XML的处理。
1. 其它功能，包括国际化支持、数学运算、HASH、Tkinter等

Python社区提供了大量的第三方模块，使用方式与标准库类似。它们的功能覆盖科学计算、Web开发、数据库接口、图形系统多个领域。第三方模块可以使用Python或者C语言编写。SWIG,SIP常用于将C语言编写的程序库转化为Python模块。Boost C++ Libraries包含了一组库，Boost.Python，使得以Python或C++编写的程序能互相调用。Python常被用做其他语言与工具之间的“胶水”语言。
## 2.3 Python深入--第三方库	
### 2.3.1 Web框架
- Django： 开源Web开发框架，它鼓励快速开发,并遵循MVC设计，开发周期短。
- Flask：  轻量级的Web框架。
- Pyramid： 轻量，同时有可以规模化的Web框架，Pylon projects 的一部分。
- ActiveGrid： 企业级的Web2.0解决方案。
- Karrigell： 简单的Web框架，自身包含了Web服务，py脚本引擎和纯python的数据库PyDBLite。
- Tornado： 一个轻量级的Web框架，内置非阻塞式服务器，而且速度相当快
- webpy： 一个小巧灵活的Web框架，虽然简单但是功能强大。
- CherryPy： 基于Python的Web应用程序开发框架。
- Pylons： 基于Python的一个极其高效和可靠的Web开发框架。
- Zope： 开源的Web应用服务器。
- TurboGears： 基于Python的MVC风格的Web应用程序框架。
- Twisted： 流行的网络编程库，大型Web框架。
- Quixote： Web开发框架。
### 2.3.2 科学计算
- Matplotlib： 用Python实现的类matlab的第三方库，用以绘制一些高质量的数学二维图形。
- Pandas： 用于数据分析、数据建模、数据可视化的第三方库。
- SciPy： 基于Python的matlab实现，旨在实现matlab的所有功能。
- NumPy： 基于Python的科学计算第三方库，提供了矩阵，线性代数，傅立叶变换等等的解决方案。
### 2.3.3 GUI
- PyGtk： 基于Python的GUI程序开发GTK+库。
- PyQt： 用于Python的QT开发库。
- WxPython： Python下的GUI编程框架，与MFC的架构相似。
### 2.3.4 其他库
- BeautifulSoup： 基于Python的HTML/XML解析器，简单易用。
- gevent： python的一个高性能并发框架,使用了epoll事件监听、协程等机制将异步调用封装为同步调用。
- PIL： 基于Python的图像处理库，功能强大，对图形文件的格式支持广泛。目前已无维护，另一个第三方库Pillow实现了对PIL库的支持和维护。
- PyGame： 基于Python的多媒体开发和游戏软件开发模块。
- Py2exe： 将python脚本转换为windows上可以独立运行的可执行程序。
- Requests： 适合于人类使用的HTTP库，封装了许多繁琐的HTTP功能，极大地简化了HTTP请求所需要的代码量。
- scikit-learn： 机器学习第三方库，实现许多知名的机器学习算法。
- TensorFlow： Google开发维护的开源机器学习库。
- Keras： 基于TensorFlow，Theano与CNTK的高级神经网络API。
- SQLAlchemy： 关系型数据库的对象关系映射(ORM)工具

##	2.4 Python实战：Django轻松搞定用户管理系统
### 2.4.1 Django简介
> Django是什么

Django是一个开放源代码的Web应用框架，由Python写成。采用了MVC的软件设计模式，即模型M，视图V和控制器C。它最初是被开发来用于管理劳伦斯出版集团旗下的一些以新闻内容为主的网站的。并于2005年7月在BSD许可证下发布。这套框架是以比利时的吉普赛爵士吉他手Django Reinhardt来命名的。 Django的主要目标是使得开发复杂的、数据库驱动的网站变得简单。Django注重组件的重用性和“可插拔性”，敏捷开发和DRY法则（Don't Repeat Yourself）。在Django中Python被普遍使用，甚至包括配置文件和数据模型。

> Django开发模型

Django是一个基于MVC构造的框架。但是在Django中，控制器接受用户输入的部分由框架自行处理，所以 Django 里更关注的是模型（Model）、模板(Template)和视图（Views），称为 MTV模式。它们各自的职责如图2-1 所示：
<center>

![](https://i.imgur.com/smjaw0A.png)

图2-1 Django开发模型图
</center>

1. 模型（Model），即数据存取层 处理与数据相关的所有事务： 如何存取、如何验证有效性、包含哪些行为以及数据之间的关系等。
1. 视图（View），即表现层 处理与表现相关的决定： 如何在页面或其他类型文档中进行显示。
1. 模板(Template)，即业务逻辑层 存取模型及调取恰当模板的相关逻辑。模型与模板的桥梁。

> Django的架构

让我们一览 Django 全貌：

- urls.py 网址入口，关联到对应的views.py中的一个函数（或者generic类），访问网址就对应一个函数。
- views.py 处理用户发出的请求，从urls.py中对应过来, 通过渲染templates中的网页可以将显示内容，比如登陆后的用户名，用户请求的数据，输出到网页。
- models.py 与数据库操作相关，存入或读取数据时用到这个，当然用不到数据库的时候 你可以不使用。
- forms.py 表单，用户在浏览器上输入数据提交，对数据的验证工作以及输入框的生成等工作，当然你也可以不使用。
- templates 文件夹 views.py 中的函数渲染templates中的Html模板，得到动态内容的网页，当然可以用缓存来提高速度。
- admin.py 后台，可以用很少量的代码就拥有一个强大的后台。
- settings.py Django 的设置，配置文件，比如 DEBUG 的开关，静态文件的位置等。

上面的py文件不理解也没有关系，后面会详细介绍。一图胜千言，架构全貌工作机制如图2-2所示：

<center>

![](https://i.imgur.com/XUfmzHe.png)

图2-2 Django架构图

</center>

> Django商业网站

Sohu 邮箱  、果壳网  、 豆瓣  、 爱调研 、 易度在线云办公 、 优容网  、 快玩游戏、九九房、贷帮网 、 趣奇网 、知乎、时尚时空 、游嘻板: YxPad webpy、DNSPod 国际版 、下厨房  、 贝太厨房 、 Wopus问答 、 咕咚网 、扇贝网 、站长工具、易度文档管理系统、个人租房、 在线文档查看-易度云查看 、 FIFA310 足球数据分析专家、 搜狐随身看等等。


### 2.4.2 Django安装配置
> 前置条件

- 假设读者具备Python、web开发、html、css、js、SQL基础。
- Anaconda(包含pip和python插件)、sublime环境已经安装。其中pip用来在线安装工具包。
- 系统环境：WIN10 64bit
- 开发环境：sublime+Anaconda
- 数据库：Mysql 5.6.17
- 语言：python3.5
- 框架：django1.11

通过“Win+R”键打开运行对话框，输入“pip”查看是否安装成功。如果pip输入报错，则需要自行下载安装即可。如果成功安装如图2-3所示：
<center>
![](https://i.imgur.com/rboSP9T.png)

图2-3 pip安装成功图
</center>


> 在线安装Django

通过“Win+R”键打开运行对话框，输入“pip install django”代码，自动运行结束后。打开Sublime编辑器，点击“F6”切换的编辑环境，输入如下代码查看django是否安装成功。

<pre>
>>> import django
>>> django.VERSION
(1, 11, 0, 'final', 1)
</pre>

### 2.4.3 创建用户管理项目
> 创建项目和App

（1） 通过“Win+R”键打开运行对话框，并在电脑的E盘根目录下创建名为UserProject的项目,输入如下创建命名：
<pre>
django-admin startproject xmjc_analysis
</pre>
命令执行完成，通过Sublime Text3打开菜单“File->Open Folder”选择刚刚创建的UserProject文件夹，如图2-4所示：
<center>
![](https://i.imgur.com/h0AgYXf.png)

图2-4 新建django项目
</center>

- settings.py 项目的设置文件
- urls.py 总的urls配置文件
- wsgi.py 部署服务器文件
- __ init__.py python包的目录结构必须的，与调用有关


（2）  进入UserProject文件夹下创建App名为myuser，执行如下命令，命令成功后如图2-5所示：
<pre>
django-admin startapp myuser
</pre>
<center>

![](https://i.imgur.com/Bc6jJGN.png)

图2-5 执行app创建命令
</center>

一个项目可以包含多个App，执行完app创建命令后，打开项目查看如图2-6所示：
<center>

![](https://i.imgur.com/2yOopSh.png)

图2-6 创建app成功图
</center>

- admin.py  后台，可以用很少量的代码就拥有一个强大的后台。
- apps.py   本app项目名称等配置。
- models.py 与数据库操作相关，存入或读取数据时用到这个，当然用不到数据库的时候 你可以不使用。
- tests.py  单元测试文件
- views.py  处理用户发出的请求，从urls.py中对应过来, 通过渲染templates中的网页可以将显示内容，比如登陆后的用户名，用户请求的数据，输出到网页。

（3） 将新定义名为“myuser”的app添加到UserProject项目中。修改UserProject/UserProject/settings.py代码如下：

<pre>
# Application definition

INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',

    # 添加新建app
    'myuser',
]
</pre>

到此，完成项目的创建和app的添加。是不是很简单，下面我们创建一个新的欢迎界面。

> 第一个欢迎页面

（1） 在myuser文件夹下，打开UserProject/myuser/views.py文件,修改里面的代码如下：
<pre>
'''
第一个页面
author：白宁超
site：http://www.cnblogs.com/baiboy/
'''
#coding:utf-8
from django.shortcuts import render
from django.http import HttpResponse

def index(request):
    return HttpResponse(u"欢迎进入第一个Django页面!")
</pre>

第一行是声明编码为utf-8, 因为我们在代码中用到了中文,如果不声明就报错.

第二行引入HttpResponse，它是用来向网页返回内容的，就像Python中的 print 一样，只不过 HttpResponse 是把内容显示到网页上。

我们定义了一个index()函数，第一个参数必须是 request，与网页发来的请求有关，request 变量里面包含get或post的内容。

（2）我们打开UserProject/UserProject/urls.py 这个文件, 修改其中的代码

<pre>
from django.conf.urls import url
from django.contrib import admin

# 导入myuser下的视图文件
from myuser import views as myuser_views


urlpatterns = [
    # 第一个欢迎界面的配置
    url(r'^index/$', myuser_views.index,name='index'),

    url(r'^admin/', admin.site.urls),
]
</pre>

（3） 在UserProject目录下输入“python manage.py runserver”命令本地运行服务器，如图2-7所示：

<center>
![](https://i.imgur.com/fwjrzhr.png)

图2-7 运行本地服务器
</center>

（4） 将图2-7的本地网址复制到浏览器访问，本地网址后面输入刚刚配置的方法名“index”即可访问我们刚刚设计的网页。如图2-8所示：

<center>

![](https://i.imgur.com/JbWX3aW.png)

图2-8 django运行的欢迎界面
</center>

> 带参数的欢迎页面

（1） 打开UserProject/myuser/views.py文件,修改里面的代码如下：
<pre>
'''
#coding:utf-8
from django.shortcuts import render
from django.http import HttpResponse

# 访问第一个页面
def index(request):
    return HttpResponse(u"欢迎进入第一个Django页面!")

# 访问第一个带参数的页面
def indexPara(request):
    name = request.GET['name']
    return HttpResponse(u"欢迎进入\t"+name+",第一个Django页面!")
</pre>

（2）我们打开UserProject/UserProject/urls.py 这个文件, 修改其中的代码

<pre>
from django.conf.urls import url
from django.contrib import admin

# 导入myuser下的视图文件
from myuser import views as myuser_views

urlpatterns = [
    # 带参数的欢迎界面的配置
    url(r'^para/$', myuser_views.indexPara,name='para'),
    # 第一个欢迎界面的配置
    url(r'^index/$', myuser_views.index,name='index'),

    url(r'^admin/', admin.site.urls),
]
</pre>
（3） 如果服务器关闭，需要如上方法重新打开。反之，直接输入网址查看，如图2-9所示：

<center>

![](https://i.imgur.com/CGTI72H.png)

图2-9 django运行带参数的欢迎界面
</center>

> 单数据库配置

（1） 在UserProject/UserProject/settings.py文件下,默认sqlites数据库，现在假设项目需求是mysql数据库。具体修改如下：

<pre>
# Database
# https://docs.djangoproject.com/en/1.11/ref/settings/#databases

DATABASES = {
    # 配置默认为mysql数据库
    'default': {
        'ENGINE': 'django.db.backends.mysql', # 设置数据库引擎
        'NAME': 'test',                       # 数据库名
        'USER': 'test',                       # 数据库登陆名
        'PASSWORD': 'test123',                # 数据库登陆密码
        'HOST':'localhost',                   # 数据库服务器IP，默认设置本地
        'PORT':'3306',                        # 端口号
    },

    # 默认配置为sqlite3数据库
    # 'default': {
    #     'ENGINE': 'django.db.backends.sqlite3',
    #     'NAME': os.path.join(BASE_DIR, 'db.sqlite3'),
    # }
}
</pre>

UserProject/UserProject/__ init__.py文件添加如下代码：
<pre>
import pymysql
pymysql.install_as_MySQLdb()
</pre>
（2） 在UserProject/myuser/models.py下设计数据库表，采用ORM方式，完整代码如下：
<pre>
from django.db import models
 
# Create your models here.
class User(models.Model):
    username = models.CharField('用户名', max_length=30)
    userpass = models.CharField('密码',max_length=30)
    useremail = models.EmailField('邮箱',max_length=30)
    usertype = models.CharField('用户类型',max_length=30)
 
    def __str__(self):
        return self.username
</pre>

（3） 在analysis/admin.py中定义显示数据

<pre>
from django.contrib import admin
from .models import User
 
class UserAdmin(admin.ModelAdmin):
    list_display = ('username','userpass','useremail') # 自定义显示字段
 
admin.site.register(User,UserAdmin)
</pre>

（4） 打开对话框，在“UserProject”下将生成的py文件应用到mysql数据库。输入如下命令：
<pre>
python manage.py makemigrations
python manage.py migrate
</pre>
运行效果如果2-10所示：
<center>

![](https://i.imgur.com/CblSJwf.png)

图2-10 ORM创建单例MySQL数据库
</center>

（5）创建超级管理员：用户名，admin1；密码密码：admin123，如图2-11、2-12所示
<pre>
python manage.py createsuperuser
</pre>

<center>

![](https://i.imgur.com/7YJgJ9v.png)

图2-11 创建后台超级管理员
</center>

<center>

![](https://i.imgur.com/P8o9jPw.png)

图2-12 创建后台超级管理员
</center>
（6）登录后台查看信息

可以看到后台信息，并对数据表进行增删改查操作，但是后台全部英文如图2-13所示，可以改为中文显示？

<center>

![](https://i.imgur.com/SWDbf6o.png)

图2-13 英文管理界面
</center>
后台管理设置为中文显示,UserProject/UserProject/settings.py下修改代码：
<pre>LANGUAGE_CODE = 'zh-Hans' # 中文显示</pre>
再去查看：
<center>

![](https://i.imgur.com/yCz4Atj.png)

图2-14 中文后台管理界面
</center>



### 2.4.4 Django数据库操作

> QuerySet API，shell玩转MySql

在UserProject项目下输入【 python manage.py shell】，然后查询数据表如图2-15所示：

<center>

![](https://i.imgur.com/MwMAay7.png)

图2-15 Shell操作MySQL数据库
</center>

创建一条用户信息，输入如下shell命令：
<pre>
User.objects.create(username="李白", userpass="libai123",useremail="libai@163.com",usertype="超级管理员")

</pre>
登录项目后台查看，如图2-16所示。

<center>
![](https://i.imgur.com/tDHK2vF.png)

图2-16 后台查看新加用户信息
</center>

> 其他shell操作语句

<pre>
# 方法 1
User.objects.create(username="李白", userpass="libai123",useremail="libai@163.com",usertype="超级管理员")
# 方法 2
twz =User(username="李白", userpass="libai123",useremail="libai@163.com",usertype="超级管理员")
twz.save()
# 获取对象：
Person.objects.all()
# 满足条件查询
User.objects.filter(username="李白")
# 迭代查询：
es = Entry.objects.all()
for e in es:
    print(e.headline)
# 查询排序：
User.objects.all().order_by('username')
# 链式查询：
User.objects.filter(name__contains="WeizhongTu").filter(email="tuweizhong@163.com")
# 去重查询：
qs = qs.distinct()
# 删除操作：
User.objects.all().delete()
# 更新操作：
Person.objects.filter(name__contains="abc").update(name='xxx')
# 数据的导出：
python manage.py dumpdata [appname] > appname_data.json
python manage.py dumpdata blog > blog_dump.json
# 导出用户数据
python manage.py dumpdata auth > auth.json # 导出用户数据
</pre>



> 批量向数据表导入数据

（1） 将name.txt导入数据库，数据内容如下：
<pre>
张一|admin|zhang1@qq.com|超级管理员
张二|admin|zhang2@qq.com|超级管理员
张三|admin|zhang3@qq.com|超级管理员
张四|admin|zhang4@qq.com|超级管理员
张五|admin|zhang5@qq.com|超级管理员
张六|admin|zhang6@qq.com|超级管理员
张七|admin|zhang7@qq.com|超级管理员
张八|admin|zhang8@qq.com|超级管理员
张九|admin|zhang9@qq.com|超级管理员
</pre>

（2） 文本数据批量导入mysql数据库中，核心源码如下：
<pre>
def main():
    from analysis.models import User
    f = open('./readme/files/name.txt',encoding='utf-8')
    for line in f:
        name,pwd,email,type = line.split('|')
        User.objects.create(username=name,userpass=pwd,useremail=email,usertype=type)
    f.close()
</pre>

重新登录“用户信息管理后台”，查看结果如图2-17所示：


<center>
![](https://i.imgur.com/g99epdw.png)

图2-17 导入文本数据到数据库
</center>

源码请访问github（[[https://github.com/BaiNingchao/NLPDome/blob/master/01chapter.zip](https://github.com/BaiNingchao/NLPDome/blob/master/01chapter.zip)]