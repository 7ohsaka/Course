# Course
Something about my software learning
* 软件安装来自guide/doc/BuildingSoftwareEnvironment.md 
## 0305
1. Numpy : N-dimensiona
2. scipy  scientific computing
3. matplotlib Comprehensive 2-D plotting
4. pandas :Data structure analysis
### 成绩说明
* 线上点名+课堂练习 20
* 编码练习 50
* 期末考试 30
### 编程练习（practice）说明
* 比较综合性，有一定代码量和一定难度，注意截止时间，用email提交
1. data analysis（基本数据处理）
2. object-oriented programming（面向对象：朗肯循环，参考例程）
3. C/C++ progranmming（GCC）
### Unit1-1-INTRODUCTION_TO_PYTHON
tips：
1. ./是当前目录；./home当前目录下的home目录
2. %对行；%%对单元块（格）
内容；
1. -c 编译
2. -0 编译的输出文件名
3. ！ 是执行系统命令
4. dir查找指定的文件，* 是通配符
5.%ldir  显示目录下所有内容
6 %lsmagic 显示所有魔法命令
## 0312
tips:  
1. python是动态的，C语言是静态的；  
2. python更灵活，但是结果容易出错；  
3. python对大小写敏感
4. bool型——True和False
5. 空类型 None 不是0没有值
6. // 向下取整
7. 单行字符串''或者''... '';多行字符串 '''...'''
8. 编号从0开始，跟C语言一样
9. python范围是“左闭右开”原则（！分片等操作时应该注意！）
10. 字符串定义之后不能直接改变其中某项，需要使用函数或者切片方法
11. 分片操作高级用法：s[i:j:k] 表示从i开始到j-1项，步长为k
12. 上例中若k为负数，表示从右往左取；若i，j为负数，则对应从右往左的范围，注意最末尾项为-1
13. 不想进行转义的时候在前面加上r （row）
## 0316
### Unit1-2-Control-Flow
tips：  
1. python用对齐的方式来代替花括号，简洁明了
2. Improper indent: Syntax error 语法错误，比较容易发现
3. Improper indentation: Semantic error 语意错误，语法虽然正确，不容易发现
4. if语句条件后记得加**冒号**
5. 行连续可以用括号进行处理，括号务必匹配
6. for循环for i in range：  
range(stop)  
range(start, stop)  
range(start, stop[, step])  
7. continue 跳出本次循环后面的语句，进行下一次循环
8. [进一步开发的官方指导](https://www.python.org/dev/peps/pep-0020/) ，有对应编号PEP
9. import this 可以展示出the zen of python。zen即日语中的“禅”
10. 谷歌也有自己的python style：[英文版](http://google.github.io/styleguide/pyguide.html) or  
[中文版](https://github.com/zh-google-styleguide/zh-google-styleguide)
## 0319
### Unit1-3-FUNCTIONS_SCOPING_AND_ABSTRACTION
tips:  
1. 函数定义关键字：def，结尾必须加 **冒号**
2. 位置变量和关键词变量：位置变量是在对应位置输入实参，关键词变量是写出实参赋值给形参。注意！关键词变量一旦开始使用，后面的都得用关键词变量！
3. e.g. 二分法练习
4. 函数定义也可以用lambda方法定义：adder = lambda x, y: x+y  
adder为函数名，x，y为形参
5. print函数：可以控制输出的格式等等  
    print(value, ..., sep=' ', end='\n', file=sys.stdout, flush=False)  
    Prints the values to a stream, or to sys.stdout by default.   
    Optional keyword arguments:      
    file:  a file-like object (stream); defaults to the current sys.stdout.        
    sep:   string inserted between values, default a space.      
    end:   string appended after the last value, default a newline.      
    flush: whether to forcibly flush the stream.  
6. print(str.format())用于输出字符串的格式控制：  
:4d for integer,  
:6.2f for floating-point number  6-距离 2-小数保留位数
:5s for string  
< 和 >左右对齐  
^ 中间对齐  
7. 函数定义时加上文档串便于help()查找用法,也方便自己理解，可用print(函数名,_ doc _ 调用)
8. “>> 输出重新定向：e.g. !python -m pydoc abs>>. / abs.txt ”可以把结果生成一个text并存储
9. % load是jupyter魔法命令，可以打开外部文件
10. !python -m pydoc -b 1234 可以查看自己所有的代码文档
11. 工具推荐 sphinx、Read The Docs
## 0326
tips:  
1. 模块的引用：import / from .. import *(*表示所有变量)
2. 寻找路径首先在当前路径下寻找、然后找是否是内置函数、安装包里面找
3. sys.path.append()可以加入到路径
4. move 可以移除路径
5. run as a script _ name__  is' __ main __ '，只作为脚本时运行需要加上条件，可以使得引用时不运行，双下划线
6. Packages软件包进行脚本文件管理：__ init__.py can just be an empty file,用于简化导入语句，不用再一层一层去找
7. python的主要结构类型：元组（tuple）、列表（list）、字典（dict）
8. tuple用圆括号加**，**定义，里面不一定是同一类型
9. 元组可以进行索引（**从0开始**）、分片、相加等操作
10. 元组不可直接对某个项进行赋值，跟str一样；可以用分片方法进行操作
11. 元组也是序列类型，可以用for遍历
12. 元组的常用操作或函数：len(),max(),min(),sum(),tup.count(),tup.index()
13. 函数可以返回元组类型
## 0330
tips：  
1. 列表用[]定义
2. 列表是可变的，不像元组需要创立一个新的元组,可对其中元素进行编辑
3. list.append()和‘+’运算的结果不相同，前者是把整体作为一个元素合并，后者是把每个元素合并
4. list.extend()和‘+’运算的效果一样，都是添加的每一项，但是不创建新的列表
5. [更多的列表用法](https://docs.python.org/tutorial/datastructures.html#more-on-lists)
6. list.count()\list.index()——计数、索引
7. 
* del L[i]: delete the item at index i in L 

* L.clear(), remove all the items from the lst and return None; same as del L[:].

* L.remove(e),  deletes the first occurrence of e from L

* L.append(e), adds the **object** e to the end of L.

* L1.extend(L2), adds **items** in the list L2 to the end of list L1

* L.insert(i, e), inserts the object e into L at index i.

* L.pop(i), removes and returns the item at index i; i defaults to -1. Raises IndexError if L
is empty.

* L.copy(): return a copy of L; same as L[:]

* L.reverse(): has the side effect of reversing the order of the elements in L.

* L.sort(): arranges the elements of the list from low to high.
8. pop和remove的区别：pop返回的是你弹出的那个数值；remove 是删除首个符合条件的元素。并不是删除特定的索引
9. 值相等不等于对象相等，还应该有地址相等
10. 列表不能直接复制给另外一个列表，实际a=b只是赋值了名字，没有赋值内容（其他对象也是一样，python特色）
11. 一般用克隆的方法解决上面的问题，分片克隆方法或者浅\深拷贝
12. 克隆方法汇总      
<strong style="color:blue;font-size:100%">slicing：L1[:]</strong>  

<strong style="color:blue;font-size:100%">list(L1)</strong>  

<strong style="color:blue;font-size:100%">copy.copy(x)</strong>  

<strong style="color:blue;font-size:100%">copy.deepcopy(x)</strong>  
13. [expr for var in list] 对列表元素进行操作，相当于一个循环语句
## 0402
tips：
1. 字符串分离可以指定分割符号：`str.split()`,里面不带任何参数按照默认的符号作为分割
2. 字典用花括号定义，每个元素是`key:value` 组成
3. **字典里没有索引的，是无序的，通过key来找值**
4. key只能是不可变类型，比如列表就不能作为key
5. 字典跟列表一样，是可变类型；元组和字符串是不可变的
6. 普通的遍历循环输出不是输出整个键值对，而是输出key；遍历`dic.items()`可以输出键值对
7.  
* **dict.keys()** :reture is a `dict_keys` object, which is an iterator 
        
* **dict.values()** reture is a `dict_values` object, which is an iterator 
    
* **dict.items()**:reture is a `dict_items` object, which is an iterator that iterates the `key-value` pairs
8. 字典常用方法汇总：  
* `d.keys()`： returns a view of the keys in d.

* `d.values()`： returns a view of the values in d.

* `d.items()`： return a new view of the dictionary’s items <strong style="color:blue">(key, value)</strong> pairs  in **tuple** 

* `d[k]` ：returns the item in d with key k. Raises KeyError if k is not in d.

*  `d[k] = v`： associates the value v with the key k. If there is already a value associated
with k, that value is replaced.

* `for k in d` iterates over the keys in d.

* `d.update(d1)`: merge the given dictionary d1 into d. Override the value if key exists, else, add new key-value.

* `len(d)`： returns the number of items in d.

* `d.pop()`: simultaneously returns the value and deletes the key

* `d.has_key()`:

* `k in d` ：returns True if key k is in d.

* `d.get(k, v)`： returns d[k] if k in d, and v otherwise.

* `del d[k]`： removes element with key k from d. Raises KeyError if k is not in d.

* `d.clear()`: removes all elements from d

* `d.copy()`: return a copy of  d
9. 现代C++:[Welcome back to C++ - Modern C++](https://docs.microsoft.com/en-us/cpp/cpp/welcome-back-to-cpp-modern-cpp?view=vs-2019)
