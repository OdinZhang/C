# break和continue语句

`break;`

终止switch或循环语句的执行，跳出当前break所在的控制结构，转去执行后继语句

1. 只能在循环体内和switch语句体内使用break语句
2. 在多重循环嵌套中，break语句仅跳出它所在的那一层循环结构，不能跳出（或终止）多层循环结构

`continue;`

终止本次循环的执行，直接开始下一次循环的执行

> **[warning] 注意**
>
> 1. continue语句只能用于循环语句
> 2. 在（do-）while中continue立即去检查循环控制表达式，在for中立即转向执行表达式3