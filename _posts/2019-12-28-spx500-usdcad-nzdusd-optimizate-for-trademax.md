---
author:  guanbo
title: "风控倍数及SPX500/USDCAD/NZDUSD在TradeMax平台优化"
symbol: 
  - "spx500"
  - "usdcad"
  - "nzdusd"
report_name: "20191228"
---
在TradeMax对SPX500/USDCAD/NZDUSD低保证金使用率（2%）向低损失方向优化。引入风控倍数，确立资金管理低风险目标，保证一定开仓频率的情况下。

设定账户净值最大回撤15%左右，最大开仓商品数5张。通过调节系统Stopout Level（通常在40%～100%）的风控倍数来实现开仓数量。

计算公式：    
（1-保证金使用率）^5=系统StopoutLevel x 风控倍数 / (1+系统StopoutLevel x 风控倍数)。

### RESULT  

| 商品 | 回撤<3% | 15周收益>3% | 赢率>75% | 最大损失<2%|    
|:-|:-:|:-:|:-:|:-:|
| `SPX500`| &#9989; | &#9989; | &#9989; | &#9989; |     
| `USDCAD`| &#9989; | &#9989; | &#9989; | &#9989; |     
| `NZDUSD`| &#9989; | &#9989; | &#9989; | &#9989; |     

### WIP
在大Spread，低止损情况下的优化以下商品。
- GBP
- USDCHF
- USA.30
- USDJPY
- AUDUSD

### TODO
- 在低损失情况下，提高部分货币对商品开仓频率。
