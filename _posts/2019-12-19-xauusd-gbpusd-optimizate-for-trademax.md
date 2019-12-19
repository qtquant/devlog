---
author:  guanbo
title: "XAUUSD/GBPUSD在TradeMax平台的优化"
symbol: 
  - "xauusd"
  - "gbpusd"
report_name: "20191219"
---
尝试USIndexExpert对XAUUSD/GBPUSD在TradeMax进行优化。XAUUSD在2%保证金使用率情况可以获得满意的结果；GBPUSD在10%保证金使用率下也达成既定目标。

目前已经在6个商品上挂载了EA但开仓频率不是很理想。
- 指数类CFD目前只在TradeMax平台开仓2单/72小时，且效果不好。
- GBPUSD在挂载后24小时内开仓获利，但从回测报告来看其开仓频率2.5单/周。
- EURUSD48小时内没有开单，其回测开仓频率2单/周

下面需要在兼顾胜率的情况，提升开仓频率。

### 目标
- 回撤比例不大于10%。
- 最近三个月的总收益大于20%。

### 结果
- 回撤比例目标达成。
- 总收益目标全部达成。

### TODO
- 优化USDJPY参数。
- 继续优化SPX500参数。
- 优化提高USA30的胜率。