作者：Siyuan Liu
年份：2018
出版：IEEE

结论:
1.新的计算特征[OC OH OL CH CL LH]
2.计算MA & EMA
3.LSTM模型预测

方法流程：

图1

其中：

图2

细节：

图3

A.数据源(CSI 603899 Index from 2014-05-18 to 2017-01-29,2016-12-26 to 2017-01-29为测试集)

B.数据预处理

图4

移动平均MA-Moving Average

图5

指数移动平均EMA-Exponential Moving Average

图6

X是变量,N是某一天,Y是EMA的周期。
从百度wiki中深入了解EMA

图7

平滑系数α通常设置为2 / (N + 1), 在EMA计算MACD时，N选择12或26日，则α为2/13或2/27。
特征列表：

图8

C.LSTM模型