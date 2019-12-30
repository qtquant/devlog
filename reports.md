---
layout: default
title: "全部报告"
---
## {{ page.title }}

{% assign symbols = site.static_files | where_exp: "file", "file.path contains '/reports/'" | where: "extname", ".htm" | group_by_exp: "item", "item.path | slice: 9, 6" %}
{% for symbol in symbols %}
### [{{ symbol.name | upcase }} - {{symbol.items[0].basename}}]({{symbol.items[0].path | relative_url }}){:target="_blank"} 

<details style="margin:10px">   
  <summary>历史报告</summary>     
<ul>
{% for report in symbol.items %}
  <li>
    <a href="{{ report.path | relative_url }}" target="_blank">{{ report.basename }}</a>
  </li>
{% endfor %}
</ul>
</details>    

{% endfor %}
