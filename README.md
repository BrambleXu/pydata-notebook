# 利用Python进行数据分析 2017 第二版 （Python for Data Analysis, 2nd Edition）中文翻译笔记

这本书的英文版github仓库：[pydata-book](https://github.com/wesm/pydata-book)

作者[Wes McKinney](https://github.com/wesm)是pandas的创作者，所以书中关于pandas的讲解也是最实用的部分。我也直接联系过了Wes本人，这个笔记不会有任何版权问题，当然，也不会用于任何商业用途。

这本书自2013年第一版发行后，就广受好评。第一版的时候作者用的是Python2，不过随着Python2的维护年限将近（2020），以及Python3的推广，整个社群向Python3转变已经成为不可扭转的趋势。所以在第二版里，作者使用了Python3.6。而我实际写的代码则是基于Python3.5，使用上没有任何差别。


> 2017第二版主要更新：
>1. 所有代码，包括Python教程，都升级到了Python3.6（第一版用的是Python2.7）
>2. 更新了Python的安装介绍。这次改用Anaconda Python发行版，以及其他一些需要的Python包
>3. 使用了最新的2017版pandas
>4. 新增了一章，用来介绍pandas的高级应用工具，和其他一些有用的小贴士
>5. 简单介绍了如何使用statsmodels和scikit-learn


本来很早就知道这本书了，直到最近才终于有时间，打算把这本书完整过一遍，顺便用jupyter做成笔记方便以后查阅。结果我在看第一版第三章的时，突然发现作者已经在2017年推出了第二版，不过暂时还没有中文版。想了想反正也要做成笔记，索性直接把英文翻译成中文，做一个简洁版的Notebook版本分享出来好了，也算是为开源世界做点小贡献。

在写笔记的时候，我尽量写中文，不过有一些专有名字我是直接写英文，然后配上中文翻译，毕竟有时候知道英文单词的话查找英文的文档也方便一些，而且我相信这样做对提升中文和英文专业名字的对照关系有帮助。毕竟在程序员的世界里，不懂英语会很艰难，即使是一些简单的单词，也是我们走向新世界的起点。

另外我并不是逐字逐句翻译，因为这样翻译出来的效果洋味十足，很难懂。我尽可能按方便理解的方式进行翻译，其他一些没有用的话我不进行翻译，就像上面说的，这是一个简洁版的笔记，只翻译书中有用的东西。不过因为是一个人在翻译整本书，工作量比较大，难免有错误和疏漏的地方，或者有读起来觉得奇怪的地方，如果有发现的话不要客气，请尽管说出来，欢迎任何改进和Pull Request。


## Jupyter Notebooks:


* [CHAPTER 1：Preliminaries（预备知识）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-01/)
  - [1.1 What Is This Book About?（这本书是关于什么的）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.1%20What%20Is%20This%20Book%20About%3F%EF%BC%88%E8%BF%99%E6%9C%AC%E4%B9%A6%E6%98%AF%E5%85%B3%E4%BA%8E%E4%BB%80%E4%B9%88%E7%9A%84%EF%BC%89.ipynb)
  - [1.2 Why Python for Data Analysis?（为什么使用Python做数据分析）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.2%20Why%20Python%20for%20Data%20Analysis%3F%EF%BC%88%E4%B8%BA%E4%BB%80%E4%B9%88%E4%BD%BF%E7%94%A8Python%E5%81%9A%E6%95%B0%E6%8D%AE%E5%88%86%E6%9E%90%EF%BC%89.ipynb)
  - [1.3 Essential Python Libraries（一些重要的Python库）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.3%20Essential%20Python%20Libraries%EF%BC%88%E4%B8%80%E4%BA%9B%E9%87%8D%E8%A6%81%E7%9A%84Python%E5%BA%93%EF%BC%89.ipynb)
  - [1.4 Installation and Setup（安装和设置）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.4%20Installation%20and%20Setup%EF%BC%88%E5%AE%89%E8%A3%85%E5%92%8C%E8%AE%BE%E7%BD%AE%EF%BC%89.ipynb)
  - [1.5 Community and Conferences（社区和讨论组）+ 私货](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.5%20Community%20and%20Conferences%EF%BC%88%E7%A4%BE%E5%8C%BA%E5%92%8C%E8%AE%A8%E8%AE%BA%E7%BB%84%EF%BC%89.ipynb)
  - [1.6 Navigating This Book（本书导航）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-01/1.6%20Navigating%20This%20Book%EF%BC%88%E6%9C%AC%E4%B9%A6%E5%AF%BC%E8%88%AA%EF%BC%89.ipynb)



* [Chapter 2: Python Language Basics, IPython, and Jupyter Notebooks (Python语言基础，Ipython和Jupyter Notebooks)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-02/)
  - [chp02-Introduction(2013)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/chp02-Introduction%282013%29.ipynb)
  - [2.1 The Python Interpreter（python解释器）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/2.1%20The%20Python%20Interpreter%EF%BC%88python%E8%A7%A3%E9%87%8A%E5%99%A8%EF%BC%89.ipynb)
  - [2.2 IPython Basics (IPython基础)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/2.2%20IPython%E5%9F%BA%E7%A1%80.ipynb)
  - [2.3 Python语言基础)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-02/2.3%20Python%E8%AF%AD%E8%A8%80%E5%9F%BA%E7%A1%80.ipynb)



* [Chapter 3: Built-in Data Structures, Functions, and Files (内建数据结构，函数和文件)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-03/)
  - [3.1 Data Structures and Sequences (数据结构与序列)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.1%20Data%20Structures%20and%20Sequences%20%28%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%E4%B8%8E%E5%BA%8F%E5%88%97%29.ipynb)
  - [3.2 Functions (函数)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.2%20Functions%20%28%E5%87%BD%E6%95%B0%29.ipynb)
  - [3.3 Files and the Operating System (文件以及操作系统)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-03/3.3%20Files%20and%20the%20Operating%20System%20%28%E6%96%87%E4%BB%B6%E4%BB%A5%E5%8F%8A%E6%93%8D%E4%BD%9C%E7%B3%BB%E7%BB%9F%29.ipynb)


* [Chapter 4: NumPy Basics: Arrays and Vectorized Computation（NumPy基础：数组和向量化计算）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-04/)
  - [4.1 The NumPy ndarray: A Multidimensional Array Object（ndarray: 多维数组对象)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.1%20The%20NumPy%20ndarray%EF%BC%88%E5%A4%9A%E7%BB%B4%E6%95%B0%E7%BB%84%E5%AF%B9%E8%B1%A1%EF%BC%89.ipynb)
  - [4.2 Universal Functions: Fast Element-Wise Array Functions（通用函数：快速点对点数组函数）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.2%20Universal%20Functions%20%28%E9%80%9A%E7%94%A8%E5%87%BD%E6%95%B0%29.ipynb)
  - [4.3 Array-Oriented Programming with Arrays（数组导向编程）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.3%20Array-Oriented%20Programming%20with%20Arrays%EF%BC%88%E6%95%B0%E7%BB%84%E5%AF%BC%E5%90%91%E7%BC%96%E7%A8%8B%EF%BC%89.ipynb)
  - [4.4 File Input and Output with Arrays（通过数组来进行文件的输入和输出）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.4%20File%20Input%20and%20Output%20with%20Arrays%EF%BC%88%E9%80%9A%E8%BF%87%E6%95%B0%E7%BB%84%E6%9D%A5%E8%BF%9B%E8%A1%8C%E6%96%87%E4%BB%B6%E7%9A%84%E8%BE%93%E5%85%A5%E5%92%8C%E8%BE%93%E5%87%BA%EF%BC%89.ipynb)
  - [4.5 Linear Algebra (线性代数)](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.5%20Linear%20Algebra%20%28%E7%BA%BF%E6%80%A7%E4%BB%A3%E6%95%B0%29.ipynb)
  - [4.6 Pseudorandom Number Generation（伪随机数生成）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.6%20Pseudorandom%20Number%20Generation%EF%BC%88%E4%BC%AA%E9%9A%8F%E6%9C%BA%E6%95%B0%E7%94%9F%E6%88%90%EF%BC%89.ipynb)
  - [4.7 Example Random Walks（例子：随机漫步）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-04/4.7%20Example%20Random%20Walks%EF%BC%88%E4%B8%80%E4%B8%AA%E4%BE%8B%E5%AD%90%EF%BC%9A%E9%9A%8F%E6%9C%BA%E6%BC%AB%E6%AD%A5%EF%BC%89.ipynb)


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


