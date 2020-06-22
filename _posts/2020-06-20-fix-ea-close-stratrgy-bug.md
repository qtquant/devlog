---
author:  guanbo
title: "修复EA中关闭交易中的Bug"
tags: 
  - "USDCHF"
  - "EURUSD"
  - "USDCAD"
  - "GBPUSD"
  - "NZDUSD"
  - "AUDUSD"
  - "USDJPY"
report_name: "20200621"
---

由交易记录观察发现，获利记录达到阙值后回撤50%并没有获利了结。

Review发现数值计算的比较单位有问题，造成这条动态止盈退出路径无法生效。B2或S2实际只能通过TP/SL以及Boll中线获利了结。

观察发现交易频率高的参数组合在实际运行中与回测结果拟合度更好，也就是**交易频率**的重要性要高于**获利率**指标。

### FXDD趋势图
#### 20200620_m30
[1]: {{site.url}}{{site.baseurl}}/assets/images/20200620_m30.png
[![20200620_m30][1]][1]{:target="_blank"}

本周**USDCHF/NZDUSD/AUDUSD**都存在跨2天以上的仓位并且USDCHF最后到周五清仓才关闭，需要优化。周五美盘时间**NZDUSD/AUDUSD/EURUSD**都被洗，造成一周收益回吐。另外就是USDJPY/EURUSD的开仓频率过低。考虑EA修复Bug后会对参数有较大影响，全部品种都要从新优化。

#### 20200620_h1
[2]: {{site.url}}{{site.baseurl}}/assets/images/20200620_h1.png
[![20200620_h1][2]][2]{:target="_blank"}

开仓频率过低，损失不大但无法判断效果。为了需要针对开仓频率做改进。

### Dukascopy
在整体趋势上类似与FXDD接近，但总体收益略差。考虑直接采用FXDD的参数运行，比较FXDD的数据质量好于Dukascopy的模拟环境。

### TODO
- 计划任务检查品种趋势，按无交易、收益下降等劣化条件自动触发优化。
- 基于历史行情利用Python在TensorFlow上做融合GAN的强化学习系统。
