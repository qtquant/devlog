---
author:  guanbo
title: "分析交易历史趋势触发优化"
tags: 
  - "USDCHF"
  - "EURUSD"
  - "USDCAD"
  - "GBPUSD"
  - "NZDUSD"
report_name: "20200606"
---

利用历史交易的数据按Symbol分组绘制最近30天的趋势图，从而直观的分辨出需要优化的商品品种。

#### 20200605_m30
![20200605_m30]({{site.url}}{{site.baseurl}}/assets/images/20200605_m30.png)

M30趋势表明EURUSD和USDCHF的策略劣化的厉害，需要及时优化。USDCAD的趋势也已经劣化，而且前期的也处于盈亏线震荡。也有优化的需求。

#### 20200605_h1
![20200605_h1]({{site.url}}{{site.baseurl}}/assets/images/20200605_h1.png)

H1趋势同样表明EURUSD和USDCHF的策略劣化的厉害，需要及时优化。NZDUSD在一段时间内无交易，策略失效需要重新优化。GBPUSD长期盈亏线以下运行，并且最近一周向下运行，需要优化。


修复EA的在BollBand震荡策略的Bug。由于没有将StdDev与Point进行换算，造成StdDev的永远小于MinStdDev进而震荡策略失效。


### WIP

#### 震荡策略优化
- USDJPY
- GBPUSD
- USDCAD
- NZDUSD
- AUDUSD

### TODO
- 计划任务检查品种趋势，按无交易、收益下降等劣化条件自动触发优化。
