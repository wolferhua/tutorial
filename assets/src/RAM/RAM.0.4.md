### Deeplearning Algorithms tutorial
谷歌的人工智能位于全球前列，在图像识别、语音识别、无人驾驶等技术上都已经落地。而百度实质意义上扛起了国内的人工智能的大旗，覆盖无人驾驶、智能助手、图像识别等许多层面。苹果业已开始全面拥抱机器学习，新产品进军家庭智能音箱并打造工作站级别Mac。另外，腾讯的深度学习平台Mariana已支持了微信语音识别的语音输入法、语音开放平台、长按语音消息转文本等产品，在微信图像识别中开始应用。全球前十大科技公司全部发力人工智能理论研究和应用的实现，虽然入门艰难，但是一旦入门，高手也就在你的不远处！
AI的开发离不开算法那我们就接下来开始学习算法吧！
回归方法是对数值型连续随机变量进行预测和建模的监督学习算法。其特点是标注的数据集具有数值型的目标变量。回归的目的是预测数值型的目标值。


常用的回归方法包括:
* 线性回归：使用超平面拟合数据集 
* 最近邻算法：通过搜寻最相似的训练样本来预测新样本的值
* 决策树和回归树：将数据集分割为不同分支而实现分层学习
* 集成方法：组合多个弱学习算法构造一种强学习算法，如随机森林（RF）和梯度提升树（GBM）等
* 深度学习：使用多层神经网络学习复杂模型

#### 多元自适应回归样条
多元自适应回归样条(Multivariate Adaptive Regression Splines,MARS)是由美国的统计学家Jerome Friedman于1991年提出的一种数据分析方法。
该方法以样条函数的张量积作为基函数,分为前向过程、后向剪枝过程与模型选取三个步骤。其优势在于能够处理数据量大、维度高的数据,而且计算快捷、模型精确。
文章在一般回归分析理论和样条理论的基础上,系统地研究了MARS的建模过程,提出引入Bernstein基函数建模的思想,并针对冶金工业领域一类数据分析其成分优化问题,应用该方法进行建模和预测。
在前向过程中,通过自适应的选取节点对数据进行分割,每选取一个节点就生成两个新的基函数,前向过程结束后生成一个过拟合的模型。后向剪枝过程中在保证模型准确度的前提下,删除过拟合模型中对模型贡献度小的基函数,最后选取一个最优的模型作为回归模型。
研究过程中对采集的原始数据进行了消除负差、剔除异常数据、数据标准化等预处理工作,选取精华样本,分别建立了线性模型、非线性模型、神经网络模型等,并与MARS方法做比较。得到如下结论:由于模型的限制,线性回归模型精度较低,与实际经验不符;
神经网络对部分元素的描述优于线性回归模型,但不能得出相应的显式表达式,同时线性回归与神经网络都未能考虑变量间的交互作用;MARS模型对问题的描述比较符合实际经验,同时能够反映元素间的交互作用,能够对两个变量做可视化处理,并能够给出显式表达式。
论文以数据科学为背景,属于问题驱动的应用数学研究,不仅对多元自适应回归方法进行了理论探索,也为工业领域的数据分析与优化提供了理论依据。