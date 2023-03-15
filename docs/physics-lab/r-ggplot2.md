[^1]: [R 语言教程 李东风](https://www.math.pku.edu.cn/teachers/lidf/docs/Rbook/html/_Rbook/index.html)

## 基础语法

### IO 交互

`print()` 函数

```
print("RUNOOB")
print(123)
print(3e2)
[1] "RUNOOB"
[1] 123
[1] 300
```

`cat()` 函数

```
cat(1, "加", 1, "等于", 2, '\n')`
```

`cat()` 会在每两个拼接元素之间自动加上空格。

### 运算符

下表列出了主要的数学运算符以及他们的运算顺序：

| 优先级 | 符号 | 含义     |
| :----- | :--- | :------- |
| 1      | `()`   | 括号     |
| 2      | `^`   | 乘方运算 |
| 3      | `%%`   | 整除求余 |
|        | `%/%`  | 整除     |
| 4      | `*`    | 乘法     |
|        | `/`    | 除法     |
| 5      | `+`    | 加法     |
|        | `-`    | 减法     |

下表列出了主要的逻辑运算符

|运算符|描述|
|:---|:---| 
|`&`|元素逻辑与运算符，将第一个向量的每个元素与第二个向量的相对应元素进行组合，如果两个元素都为 TRUE，则结果为 TRUE，否则为 FALSE。|
|`|`|元素逻辑或运算符，将第一个向量的每个元素与第二个向量的相对应元素进行组合，如果两个元素中有一个为 TRUE，则结果为 TRUE，如果都为 FALSE，则返回 FALSE。|
|`!`|逻辑非运算符，返回向量每个元素相反的逻辑值，如果元素为 TRUE 则返回 FALSE，如果元素为 FALSE 则返回 TRUE。|
|`&&`|逻辑与运算符，只对两个向量对第一个元素进行判断，如果两个元素都为 TRUE，则结果为 TRUE，否则为 FALSE。|
|`||`|逻辑或运算符，只对两个向量对第一个元素进行判断，如果两个元素中有一个为 TRUE，则结果为 TRUE，如果都为 FALSE，则返回 FALSE。|

### 数据类型

!!! warning "下标从 1 开始"
    R 语言中的**下标**不代表偏移量，而代表第几个，也就是说是从 1 开始的！

**vector**

`c()` 是一个创造向量的函数。

```
> a = c(3, 4)
> b = c(5, 0)
> a + b
[1] 8 4
```

### 流控制语句

!!! note "相同点"
    R 语言中的 `if` 语句和 `while` 语句与 C 语言中的相同。

    `break`

## ggplot 绘图

[^3]: [ggplot2: elegant graphics for data analysis](https://ggplot2-book.org/)
[^2]: [ggplot 作图入门](https://www.math.pku.edu.cn/teachers/lidf/docs/Rbook/html/_Rbook/ggplot2.html)

### 安装

```
install.packages("ggplot2")
```

### 快速上手

## 参考
