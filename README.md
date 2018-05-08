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

另外我并不是逐字逐句翻译，因为这样翻译出来的效果洋味十足，很难懂。我尽可能按方便理解的方式进行翻译，其他一些没有用的话我不进行翻译。这本书中的翻译并不是经过特别考究的，内容上也会有很多个人的解释。推荐大家等正式的中文版推出后进行购买，翻译质量肯定会比我的有保障。不过因为是一个人在翻译整本书，工作量比较大，难免有错误和疏漏的地方，或者有读起来觉得奇怪的地方，如果有发现的话不要客气，请尽管说出来，欢迎任何改进和Pull Request。

## 声明

我的翻译行为完全是出于自己的兴趣，并没有经过国内出版社的授权。经一些朋友的提醒，国外的作者本人是不享有翻译权的，即使我获得了原作者的许可，也不能私自进行翻译。为了尊重版权和国内译者的劳动，这个笔记只保留一部分翻译内容。我挑选了一些相对基础的章节留了下来，可以用于了解Numpy和Pandas，如果想要看完整版内容的话，读者朋友们可以期待即将出版的中文版书籍。


* [Chapter 4: NumPy Basics: Arrays and Vectorized Computation（NumPy基础：数组和向量化计算）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-04/)
  - [4.1 The NumPy ndarray: A Multidimensional Array Object（ndarray: 多维数组对象)](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-04/4.1%20The%20NumPy%20ndarray%EF%BC%88%E5%A4%9A%E7%BB%B4%E6%95%B0%E7%BB%84%E5%AF%B9%E8%B1%A1%EF%BC%89.ipynb)
  - [4.2 Universal Functions: Fast Element-Wise Array Functions（通用函数：快速点对点数组函数）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-04/4.2%20Universal%20Functions%20%28%E9%80%9A%E7%94%A8%E5%87%BD%E6%95%B0%29.ipynb)
  - [4.3 Array-Oriented Programming with Arrays（数组导向编程）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-04/4.3%20Array-Oriented%20Programming%20with%20Arrays%EF%BC%88%E6%95%B0%E7%BB%84%E5%AF%BC%E5%90%91%E7%BC%96%E7%A8%8B%EF%BC%89.ipynb)



* [Chapter 5: Getting Started with pandas（开始使用pandas）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-05/)
  - [5.1 Introduction to pandas Data Structures（pandas的数据结构）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-05/5.1%20Introduction%20to%20pandas%20Data%20Structures%EF%BC%88pandas%E7%9A%84%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84%EF%BC%89.ipynb)
  - [5.2 Essential Functionality（主要功能）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-05/5.2%20Essential%20Functionality%EF%BC%88%E4%B8%BB%E8%A6%81%E5%8A%9F%E8%83%BD%EF%BC%89.ipynb)
  - [5.3 Summarizing and Computing Descriptive Statistics（汇总和描述性统计）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-05/5.3%20Summarizing%20and%20Computing%20Descriptive%20Statistics%EF%BC%88%E6%80%BB%E7%BB%93%E5%92%8C%E6%8F%8F%E8%BF%B0%E6%80%A7%E7%BB%9F%E8%AE%A1%EF%BC%89.ipynb)



* [Chapter 7: Data Cleaning and Preparation（数据清洗和准备）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-07/)
  - [7.1 Handling Missing Data（处理缺失数据）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-07/7.1%20Handling%20Missing%20Data%EF%BC%88%E5%A4%84%E7%90%86%E7%BC%BA%E5%A4%B1%E6%95%B0%E6%8D%AE%EF%BC%89.ipynb)
  - [7.2 Data Transformation（数据变换）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-07/7.2%20Data%20Transformation%EF%BC%88%E6%95%B0%E6%8D%AE%E5%8F%98%E6%8D%A2%EF%BC%89.ipynb)
  - [7.3 String Manipulation（字符串处理）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-07/7.3%20String%20Manipulation%EF%BC%88%E5%AD%97%E7%AC%A6%E4%B8%B2%E5%A4%84%E7%90%86%EF%BC%89.ipynb)



* [Chapter 11: Time Series（时间序列）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-11/)
  - [11.1 Date and Time Data Types and Tools（日期和时间数据类型及其工具）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-11/11.1%20Date%20and%20Time%20Data%20Types%20and%20Tools%EF%BC%88%E6%97%A5%E6%9C%9F%E5%92%8C%E6%97%B6%E9%97%B4%E6%95%B0%E6%8D%AE%E7%B1%BB%E5%9E%8B%E5%8F%8A%E5%85%B6%E5%B7%A5%E5%85%B7%EF%BC%89.ipynb)
  - [11.2 Time Series Basics（时间序列基础）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-11/11.2%20Time%20Series%20Basics%EF%BC%88%E6%97%B6%E9%97%B4%E5%BA%8F%E5%88%97%E5%9F%BA%E7%A1%80%EF%BC%89.ipynb)
  - [11.3 Date Ranges, Frequencies, and Shifting（日期范围，频度，和位移）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-11/11.3%20Date%20Ranges%2C%20Frequencies%2C%20and%20Shifting%EF%BC%88%E6%97%A5%E6%9C%9F%E8%8C%83%E5%9B%B4%EF%BC%8C%E9%A2%91%E5%BA%A6%EF%BC%8C%E5%92%8C%E4%BD%8D%E7%A7%BB%EF%BC%89.ipynb)



* [Chapter 12: Advanced pandas（高级pandas用法）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-12/)
  - [12.1 Categorical Data（类别数据）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-12/12.1%20Categorical%20Data%EF%BC%88%E7%B1%BB%E5%88%AB%E6%95%B0%E6%8D%AE%EF%BC%89.ipynb)



* [Chapter 14: Data Analysis Examples（数据分析实例）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/tree/master/Chapter-14/)
  - [14.1 USA.gov Data from Bitly（USA.gov数据集）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-14/14.1%20USA.gov%20Data%20from%20Bitly%EF%BC%88USA.gov%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [14.2 MovieLens 1M Dataset（MovieLens 1M数据集）](http://nbviewer.jupyter.org/github/LearnXu/pydata-notebook/blob/master/Chapter-14/14.2%20MovieLens%201M%20Dataset%EF%BC%88MovieLens%201M%E6%95%B0%E6%8D%AE%E9%9B%86%EF%BC%89.ipynb)
  - [14.3 US Baby Names 1880–2010（1880年至2010年美国婴儿姓名）](http://nbviewer.jupyter.org/github/BrambleXu/pydata-notebook/blob/master/Chapter-14/14.3%20US%20Baby%20Names%201880%E2%80%932010%EF%BC%881880%E5%B9%B4%E8%87%B32010%E5%B9%B4%E7%BE%8E%E5%9B%BD%E5%A9%B4%E5%84%BF%E5%A7%93%E5%90%8D%EF%BC%89.ipynb)

> commit 94ab376，我只能帮到这里了

## License

The code in this repository, including all code samples in the notebooks listed
above, is released under the [MIT license](LICENSE-CODE). Read more at the
[Open Source Initiative](https://opensource.org/licenses/MIT).
