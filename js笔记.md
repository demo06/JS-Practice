### script标签的属性  
属性 | 值 | 描述
:----:|:----:|:----
async | async | 异步下载脚本,不影响下载HTML(仅适用于外部脚本)
charset |utf-8 | 规定外部脚本文件中使用的字符编码
defer | defer | 规定是否对脚本执行进行延迟加载,直到页面加载为止
src | url |规定外部脚本文件的URL
----
**例子:**
```javascript
<script type="text/javascript" defer charset="UTF-8"></script>
<script type="text/javascript" src="" async="async" charset="UTF-8"></script>
// type属性可省略