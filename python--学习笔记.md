print(" "*N)---将字符串输出N次

input()---输入函数----用法temp=input()

---------------------------若括号内有字符串会输出

---------------------------若要读取输入的数字要用 E = int(temp)(E是范型)

Tab----按键的使用：

（1）缩进----一定要严格格式化不然程序会出错

（2）正确用冒号IDLE会自动缩进

BIF-----是内置函数----dir(__ builtins __)可以查看所有内置函数

------------------------help()这个BIF用于显示BIF的功能描述





random 模块有一个函数randint()-----返回一个随机数

布尔类型  true---相当整型1；false---相当整型0

类型转换---int(),float(),str()--转换为字符串

获得关于类型的信息----type()----获得数据类型的函数

------------------------------isinstance()----判断两个类型是否一样----返回true，false

算数操作符-----+ - * / % ** // *= += /= -=

------ 3//2=1;3.0//2=1.0

优先级问题---- -3*2+5/-2-4---->(-3) * 2+5/(-2) - 4 

** ----- 进行次幂运算 -----》 - 3 ** 2= - 9   ------3 ** - 2=0.111111111111

比较操作符------- < <= > >= == !=

逻辑操作符------- and    or       m   not



python中分支语句只有if---else----语句

三元操作符  a = x if 条件 else y-----------

assert 称为”断言“-----当这个关键字后边的条件为假时程序直接自动崩溃抛出AssertionError的异常

![image-20220117120547223](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220117120547223.png)

**for 循环语句**     他会自动调用迭代器的next()方法--会自动捕获StopIteration异常并自动结束循环

range()函数----range([start,] stop [,step=1])

for i in range(5):

​    print(i)  ------------------------->0 1 2 3 4

   range----中包括start不包括stop

break---跳出循环

continue---终止本轮循环并开始下一轮循环



**列表**--------python中没有数组是列表

（1）创建列表：number= [1,2,3,4,5]----number=[]---number = [1,"小甲鱼“,3.14,[1,2,3]]

（2）向列表添加元素：用append()方法----number = [1,2,3,4,5]------number.append(6)

















Python ------廖雪峰











![image-20220308232411052](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308232411052.png)

![image-20220308232616206](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308232616206.png)

标识符 ![image-20220308235556717](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308235556717.png)

![image-20220308235615493](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308235615493.png)

![image-20220308235651597](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308235651597.png)

![image-20220308235723012](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220308235723012.png)

![image-20220309000214053](C:\Users\Zqh041009\AppData\Roaming\Typora\typora-user-images\image-20220309000214053.png)

创造main.py文件实现功能（相当于测试）具体的实现代码在其他文件写

