# CMPEN 472 Homework 7

## 1. 作业目标
- 学习如何使用算术指令、简单的命令行解析以及编写基本的I/O系统子例程。

## 2. 作业要求
### 2.1程序功能
- 编写一个程序，在连接到HCS12板的超级终端上实现一个基本的计算器。
### 2.2输入规则
- 仅输入正的十进制整数。
- 输入和输出的数字最多为四位。
- 有效的运算符为：+，-，*，/。
- 输入带前导零的数字是可以的。
- 仅输入两个数字和它们之间的一个运算符，不允许有空格。
### 2.3输出规则
- 显示'Ecalc> '提示符，并回显用户的按键，直到按下回车键。
- 重复打印用户输入，并在'='符号后打印答案。
### 2.4错误处理
- 如果输入格式无效，重复打印用户输入直到错误字符，并在下一行打印错误消息：'Invalid input format'。
- 保持16位内部二进制数格式，检测并标记溢出错误。
- 使用整数除法并截断任何分数。
### 2.5程序设计
- 程序从$3100开始，数据从$3000开始。
- 要添加大量注释，以便评分者和其他人能够清晰快速地理解程序。

## 3. 示例输入输出
### 3.1 正确输入输出
```
Ecalc>
Ecalc> 123+4
       123+4=127
Ecalc> 96*15
       96*15=1440
Ecalc> 003-678
       003-678=-675
Ecalc> 555/3
       555/3=185
```
### 3.2 错误输入输出
```
Ecalc> 456@5
       456@
       Invalid input format
Ecalc> 7h4*12
       7h
       Invalid input format
Ecalc> 3*54312
       3*54312
       Invalid input format ;due to 5th digit
Ecalc> 100+999*2
       100+999*
       Invalid input format
Ecalc> 7*(45+123)
       7*(
       Invalid input format
Ecalc> 78*9999
       78*9999
       Overflow error
Ecalc> -2*123
       -
       Invalid input format
```

## 4. 提交要求
- 将'main.asm'文件复制为'cmpen472hw7_YourLastName.asm'（例如'main.asm'为我的文件，复制后为'cmpen472hw7_choi.asm'），不要压缩文件。
- 通过宾夕法尼亚州立大学的CANVAS提交项目源代码文件。将源代码文件上传到CANVAS作业的作业提交中，确保选择CMPEN 472课程和正确的作业编号以及正确的文件名。
# CMPEN472 Homework 7

# CS Tutor | 计算机编程辅导 | Code Help | Programming Help

# WeChat: cstutorcs

# Email: tutorcs@163.com

# QQ: 749389476

# 非中介, 直接联系程序员本人
