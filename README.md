# 数据结构上级题解合辑
吉林大学计算机系数据结构上机实验题,题解合辑

发现任何bug或者使用中的问题,欢迎email davidparkerhl@gmail.com
pdf题目下载链接:https://pan.baidu.com/s/1b9uJZUcrhpMXJi3xag5eew


编写基本原则:
除了进行函数传参之外,关键数据结构不使用任何c++ stl模板
有输出的函数只输出数据,不进行格式控制
所有的输入输出注释都为中文
所有的函数,除了专门做输出的函数只返回错误值不输出错误,错误处理由主调函数视返回值决定

技巧:
在编写有指针的数据结构中,每个push或pop函数需要注意 头尾指针,结构长度,当前状态(空结构,一个节点,多个节点)
本套代码编写时对于空结构,一个节点和多个节点均用不同的函数处理
尽量编写不同的函数处理不同的情况,良好的调用结构能很大程度上避免bug


第一周:

题目 1: 单链表相关算法的实验验证

[实验目的] 验证单链表及其上的基本操作。

[实验内容及要求]
1、 定义单链表类。
2、 实验验证如下算法的正确性、各种功能及指标:
1)创建单链表;
2)插入操作:分别在当前结点后、表头、表尾插入值为 x 的结点;
3)删除操作:分别删除表头结点、表尾结点和当前结点的后继结点;
4)存取操作:分别存取当前结点的值和单链表中第 k 个结点的值;
5)查找操作:查找值为 x 的元素在单链表中出现的位置(是链表中的第几个元素)。

3、 为便于观察程序的运行结果，设计的输出函数能在屏幕上以规范、直观的形式输出计算结果。例如将链 表输出成如下形式: [1]->[2] -> [3] -> [4] -> [5]
4、 测试程序时，对所有输入变量取遍各种有代表性的值。
5、 为了增强程序的可读性，程序中要有适当的注释。


题目 2:应用单链表实现一元多项式及其相加

[实验目的]应用单链表解决实际应用问题。

[实验内容及要求]
1、 使用自己在题目中已定义的单链表类。
2、 编写程序实现一元多项式的输入、输出和加法运算。
例如，一元多项式 1:x2+5x+3;一元多项式 2:2x2+5;加法运算结果:3x2+5x+8。
3、 为便于观察程序的运行结果，设计的输出函数能在屏幕上按照变量指数由高到低的形式输出多项式，例
如:3x^2+5x+8。
4、 为程序制定测试方案，对所有输入变量取遍各种有代表性的值。
5、 为了增强程序的可读性，程序中要有适当的注释。


第二周:
题目 1 堆栈相关算法的实验验证

[实验目的] 验证顺序存储的堆栈及其上的基本操作。

[实验内容及要求]
1、 定义顺序存储的堆栈类。
2、 实验验证如下算法的正确性、各种功能及指标:
1)创建顺序栈;
2)插入操作:向栈顶压入值为 x 的元素;
3)删除操作:弹出栈顶元素;
4)存取操作:读取栈顶元素。
3、 为了增强程序的可读性，程序中要有适当的注释。
4、 由教师随机给出栈操作指令序列，完成程序验证。
例如:(压栈 a，压栈 b，压栈 c，压栈 d，弹栈，弹栈，弹栈，压栈 e，弹栈，读栈顶，弹栈。屏幕应输出 d,c,b,e,a,a)

题目 2 链式队列相关算法的实验验证

[实验目的] 验证链接存储的队列及其上的基本操作

[实验内容及要求]
1、 定义链式队列类。
2、 实验验证如下算法的正确性、各种功能及指标:
1)创建链式队列;
2)插入操作:向队尾插入值为 x 的元素;
3)删除操作:删除队首元素;
4)存取操作:读取队首元素。
3、 为了增强程序的可读性，程序中要有适当的注释。
4、 由教师随机给入队出队操作指令序列，完成程序验证。


题目 3:检查一个算术表达式中的括号是否正确匹配
[实验目的]
检查存储在循环链表中的算术表达式s所包含的括号—— “(” 与 “)”、“[” 与 “]”、“{”与 “}”是否正确匹配

[实验内容及要求]
1、实现循环链表类。
2、创建循环链表s，通过用户逐个字符输入，完成s的初始化。
3、编写程序实现函数Check，并输出检查结果。
4、为增强程序的可读性，对程序中较难理解的语句要有准确、清晰的注释。
5、由教师随机给出测试数据，程序能够反馈括号是否匹配，如果不匹配，指出第一个不匹配所在位置。

题目 4:字符串替换

[实验内容及要求]
用户输入字符串 S1, S2 和 S3，试设计并实现满足如下要求的程序:
1. 若S2是S1的子串，用串S3代替串S1中的所有S2 子串(S2在S1中可能 出现 1 次或多次);
2. 若 S2 不是 S1 的字串，用 S3 的逆序列替换 S1 的最后 n 位字符，n 是 S3 中的字符数量。

例如:
若S1=“aabacdacaabcca”,S2=“abac”,S3=“acccaea” 替换后 S1=“aacccaeadacaabcca”
若 S1=“accadadacaabcca”,S2=“abac”,S3=“acccaea” 替换后 S1=“accadadaaeaccca”

第三周
题目 1:二叉树相关算法的实验验证
[实验目的] 验证二叉树的链接存储结构及其上的基本操作

[实验内容及要求]
1、 定义链接存储的二叉树类
2、 实验验证如下算法的正确性、各种功能及指标:
1)创建一棵二叉树，并对其初始化;
2)先根、中根、后根遍历二叉树;
3)在二叉树中搜索给定结点的父结点;
4)搜索二叉树中符合数据域条件的结点;
3、 由教师随机指定树结构，测试上述功能;

题目 4:
题目: 判别给定二叉树是否为完全二叉树
[实验目的]
在掌握二叉树的链接存储及基本操作的基础上，设计解决问题的算法。

[实验内容及要求]
设计算法判别给定二叉树 t 是否为完全二叉树;实现链接存储的二叉树类。

第四周
题目 1:树和森林的遍历算法的实验验证
[实验目的] 验证树和森林的遍历算法
[实验内容及要求]
1、 定义左儿子—右兄弟链接存储的树类和森林类。
2、 实验验证如下算法的正确性、各种功能及指标:
1)创建树和森林;
2)树和森林的先根遍历的递归和迭代算法;
3)树和森林的后根遍历的递归和迭代算法;
4)树和森林的层次遍历算法。


第五周
题目 邻接表存储的图相关算法的实验验证
[实验目的] 验证邻接表存储的图及其上的基本操作
[实验内容及要求]
1. 定义邻接表存储的图类。
2. 实验验证如下算法的正确性、各种功能及指标:
1)创建一个邻接表存储的图;
2)返回图中指定边的权值;
3)插入操作:向图中插入一条边;
4)删除操作:从图中删除一条边。
5)查找图中某顶点的第一个邻接顶点
6)图的深度优先遍历和广度优先遍历
3. 为了增强程序的可读性，程序中要有适当的注释。

第六周
题目 1:快速排序算法的实验验证
[实验目的] 验证快速排序算法。
[实验内容及要求]
实现快速排序算法
理论分析并实验测试算法在最好、最坏及平均情况下的时间复杂性。


题目 2:堆排序算法的实验验证
[实验目的] 验证堆排序算法
[实验内容及要求]
实现堆排序算法，理论分析并实验测试算法在最好、最坏及平均情况下的时间复杂性。
