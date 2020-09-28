### 格式化输出

%s

``` python
person = '大圣'
address = '北京市海淀区中关村'
phone = '15858588888'
# 占位符，字符串的格式化输出
print('姓名：%s,收货地址：%s，联系方式：%s' % (person, address, phone))
```

%d

```python
age = 18
print('年龄是：%s' % age)	# %s --> str简写  底层：str(age) --> '18'
# 年龄是：18
print('年龄是：%d' % age)
# 年龄是：18
age = 18.5
# %d --> digit简写  底层: int(age) --> 18
print('年龄是：%d' % age)	# 年龄是：18
```

%f

```py
print('%.1f' % 2001.26)		# 2001.3
```

format

format是一个字符串中的函数，.format() 中的'.'是调用的意思

---

print() 

输出

变量，常量（大写）

格式化输出：

输出字符串：

1. 占位符 %s %d %f

   ```py
   print('%s%d%f' % (value, value, value))
   ```

   类型转换：

   int --> str

   age = 18 --> int

   str(age) -->'18'

   

   str --> int

   s = '18'

   int(s) --> 18

   s = '18a'

   int(s) --> TypeError

   

2. format

```py
print('{},{}'.format(value, value))
```



运算符

1. 算数运算符

```
+ - * / % ** //
```

2. 赋值运算符

```
= += -=
```

3. 关系运算符

```
< <= > >= == != is, is not
```

is 通过id()函数进行判断

小整数对象池[-5,256]的id是定义好的，id值一样，大整数在终端id不一样，在pycharm中有大整数对象池，id是一样的

4. 逻辑运算符/布尔运算

```
and, or, not
```

5. 位运算

```
| 或, ^ 异或, & 与, x << n 左移n位, x >> n 右移n位, ~x 逐位取反
```

正负数的二进制表示，补码运算(整数取反+1)

进制转换

0b 二进制 0o 八进制 0x 十六进制

6. 三目运算符

   格式：结果（真） if 表达式  else 结果（假）

7. 运算符的优先级

   由高到低排序：

   **

   ~

   +-(符号运算符)

   */ // %

   +- 加减

   << >>

   &

   ^

   |

   == != > >= < <=

   is is not

   not

   and

   or

if语法：

```
if 条件1:
	符合条件1（条件为True）才会执行的语句
elif 条件2:
	符合条件2（条件为True）才会执行的语句
else:
	其他
```

for语法：

```
for 变量名 in 集合:
	语句
```

应用场景：

1. 猜大小--反复猜
2. 消消乐--反复充值
3. 用户登录--登录多次

