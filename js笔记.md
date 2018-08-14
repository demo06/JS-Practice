#JavaScript学习笔记
----
### script标签的属性  
属性 | 值 | 描述
:----:|:----:|:----
async | async | 异步下载脚本,不影响下载HTML(仅适用于外部脚本)
charset |utf-8 | 规定外部脚本文件中使用的字符编码
defer | defer | 规定是否对脚本执行进行延迟加载,直到页面加载为止
src | url |规定外部脚本文件的URL

**例子:**
```javascript
<script type="text/javascript" defer charset="UTF-8"></script>
<script type="text/javascript" src="" async="async" charset="UTF-8"></script>
// type属性可省略
```

**标识符规范**
* 第一个字符必须是字母,下划线或者美元符号$  
* 其他的字符可以是字母,下划线,数字  
* 例如:
`footerBar`  `bannerArea` `_userName` `$home2`
* 错误例子:
`88Bar` `&demo` `address(info)`

**直接量**
在程序中直接使用的数据的值  
* 数字  18
* 小数  1.2
* 字符串  "sdadas"
* 布尔值  true false
* 数组 \[\]  \{a\:8\;\}

**javascript 语句**

    变量定义都通过var关键字  
    变量可以先声明,后进行赋值;

**关键字和保留字**  
[保留关键字](http://www.runoob.com/js/js-reserved.html)

**数据类型**
* 数值类型(number)
`123,0.2,100.3,-4,-9.0,10e10`
`正整数,小数` 
* 布尔类型(Boolean)
`true false`
* 字符串类型(string)
`"1dasda","adasdasd"`
* 未定义类型(undefined)
`undefined`
* null类型(本质上是一个特殊类型的object)
`null`  
`var t=null; t就是null类型`
`vat m; //m==undefined`
* object类型(引用类型)
* function类型(函数类型)
`注释:typeof函数用来取值的类型`

**数据的表示范围**
* 数字的最大值,并不是所有浏览器都只支持到这个值,某些浏览器是可以超过的
`Number.MAX_VALUE;`
* 最小值
`Number.MIN_VALUE;`
* 超过最大值或最小值范围后将会显示:(正负无限)
    * 正Infinity
    * 负Infinity
* NaN
  * Not a number,非数字值,是数字类型,但是非常特殊的数字类型值
  * parseInt("s");把数字转换成整数,此时转换失败会返回NaN
  * 涉及到NaN的所有的操作都会返回NaN 
  * 判断是否是NaN使用isNaN方法
  * 数字除以0的时候,都返回NaN
