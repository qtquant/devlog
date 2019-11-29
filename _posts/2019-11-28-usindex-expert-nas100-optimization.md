---
author:  guanbo
title: "USIndexExpert针对NAS100的优化"
symbol: "nas100"
report_name: "20191129"
---
考虑美股三指数形势类似，将为USA.30设计的USIndexExpert量化交易程序针对NAS100做参数优化。目标是可以在趋势合适的时候增加开仓的几率。

近三个月优化回测结果符合预期。

### TODO
- Boll进线后的到中线附近平仓的策略调整为在顺势下开仓以提高胜率。
- Boll中线平仓策略改善为平仓50%，然后止损点调整为开仓价格的策略。