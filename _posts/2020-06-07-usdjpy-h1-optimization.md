---
author:  guanbo
title: "USDJPY优化H1周期"
tags: 
  - "USDJPY"
report_name: "20200607"
---

USDJPY的H1周期虽然最近30天有2%收益，但考虑到策略稳定性TrackPeriod多在15或20个单位，需要优化。

所以也针对H1周期的USDJPY在涵盖震荡策略的情况下进行优化。震荡策略未充分优化，采用的是标准的BollBand参数进行优化。

### WIP

#### 震荡策略优化
- USDJPY
- GBPUSD
- USDCAD
- NZDUSD
- AUDUSD

### TODO
- 计划任务检查品种趋势，按无交易、收益下降等劣化条件自动触发优化。
- 尝试取消TRRR参数。
