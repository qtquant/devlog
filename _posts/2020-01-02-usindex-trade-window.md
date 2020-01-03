---
author:  guanbo
title: "USIndexExpert的交易时间窗口管理"
tags: 
  - "EA"
---
新年开盘的EA仓被跳空误导开仓，其中还有一个因点差过大的问题被止损。所以引入时间窗口管理规避开盘数据的扰动。

### 现状
已经在平仓策略中加入周五23点强平所有仓位，防止下周的跳空来不及止损。之前FXDD平台短期测试内没有观察到开盘数据扰动影响到EA开仓。

### 解决方案

引入下面代码管理开盘和周五闭市的交易时间窗口

```C++
bool QTrade::CheckTradeWindow(bool isOpen=true)
  {
   if(isOpen)
     {
      return Hour()>0;
     }
   else
     {
      return (Hour()==23&&DayOfWeek()==5);
     }
  }
```

### TODO

上述代码仅解决部分场景，对于公众假期各国存在差异的情况并没有解决。未来分两步走：
1. 世界通行的假期固定代码中，全面平仓。
2. 各国特定假期建立与Symbol的对应关系进行输出。