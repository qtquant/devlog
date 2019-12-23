---
author:  guanbo
title: "USDJPY/NZDUSD在TradeMax平台的优化"
symbol: 
  - "usdjpy"
  - "nzdusd"
report_name: "20191222"
---
尝试USIndexExpert对USDJPY和NZDUSD在TradeMax进行优化。USDJPY过程比较坎坷最终也未达标，后续继续考虑优化。NZDUSD比较顺利的达标。

USDJPY持续3天进行优化，但最终在保证金使用率在5%的时候，总收益和赢率无法达标。其中赢率也是全部商品的中最低，但短期可以尝试的方法已经全部使用过，后期可以还一种思路进行优化。

### 目标结果  

| 商品 | 回撤<10% | 15周收益>20% | 赢率>75% |    
|:-|:-:|:-:|:-:|
| `USDJPY`| &#9989; | &#10008; | &#10008; |   
| `NZDUSD`| &#9989; | &#9989; | &#9989; |   


### TODO
- 继续优化NAS100参数。
- 在验证平仓条件时候要包含commission和swap成本。
- 继续优化USDJPY参数。
