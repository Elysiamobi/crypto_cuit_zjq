# crypto_cuit_zjq
practice codes AES变换操作的实现

一、实验目的

（1）加深对AES算法的理解；

（2）阅读标准(fips-197)和文献，提高自学能力；

（3）加深对模块化设计的理解，提高编程实践能力。

二、实验内容

（1）按照AES算法，完成AES算法S盒、行移位、列混合、轮密钥加操作；

三、实验要求

（1）把AES的S盒、行移位、列混合、轮密钥加操作写成一个函数，然后再主程序中调用；

（备注：函数名称命名方式 ****_学号后2位，变量名称***_学号后2位，例如学号为“2018011263”S盒函数 SubBytes_63(unsigned char  input_63[4][4]）

（2）输入128bits一个状态矩阵，输入为16进制数。状态矩阵的录入为一行，比如:

00 11 22 33 44 55 66 77 88 99 aa bb cc dd ee ff

则轮密钥加的子密钥如：

00 01 02 03 04 05 06 07 08 09 0a 0b 0c 0d 0e 0f(请注意这里是列向优先读取数据的)

（3）与标准中的样例进行比较,输入标准中样例，测试S盒、行移位、列混合和轮密钥加算法正确。

输出要求：

（1）程序的输出部分写在主程序中，可以是4行4列，也可以为一行。若为一行，输出也要求为列向优先。

（2）实验程序测试中，二组测试结果

第1组：

状态矩阵的录入为一行，比如:

00 11 22 33 44 55 66 77 88 99 aa bb cc dd ee ff

则轮密钥加的密钥如：

00 01 02 03 04 05 06 07 08 09 0a 0b 0c 0d 0e 0f

输出轮密钥加、字节替代、行移位、列混合之后的测试结果。

下面数据来自fips197：

<img width="273" alt="image" src="https://github.com/Elysiamobi/crypto_cuit_zjq/assets/118823579/68fa7b4c-a48a-427b-a218-2e1a6690be76">

第2组 例如学号为“2018011263”

状态矩阵的录入为一行，比如:

20 18 01 12 63 00 00 00 00 00 00 00 00 00 00 0B 

则轮密钥加的密钥如：

00 01 02 03 04 05 06 07 08 09 0a 0b 0c 0d 0e 0f

输出轮密钥加、字节替代、行移位、列混合的测试结果

（3）认真填写实验报告。

（4）截图最好有个人信息，比如输出执行的文件的路径或者有学号或者姓名等。

（5）截图最好前景是运行界面，背景是运行界面未遮住的一部分代码。

（6）代码附在实验报告的后面，排版整齐美观。
