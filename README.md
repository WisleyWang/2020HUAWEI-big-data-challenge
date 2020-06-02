## 队名：无能万金油

------------------------------------
# 2020中国高校计算机大赛·华为云大数据挑战赛--热身赛
![Alt text](https://dsfile.devcloud.huaweicloud.com/CompetitionUploadService/v1/noauth/competition/downLoad/image?uuid=57e607d7236a4fc4903194e6b9e2c5a8)

热身赛：Rank 7

CSDN博客：[我的博客](https://blog.csdn.net/qq_26593695/article/details/106497958)
 **(建议直接打开`热身赛code.ipynb`，里面有详细说明)**
 
 比赛地址：[华为云大数据挑战赛--热身赛](https://competition.huaweicloud.com/information/1000037843/introduction)
## 赛题说明
```text
热身赛题——交通流量预测
随着电子信息和移动通信技术高速发展和不断融合，人工智能在各个领域都相继取得了巨大的突破，
城市智能体也应运而生，而城市交通又是城市智能体的核心。交通流量数据既是城市交通中的基础数据，
又是反应交通状况的重要指标之一，准确预测交通流量对城市交通具有重大意义。本题以交通流量预测
为目标，邀请各个队伍以历史交通流量数据建立对应的算法模型，预测目标流量数据，通过预测值和真实
值之间的对比得到预测准确率，以此来评估各队伍所提交的预测算法。
```
## requirements 
* lightgbm  2.3.0  
* sklearn
* pandas==0.24.2
* pickle
* numpy
* tqdm
* scipy  ==>1.1.0

##数据在trian文件夹下:
```text
1月12日 ~2月8日 各路口数据：
train/01-12/chongzhi_beier-east-01-12.csv、chongzhi_beier-north-01-12...
train/01-13/....
....
train/02-08/...
```
### 文件说明
* `热身赛code.ipynb`：EDA和模型搭建参考
* `customize_service` ：是华为云线上推理代码（线下得到结果，直接粘贴结果到result中）
* `processed_shenzhen_weather.csv`:爬取的天气数据
* `data/` ：生成的中间数据
* `train_TTI.csv`：“华为云杯”2020深圳开放数据应用创新大赛 ·深圳北站周边交通拥堵指数预测
数据

### 模型说明:
```text
主要模型还是回归模型，对于数据的效果最佳
初试采用回归预测，后期主要启发式人工融合数据来拟合线上数据

```





