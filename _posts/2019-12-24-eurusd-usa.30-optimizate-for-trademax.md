---
author:  guanbo
title: "EURUSD/USA.30在TradeMax平台的优化"
symbol: 
  - "eurusd"
  - "usa.30"
report_name: "20191224"
---
在TradeMax对EURUSD降低保证金使用率的再优化，以及USA.30固定动态止盈率再优化。

### RESULT  

| 商品 | 回撤<10% | 15周收益>20% | 赢率>75% |    
|:-|:-:|:-:|:-:|
| `EURUSD`| &#9989; | &#9989; | &#9989; |   
| `USA.30`| &#9989; | &#9989; | &#9989; |   

- EURUSD虽然达标但回撤逼近10%，有进一步提高的空间。
- USA.30有过拟合的嫌疑，需要再观察。
- 目前USIndexExpert平仓时已经包含commission和swap成本的计算。

### WIP
目前尝试的优化方法是将动态止盈的参数固定在30%～50%间，而通过TakeProfit来调节。这样做目的是减少优化的时间，特别是在做大量商品的全局优化时有帮助。

### TODO
- 继续优化USDJPY参数。
- 提高AUDUSD的开仓频率。
