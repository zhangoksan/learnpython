python是一门解释型的编程语言。

编译型：专门的编译器针对特定平台，翻译成该平台硬件执行的机器码，并包装成该平台所能识别的可执行程序的格式，这个转换过程称为编译（compile）。

跨平台不可用

解释型：专门的解释器对源程序逐行解释成特定平台的机器码并立即执行的语言。

python 3.6.5 包含（解释器 + lib + pip）

安装中的问题：

1. runtime error 缺失程序，缺少一个Windows补丁

2. path环境变量配置（python、pip）

   python: program\python\python36

   pip: program\python\python36\scripts

3. 卸载：卸载 + 需要删除安装目录

### 1.1 DOS命令

**DOS命令在C:\Windows\System32目录下**

1. cd 切换目录
2. dir 浏览目录
3. mkdir 创建新的目录
4. rmdir 删除目录
5. ipconfig 查看ip地址
6. ping 测试网络连接

---

设置python的环境变量

```python
python # 进入Python环境，写python程序
exit() # 退出环境
```

### 1.2 pip 包管理器

```python
pip		# 列出pip命令的说明
pip -V	# pip的版本
pip list	# pip 安装的包目录
pip install package	# 安装包
pip uninstall package # 卸载包
pip install package==version	# 安装指定版本的包
pip command --help	# 查看pip命令的使用帮助
pip freeze --help	# 把包名输出到指定文件
pip freeze > requirements.txt	# 将包输出到当前目录的requirements.txt文档
pip install -r requirements.txt	# 使用pip安装requirements.txt中依赖的文件
python -m pip install --upgrade pip	# 升级pip
```

pip安装的包在lib\site-packages文件夹中

---

### 1.3 执行程序

在cmd中先进入程序所在文件夹，输入

```python
python demo01.py
```

就可以执行python程序了。

### 变量

声明变量实际上就是给内存要空间。

变量类型：字符串，整型，浮点数，布尔类型，列表，字典，集合，元组

弱类型：声明的变量赋什么值就是什么类型的

```python
type(变量名) # 返回该变量的类型
```

变量命名规则：

- 由字母，数字，_ 组成，不能以数字开头
- 严格区分大小写
- 不能使用python的关键字

查看python的关键字

```python
import keyword
print(keyword.kwlist)
```

['False', 'None', 'True', 'and', 'as', 'assert', 'async', 'await', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']

建议：

- 驼峰式

  第一个单词之外以后的每个单词的首字母大写。

  如果定义类名，每个单词的首字母大写。

- 下划线式

  python中变量、函数命名推荐下划线式

---

### print函数

```python
# 1.用法
print('hello world!')
name = '小白'
print(name)

# 2.用法：print(name,age,gender)
age = 18
gender = 'boy'

print(name,age,gender) # sep默认的分割空格

# print(value,..., sep=' ', end='\n', file=sys.stdout, flush=False)
print(name,age,gender,sep='-') # sep='*' sep='$'

# 转义字符: \n 换行
print('hello\nkitty')
```

---

### 转义字符

```
# \n 换行 \t 制表符 \' \" \r 回车 \\ 
```

