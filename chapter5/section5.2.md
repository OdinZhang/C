# 二维数组

#### 1. 定义

一般形式为：

`类型名 数组名[常量表达式1][常量表达式2]`

其中二维数组命名规则、类型名与一维数组相同，但[常量表达式1]用来指定二维数组的行数，[常量表达式2]用来指定二维数组的列数

#### 2. 二维数组元素的引用

引用形式为：

`数组名[下标值1][下标值2]`

其余特性与一维数组相似

同样的，还可以定义多维数组：

`int a[4][5][6];`

#### 3. 二维数组的初始化

二维数组的初始化有两种方法：

* 对数组的全部元素赋初值：

  1. 整体赋初值：

     `int a[3][4] = {1,2,3,4,5,6,7,8,9,10,11,12};`

  2. 分行赋初值：

     int a[3][4] = \{\{1,2,3,4},{5,6,7,8},{9,10,11,12\}\};

     在对全部元素赋初值时，第一维的长度可以省略，如：

     int a[][4] = \{\{1,2,3,4},{5,6,7,8},{9,10,11,12}};

* 对数组的部分元素赋初值

  部分赋值是对数组中各行对应位置的元素赋初值，没有指定元素则自动赋值为0

  在对数组的部分元素赋初值时同样可以省略第一维长度的指定

#### 4. 二维数组的输入/输出

二维数组的输入输出需要两重循环，例如：

```c
# include<stdio.h>
main()
{
    int a[3][2];
    int i,j;
    for(i = 0;i < 3;i++)
        for(j = 0;j < 2;j++)
            scanf("%d",&a[i][j]);
    for(i = 0;i < 3;i++)
    {
        for(j = 0;j < 2;j++)
            printf("%d",&a[i][j]);
    	printf("\n");
    }
    printf("\n");
}
```