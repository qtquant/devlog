---
author:  guanbo
title: "尝试Dukascopy平台及优化FXDD"
tags: 
  - "USDCHF"
  - "EURUSD"
  - "USDCAD"
  - "GBPUSD"
  - "NZDUSD"
  - "AUDUSD"
  - "USDJPY"
report_name: "20200613"
---

在Dukascopy的模拟环境运行EA，持续跟踪最近30天FXDD的趋势图。


### Dukascopy
在其模拟环境优化了2个品种**NZDUSD/AUDUSD**并挂上EA运行，同时以FXDD的参数EA运行了**USDJPY/GBPUSD**。由于Dukascopy的模拟环境数据质量不高回测结果可能存在偏差。从官方下载的K线数据估计是正式环境的，与模拟环境的数据不兼容。

### FXDD趋势图
#### 20200613_m30
[1]: {{site.url}}{{site.baseurl}}/assets/images/20200613_m30.png
[![20200613_m30][1]][1]{:target="_blank"}

**GBPUSD**的本周劣化比较明显需要再优化，**AUDUSD/NZDUSD/USDJPY/USDCAD**虽然总体震荡上行考虑震荡策略的改进需要全部优化，EURUSD/USDCHF上线一周还有待观察。


#### 20200613_h1
[2]: {{site.url}}{{site.baseurl}}/assets/images/20200613_h1.png
[![20200613_h1][2]][2]{:target="_blank"}

EURUSD/USDCHF/USDJPY有待继续观察，**AUDUSD**从震荡策略优化的角度考虑需要更新，其他**GBPUSD/USDCAD/NZDUSD**都亟需改进。特别是USDCAD已经持续进行劣化。此外H1的开仓比较少需要通过震荡策略优化提升交易数量。

### WIP

#### 震荡策略优化
- GBPUSD
- USDCAD
- NZDUSD

### TODO
- 计划任务检查品种趋势，按无交易、收益下降等劣化条件自动触发优化。
