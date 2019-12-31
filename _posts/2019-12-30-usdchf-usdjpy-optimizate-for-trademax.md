---
author:  guanbo
title: "USDCHF/USDJPY在TradeMax平台优化"
tags: 
  - "usdchf"
  - "usdjpy"
report_name: "20191230"
---
在TradeMax对USDCHF/USDJPY低保证金使用率（2%）向低损失方向优化。

同时开发动态止盈的EA，并实现日内清算功能。

### RESULT  

| 商品 | 回撤<3% | 15周收益>3% | 赢率>75% | 最大损失<2%|    
|:-|:-:|:-:|:-:|:-:|
| `USDCHF` | &#10008; | &#9989;  | &#9989;  | &#9989;  |     
| `USDJPY` | &#10008; | &#9989;  | &#10008; | &#9989;  |     

结果不能全部达标，优化难度在于回撤。USDJPY的胜率也是问题。同时货币对的开仓频率也受回撤率影响走低。

### WIP
在大Spread，低止损情况下的优化以下商品。
- GBPUSD
- USDCHF
- USDJPY
- AUDUSD
- XAUUSD

### TODO
- 在低损失情况下，提高部分货币对商品开仓频率。
