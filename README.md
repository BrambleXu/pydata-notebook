# 利用Python进行数据分析 2017 第二版 （Python for Data Analysis, 2nd Edition）笔记

这里是作者的[英文版github地址](https://github.com/wesm/pydata-book)

可以直接购买英文版：[Buy the book on Amazon][1]

> 2017第二版主要更新：
>1. 所有代码，包括Python教程，都升级到了Python3.6（第一版用的是Python2.7）
>2. 更新了Python的安装介绍。这次改用Anaconda Python发行版，以及其他一些需要的Python包
>3. 使用了最新的2017版pandas
>4. 新增了一章，用来介绍pandas的高级应用工具，和其他一些有用的小贴士
>5. 简单介绍了如何使用statsmodels和scikit-learn


作者[Wes McKinney](https://github.com/wesm)是pandas的创作者，所以说，还有什么比作者本人来直接告诉你pandas哪些用法更实用的呢。

这本书自2013年第一版发行后，就广受好评。最近打算把这本书完整过一遍，顺便通过jupyter记录下笔记分享给大家。

我在做第一版第三章的笔记时，才发现作者已经在2017年推出了第二版，不过暂时还没有中文版。
所以这里我打算直接把书里的内容翻译成中文，做一个简洁版的Notebook版本。

第一版的时候作者用的是Python2，不过随着Python2的维护年限将近（2020），以及Python3的推广，整个社群向Python3转变已经成为不可扭转的趋势。
所以在第二版里，作者使用了Python3.6。而我实际写的代码则是基于Python3.5，使用上没有任何差别。

在写笔记的时候，我尽量写中文，不过有一些专有名字我是直接写英文，然后配上中文翻译，毕竟有时候知道英文单词的话查找英文的文档也方便一些，而且我相信这样做对提升中文和英文专业名字的对照关系有帮助。毕竟在程序员的世界里，不懂英语会很艰难，即使是一些简单的单词，也是我们走向新世界的起点。

另外我并不是逐字逐句翻译，因为这样翻译出来的结果就是洋味十足，看不懂。我尽量按方便理解的方式进行翻译，其他一些没有用的话我不进行翻译，就像上面说的，这是一个简洁版的笔记，只翻译书中有用的东西。

如果觉得有帮助的话，就点个Star吧：）

## IPython Notebooks:

* [Chapter 2: Python Language Basics, IPython, and Jupyter Notebooks (Python语言基础，Ipython和Jupyter Notebooks)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-02/)
  - [chp02-Introduction(2013)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/chp02-Introduction%282013%29.ipynb)
  - [2.2 IPython Basics (IPython基础)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/2.2%20IPython%20Basics.ipynb)
  - [2.3 Python语言基础)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/2.3%20Python%E8%AF%AD%E8%A8%80%E5%9F%BA%E7%A1%80.ipynb)


* [Chapter 3: Built-in Data Structures, Functions, and Files (内建数据结构，函数和文件)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-03/)
  - [3.1 Data Structures and Sequences (数据结构与序列)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.1%20Data%20Structures%20and%20Sequences%20%28%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E5%BA%8F%E5%88%97%29.ipynb)
  - [3.2 Functions (函数)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.2%20Functions%20%28%E5%87%BD%E6%95%B0%29.ipynb)
  - [3.3 Files and the Operating System (文件以及操作系统)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.3%20Files%20and%20the%20Operating%20System%20%28%E6%96%87%E4%BB%B6%E4%BB%A5%E5%8F%8A%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F%29.ipynb)


* [Chapter 4: NumPy Basics: Arrays and Vectorized Computation(NumPy基础：数组和向量化计算)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-04/)
  - [4.1 The NumPy ndarray: A Multidimensional Array Object（ndarray: 多维数组对象)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.1%20The%20NumPy%20ndarray%EF%BC%88%E5%A4%9A%E7%BB%B4%E6%95%B0%E7%BB%84%E5%AF%B9%E8%B1%A1%EF%BC%89.ipynb)
  - [4.2 Universal Functions: Fast Element-Wise Array Functions（通用函数：快速点对点数组函数）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.2%20Universal%20Functions%20%28%E9%80%9A%E7%94%A8%E5%87%BD%E6%95%B0%29.ipynb)
  - [4.3 Array-Oriented Programming with Arrays（数组导向编程）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.3%20Array-Oriented%20Programming%20with%20Arrays%EF%BC%88%E6%95%B0%E7%BB%84%E5%AF%BC%E5%90%91%E7%BC%96%E7%A8%8B%EF%BC%89.ipynb)
  - [4.4 File Input and Output with Arrays（通过数组来进行文件的输入和输出）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.4%20File%20Input%20and%20Output%20with%20Arrays%EF%BC%88%E9%80%9A%E8%BF%87%E6%95%B0%E7%BB%84%E6%9D%A5%E8%BF%9B%E8%A1%8C%E6%96%87%E4%BB%B6%E7%9A%84%E8%BE%93%E5%85%A5%E5%92%8C%E8%BE%93%E5%87%BA%EF%BC%89.ipynb)
  - [4.5 Linear Algebra (线性代数)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.5%20Linear%20Algebra%20%28%E7%BA%BF%E6%80%A7%E4%BB%A3%E6%95%B0%29.ipynb)
  - [4.6 Pseudorandom Number Generation（伪随机数生成）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.6%20Pseudorandom%20Number%20Generation%EF%BC%88%E4%BC%AA%E9%9A%8F%E6%9C%BA%E6%95%B0%E7%94%9F%E6%88%90%EF%BC%89.ipynb)
  - [4.7 Example Random Walks（一个例子：随机漫步）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.7%20Example%20Random%20Walks%EF%BC%88%E4%B8%80%E4%B8%AA%E4%BE%8B%E5%AD%90%EF%BC%9A%E9%9A%8F%E6%9C%BA%E6%BC%AB%E6%AD%A5%EF%BC%89.ipynb)


