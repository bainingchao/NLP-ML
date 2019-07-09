 # 自然语言处理理论与实战源码下载
 
> 机器学习和自然语言（QQ群号：436303759）是一个研究深度学习、机器学习、自然语言处理、数据挖掘、图像处理、目标检测、数据科学等AI相关领域的技术群。其宗旨是纯粹的AI技术圈子、绿色的交流环境。


## 内容介绍

本书分四个部分，第一部分主要介绍基础知识，包括认识机器学习和自然语言处理、快速上手Python、线性代数、概率论和统计学；第二部分主要介绍自然语言处理技术，包括自然语言处理介绍、语料库技术、中文分词、数据预处理、马尔科夫模型、条件随机场、模型评估、剖析自然处理工具背后的原理；第三部分主要介绍机器学习技术，包括认识机器学习、常见机器学习算法、机器学习算法案例源码实现。第四部分主要介绍工程项目实践，包括Python项目实战、自然语言处理项目实战、机器学习结合自然语言处理综合项目实战。




# 自然语言处理理论与实战修正

> 本书源码下载地址： <https://github.com/BaiNingchao/NLP-ML/> 

（1）页码：30  •  行数：10

堆栈应该是后进先出，队列应该是先进先出

![img](http://download.broadview.com.cn/Original/19030c92007afb783abd)

（2）页码：42  •  行数：倒数第一  

设向量a（x1,y1）向量b（x2,y2），若向量a平行向量b 则x1y2=y1x2 （内向等于外向），而不是**x1y1=y2x2**

（3）页码：45    行数：10  

数乘向量的消去律(2)修改为：

![1562661058162](https://github.com/bainingchao/imgurl/blob/master/typoraImg/20190709/1562661058162.png?raw=true)

​                                           

（4）页码：46   行数：13 

向量积运算率第二条修改如下：

   ![1562661092346](https://github.com/bainingchao/imgurl/blob/master/typoraImg/20190709/1562661092346.png?raw=true)

（5）页码：76   行数：第8行 

![1562661120585](https://github.com/bainingchao/imgurl/blob/master/typoraImg/20190709/1562661120585.png?raw=true)

 （6）页码：187 行数：7-11行

Jar包和相关文件。后面修正为：

- Jar1.8下载：可以到‘[软件必备包下载](https://github.com/BaiNingchao/NLP-ML/blob/master/08chapter/%E8%BD%AF%E4%BB%B6%E5%8C%85%E4%B8%8B%E8%BD%BD.txt).txt’下载。

- nltk-develop下载：可以到‘[软件必备包下载](https://github.com/BaiNingchao/NLP-ML/blob/master/08chapter/%E8%BD%AF%E4%BB%B6%E5%8C%85%E4%B8%8B%E8%BD%BD.txt).txt’下载。

- stanfordNLP下载：作者已经封装在‘[软件必备包下载](https://github.com/BaiNingchao/NLP-ML/blob/master/08chapter/%E8%BD%AF%E4%BB%B6%E5%8C%85%E4%B8%8B%E8%BD%BD.txt).txt’，下文讲解具体配置。

首先下载jar1.8和nltk-develop并安装成功后，将tools拷贝都E盘，或者读者自定义盘符下，运行即可。以上软件包下载地址：<https://github.com/bainingchao/NLP-ML/blob/master/08chapter/%E8%BD%AF%E4%BB%B6%E5%8C%85%E4%B8%8B%E8%BD%BD.txt>

（7） 页码：187 行数：倒数第5行

图片更换为：  

![1562661307912](https://github.com/bainingchao/imgurl/blob/master/typoraImg/20190709/1562661307912.png?raw=true)

（8）页码：188 行数：1-12行

- 句法分析依赖：stanford-parser.jar、stanford-parser-3.9.1-models.jar、classifiers。

- 依存句法分析依赖：stanford-parser.jar、stanford-parser-3.9.1-models.jar、classifiers。

压缩包和源码分析：（选学内容）

- 分词压缩包：StanfordSegmenter和StanfordTokenizer:下载stanford-segmenter-2015-12-09.zip (<https://pan.baidu.com/s/1kVc20ib>)，解压获取目录中的 stanford-segmenter-3.6.0.jar 拷贝为 stanford-segmenter.jar和 slf4j-api.jar

- 词性标注压缩包：下载stanford-postagger-full-2015-12-09.zip (https://pan.baidu.com/s/1hrVMSE4) 解压获取stanford-postagger.jar

- 命名实体识别压缩包：下载stanford-ner-2015-12-09.zip (https://pan.baidu.com/s/1skOJb5r)，将解压获取stanford-ner.jar和classifiers文件

- 句法分析、句法依存分析：下载stanford-parser-full-2015-12-09.zip (http://pan.baidu.com/s/1nv6Q2bZ) 解压获取stanford-parser.jar 和 stanford-parser-3.6.0-models.jar

 （9）页码：192 -194

- E:\tools\stanfordNLTK\jar\stanford-parser-3.6.0-models.jar修改为：

E:\tools\stanfordNLTK\jar\stanford-parser-3.9.1-models.jar 

- E:\tools\stanfordNLTK\jar\stanford-parser-3.6.0-models.jar修改为：

E:\tools\stanfordNLTK\jar\stanford-parser-3.9.1-models.jar 

- E:\tools\stanfordNLTK\jar\stanford-parser-3.6.0-models.jar修改为：

E:\tools\stanfordNLTK\jar\stanford-parser-3.9.1-models.jar 

- E:\tools\stanfordNLTK\jar\stanford-parser-3.6.0-models.jar修改为：

E:\tools\stanfordNLTK\jar\stanford-parser-3.9.1-models.jar 

（10）页码：241  •  行数：1 

本章数据预处理部分，新增了数据预处理全过程的封装代码包：[数据预处理全过程代码封装](https://github.com/BaiNingchao/NLP-ML/blob/master/10chapter/text_preprocessing.py)
包括：

1. 高效的读取文本文件
2. 处理文本的HTML标签、特殊符号（如微博文本）
3. 分词去停用词
4. 特征词选取并转换成文本向量
5. 自定义规则提取特征词

![img](http://download.broadview.com.cn/Original/1807b735689c8584c790)



