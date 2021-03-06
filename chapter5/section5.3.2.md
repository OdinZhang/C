# 字符串处理函数

#### 1. `strlen()`函数

用来测试字符串的长度，一般形式为：

`strlen(字符数组)`

其中：

1. 该参数会返回一个整数，数值即字符串的实际长度值（不包括'\0'在内）
2. 参数可以写成字符数组名，也可以是一个字符串常量

#### 2. `strcmp()`函数

该函数是用来比较两个字符串的大小，一般形式为：

`strcmp(字符串1,字符串2)`

其中：

1. 两字符串可以是字符数组名或字符串常量
2. 两字符串比较结果与返回值关系如下：
   1. 若字符串1等于字符串2则返回0
   2. 若字符串1大于字符串2则返回正数
   3. 若字符串1小于字符串2则返回负数

3. 字符串的比较规则：

   对两字符串从左到右逐个字符相比（按ASCII码值大小比较），直到出现不同或遇到”\0“为止，若全部字符相同，则认为相等，否则，以第一个不同字母的ASCII值比较结果为准

   若直接比较大小（`str1>str2`类型比较的是两个字符串的首地址

#### 3. `strcat()`函数

该函数是连接两个字符串，一般形式为：

`strcat(字符数组1,字符数组2)`

其中：

1. 把字符串2的结果连接到字符串1的后面，结果放在字符串数组1中，函数会返回字符数组1的地址，字符数组1必须写成数组名，字符数组2既可以为数组名也可以为字符串常量
2. 字符数组1的长度要足够大以容纳连接的字符串
3. 连接前，两字符数组末尾都有"\0"，连接后仅第二个后面有

#### 4. `strcpy()`函数和`strncpy()`函数

这两个函数是字符串复制函数，一般形式为：
`strcpy(字符数组1,字符数组2)`

把字符数组2的值复制进字符数组1中

`strncpy(字符数组1,字符数组2,n)`

把字符数组2的前n个字符复制进字符数组1中

其中:

1. 字符数组1要足够大来容纳复制的字符串
2. 函数的返回值是字符数组1的地址
3. 字符数组1必须写成数组名，字符数组2既可以为数组名也可以为字符串常量

> **[danger] 注意**
>
> `strcpy()`会把字符数组2后的” \0“一并复制进字符数组1

另：

> **[warning] 注意**
>
> 不能将一个字符串常量或字符数组直接赋值给一个字符数组

