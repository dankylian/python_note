# 1.列表
## 标志
- 列表是Python中的一个对象
    - 对象（object）就是内存中专门用来存储数据的一块区域
    - 之前我们学习的对象，像数值，它只能保存一个单一的数据
    - 列表中可以保存多个有序的数据
    - 列表是用来存储对象的对象

## 基本操作(创建，append( )，pop( ) ,del( ), 拷贝）
- 创建列表

```python
# 创建列表，通过[]来创建列表
my_list = [] # 创建了一个空列表
```
- 切片

append（添加元素）
pop(移除列表中的一个元素（默认最后一个元素），并且返回该元素的值)
del（删除元素）
拷贝
```python
# 字符串的复制（将字符串和数字相乘）
a = 'abc'
# * 在语言中表示乘法
# 如果将字符串和数字相乘，则解释器会将字符串重复指定的次数并返回
a = a * 20
print(a)
```
### 列表相关方法

序号|方法|作用
---|:--:|---:
1|list.append(obj)|在列表末尾添加新的对象
2|list.count(obj)|统计某个元素在列表中出现的次数
3|list.extend(seq)|在列表末尾一次性追加另一个序列中的多个值（用新列表扩展原来的列表）
4|list.index(obj)|从列表中找出某个值第一个匹配项的索引位置
5|list.insert(index, obj)|将对象插入列表
6|list.pop([index=-1])|移除列表中的一个元素（默认最后一个元素），并且返回该元素的值
7|list.remove(obj)|移除列表中某个值的第一个匹配项
8|list.reverse()|反向列表中元素
9|list.sort( key=None, reverse=False)|对原列表进行排序
10|ist.clear()|清空列表
11|list.copy()|复制列表

列表包含的函数

序号|函数|作用
---|:--:|---:
1|len(list)|列出列表元素个数
2|max(list)|返回列表元素最大值
3|min(list)|返回列表元素最小值
4|list(seq)|将元组转换为列表


# 2.元组
## 标志
- 元组是一个不可变的序列
- 它的操作的方式基本上和列表是一致的
- 所以你在操作元组时，就把元组当成是一个不可变的列表就ok了
- 一般当我们希望数据不改变时，就使用元组，其余情况都使用列表

## 基本操作（创建及不可变性）
- 创建元组
```python
# 创建元组
# 使用()来创建元组
my_tuple = () # 创建了一个空元组
```
- 元组的不可变性
```python
my_tuple = (1,2,3,4,5) # 创建了一个5个元素的元组
# 元组是不可变对象，不能尝试为元组中的元素重新赋值
 my_tuple[3] = 10 
 print(my_tuple[3]) TypeError: 'tuple' object does not support item assignment
```

# 3.string字符串
定义及基本操作（`+`，`*`，读取方式）
- 字符串用来表示一段文本信息，字符串是程序中使用的最多的数据类型
- 在Python中字符串需要使用引号引起来
`+`字符串连接,拼串处理
`*`重复输出字符串
## 使用四种方式来输出，欢迎 xxx 光临
### 拼串
```python
print('欢迎 '+name+' 光临！')
```
### 多个参数
```python
print('欢迎',name,'光临！')
```
### 占位符
```python
print('欢迎 %s 光临！'%name)
```
### 格式化字符串
```python
print(f'欢迎 {name} 光临！')
```
## 字符串相关方法
[字符串操作方法大全](https://www.cnblogs.com/printN/p/6924077.html)
### 转义字符
可以使用 \ 作为转义字符，通过转义字符，可以在字符串中使用一些特殊的内容
例子：
  \' 表示'
  \" 表示"
  \t 表示制表符
  \n 表示换行符
  \\ 表示反斜杠
  \uxxxx 表示Unicode编码
# 4.字符串格式化问题
Python 支持格式化字符串的输出 。尽管这样可能会用到非常复杂的表达式，但最基本的用法是将一个值插入到一个有字符串格式符 %s 的字符串中。
[字符串格式化代码]（）