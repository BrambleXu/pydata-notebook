# 利用Python进行数据分析 2017 第二版 （Python for Data Analysis, 2nd Edition）笔记

这里是作者的[英文版github地址](https://github.com/wesm/pydata-book)。

这本书自2013年第一版发行后，就广受好评。最近打算把这本书完整过一遍，顺便通过jupyter记录下笔记分享给大家。
不过在开始做第三章的笔记时，发现作者已经在2017推出了第二版，不过还没有中文版。
所以这里我打算直接把书里的内容翻译成中文，做一个简洁版的Notebook版本。

第一版的时候作者用的是Python2，不过随着Python2的维护年限将近（2020），以及Python3的推广，整个社群向Python3转变已经成为不可扭转的趋势。
所以在第二版里，作者使用了Python3.6。而我实际写的代码则是基于Python3.5，不过应该没什么差别就是了。

在写笔记的时候，我尽量写中文，不过有一些专有名字我是直接写英文，然后配上中文翻译，毕竟有时候知道英文单词的话查找英文的文档也方便一些，而且我相信这样做对提升中文和英文专业名字的对照关系有帮助。毕竟在程序员的世界里，不懂英语会很艰难，即使是一些简单的单词，也是我们走向新世界的起点。

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
  

* [Chapter 5: Getting Started with pandas](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-05/)
  - [5.1 Introduction to pandas Data Structures（pandas的数据结构）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.1%20Introduction%20to%20pandas%20Data%20Structures%EF%BC%88pandas%E7%9A%84%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%EF%BC%89.ipynb)
  - [5.2 Essential Functionality（主要功能）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.2%20Essential%20Functionality%EF%BC%88%E4%B8%BB%E8%A6%81%E5%8A%9F%E8%83%BD%EF%BC%89.ipynb)
  - [5.3 Summarizing and Computing Descriptive Statistics（汇总和描述性统计）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-05/5.3%20Summarizing%20and%20Computing%20Descriptive%20Statistics%EF%BC%88%E6%80%BB%E7%BB%93%E5%92%8C%E6%8F%8F%E8%BF%B0%E6%80%A7%E7%BB%9F%E8%AE%A1%EF%BC%89.ipynb)


<!--

* [Chapter 6: Data Loading, Storage, and File Formats]()
* [Chapter 7: Data Cleaning and Preparation]()
* [Chapter 8: Data Wrangling: Join, Combine, and Reshape]()
* [Chapter 9: Plotting and Visualization](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch09.ipynb)
* [Chapter 10: Data Aggregation and Group Operations](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch10.ipynb)
* [Chapter 11: Time Series](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch11.ipynb)
* [Chapter 12: Advanced pandas](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch12.ipynb)
* [Chapter 13: Introduction to Modeling Libraries in Python](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch13.ipynb)
* [Chapter 14: Data Analysis Examples](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/ch14.ipynb)
* [Appendix A: Advanced NumPy](http://nbviewer.ipython.org/github/pydata/pydata-book/blob/2nd-edition/appa.ipynb) -->

## License

### Code

The code in this repository, including all code samples in the notebooks listed
above, is released under the [MIT license](LICENSE-CODE). Read more at the
[Open Source Initiative](https://opensource.org/licenses/MIT).
