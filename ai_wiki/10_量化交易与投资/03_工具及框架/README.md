# 0. 简介

&emsp;&emsp;股票类相关开源库汇总。

## 0.1 Python常用库

1. [vinta/awesome-python: A curated list of awesome Python frameworks, libraries, software and resources (github.com)](https://github.com/vinta/awesome-python)

   * 141k星，各类常用python包分类汇总

# 1. 数据

## 1.1 收费类接口

&emsp;&emsp;仅部分免费，但数据质量相对高。

1. [JoinQuant/jqdatasdk: 简单易用的量化金融数据包(easy utility for getting financial market data of China) (github.com)](https://github.com/JoinQuant/jqdatasdk)

   * 聚宽平台数据接口
   * 仅有3个月免费试用
   * 据描述质量较好，可以实盘使用


2. Tushare [**https://tushare.pro/**](https://tushare.pro/)

   * （*****）推荐使用
   * 质量高，使用人数多。但存在很多限制，需要收费才能获取更多的数据。


## 1.2 基于爬虫的开源库

1. akshare [https://github.com/akfamily/akshare](https://github.com/akfamily/akshare)

   * （*****）推荐使用
   * 非常完善的数据获取库，主要基于爬虫获取(目前我安装后，总是报错，尚未解决)


2. efinance [https://github.com/Micro-sheep/efinance](https://github.com/Micro-sheep/efinance)

   * （*****）推荐使用
   * 非常完善的数据获取库，主要基于爬虫获取
   * 缺点: 没有大盘指数的接口
   

## 1.3 基于网页API接口封装的库

1. [shidenggui/easyquotation: 实时获取新浪 / 腾讯 的免费股票行情 / 集思路的分级基金行情 (github.com)](https://github.com/shidenggui/easyquotation)

   * 3.6k星，MIT协议，纯python代码，已8个月没有更新


2. [bosspen1/stock: 股票行情数据 东方财富交易接口 股票自动交易 (github.com)](https://github.com/bosspen1/stock)

   * 主要基于Java等开发

## 1.4 美股数据

1. yfinance

   * （***）推荐使用 (貌似只能获取国外股票行情数据)
   * 前身是pandas_datareader，后来雅虎关闭api后，通过一些非官方方法获取数据
   * 优点是数据免费、可以获取分钟级数据
   

2. pandas_datareader

   - 库以失效，无法获取数据，但可获取宏观经济数据

## 1.5 数据库

1. [microsoft/qlib-server: Qlib-Server is the data server system for Qlib. It enable Qlib to run in online mode. Under online mode, the data will be deployed as a shared data service. The data and their cache will be shared by all the clients. The data retrieval performance is expected to be improved due to a higher rate of cache hits. It will consume less disk space, too. (github.com)](https://github.com/microsoft/qlib-server)

   * qlib配套数据库，提供一个全新的数据库，据说速度比现有任何数据库速度都快。


2. [Time Series Data Products | InfluxData](https://www.influxdata.com/products/)

   * Go写的分布式时间序列数据库


3. [man-group/arctic: High performance datastore for time series and tick data (github.com)](https://github.com/man-group/arctic)

   * 2.8K星，LGPL-2.1协议，商用不友好
   * 基于mongodb和python的高性能时间序列和tick数据存储


4. [KX: The Leading Provider of Time-Series Database Technology](https://kx.com/)

   * 收费的高性能金融序列数据库解决方案


5. [Schema Design for Time Series Data in MongoDB | MongoDB](https://www.mongodb.com/blog/post/schema-design-for-time-series-data-in-mongodb)

   * 用mongodb存储时间序列数据


6. [kairosdb/kairosdb: Fast scalable time series database (github.com)](https://github.com/kairosdb/kairosdb)

   * 1.7K星，Apache-2.0协议
   * 基于Cassandra的时间序列数据库


7. [OpenTSDB/opentsdb: A scalable, distributed Time Series Database. (github.com)](https://github.com/OpenTSDB/opentsdb)

   * 4.7K星，LGPL-2.1,GPL-3.0协议
   * 基于HBase的时间序列数据库


8. [SQLite Home Page](https://www.sqlite.org/index.html)

   * 轻量级数据库

# 2. 数据处理及因子计算

## 2.1 数据处理

1. [pandas-dev/pandas: Flexible and powerful data analysis / manipulation library for Python, providing labeled data structures similar to R data.frame objects, statistical functions, and much more (github.com)](https://github.com/pandas-dev/pandas)

   * 35.1k星，BSD-3协议
   * 必备库，用于处理表格类数据，还包含金融类公式计算


2. [numpy/numpy: The fundamental package for scientific computing with Python. (github.com)](https://github.com/numpy/numpy)

   * 21.4K星，BSD-3协议
   * 矩阵计算必备库


3. [scipy/scipy: SciPy library main repository (github.com)](https://github.com/scipy/scipy)

   * 10.1k星，BSD-3协议
   * 科学计算库，使用频率相对低



## 2.2 特征提取

1. [alteryx/featuretools: An open source python library for automated feature engineering (github.com)](https://github.com/alteryx/featuretools)

   * 6.3k星，BSD-3协议
   * 可以自动繁衍特征，适合表格类数据，但非常消耗内存，普通PC可能会爆内存


2. [blue-yonder/tsfresh: Automatic extraction of relevant features from time series: (github.com)](https://github.com/blue-yonder/tsfresh)

   * 6.6k星，MIT协议，自动抽取时间序列特征
   * 文档：[https://tsfresh.readthedocs.io/en/latest/](https://tsfresh.readthedocs.io/en/latest/)


3. [johannfaouzi/pyts: A Python package for time series classification (github.com)](https://github.com/johannfaouzi/pyts)

   * 1.3K星，BSD-3协议
   * 包含时间序列特征抽取，分类算法和绘图等
   * 文档：[Welcome to pyts documentation! — pyts 0.12.0 documentation](https://pyts.readthedocs.io/en/stable/)


## 2.3 因子计算

1. [microsoft/qlib: Qlib is an AI-oriented quantitative investment platform, which aims to realize the potential, empower the research, and create the value of AI technologies in quantitative investment. With Qlib, you can easily try your ideas to create better Quant investment strategies. An increasing number of SOTA Quant research works/papers are released in Qlib. (github.com)](https://github.com/microsoft/qlib)

   * 9.5k星，MIT协议，现阶段最完善的机器学习/深度学习平台，仅有一个强化学习示例
   * 包含国内/美股市场数据获取，模型训练流程控制及回测全流程
   * 包含技术指标因子158和360


2. [mrjbq7/ta-lib: Python wrapper for TA-Lib (http://ta-lib.org/). (github.com)](https://github.com/mrjbq7/ta-lib)

   * 7K星，BSD协议，有C++接口，提供约260+技术指标计算
   * 官网：[TA-Lib : Technical Analysis Library - Home](https://ta-lib.org/)
   * 文档中文翻译：[HuaRongSAO/talib-document: talib学习 talib中文翻译 talib中文文档 (github.com)](https://github.com/HuaRongSAO/talib-document)


3. [yli188/WorldQuant_alpha101_code: Code implementation of the Quantigic 101 Formulaic Alphas (github.com)](https://github.com/yli188/WorldQuant_alpha101_code)

   * World Quant公司开源的101因子计算公式，包含详细的公式介绍以及代码，代码通过pandas编写
   * 151星，无协议


## 2.4 因子分析

1. [quantopian/alphalens: Performance analysis of predictive (alpha) stock factors (github.com)](https://github.com/quantopian/alphalens)

   * 2.4K星，Apache-2.0协议，2年未更新
   * 它是全球最大量化网站quantopian开发维护的量化三件套之一，用于股票因子(alpha)的性能分析。alphalens与zipline以及pyfolio常常一同使用，其中，pyfolio提供财务组合的性能和风险分析，zipline用于量化策略回测。alphalens的主要功能包括对一个alpha因子进行统计和绘图，包括：因子收益分析、因子信息系数分析、换手率分析以及分组分析。
   * 文档链接：https://github.com/quantopian/alphalens


# 3. 回测框架

&emsp;&emsp;部分回测框架包含数据获取功能。

## 3.1 主流开源回测框架

1. [mementum/backtrader: Python Backtesting library for trading strategies (github.com)](https://github.com/mementum/backtrader)

   * 9.3k星，GPL-3.0协议，14个月没有更新
   * 文档非常详细，所有开源回测框架，首推选择，优于易用性和详尽的文档
   * 速度可以说是里面最慢的了，但是在python的事件驱动框架里又算快的了。自定义程度很高，而且不用自己造轮子，回测代码非常简洁且逻辑清晰，文档非常详细，而且有大量的例子，甚至有论坛，可以说是这几个里面对用户最友好的框架了


2. [quantopian/zipline: Zipline, a Pythonic Algorithmic Trading Library (github.com)](https://github.com/quantopian/zipline)

   * 由Quantopian开源，目前国内的很多Python编程语言的在线量化回测平台都是以zipline为模板开发应用的
   * 速度很慢，用于国内市场，需要修改内部数据接口
   * 15.4k星，apache 2.0，2年未更新，文档链接已失效
   * 它是全球最大量化网站quantopian开发维护的量化三件套之一，alphalens与zipline以及pyfolio常常一同使用，其中，pyfolio提供财务组合的性能和风险分析，zipline用于量化策略回测。alphalens的主要功能包括对一个alpha因子进行统计和绘图，包括：因子收益分析、因子信息系数分析、换手率分析以及分组分析


3. [vnpy/vnpy: 基于Python的开源量化交易平台开发框架 (github.com)](https://github.com/vnpy/vnpy)

   * 更多被作为实盘接口，回测框架大多选用上面2个中的一个
   * 可以实盘，丰富的各类接口，提供策略开发软件
   * 各类机构应用广泛
   * 纯中文项目，纯python开发
   * 19.1k星，MIT协议，商用友好，开发度活跃
   * 据说回测是不如backtrader的，如果有技术，可以用backtrader回测，用vnpy下单
   * 更加适合期货，以及作为实盘接口


## 3.2. 实盘接口

1. [vnpy/vnpy: 基于Python的开源量化交易平台开发框架 (github.com)](https://github.com/vnpy/vnpy)

   * 可以实盘，丰富的各类接口，提供策略开发软件
   * 各类机构应用广泛
   * 纯中文项目，纯python开发
   * 19.1k星，MIT协议，商用友好，开发度活跃
   * 据说回测是不如backtrader的，如果有技术，可以用backtrader回测，用vnpy下单
   * 更加适合期货，以及作为实盘接口


2. [shidenggui/easytrader: 提供同花顺客户端/国金/华泰客户端/雪球的基金、股票自动程序化交易以及自动打新，支持跟踪 joinquant /ricequant 模拟交易 和 实盘雪球组合, 量化交易组件 (github.com)](https://github.com/shidenggui/easytrader)

   * 主要可以跟踪聚宽实盘模拟交易，以及实盘
   * 6.7k星，MIT协议，已2年没有更新


3. [yutiansut/QUANTAXIS: QUANTAXIS 支持任务调度 分布式部署的 股票/期货/期权 数据/回测/模拟/交易/可视化/多账户 纯本地量化解决方案 (github.com)](https://github.com/yutiansut/QUANTAXIS)

   * 6.7K星，MIT协议，4个月未更新
   * 提供数据/因子库/模拟盘实盘接口


## 3.3 国外开源框架

1. [enzoampil/fastquant: fastquant — Backtest and optimize your trading strategies with only 3 lines of code! (github.com)](https://github.com/enzoampil/fastquant)

   * 仅支持获取US股市数据，如果使用国内数据，可能需要修改内部代码
   * 支持各类传统规则类策略，支持超参数搜索
   * 支持文本情感分析
   * MIT协议，商用友好
   * 2022.03.03最后一次更新，活跃度不高


2. [pmorissette/bt: bt - flexible backtesting for Python (github.com)](https://github.com/pmorissette/bt)

   * 1.5K星，MIT协议
   * 基于FFN量化金融指标计算库构建 [pmorissette/ffn: ffn - a financial function library for Python (github.com)](https://github.com/pmorissette/ffn)
   * 文档：[bt - Flexible Backtesting for Python — bt 0.2.10 documentation (pmorissette.github.io)](http://pmorissette.github.io/bt/index.html)


## 3.4 国产开源框架

1. [ricequant/rqalpha: A extendable, replaceable Python algorithmic backtest trading framework supporting multiple securities (github.com)](https://github.com/ricequant/rqalpha)

* 米筐网提供免费开源框架，米筐量化平台官网：https://www.ricequant.com/welcome/
* 包含数据获取（不确定是否包含免费数据）
* 仅限非商用
* 4.7k星，持续根性，值得推荐


2. [fasiondog/hikyuu: Hikyuu Quant Framework 基于C++/Python的开源量化交易研究框架 (github.com)](https://github.com/fasiondog/hikyuu)

   * 2019码云最有价值项目，1.4k星，更新活跃度高，C++底层速度快，值得推荐
   * 码云地址：[Hikyuu - Quant Framework (gitee.io)](http://fasiondog.gitee.io/hikyuu/)
   * MIT协议，商用友好
   * 百万级别的K线，2秒就能跑完，缺点是基本上只支持国内的股票数据，自定义数据很困难，而且可以说是几乎没有文档


3. [zvtvz/zvt: modular quant framework. (github.com)](https://github.com/zvtvz/zvt)

   * 比较完善的回测框架，同时包含数据获取，基本面、财务、消息类数据，图标展示很完备
   * 数据源多样，同时包含免费数据源
   * MIT协议，商用友好
   * 2.1k星，持续更新中，值得推荐
   * 老代码仓已不维护，老仓库地址：https://github.com/foolcage/fooltrader


4. [josephchenhk/qtrader: A Light Event-Driven Algorithmic Trading Engine (github.com)](https://github.com/josephchenhk/qtrader)

   * 162星，轻量级的回测框架，实时绘图跟踪部分比较好


5. [refraction-ray/xalpha: 基金投资管理回测引擎 (github.com)](https://github.com/refraction-ray/xalpha)

   * 基金回测框架
   * 1.3K星，MIT协议


## 3.5 无编程基础框架

1. [bbfamily/abu: 阿布量化交易系统(股票，期权，期货，比特币，机器学习) 基于python的开源量化交易，量化投资架构 (github.com)](https://github.com/bbfamily/abu)

   * 有电脑版和手机APP，主要利用传统量化和机器学习辅助操盘，更加适合无代码基础人使用
   * 纯中文项目，纯python开发
   * 9.3k星，值得推荐
   * GPL协议，商用不友好
   * APP下载地址:  https://www.abuquant.com/download
   * 电脑浏览器访问地址: https://www.abuquant.com/
   * 量化交易之路源码地址：https://github.com/bbfamily/abu
   * 量化知识：https://blog.abuquant.com/category/lecture/
   * K线课堂https://blog.abuquant.com/category/lecture/


# 4. 策略平台

&emsp;&emsp;上述2中开源项目以回测框架为主，也包含了部分策略，本节项目以策略未主打，
也包含回测的功能。


## 4.1 机器学习/深度学习

1. [microsoft/qlib: Qlib is an AI-oriented quantitative investment platform, which aims to realize the potential, empower the research, and create the value of AI technologies in quantitative investment. With Qlib, you can easily try your ideas to create better Quant investment strategies. An increasing number of SOTA Quant research works/papers are released in Qlib. (github.com)](https://github.com/microsoft/qlib)

   * 9.5k星，MIT协议，现阶段最完善的机器学习/深度学习平台，仅有一个强化学习示例
   * 包含国内/美股市场数据获取，模型训练流程控制及回测全流程
   * 提供一个全新的数据库，速度比现有任何数据库速度都快，网址[microsoft/qlib-server: Qlib-Server is the data server system for Qlib. It enable Qlib to run in online mode. Under online mode, the data will be deployed as a shared data service. The data and their cache will be shared by all the clients. The data retrieval performance is expected to be improved due to a higher rate of cache hits. It will consume less disk space, too. (github.com)](https://github.com/microsoft/qlib-server)
   * 硬件仅需16G内存，5G空间，个人PC跑无压力
   * 缺点：(1) 很多样例依赖的pytorch版本都不一样，而且有些偏老；(2) 数据采用一次性加载到内存，数据太多，
     可能会崩（有待确认是否存在分批加载机制，目前看没有找到）；(3) 机器学习部分由于库本身的限制，不支持
     mini-batch训练，且不支持3D数据，时间维采取统计方式进行压缩成1维


2. [ailabx: AI量化实验室，专注将前沿人工智能技术(深度学习/强化学习/知识图谱)应用于金融量化投资。 (gitee.com)](https://gitee.com/ailabx/ailabx)

   * Github更新较慢，且11个月没有更新，建议访问码云上的代码，地址：[ailabx/ailabx: AI量化实验室，专注将前沿人工智能技术(深度学习/强化学习/知识图谱)应用于金融量化投资。 (github.com)](https://github.com/ailabx/ailabx)
   * Github 297星，无协议声明。码云上，89星，GPL-3.0协议，商用不友好。
   * 对应公众号文章较多，量化知识覆盖面较广


## 4.2. 强化学习

1. [wangshub/RL-Stock: 📈 如何用深度强化学习自动炒股 (github.com)](https://github.com/wangshub/RL-Stock)

   * 只对一支股票操作，精简易懂，是一个很好的强化学习入门项目
   * 2.3k星，值得推荐


2. [AI4Finance-Foundation/FinRL: FinRL: Financial Reinforcement Learning. Please star. 🔥 (github.com)](https://github.com/AI4Finance-Foundation/FinRL)

   * 6k星，MIT协议，有大量论文支撑，哥伦比亚大学大学中国学生开发
   * 支持各类数据源
   

## 4.3 投资组合管理

1. [tradytics/eiten: Statistical and Algorithmic Investing Strategies for Everyone (github.com)](https://github.com/tradytics/eiten)

   * 2.4k星，2年没有更新了，GPL-3.0协议，商用不友好
   * 股票投资组合管理方案值得学习借鉴


2. [Tradytics - Artificial Intelligence Driven Trading Toolkit](https://tradytics.com/)

   * 开源，该网站时国外的量化投资APP，有手机版


## 4.4 传统技术分析方法

1. [yijixiuxin/chanlun-pro: 基于缠中说禅所讲缠论理论，以便量化分析市场行情的工具 (github.com)](https://github.com/yijixiuxin/chanlun-pro)

   * 缠论web分析项目
   * 102星，apache 2.0协议
   * 网页分析界面非常好
   * 码云地址：https://gitee.com/wang-student/chanlun-pro


## 4.5 研报复现

1. [hugo2046/Quantitative-analysis: 量化研究-券商金工研报复现 (github.com)](https://github.com/hugo2046/Quantitative-analysis)

   * 相对都是因子，以及传统统计类策略
   * 主要基于聚宽数据
   * 无开源协议
   * 569颗星，值得推荐


# 5. 量化分析评估

## 5.1 指标计算

1. [QuantLib, a free/open-source library for quantitative finance](https://www.quantlib.org/)

   * 金融计算库，所提供的功能聚焦在两大领域：(1) 期权定价以及相关计算；(2) 固定收益产品定价以及相关计算。
   * C++编写，速度很快，BSD协议，3.4K星
   * [lballabio/QuantLib: The QuantLib C++ library (github.com)](https://github.com/lballabio/quantlib)
   * [enthought/pyql: Cython QuantLib wrappers (github.com)](https://github.com/enthought/pyql)


2. [pmorissette/ffn: ffn - a financial function library for Python (github.com)](https://github.com/pmorissette/ffn)

   * 1.3K星，MIT协议
   * 各类指标计算，如回测评估之类指标
   * [Quickstart — ffn 0.3.6 documentation (pmorissette.github.io)](http://pmorissette.github.io/ffn/quick.html)
   * 配套回测框架  [pmorissette/bt: bt - flexible backtesting for Python (github.com)](https://github.com/pmorissette/bt)


3. [quantopian/pyfolio: Portfolio and risk analytics in Python (github.com)](https://github.com/quantopian/pyfolio)

   * 投资组合和风险评估分析
   * 4.6K星，Apache-2.0协议
   * 它是全球最大量化网站quantopian开发维护的量化三件套之一，alphalens与zipline以及pyfolio常常一同使用，其中，pyfolio提供财务组合的性能和风险分析，zipline用于量化策略回测。alphalens的主要功能包括对一个alpha因子进行统计和绘图，包括：因子收益分析、因子信息系数分析、换手率分析以及分组分析


4. [bsolomon1124/pyfinance: Python package designed for general financial and security returns analysis. (github.com)](https://github.com/bsolomon1124/pyfinance)

   * 282星，MIT协议
   * pyfinance是为投资管理和证券收益分析而构建的Python分析包，主要是对面向定量金融的现有包进行补充，如pyfolio和pandas-datareader等
   * 文档链接：https://github.com/bsolomon1124/pyfinance


## 5.2 绘图工具

1. [matplotlib/matplotlib: matplotlib: plotting with Python (github.com)](https://github.com/matplotlib/matplotlib)

   * 16.1K星，无协议说明


2. [mwaskom/seaborn: Statistical data visualization in Python (github.com)](https://github.com/mwaskom/seaborn)

   * 9.8K星，BSD-3协议，统计类图形绘图


3. [pyecharts/pyecharts: 🎨 Python Echarts Plotting Library (github.com)](https://github.com/pyecharts/pyecharts)

   * 12.7K，MIT协议
   * 是一个由百度开源的数据可视化，有良好的交互性，精巧的图表设计


# 6. 机器学习库

## 6.1 通用机器学习

1. [scikit-learn: machine learning in Python — scikit-learn 1.1.2 documentation](https://scikit-learn.org/stable/)

   * 应用最广泛的机器学习库，包含各类传统机器学习算法
   * Github网址：[scikit-learn/scikit-learn: scikit-learn: machine learning in Python (github.com)](https://github.com/scikit-learn/scikit-learn)
   * 51.3k星，BSD-3协议
   * 中文文档开源项目：[apachecn/sklearn-doc-zh: [译] scikit-learn（sklearn） 中文文档 (github.com)](https://github.com/apachecn/sklearn-doc-zh)


2. [automl/auto-sklearn: Automated Machine Learning with scikit-learn (github.com)](https://github.com/automl/auto-sklearn)

   * 自动选择sklearn中最优的模型和参数，auto-ml
   * 6.5k星，BSD-3协议


3. [statsmodels/statsmodels: Statsmodels: statistical modeling and econometrics in Python (github.com)](https://github.com/statsmodels/statsmodels)

   * 常用统计模型，7.7k星，BSD协议，维护状态良好
   * 文档：[Introduction — statsmodels](https://www.statsmodels.org/stable/index.html)


## 6.2 时间序列

1. [tslearn-team/tslearn: A machine learning toolkit dedicated to time-series data (github.com)](https://github.com/tslearn-team/tslearn)

   * tslearn是一个开源的时间序列机器学习python工具包，其中包括了一些基本的时间序列预测或者分类模型，主要包含传统机器学习相关模型
   * 2.2k星，BSD-2协议


2. [bashtage/arch: ARCH models in Python (github.com)](https://github.com/bashtage/arch)

   * 982星，无协议说明


3. [twosigma/flint: A Time Series Library for Apache Spark (github.com)](https://github.com/twosigma/flint)

   * Spark的时间序列库，959星，Apache-2.0协议，3年未更新


4. [johannfaouzi/pyts: A Python package for time series classification (github.com)](https://github.com/johannfaouzi/pyts)

   * 1.3K星，BSD-3协议
   * 包含时间序列特征抽取，分类算法和绘图等
   * 文档：[Welcome to pyts documentation! — pyts 0.12.0 documentation](https://pyts.readthedocs.io/en/stable/)


# 7. 深度学习库

## 7.1 通用库

1. [pytorch/pytorch: Tensors and Dynamic neural networks in Python with strong GPU acceleration (github.com)](https://github.com/pytorch/pytorch)

   * 58.6k星，1.5版本后包含GPL-3.0, LPGL协议
   * 当前最火的FACEBOOK开源的深度学习框架


2. [tensorflow/tensorflow: An Open Source Machine Learning Framework for Everyone (github.com)](https://github.com/tensorflow/tensorflow)

   * 当前最火的Google开源的深度学习框架
   * 168k星，Apache-2.0协议，不确定是否引用了GPL-3.0的第三方库


## 7.2 时间序列

1. [jdb78/pytorch-forecasting: Time series forecasting with PyTorch (github.com)](https://github.com/jdb78/pytorch-forecasting)

* 基于Pytorch的时间序列预测库，包含Transformer, n-beats, N-HiTs, DeepAR, LSTM等时下最先经的深度学习模型
* 采用pytorch-lighting接口简单易用，类似sk-learn
* 2.2K星，MIT协议


2. [Alro10/deep-learning-time-series: List of papers, code and experiments using deep learning for time series forecasting (github.com)](https://github.com/Alro10/deep-learning-time-series)

   * 近几年时间序列预测论文汇总，同时包含代码，3年未更新
   * 1.8K星，Apache-2.0协议


# 8. 部署发布

## 8.1 C++通用库

1. [fffaraz/awesome-cpp: A curated list of awesome C++ (or C) frameworks, libraries, resources, and shiny things. Inspired by awesome-... stuff. (github.com)](https://github.com/fffaraz/awesome-cpp)
   * C/C++常用库汇总，39.9k星，MIT协议，持续维护中


2. [rigtorp/awesome-modern-cpp: A collection of resources on modern C++ (github.com)](https://github.com/rigtorp/awesome-modern-cpp)
   * 现代C++常用库汇总，9.5K星，无协议说明
   

## 8.2 指标计算

1. [mrjbq7/ta-lib: Python wrapper for TA-Lib (http://ta-lib.org/). (github.com)](https://github.com/mrjbq7/ta-lib)* 7K星，BSD协议，有C++接口，提供约260+技术指标计算

   * 官网：[TA-Lib : Technical Analysis Library - Home](https://ta-lib.org/)
   * 文档中文翻译：[HuaRongSAO/talib-document: talib学习 talib中文翻译 talib中文文档 (github.com)


2. [QuantLib, a free/open-source library for quantitative finance](https://www.quantlib.org/)

   * 金融计算库，所提供的功能聚焦在两大领域：(1) 期权定价以及相关计算；(2) 固定收益产品定价以及相关计算。
   * C++编写，速度很快，BSD协议，3.4K星
   * Github: [lballabio/QuantLib: The QuantLib C++ library (github.com)](https://github.com/lballabio/quantlib)
   * [enthought/pyql: Cython QuantLib wrappers (github.com)](https://github.com/enthought/pyql)


## 8.3 交易接口

1. [libtrading/libtrading: Libtrading, an ultra low-latency trading connectivity library for C and C++. (github.com)](https://github.com/libtrading/libtrading)

   * 低时延交易接口
   * 652星，无协议说明，5年未维护


## 8.4 机器学习部署

1. [microsoft/onnxruntime: ONNX Runtime: cross-platform, high performance ML inferencing and training accelerator (github.com)](https://github.com/microsoft/onnxruntime)

   * 7.4K星，MIT协议，模型推理框架
   * sklearn, pytorch/tensorflow等框架模型均可转换成ONNX之后，通过onnxruntime部署
   * 支持CPU/GPU等各类硬件加速，CPU下暂不支持指令集加速
   * pytorch算子和动态shape支持度有限，但在逐渐完善


## 8.5 深度学习部署

1. [NVIDIA/TensorRT: TensorRT is a C++ library for high performance inference on NVIDIA GPUs and deep learning accelerators. (github.com)](https://github.com/NVIDIA/TensorRT)

   * 5.9K星，Apache-2.0协议，英伟达显卡对应的深度学习推理加速库，速度快于CUDA，且开发比CUDA更容易
   * 当前对各类算子支持度不如onnx-runtime支持的好，使用fp16过程，容易出现溢出导致的结果对不上的问题


2. [alibaba/MNN: MNN is a blazing fast, lightweight deep learning framework, battle-tested by business-critical use cases in Alibaba (github.com)](https://github.com/alibaba/MNN)

   * 阿里巴巴出品深度学习推理加速框架，支持CPU/GPU/NPU指令集加速
   * 7K星，Apache-2.0协议


3. [huawei-noah/bolt: Bolt is a deep learning library with high performance and heterogeneous flexibility. (github.com)](https://github.com/huawei-noah/bolt)

   * 750星，MIT协议
   * 华为诺亚出品CPU深度学习加速框架，支持ARM/X86指令集加速，更轻量级，适合端侧部署


4. [pytorch/pytorch: Tensors and Dynamic neural networks in Python with strong GPU acceleration (github.com)](https://github.com/pytorch/pytorch)

   * 58.6k星，1.5版本后包含GPL-3.0, LPGL协议
   * 当前最火的FACEBOOK开源的深度学习框架
   * 使用jit export到处模型，可以用C++接口调用，jit对python编写格式有一定要求，另外，libtorch存在漏洞，
     以及GPL协议，商用并不友好，但相对其它框架，对动态shape和各类算子是支持度最好的


## 8.6 绘图

1. [lava/matplotlib-cpp: Extremely simple yet powerful header-only C++ plotting library built on the popular matplotlib (github.com)](https://github.com/lava/matplotlib-cpp)
   * matplot C++版本
   * 3.4K星，MIT协议
