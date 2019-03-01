# switch语句

一般形式：

```c
switch(表达式)
{
    case 常量表达式1: 语句1;
        break;
    case 常量表达式2: 语句2;
        break;
    …
    case 常量表达式n: 语句n;
        break;
    default: 语句n+1;
}
```

在执行时先计算switch后的表达式的值，再与1~n个常量表达式的值进行比较，当表达式的值与某个case后常量表达式的值相等时，则执行该case后的语句，然后执行break语句跳出switch结构，若所有常量表达式的值都不等于switch后表达式的值，则执行default后的语句

### 注意：

1. case后的常量表达式的值应与switch后的表达式的值类型一致且都为整型或字符型
2. 同一个switch语句中所有case后常量表达式的值必须互不相同，否则会发生冲突
3. 当表达式的值与某个case后常量表达式的值相等时，则执行该case后的语句，然后执行break语句跳出switch结构，若所有常量表达式的值都不等于switch后表达式的值，则执行default后的语句
4. 各case和default顺序可以改变，但default前置时要加`break;`，最后的语句可以不加`break;`
5. 多个case可以用一组执行语句，直到遇到`break;`才停止，否则执行其后所有case（default）的执行语句
6. 每个case后可有任意多个语句，且无需使用花括号