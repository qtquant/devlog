---
author:  guanbo
title: "AUDUSD/NAS100在TradeMax平台的优化"
symbol: 
  - "audusd"
  - "nas100"
report_name: "20191223"
---
在TradeMax对AUDUSD进行首次优化，以及NAS100面向赢率再优化。

### RESULT  

| 商品 | 回撤<10% | 15周收益>20% | 赢率>75% |    
|:-|:-:|:-:|:-:|
| `AUDUSD`| &#9989; | &#9989; | &#9989; |   
| `NAS100`| &#9989; | &#9989; | &#9989; |   

AUDUSD虽然达标但开仓频率过低，有进一步提高的空间。

### WIP
目前尝试的优化方法是将动态止盈的参数固定在30%～50%间，而通过TakeProfit来调节。这样做目的是减少优化的时间，特别是在做大量商品的全局优化时有帮助。

USIndexExpert的平仓策略已经将commission和swap成本计入，需要对所以运行的商品做回归后在挂载。

### TODO
- 在验证平仓条件时候要包含commission和swap成本。
- 继续优化USDJPY参数。
- 提高AUDUSD的开仓频率。
