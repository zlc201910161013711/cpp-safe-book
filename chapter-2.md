# 第2章-字符串



## 2.1 字符串

### 2.1.1字符串数据类型

字符串由第一个空字符作为结束的连续字符序列组成，并包含此空字符。

一个指向字符串的指针实际上指向该字符串的起始字符。

字符串长度指空字符之前的字节数。

字符串的值则是它所包含的按顺序排列的字符值的序列。

`hello`的字符串表示形式：

h | e | l | l | 0 | \0

定义：

**界限（Bound）**

数组中元素个数

**低位地址（Lo）**

数组首元素地址

**高位地址（Hi）**

数组末元素地址

**TooFar**

数组最远端的元素加1位置的元素地址，这个元素正好在Hi元素之后。

**目标大小（Tsize）**

与`sizeof(array)`相同

C标准允许创建指向数组对象的末元素之后加1位置的指针。虽然这些指针无法在不产生未定义行为的状况下解引用。在处理字符串时，以下额外的术语也很有用。

**空字符结尾**

在Hi或它之前，存在空终结符。

**长度**

空终结符之前的字符数量。

