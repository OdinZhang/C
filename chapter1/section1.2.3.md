# C程序语句

- 执行语句

  - 表达式语句`t=a; a++`
  - 函数调用语句`printf("a=%d,b=%d\n",a,b);`
  - 流程控制语句

- 声明语句

  - `int a,b,t;`为声明语句，旨在给变量分配空间以方便存储数据
  - `;`为空语句，即在要求至少有一条语句但不做执行时使用

- 块语句

  - 语法中要求只能有一条语句，但难以用一条语句表达
  - 形成局部化封装体，一般语句块中定义的量仅在语句块中有效

  ```c
  #include "stdio.h"
  main()
  {
      int x = 1;
      {
          int x = 2;
          {
              int x = 3;
              printf("%d\n",x);
          }
          printf("%d\n",x);
      }
      printf("%d\n",x);
  }
  ```

  程序的运行结果为

  ```
  3
  2
  1
  ```