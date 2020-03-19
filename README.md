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
8. https://www.python.org/dev/peps/pep-0020/ 进一步开发的官方指导，有对应编号PEP
9. import this 可以展示出the zen of python。zen即日语中的“禅”
10. 谷歌也有自己的python style：英文版http://google.github.io/styleguide/pyguide.html or  
中文版  https://github.com/zh-google-styleguide/zh-google-styleguide
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
8.  > > 输出重新定向：e.g. !python -m pydoc abs>>. / abs.txt 可以把结果生成一个text并存储
9. % load是jupyter魔法命令，可以打开外部文件
10. !python -m pydoc -b 1234 可以查看自己所有的代码文档
11. 工具推荐 sphinx、Read The Docs
