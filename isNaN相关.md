# ISNaN函数
### NaN原理以及自身的特殊性
1. NaN 是唯一与自身不等的值。 
2. 如果isNaN函数的参数不是Number类型, isNaN()会首先尝试将这个参数转换为数值，然后才会对转换后的结果是否是NaN进行判断。
3. 如果是一个空串或是一个空格，而isNaN是做为数字0进行处理的
 布尔值会被强制转换为数值0或1

### NaN常见的特殊情况
> isNaN(NaN);       // true

>isNaN(undefined); // true

>isNaN(null);      // false

>isNaN(true);      // false


```
isNaN("37");      // false: 可以被转换成数值37
isNaN("37.37");   // false: 可以被转换成数值37.37
isNaN("");        // false: 空字符串被转换成0
isNaN(" ");       // false: 包含空格的字符串被转换成0
isNaN("blabla")   // true: "blabla"不能转换成数值

// dates
isNaN(new Date());                // false
isNaN(new Date().toString());     // true
isNaN({});        // true
```



 
 
 
 
 