* [Chapter 8: Data Wrangling: Join, Combine, and Reshape（数据加工：加入, 结合, 变型）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-08/)
  - [8.1 Hierarchical Indexing（分层索引）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.1%20Hierarchical%20Indexing%EF%BC%88%E5%88%86%E5%B1%82%E7%B4%A2%E5%BC%95%EF%BC%89.ipynb)
  - [8.2 Combining and Merging Datasets（合并数据集）
  ](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.2%20Combining%20and%20Merging%20Datasets%EF%BC%88%E5%90%88%E5%B9%B6%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [8.3 Reshaping and Pivoting（整形和旋转）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-08/8.3%20Reshaping%20and%20Pivoting%EF%BC%88%E6%95%B4%E5%BD%A2%E5%92%8C%E6%97%8B%E8%BD%AC%EF%BC%89.ipynb)


* [Chapter 9: Plotting and Visualization（绘图和可视化）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-09/)
  - [9.1 A Brief matplotlib API Primer（简单的matplotlib API入门）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-09/9.1%20A%20Brief%20matplotlib%20API%20Primer%EF%BC%88%E4%B8%80%E4%B8%AA%E7%AE%80%E5%8D%95%E7%9A%84matplotlib%20API%E5%85%A5%E9%97%A8%EF%BC%89.ipynb)
  - [9.2 Plotting with pandas and seaborn（用pandas和seaborn绘图）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-09/9.2%20Plotting%20with%20pandas%20and%20seaborn%EF%BC%88%E7%94%A8pandas%E5%92%8Cseaborn%E7%BB%98%E5%9B%BE%EF%BC%89.ipynb)
  - [9.3 Other Python Visualization Tools（其他一些Python可视化工具）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-09/9.3%20Other%20Python%20Visualization%20Tools%EF%BC%88%E5%85%B6%E4%BB%96%E4%B8%80%E4%BA%9BPython%E5%8F%AF%E8%A7%86%E5%8C%96%E5%B7%A5%E5%85%B7%EF%BC%89.ipynb)


* [Chapter 10: Data Aggregation and Group Operations（数据汇总和组操作）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-10/)
  - [10.1 GroupBy Mechanics（分组机制）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-10/10.1%20GroupBy%20Mechanics%EF%BC%88%E5%88%86%E7%BB%84%E6%9C%BA%E5%88%B6%EF%BC%89.ipynb)
  - [10.2 Data Aggregation（数据聚合）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-10/10.2%20Data%20Aggregation%EF%BC%88%E6%95%B0%E6%8D%AE%E8%81%9A%E5%90%88%EF%BC%89.ipynb)
  - [10.3 Apply：General split-apply-combine（应用：通用的分割-应用-合并）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-10/10.3%20Apply%EF%BC%9AGeneral%20split-apply-combine%EF%BC%88%E5%BA%94%E7%94%A8%EF%BC%9A%E9%80%9A%E5%B8%B8%E7%9A%84%E5%88%86%E5%89%B2-%E5%BA%94%E7%94%A8-%E5%90%88%E5%B9%B6%EF%BC%89.ipynb)
  - [10.4 Pivot Tables and Cross-Tabulation（数据透视表和交叉表）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-10/10.4%20Pivot%20Tables%20and%20Cross-Tabulation%EF%BC%88%E6%95%B0%E6%8D%AE%E9%80%8F%E8%A7%86%E8%A1%A8%E5%92%8C%E4%BA%A4%E5%8F%89%E8%A1%A8%EF%BC%89.ipynb)



* [Chapter 11: Time Series（时间序列）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-11/)
  - [11.1 Date and Time Data Types and Tools（日期和时间数据类型及其工具）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.1%20Date%20and%20Time%20Data%20Types%20and%20Tools%EF%BC%88%E6%97%A5%E6%9C%9F%E5%92%8C%E6%97%B6%E9%97%B4%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B%E5%8F%8A%E5%85%B6%E5%B7%A5%E5%85%B7%EF%BC%89.ipynb)
  - [11.2 Time Series Basics（时间序列基础）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.2%20Time%20Series%20Basics%EF%BC%88%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E5%9F%BA%E7%A1%80%EF%BC%89.ipynb)
  - [11.3 Date Ranges, Frequencies, and Shifting（日期范围，频度，和位移）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.3%20Date%20Ranges%2C%20Frequencies%2C%20and%20Shifting%EF%BC%88%E6%97%A5%E6%9C%9F%E8%8C%83%E5%9B%B4%EF%BC%8C%E9%A2%91%E5%BA%A6%EF%BC%8C%E5%92%8C%E4%BD%8D%E7%A7%BB%EF%BC%89.ipynb)
  - [11.4 Time Zone Handling（时区处理）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.4%20Time%20Zone%20Handling%EF%BC%88%E6%97%B6%E5%8C%BA%E5%A4%84%E7%90%86%EF%BC%89.ipynb)
  - [11.5 Periods and Period Arithmetic（周期和周期运算）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.5%20Periods%20and%20Period%20Arithmetic%EF%BC%88%E5%91%A8%E6%9C%9F%E5%92%8C%E5%91%A8%E6%9C%9F%E8%BF%90%E7%AE%97%EF%BC%89.ipynb)
  - [11.6 Resampling and Frequency Conversion（重采样和频度转换）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.6%20Resampling%20and%20Frequency%20Conversion%EF%BC%88%E9%87%8D%E9%87%87%E6%A0%B7%E5%92%8C%E9%A2%91%E5%BA%A6%E8%BD%AC%E6%8D%A2%EF%BC%89.ipynb)
  - [11.7 Moving Window Functions（移动窗口函数）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-11/11.7%20Moving%20Window%20Functions%EF%BC%88%E7%A7%BB%E5%8A%A8%E7%AA%97%E5%8F%A3%E5%87%BD%E6%95%B0%EF%BC%89.ipynb)



* [Chapter 12: Advanced pandas（高级pandas用法）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-12/)
  - [12.1 Categorical Data（类别数据）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-12/12.1%20Categorical%20Data%EF%BC%88%E7%B1%BB%E5%88%AB%E6%95%B0%E6%8D%AE%EF%BC%89.ipynb)
  - [12.2 Advanced GroupBy Use（高级GroupBy用法）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-12/12.2%20Advanced%20GroupBy%20Use%EF%BC%88%E9%AB%98%E7%BA%A7GroupBy%E7%94%A8%E6%B3%95%EF%BC%89.ipynb)
  - [12.3 Techniques for Method Chaining（方法链接的技巧）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-12/12.3%20Techniques%20for%20Method%20Chaining%EF%BC%88%E6%96%B9%E6%B3%95%E9%93%BE%E6%8E%A5%E7%9A%84%E6%8A%80%E5%B7%A7%EF%BC%89.ipynb)



* [Chapter 13: Introduction to Modeling Libraries in Python（Python中建模库的介绍）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-13/)
  - [13.1 Interfacing Between pandas and Model Code（pandas与建模代码间的交互）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-13/13.1%20Interfacing%20Between%20pandas%20and%20Model%20Code%EF%BC%88pandas%E4%B8%8E%E5%BB%BA%E6%A8%A1%E4%BB%A3%E7%A0%81%E9%97%B4%E7%9A%84%E4%BA%A4%E4%BA%92%EF%BC%89.ipynb)
  - [13.2 Creating Model Descriptions with Patsy（利用Patsy创建模型描述）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-13/13.2%20Creating%20Model%20Descriptions%20with%20Patsy%EF%BC%88%E5%88%A9%E7%94%A8Patsy%E5%88%9B%E5%BB%BA%E6%A8%A1%E5%9E%8B%E6%8F%8F%E8%BF%B0%EF%BC%89.ipynb)
  - [13.3 Introduction to statsmodels（statsmodels简介）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-13/13.3%20Introduction%20to%20statsmodels%EF%BC%88statsmodels%E7%AE%80%E4%BB%8B%EF%BC%89.ipynb)
  - [13.4 Introduction to scikit-learn（scikit-learn简介）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-13/13.4%20Introduction%20to%20scikit-learn%EF%BC%88scikit-learn%E7%AE%80%E4%BB%8B%EF%BC%89.ipynb)



* [Chapter 14: Data Analysis Examples（数据分析实例）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/tree/master/Chapter-14/)
  - [14.1 USA.gov Data from Bitly（USA.gov数据集）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.1%20USA.gov%20Data%20from%20Bitly%EF%BC%88USA.gov%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [14.2 MovieLens 1M Dataset（MovieLens 1M数据集）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.2%20MovieLens%201M%20Dataset%EF%BC%88MovieLens%201M%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [14.3 US Baby Names 1880–2010（1880年至2010年美国婴儿姓名）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.3%20US%20Baby%20Names%201880%E2%80%932010%EF%BC%881880%E5%B9%B4%E8%87%B32010%E5%B9%B4%E7%BE%8E%E5%9B%BD%E5%A9%B4%E5%84%BF%E5%A7%93%E5%90%8D%EF%BC%89.ipynb)
  - [14.4 USDA Food Database（美国农业部食品数据库）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.4%20USDA%20Food%20Database%EF%BC%88USDA%E9%A3%9F%E5%93%81%E6%95%B0%E6%8D%AE%E5%BA%93%EF%BC%89.ipynb)
  - [14.5 2012 Federal Election Commission Database（2012联邦选举委员会数据库）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.5%202012%20Federal%20Election%20Commission%20Database%EF%BC%882012%E8%81%94%E9%82%A6%E9%80%89%E4%B8%BE%E5%A7%94%E5%91%98%E4%BC%9A%E6%95%B0%E6%8D%AE%E5%BA%93%EF%BC%89.ipynb)




<!--


* [Appendix A: Advanced NumPy]()
- []()
- []()
- []()

-->

## License

The code in this repository, including all code samples in the notebooks listed
above, is released under the [MIT license](LICENSE-CODE). Read more at the
[Open Source Initiative](https://opensource.org/licenses/MIT).

## Sponsor

如果觉得有帮助，可以赞个助，不论多少都是对我工作的肯定：）

- ETH: 0x0d9e310313a55cb8e48d69a2db27209db1b5a793
- EOS：0xb5f0a94f77e007b596a6e53a75f4ee04f0c72899
- NEO：ASCc7rEZ1SAg2hnLicwkaVBMF9MyqWFKMz


微信:

![wechat](http://oydgk2hgw.bkt.clouddn.com/pydata-book/ynv08.jpeg)

支付宝：

![alipay](http://oydgk2hgw.bkt.clouddn.com/pydata-book/n0det.jpeg)


[1]: http://amzn.to/2vvBijB
