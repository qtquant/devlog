---
author:  guanbo
title: "改进USIndexExpert突破规则"
symbol: "nas100"
---
在判断突破标准的时候，可能有重复的嫌疑。计划取消绝对值，以ATR的比例来判断突破信号。

当前突破在对True Range判断时采用了多个维度，形式上引入了多个参数标准。

### TODO
- 突破压力位开仓的止损点设置过大，需要修改代码调整为较小的区间。
- 进线开仓的止损点也过大，可以通过优化StopLoss参数改进。
- 由于现在策略调整为多个商品可以开单，需要调低保证金使用比例到5%，否则可能会因为保证金不足而无法开单。