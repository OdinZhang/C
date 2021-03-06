# 运算符与表达式

学习运算符时应注意：

1. 运算符的功能
2. 运算符对运算对象的限制
   * 运算对象个数
   * 操作数
   * 运算对象的类型
3. 表达式值的类型
4. 运算符的优先级
5. 结合方向
   * 左结合
   * 右结合

C语言运算符的优先级与结合性

| 优先级 |                            运算符                            |  结合方向   |
| :----: | :----------------------------------------------------------: | :---------: |
|   1    |         () [] .（取成员）->（指向成员）++ --（后缀）         | →（左结合） |
|   2    | !（逻辑非）~（按位取反）++ --（前缀）-（负）*（间接引用）&（取地址）sizeof（容量运算） | ←（右结合） |
|   3    |                            * / %                             |      →      |
|   4    |                             + -                              |      →      |
|   5    |                 <<（左移运算）>>（右移运算）                 |      →      |
|   6    |                    < <= > >=（关系运算）                     |      →      |
|   7    |                      == !=（关系运算）                       |      →      |
|   8    |                         &（按位与）                          |      →      |
|   9    |                       ^（按位异或与）                        |      →      |
|   10   |                       &#108;（按位或）                       |      →      |
|   11   |                         &&（逻辑与）                         |      →      |
|   12   |                    &#108;&#108;（逻辑或）                    |      →      |
|   13   |                       ? :（条件运算）                        |      ←      |
|   14   |      = += -= *= /= %= <<= >>= &= ^= &#108;=（赋值运算）      |      ←      |
|   15   |                        ,（逗号运算）                         |      →      |

