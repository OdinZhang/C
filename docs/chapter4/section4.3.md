# for循环

一般形式：

```c
for(表达式1;表达式2;表达式3)
    语句;
```

说明：

1. 表达式1：一般为赋值表达式，为循环控制变量赋初值
2. 表达式2：一般为关系表达式或逻辑表达式，作为控制循环结束的条件
3. 表达式3：一般为赋值表达式，为循环控制变量增量或减量

`for(i = 1,sum = 0;i <= 100,i++)sum = sum + i`相当于

```c
i = 1,sum = 0;
while(i <= 100)
{
    sum = sum + i;
    i++;
}
```

说明：

1. for语句一般形式中表达式1可以省略，但`;`不能省略，次时应在for前给循环变量赋初值
2. 若表达式2省略，则默认始终为真
3. 表达式3也可省略，但需自行设置终止条件
4. 可以省略表达式1和3
5. 可以均省略，此时循环不会退出
6. 表达式1和3可以是任意表达式
7. 表达式2可以是关系表达式、逻辑表达式、数值表达式、字符表达式