* [Chapter 5: Getting Started with pandas（开始使用pandas）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-05/)
  - [5.1 Introduction to pandas Data Structures（pandas的数据结构）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.1%20Introduction%20to%20pandas%20Data%20Structures%EF%BC%88pandas%E7%9A%84%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%EF%BC%89.ipynb)
  - [5.2 Essential Functionality（主要功能）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.2%20Essential%20Functionality%EF%BC%88%E4%B8%BB%E8%A6%81%E5%8A%9F%E8%83%BD%EF%BC%89.ipynb)
  - [5.3 Summarizing and Computing Descriptive Statistics（汇总和描述性统计）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.3%20Summarizing%20and%20Computing%20Descriptive%20Statistics%EF%BC%88%E6%80%BB%E7%BB%93%E5%92%8C%E6%8F%8F%E8%BF%B0%E6%80%A7%E7%BB%9F%E8%AE%A1%EF%BC%89.ipynb)


* [Chapter 6: Data Loading, Storage, and File Formats（数据加载，存储，文件格式）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-06/)
  - [6.1 Reading and Writing Data in Text Format (以文本格式读取和写入数据)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-06/6.1%20Reading%20and%20Writing%20Data%20in%20Text%20Format%20%28%E4%BB%A5%E6%96%87%E6%9C%AC%E6%A0%BC%E5%BC%8F%E8%AF%BB%E5%8F%96%E5%92%8C%E5%86%99%E5%85%A5%E6%95%B0%E6%8D%AE%29.ipynb)
  - [6.2 Binary Data Formats (二进制数据格式)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-06/6.2%20Binary%20Data%20Formats%20%28%E4%BA%8C%E8%BF%9B%E5%88%B6%E6%95%B0%E6%8D%AE%E6%A0%BC%E5%BC%8F%29.ipynb)
  - [6.3 Interacting with Web APIs (网络相关的API交互)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-06/6.3%20Interacting%20with%20Web%20APIs%20%28%E7%BD%91%E7%BB%9C%E7%9B%B8%E5%85%B3%E7%9A%84API%E4%BA%A4%E4%BA%92%29.ipynb)
  - [6.4 Interacting with Databases(与数据库的交互)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-06/6.4%20Interacting%20with%20Databases%28%E4%B8%8E%E6%95%B0%E6%8D%AE%E5%BA%93%E7%9A%84%E4%BA%A4%E4%BA%92%29.ipynb)


* [Chapter 7: Data Cleaning and Preparation（数据清洗和准备）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-07/)
  - [7.1 Handling Missing Data（处理缺失数据）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-07/7.1%20Handling%20Missing%20Data%EF%BC%88%E5%A4%84%E7%90%86%E7%BC%BA%E5%A4%B1%E6%95%B0%E6%8D%AE%EF%BC%89.ipynb)
  - [7.2 Data Transformation（数据变换）
](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-07/7.2%20Data%20Transformation%EF%BC%88%E6%95%B0%E6%8D%AE%E5%8F%98%E6%8D%A2%EF%BC%89.ipynb)
  - [7.3 String Manipulation（字符串处理）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-07/7.3%20String%20Manipulation%EF%BC%88%E5%AD%97%E7%AC%A6%E4%B8%B2%E5%A4%84%E7%90%86%EF%BC%89.ipynb)


* [Chapter 8: Data Wrangling: Join, Combine, and Reshape](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-08/)
  - [8.1 Hierarchical Indexing（分层索引）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.1%20Hierarchical%20Indexing%EF%BC%88%E5%88%86%E5%B1%82%E7%B4%A2%E5%BC%95%EF%BC%89.ipynb)
  - [8.2 Combining and Merging Datasets（合并数据集）
  ](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.2%20Combining%20and%20Merging%20Datasets%EF%BC%88%E5%90%88%E5%B9%B6%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [8.3 Reshaping and Pivoting（整形和旋转）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.3%20Reshaping%20and%20Pivoting%EF%BC%88%E6%95%B4%E5%BD%A2%E5%92%8C%E6%97%8B%E8%BD%AC%EF%BC%89.ipynb)




<!--



* [Chapter 9: Plotting and Visualization]()
  - []()
  - []()
  - []()

* [Chapter 10: Data Aggregation and Group Operations]()
- []()
- []()
- []()

* [Chapter 11: Time Series]()
- []()
- []()
- []()

* [Chapter 12: Advanced pandas]()
- []()
- []()
- []()

* [Chapter 13: Introduction to Modeling Libraries in Python]()
- []()
- []()
- []()


* [Chapter 14: Data Analysis Examples]()
- []()
- []()
- []()


* [Appendix A: Advanced NumPy](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/appa.ipynb) -->

## License

### Code

The code in this repository, including all code samples in the notebooks listed
above, is released under the [MIT license](LICENSE-CODE). Read more at the
[Open Source Initiative](https://opensource.org/licenses/MIT).


[1]: http://amzn.to/2vvBijB
