JAVA
Java基础又叫JavaSe

就业方向：

JavaEE软件工程师

大数据软件工程师

Android软件工程师

JavaSE
1.1、建立编程思想
1.1.1、Java概述
Java历史
1、Java之父：詹姆斯·高斯林

2、1995年sun公司正式发布Java第一个版本

3、2009年sun公司被甲骨文公司收购

4、Java版本被使用最多的是Java7、Java11

程序：计算机执行某些操作或解决某个问题而编写的一系列有序指令的集合。 

//创建一个记事本，更改文件后缀为java


//打开此记事本，编写最简单的程序，完成1+1。
public class Test {
    public static void main(String[] args) {
        int res = 1 + 1;
        System.out.println("结果=" + res);
    }
}

/**
全选这个记事本的绝对路径并输入cmd
javac Test.java 编译这段程序，让计算机能够读懂
java Test 计算机执行这段程序
**/
Java技术体系
J2SE：
1、Java标准版
2、基础语法
3、一般用于图形化界面的开发

J2EE
1、Java企业版/网页版
2、JavaWeb开发
3、在J2SE基础上增加新的组件

Java特点
1、Java语言是面向对象的（oop）

2、Java语言是健壮的（强类型机制、异常处理、垃圾自动收集等）

3、Java语言是跨平台性的（一个编译好的.class文件可以在不同的系统下运行）

4、Java语言是解释型语言

Java运行机制
1、Text.java程序编译为Text.class。有了.java源文件，通过编译器将其编译成JVM可以识别的字节码文件。

2、通过运行工具java.exe对字节码文件进行执行，本质就是将.class装载到JVM执行。

3、因为有了JVM（Java Virtual Machine，即Java虚拟机），同一个Java程序可以在三个不同的操作系统中都可以执行。（JVM for Linux、JVM for Windows、JVM for Mac）

4、JVM是一个虚拟的计算机，具有指令集并使用不同的存储区域。负责执行指令，管理数据、内存、寄存器，包含在JDK中。 

5、.java文件为源文件、.class文件为字节码文件

6、修改过的源文件需要重新编译为字节码文件再执行。

JDK
1、JDK，全称Java Development Kit，即Java开发工具包。

2、JDK=JRE+java的开发工具（java、javac、javadoc、javap等）

3、JRE，全称Java Runtime Environment，即Java运行环境。

4、JRE=JVM+Java的核心类库（类）

5、JDK是提供给Java开发人员使用的，其中包含了java的开发工具，也包括了JRE，所以安装了JDK就不需要单独安装JRE。

6、如果只想运行一个开发好的.class文件，计算机中只需要安装JRE即可。

即JDK=JVM+java开发工具+java核心类库。

7、JDK提供开发环境、JRE提供运行环境。

查看JDK版本：命令行输入java -version

配置环境变量
为什么要配置环境变量：当前执行的程序在当前目录下如果不存在，win11系统会在系统中已有的一个名为path的环境变量指定的目录中查找，如果仍未找到，会出现‘javac’不是内部或外部命令，也不是可运行的程序或批处理文件这样的错误提示。

配置环境变量步骤：

1、我的电脑-属性-高级系统设置-环境变量

2、增加JAVA_HOME这个用户变量，指向JDK的安装目录E:\JDK\Windows\JDK8\JDK_8

3、编辑path这个用户变量，增加环境变量%JAVA_HOME%\bin

4、打开命令行，任意目录下敲入javac和java，若出现参数信息则配置成功。

Java的快速入门
/*
1、public class Hello 表示Hello是一个类，是一个public公有的类
2、Hello{} 表示一个类的开始和结束
3、public static void main(String[] args) 表示一个主方法，即我们程序的入口
4、main(){} 表示方法的开始和结束
5、System.out.println("hello,world"); 表示输出"hello,world"到屏幕
6、; 表示语句结束
*/

public class Hello {

	public static void main(String[] args){
		System.out.println("hello,world");
	}
}

/*
Sublime Text文件中有中文时，javac Hello.java编译出错如何处理：
1、首选项-Package Control-Package Control: Install Package-ConverToUTF8
2、文件-Set File Encoding to-Chinese Simplified(GBK)-保存
*/
Java开发细节
1、Java源文件以.java为扩展名，源文件的基本组成部分是类。

2、Java应用程序的执行入口是main方法，有固定的书写格式。public static void main(String[] args){}。

3、Java语言严格区分大小写。

4、Java方法由一条条语句构成，每个语句以";"结束。

5、大括号都成对出现，缺一不可。

6、一个源文件中最多只能有一个public类，其他类的个数不限。编译后，每一个类都对应一个.class字节码文件。

public class Hello{
    public static void main(String[] args){
        System.out.println("JXS Hello");
    }
}

class Dog{
    
}

class Tiger{
    
}
7、 如果源文件包含一个public类，则文件名必须按该类名命名。

8、一个源文件中最多只能有一个public类，其他类的个数不限，也可以将main方法写在非public类中，然后指定运行非public类，这样入口方法就是非public的main方法。

9、类名首字母必须大写，其余部分采用驼峰命名法（多个单词之间第二个单词首字母大写）。

10、在编写代码的过程中我们需要通过合适的缩进（tab）体现出代码的层级关系。

Java学习方法
1、需求

2、是否能使用传统技术解决

3、引出学习的新技术和知识点

4、学习新技术或者知识点的基本原理和基本语法

5、快速入门（基本程序 增删改查crud）

6、深入研究技术的注意事项、使用细节、使用规范、如何优化...

转义字符
public class ChangeChar{
	public static void main(String[] args) {
        // \t ：一个制表位，实现对齐功能
		System.out.println("北京\t天津\t辽宁\t吉宁\t黑龙江");
        // \n ：换行
		System.out.println("浙江\n福建\n广东\n广西\n贵州");
        // \\ ：一个\
		System.out.println("E:\\Downloads\\Sublime Text_Downloads");
        // \" ：一个"
		System.out.println("蒋兴树说:\"我真的很帅\"");
        // \' ：一个'
		System.out.println("蒋兴树说:\'我真的很帅\'");
        // \r ：回车
		System.out.println("蒋兴树\r丁维一");	
	}
}

/*
输出结果：
北京    天津    辽宁    吉宁    黑龙江
浙江
福建
广东
广西
贵州
E:\Downloads\Sublime Text_Downloads
蒋兴树说:"我真的很帅"
蒋兴树说:'我真的很帅'
丁维一
*/
注释（Comment）
1、介绍：用于注解说明解释程序的文字，提高了代码的阅读性；注释是一个程序员必须要具有的良好编程习惯。

2、分类：

单行注释（基本格式：//注释文字）

多行注释（基本格式：/* 注释文字 */）

被注释的文字不会被JVM解释执行；多行注释里不可有多行注释嵌套。

文档注释：注释内容可以被JDK提供的工具javadoc所解析，生成一套以网页文件形式体现的该程序的说明文档

//基本格式：
/**
 * @author 蒋兴树
 * @version 1.0.0
*/

public class JavaComment{
	public static void main(String[] args) {
	}
}

//生成对应的文档注释：javadoc -d 文件夹名 -author -version -JavaComment
标签	描述	示例
@author	标识一个类的作者	@author description
@deprecated	指名一个过期的类或成员	@deprecated description
{@docRoot}	指明当前文档根目录的路径	Directory Path
@exception	标志一个类抛出的异常	@exception exception-name explanation
{@inheritDoc}	从直接父类继承的注释	Inherits a comment from the immediate surperclass.
{@link}	插入一个到另一个主题的链接	{@link name text}
{@linkplain}	插入一个到另一个主题的链接，但是该链接显示纯文本字体	Inserts an in-line link to another topic.
@param	说明一个方法的参数	@param parameter-name explanation
@return	说明返回值类型	@return explanation
@see	指定一个到另一个主题的链接	@see anchor
@serial	说明一个序列化属性	@serial description
@serialData	说明通过writeObject( ) 和 writeExternal( )方法写的数据	@serialData description
@serialField	说明一个ObjectStreamField组件	@serialField name type description
@since	标记当引入一个特定的变化时	@since release
@throws	和 @exception标签一样.	The @throws tag has the same meaning as the @exception tag.
{@value}	显示常量的值，该常量必须是static属性。	Displays the value of a constant, which must be a static field.
@version	指定类的版本	@version info
Java开发规范
1、类、方法的注释，要以javadoc的方式来写。

2、非javadoc的注释，是给代码的维护者看的，着重告诉读者为何这样写，如何修改以及注意什么问题等。

3、使用tab操作实现缩进，相反的使用shift+tab。

4、运算符以及=两边习惯性加一个空格

5、源文件要使用utf-8编码

6、行宽度不要超过80字符

7、代码编写行尾风格、次行风格。

DOS
1、介绍：Disk Operating System-磁盘操作系统

2、基本原理：在命令行输入命令-Dos系统接收命令、解析命令、执行命令-Windows文件系统

3、路径详解

相对路径：从当前目录开始定位，形成的路径。

绝对路径：从根目录开始定位，形成的路径。

举例：从D盘下A文件夹下test1文件夹去访问D盘下B文件夹下test1文件夹下hello.txt文本文档。

相对路径：..\..\B\test1\hello.txt
绝对路径：D:\B\test1\Hello.txt
4、Dos指令

dir：查看当前目录是有什么内容（例：dir D:\B\test1 查看D盘B文件夹下test1文件夹的内容）

cd：切换磁盘，使用 /D 开关，除了改变驱动器的当前目录之外，还可改变当前驱动器。（例：cd /D C: 切换到C盘）

cd ..：切换到上一级

cd \：切换到根目录

tree：查看指定目录下所有的子级目录（tree E: 查看E盘下所有的子级目录）

cls：清屏 （记忆法：苍老师）

exit：退出DOS

md：创建目录

rd：删除目录

copy：拷贝文件（例：D:\B\test1>copy Hello.txt E:\Hello.txt 拷贝D盘B文件夹下Hello.txt文件到E盘）

del：删除文件

echo：输入内容到文件（例：E:>echo hello > Study\Hello.txt 输入hello到Study\Hello.txt文档里）

type：输入空内容到文件

move：剪切

API
1、API（Application Programming Interface），应用程序编程接口，是Java提供的基本编程接口。

2、Java语言提供了大量的基础类，因此Oracle公司也为这些基础类提供了相应的API文档，用于告诉开发者如何使用这些类，以及这些类中包含的方法。

3、Java类的组织形式：

Java 的应用程序编程接口（API）以包的形式来组织，每个包提供了大量的相关类、接口和异常处理类，这些包的集合就是 Java 的类库。

                     包1：接口

                               类（...）：字段..、构造器（构造方法）、成员方法（方法）

                               异常

JDK8、11：包2

                     包...

4、举例说明：ArrayList类有哪些方法

先找软件包，再找类，最后找方法。

1.1.2、变量
变量原理
1、变量是程序的基本组成部分

2、变量的三个基本要素：类型+名称+值

public class Test{
	public static void main(String[] args) {
		int a = 1;//定义了一个变量，类型int整型，名称a，值1
		int b = 2;//定义了一个变量，类型int整型，名称b，值2
		b = 89;//把89赋值给变量b
		System.out.println(a);
		System.out.println(b);
	}
}
3、基本原理：创建一个变量a并赋值，计算机在内存中会分配一个空间，a在内存中的体现就是一个地址，这个地址指向这个内存空间，内存空间里即变量值。（可以发生改变的容器，容器本身不变，变得是容器中的内容）

变量概念
1、变量相当于内存中一个数据存储空间的表示，可以把变量看成是一个房间的门牌号，通过门牌号我们可以找到房间，而通过变量名可以访问到变量。

2、使用变量的基本步骤

int a;
a = 60;
System.out.println(a);

//或者int a = 60;一步到位
变量入门
public class Test3{
	public static void main(String[] args) {
		int age = 16;
		double score = 88.8;
		char gender = '男';
		String name = "jiangxingshu";
		System.out.println("个人基本信息:");
		System.out.println(age);
		System.out.println(score);
		System.out.println(gender);
		System.out.println(name);
	}
}
变量细节
1、变量表示内存中的一个存储区域（不同的变量，类型不同，占用的空间大小不同）。

2、该区域有自己的名称（变量名）和类型（数据类型）。

3、变量必须先声明，后使用。

4、 该区域的数据可以在同一数据类型内不断变化。

5、变量在同一个作用域内不能重名。

6、变量三要素：变量名+数据类型+值

7、命名规则：以字母、下划线、$开头，余下的部分可以是字母、数字、$、下划线。

加号使用
1、当左右两边都是数值型时，则做加法运算。

2、当左右两边有一方为字符串，则做拼接运算。

3、运算顺序从左至右。

public class Test4{
	public static void main(String[] args) {
		System.out.println(100 + 98);
		System.out.println("100" + 98);
		System.out.println(100 + 3 + "hello");
		System.out.println("hello" + 100 + 3);
	}
}

/*
输出结果：
198
10098
103hello
hello1003
*/
数据类型
每一种数据都定义了明确的数据类型，在内存中分配了不同大小的内存空间（字节）。

1、Java数据类型：

基本数据类型：数值型：整数类型：byte[1]、short[2]、int[4]、long[8]

                                           浮点类型：float[4]、double[8]

                           字符型：char[2]，存放单个字符'a'

                           布尔型：boolean[1]，存放true，false

引用数据类型：类(class)

                           接口(interface)

                           数组([])

整型使用
byte[字节]：占用存储空间1字节，范围-2^7~2^7-1

short[短整型]：占用存储空间2字节，范围-2^15~2^15-1

int[整型]：占用存储空间4字节，范围-2^31~2^31-1

long[长整型]：占用存储空间8字节，范围-2^63~2^63-1

整型细节
1、Java各整数类型有固定的范围和字段长度，不受具体操作系统的影响，以保证Java程序的可移植性。

2、Java的整型常量默认为int型，声明long型常量需后加'l'或'L'。

public class IntDetail{
	public static void main(String[] args) {
		int a = 1;
		int b = 1L;
	}
}

/*
编译结果：
IntDetail.java:4: 错误: 不兼容的类型: 从long转换到int可能会有损失
                int b = 1L;
                        ^
1 个错误
*/
3、Java程序中变量常声明为int型，除非不足以表示大数，才使用long。

4、bit：计算机中最小的存储单位，byte：计算机中基本存储单元，1byte=8bit。

浮点数使用
浮点数=符号位+指数位+尾数位

浮点数细节
1、Java浮点类型有固定的范围和字段长度，不受具体操作系统的影响。

2、Java浮点型常量默认为double型，声明float型常量，需后加'f'或'F'。

3、浮点型常量有两种表示形式：

十进制数形式：如：5.12    512.0f    .512（相当于0.512）

科学计数法形式：如：5.12e2（5.12*10^2）    5.12E-2（5.12/10^2）

4、通常情况下，应该使用double型，因为它比float型更精确。

5、浮点数使用陷阱：2.7和8.1/3比较

public class FloatDetail{
	public static void main(String[] args) {
        //细节2
		//float num1 = 1.1;错误，不兼容的类型: 从double转换到float可能会有精度损失
		float num2 = 1.1F;
		double num3 = 1.1;
		double num4 = 1.1f;//低精度可转高精度，高精度不可转低精度

        //细节3
		System.out.println(.123);
		System.out.println(5.12e2);
     
        //细节4
		double num5 = 2.12345678;
		float num6 = 2.12345678F;
		System.out.println(num5);
		System.out.println(num6);

        //细节5
		double num7 = 2.7;
		double num8 = 8.1 / 3;
		System.out.println(num7);
		System.out.println(num8);//结果是一个接近2.7的小数，正确的方法是比较两个数差值的绝对值在某个精度范围内。
		if (num7 == num8) {
			System.out.println("相等");//错误的写法
		}
		if (Math.abs(num7 - num8) < 0.000001) {
			System.out.println(Math.abs(num7 - num8));
			System.out.println("差值非常小，到我规定的范围，认为相等");//正确的写法
		}
	}
}

/*
0.123
512.0
2.12345678
2.1234567
2.7
2.6999999999999997
4.440892098500626E-16
差值非常小，到我规定的范围，认为相等
*/
字符型使用
1、字符类型可以表示单个字符，字符类型是char，char是两个字节（可以存放汉字），多个字符我们用字符串String。

public class Char01{
	public static void main(String[] args) {
		char c1 = 'a';
		char c2 = '\t';
		char c3 = '韩';
		char c4 = 97;
		System.out.println(c1);//Sublime Text中，Ctrl+Shift+D复制光标所在整行，插到下一行。
		System.out.println(c2);//Sublime Text中，Ctrl+Shift+K删除整行。
		System.out.println(c3);
		System.out.println(c4);//当输出c4时，会输出表示97的字符。
	}
}

/*
输出结果：
a

韩
a
*/
字符型细节
1、字符常量是用单引号''括起来的单个字符。（例：char a1 = 'a'、char a1 = '中'、char a1 = '9'）

2、Java中允许使用转义字符'\'来将其后的字符转变为特殊字符型常量。（例：char c3 = '\n'）

3、Java中，char的本质是一个整数，在输出时，是unicode码对应的字符。

public class Char02{
	public static void main(String[] args){
		char c1 = 97;
		char c2 = 'a';

		char c3 = '韩';
        char c4 = 38889;

		System.out.println(c1);
		System.out.println((int)c2);

		System.out.println((int)c3);
		System.out.println(c4);
	}
}

/*
输出结果：
a
97
38889
韩
*/
4、可以直接给char赋一个整数，然后输出时会按照对应的unicode字符输出。

5、char类型是可以进行运算的，相当于一个整数，因为它都有对应的Unicode码。

public class Char03{
	public static void main(String[] args) {
		char a1 = 'a';
		char a2 = 10;
		System.out.println('a' + 10);
	}
}
//运算结果：107
课堂小测试

public class Char03{
	public static void main(String[] args) {
		char a1 = 'a' + 1;
		System.out.println(a1);
		System.out.println((int)a1);//强制转换为int型
	}
}

/*
输出结果：
98
b
*/
字符型本质
1、字符型存储到计算机中，
存储：'a'-->码值97-->二进制1100001-->存储
读取：二进制-->97-->'a'-->显示

2、字符和码值对应关系是通过字符编码表决定的。

3、字符编码表

ASCII编码表，一个字节表示，一个128个字符，（实际上一个字节可以表示256个字符，只用了128个）。Unicode编码表，固定大小的编码，使用两个字节来表示字符，字母和汉字统一都是占用两个字符（这样浪费空间）
utf-8编码表，大小可变的编码，字母使用1个字节，汉字使用3个字节。
gbk，可以表示汉字，而且范围广，字母使用1个字节，汉字使用2个字节。
gb2312，可以表示汉字，gb2312<gbk。
big5码（繁体中文，台湾，香港）

布尔类型
1、布尔类型也叫boolean类型，boolean类型数据只允许取值true和false，无null。

2、boolean类型只占1个字节。

3、boolean类型适用于逻辑运算，一般用于程序流程控制。

public class Boolean01{
	public static void main(String[] args) {
		boolean pass = false;
		if(pass == true){
			System.out.println("通过");
		}else{
			System.out.println("未通过");
		}
	}
}

//输出结果：未通过
4、不可以0或非0的整数替代false和true。

自动类型转换基础
1、自动类型转换：当Java程序在进行赋值或运算时，精度小的类型自动转换为精度大的数据类型。

2、数据类型按精度从小到大排序：

char、int、long、float、double

byte、short、int、long、float、double

public class AutoConvert{
	public static void main(String[] args) {
		int a1 = 'a';
		double a2 = 80;
		System.out.println(a1);
		System.out.println(a2);
	}
}

/*输出结果：
97
80.0
*/
自动类型转换细节
1、有多种类型的数据混合运算时，系统首先自动将所有数据转换成容量最大的那种数据类型，然后再进行运算。

2、当精度大的数据类型赋值给精度小的数据类型时就会报错，反之会自动转换。

3、byte、short、char之间不会相互自动转换。

4、byte、short、char之间可以计算，在计算时首先转换为int类型。

5、boolean类型不参与转换。

6、自动提升原则：表达式中结果的类型自动提升为操作数中最大的类型。

public class AutoConvertDetail{
	public static void main(String[] args) {
		//细节1
		int n1 = 10;

		//float d1 = n1 + 1.1; //错误，1.1默认为double类型，精度大的不可自动转换为精度小的。
        double d1 = n1 + 1.1; //或者：float d1 = n1 + 1.1F。
        System.out.println(d1);


        //细节3
        byte b1 = 10; //当把数据赋值给byte时，会先判断该数是否在byte（-128~127）范围内，如果是就可以。
        //char c1 = b1; //byte不能自动转换为char。
        
        
        //细节4
        byte b2 = 1;
        byte b3 = 2;
        short s1 = 1;
        //short s2 = b2 + s1; //错误，b2 + s1 => int
        //byte b4 = b2 + b3; //错误，b2 + b3 => int
        int n2 = b2 + s1;
        int n3 = b2 + b3;  
        System.out.println(n2);
        System.out.println(n3);


        //细节5
        boolean pass = true;
        //int n4 = pass; //boolean不参与类型的自动转换
        
        
        //细节6
        byte b4 = 1;
        short s2 = 100;
        int n5 = 1;
        double d2 = 1.2;
        double d3 = b4 + s2 + n5 + d2;
        System.out.println(d3);
	}
}

/*
输出结果：
11.1
2
3
103.2
*/
强制类型转换基础
1、自动类型转换的逆过程，将容量大的数据类型转换为容量小的数据类型。使用时要加上强制转换符()，但可能造成精度降低或溢出，格外要注意。

public class ForceConvert{
	public static void main(String[] args) {
		double d1 = 1.2;
		int n1 = (int)d1;

		int n2 = 2000;
		byte b1 = (byte)n2;

		System.out.println(n1); //造成精度缺失
		System.out.println(b1); //造成数据溢出
	}
}

/*
输出结果：
1
-48
*/
强制类型转换细节
1、当精度大的数据类型转换为精度小的数据类型时需要用到强制转换。

2、强转符号只针对最近的操作数有效，往往会使用小括号提升优先级。

3、char类型可以保存int的常量值，但不能保存int的变量值，需要强转。

public class ForceConvertDetail{
	public static void main(String[] args) {
		//细节2
		//int n1 = (int)10 * 3.5 + 6 * 1.5; //错误：从double转换到int可能会有损失
		int n2 = (int)(10 * 3.5 + 6 * 1.5);
		System.out.println(n2);

		//细节3
		char c1 = 100; //正确
		int n3 = 100; //正确
		//char c2 = n3; // 从int转换到char可能会有损失
		char c3 = (char)n3; //正确
		System.out.println(c1); //100对应的字符
	}
}
String和基本数据类型转换
1、基本数据类型转String类型：将基本类型的值+""即可。

2、String类型转基本数据类型：通过基本数据类型的包装类调用parseXX方法即可。

public class StringToBasic{
	public static void main(String[] args) {
		//基本数据类型转换为String
		int n1 = 100;
		float f1 = 1.1F;
        double d1 = 1.2;
        boolean b1 = true;

        String s1 = n1 + "";
        String s2 = f1 + "";
        String s3 = d1 + "";
        String s4 = b1 + "";

        System.out.println(s1 + " " + s2 + " " + s3 + " " + s4);



        //String转换为基本数据类型
        String s5 = "123";

        //使用 基本数据类型 对应的 包装类 的 相应方法 得到 基本数据类型。
        byte t1 = Byte.parseByte(s5);
        short h1 = Short.parseShort(s5);
        int n2 = Integer.parseInt(s5);
        long l1 = Long.parseLong(s5);
        float f2 = Float.parseFloat(s5);
        double d2 = Double.parseDouble(s5);
        boolean b2 = Boolean.parseBoolean("true");

        System.out.println("================");
        System.out.println(t1);       
        System.out.println(h1);       
        System.out.println(n2);       
        System.out.println(l1);       
        System.out.println(f2);       
        System.out.println(d2);       
        System.out.println(b2); 



        //字符串转换成char
        //s5.CharAt(0) 得到 s5 字符串的第一个字符。
        System.out.println("================");
        System.out.println(s5.charAt(0));      
	}
}

/*
输出结果：
100 1.1 1.2 true
================
123
123
123
123
123.0
123.0
true
================
1
*/
String转基本数据类型细节
1、在将String类型转换成基本数据类型时，要确保String类型能够转成有效的数据（例：我们可以把"123"转成一个整数，但不能把"hello"转成一个整数）。

2、如果格式不正确会抛出异常，程序就会终止。

public class StringToBasicDetail{
	public static void main(String[] args) {
		//String s1 = "hello";
		String s1 = "123";
		int n1 = Integer.parseInt(s1);
		System.out.println(n1);
	}
}

//输出结果：123
本章作业
public class HomeWork01{
	public static void main(String[] args) {
		int n1 = 13; //创建一个变量n1并赋值，计算机在内存中会分配一个空间，n1在内存中的体现就是一个地址，这个地址指向这个内存空间，
		int n2 = 17;
		int n3 = n1 + n2;
		System.out.println("n3=" + n3);

		int n4 = 38;
		int n5 = n4 - n3;
		System.out.println("n5=" + n5);

		
        //使用char类型，分别保存\n \t \r \\ 1 2 3等字符并打印输出。
		char c1 = '\n'; //换行
		char c2 = '\t'; //制表位
		char c3 = '\r'; //回车
		char c4 = '\\'; //\
		char c5 = '1'; //1
		char c6 = '2'; //2
		char c7 = '3'; //3
		System.out.println(c1);
		System.out.println(c2);
		System.out.println(c3);
		System.out.println(c4);
		System.out.println(c5);
		System.out.println(c6);
		System.out.println(c7);


        //保存两本书名，用+号拼接，保存两个性别，用+号拼接。
		String t1 = "《钢铁是怎样炼成的》";
		String t2 = "《草房子》";
		char c8 = '男';
		char c9 = '女';
		float f1 = 20.5F;
		double d1 = 35.50;
		System.out.println(t1 + t2); 			
		System.out.println(c8 + c9); //得到的是 男字符码值 和 女字符码值 相加。	
		System.out.println(f1 + d1);


        /*
        1、用变量名将姓名、年龄、分数、性别、兴趣存储。
        2、使用+。
        3、添加转义字符，使用一条语句输出。
        */
		String name = "蒋兴树";
		int age = 21;
		double score = 100.0;
		char gender = '男';
		String hobby = "画画";
		System.out.println("姓名\t年龄\t成绩\t性别\t爱好\n" + name + "\t" +
		age + "\t" + score + "\t" + gender + "\t" + hobby);
		//输出内容时加""表示是一个字符串，变量名不加""，"\t"：将\t变成字符串拼接。
	}
}

/*
输出结果：



\
1
2
3
《钢铁是怎样炼成的》《草房子》
52906
56.0
姓名    年龄    成绩    性别    爱好
蒋兴树  21      100.0   男      画画
*/
1.1.3、运算符
运算符介绍
运算符是一种特殊的符号，用以表示数据的运算、赋值和比较等。

算术运算符
1、正号：+

2、负号：-

3、加减乘除+、-、*、/

4、取余：%

5、自增自减：++、--
作为独立语句使用时前++、后++都等价于i=i+1
作为表达式使用时前++先自增再赋值、后++先赋值再自增

6、字符串相加：+

public class ArithmeticOperator{
	public static void main(String[] args) {
		//除法
		System.out.println(10 / 4); //从数学的角度是2.5，java中是2
		System.out.println(10.0 / 4); //java中是2.5
		int n1 = 10 / 4; //2
		double d1 = 10 / 4; //2.0
		System.out.println(n1);
		System.out.println(d1);


		//取余，也叫取模
		//在java中，%的本质看一个公式 a % b = a - a / b * b
		System.out.println(10 % 3); //1
		System.out.println(-10 % 3); //-1
		System.out.println(10 % -3); //1,10 % -3 = 10 - 10 / -3 * -3 = 10 - 9 = 1
		System.out.println(-10 % -3); //-1,-10 % -3 = -10 - -10 / -3 * -3 = -1


		//自增
		int i = 1;
		i++; //等价于 i = i + 1
		++i; //等价于 i = i + 1
		System.out.println(i);

		/*作为表达式使用
		作为表达式使用
		前++：++i先自增后赋值
		后++：i++先赋值后自增
		*/
		int j = 1;
		int k = ++j; //int j = j + 1、k = j
		int m = j++; //此时j已经为2，int m = j、j = j + 1
		System.out.println(j);
		System.out.println(k);
		System.out.println(m);
	}
}
练习

public class Test6{
	public static void main(String[] args){
		int i = 1;
		i = i++;
		System.out.println(i);
		int a = 1;
		a = ++a;
		System.out.println(a);


		int i1 = 10;
		int i2 = 20;
		int m = i1++;
		System.out.println(m); //10
		System.out.println(i1); //11
		m = --i2;
		System.out.println(m); //19
		System.out.println(i2); //19


		//456789天合计××星期××天
		int n1 = 456789;
		int n2 = 456789 / 7;
		int n3 = 456789 % 7;
		System.out.println(n2 + "星期" + n3 + "天");
		
		//定义一个华氏温度并转换为摄氏度
		double d1 = 234.5;
		double d2 = (double)5 / 9 * (d1 - 100);
		System.out.println(d2);
	}
}
关系运算符
1、相等于：==

2、不等于：!=

3、小于：<

4、大于：>

5、小于等于：<=

6、大于等于：>=

public class RelationalOperator{
	public static void main(String[] args) {
		int a = 9;
		int b = 8;
		System.out.println(a == b);
		System.out.println(a != b);
		System.out.println(a <= b);
		System.out.println(a >= b);
		System.out.println(a < b);
		System.out.println(a > b);
		boolean flag = a > b;
		System.out.println(flag);
	}
}

/*
输出结果为：
false
true
false
true
false
true
true
*/
关系运算符细节
1、关系运算符的结果都是boolean型，结果要么为true要么为false。

2、关系运算符组成的表达式，我们称为关系表达式。

3、比较运算符"=="不能误写为"="。

逻辑运算符
1、用于连接多个条件，最终结果也是boolean值。

2、

a&b：逻辑与，当a和b同时为true，则结果为true，否则为false。
a&&b：短路与，当a和b同时为true，则结果为true，否则为false。
对于逻辑与，如果第一个条件为false，后面的条件仍会判断。
对于短路与，如果第一个条件为false，后面的条件不会判断。

public class LogicOperator{
	public static void main(String[] args) {
		//短路与&& 和 逻辑与& 案例
		int age = 50;
		if (age > 20 && age < 100) {
			System.out.println("ok");
		}

		if (age > 20 & age < 100) {
			System.out.println("ok!");
		}

		//区别
		//对于短路与，如果第一个条件为false，后面的条件不会判断
		//对于逻辑与，如果第一个条件为false，后面的条件仍会判断
		int a = 4;
		int b = 9;
		if (a < 1 && ++b < 50) {
			System.out.println("ok!!");
		}
		System.out.println("a=" + a + " " + "b=" + b);

		if (a < 1 & ++b < 50) {
			System.out.println("ok!!");
		}
		System.out.println("a=" + a + " " + "b=" + b);
 	}
}
a|b：逻辑或，当a和b有一个为true，则结果为true，否则为false。
a||b：短路或，当a和b有一个为true，则结果为true，否则为false。
对于短路或，如果第一个条件为true，后面的条件不会判断，效率更高。
对于逻辑或，如果第一个条件为true，后面的条件仍会判断。

public class LogicOperator02{
	public static void main(String[] args) {
		//短路或|| 和 逻辑或| 案例
		int age = 50;
		if (age > 20 || age < 30) {
			System.out.println("ok");
		}

		if (age > 20 | age < 30) {
			System.out.println("ok!");
		}

		//区别
		//对于短路或，如果第一个条件为true，后面的条件不会判断，效率更高。
		//对于逻辑或，如果第一个条件为true，后面的条件仍会判断
		int a = 4;
		int b = 9;
		if (a > 1 || ++b < 50) {
			System.out.println("ok!!");
		}
		System.out.println("a=" + a + " " + "b=" + b);

		if (a > 1 | ++b < 50) {
			System.out.println("ok!!");
		}
		System.out.println("a=" + a + " " + "b=" + b);
 	}
}
!a：取反，当a为true，则结果为false。当a为false，则结果为true。
a^b：逻辑异或，当a和b不同时，则结果为true，否则为false。

public class InverseOperator{
	public static void main(String[] args) {
		//！：取反
		System.out.println(20 < 60);
		System.out.println(!(20 < 60));

		//^：逻辑异或，当a和b不同时结果为true，否则为false。
		boolean b = (20 < 50) ^ (20 > 10);
		boolean b1 = (10 > 20) ^ (20 < 50);
		System.out.println(b);
		System.out.println(b1);
	}
}
练习

public class Test7{
	public static void main(String[] args) {
		boolean x = true;
		boolean y = false;
		short z = 46;
		//z++ == 46为true，将trur赋值给y，if语句结束后z为48。
		if ((z++ == 46) && (y = true)) {
			z++;
		}
		//将false赋值给x，++z == 49为true，if语句结束后z为50。
		if ((x = false) || (++z == 49)) {
			z++;
		}
		System.out.println("z = " + z);
	}
}
赋值运算符
赋值运算符就是将某个运算后的值赋给指定变量。

public class AssignOperator{
	public static void main(String[] args) {
		int n1 = 10;
		n1 += 4; //n1 = n1 + 4
		System.out.println(n1);

		n1 /= 3; //n1 = n1 / 3
		System.out.println(n1);
	}
}
1、赋值运算符的左边只能是变量，右边可以是变量、表达式、常量值（int a = 20、int a = 20 * 30、int num1 = a）。

2、复合赋值运算符等价于下面效果（a += 3等价于a = a + 3）。

3、复合赋值运算符会进行类型转换。

public class AssignOperator{
	public static void main(String[] args) {
		byte b = 3;
		b += 2; //等价于 b = (byte)(b + 2)
		System.out.println(b);
	}
}
三元运算符基础
基本语法：条件表达式 ? 表达式1 : 表达式2

1、如果条件表达式为true，运算后结果是表达式1；如果条件表达式为false，运算后结果是表达式2。

public class TernaryOperator{
	public static void main(String[] args) {
		int a = 10;
		int b = 99;
		int result = a > b ? a++ : b--; //a > b为false，执行b--，先返回b的值再-1，result结果为99。
		System.out.println("result=" + result);

		//经过上方b--后b为98
		int result1 = a < b ? a++ : b--;
		System.out.println("result1=" + result1);
		System.out.println("a=" + a);
		System.out.println("b=" + b);
	}
}

/*
输出结果为：
result=99
result1=10
a=11
b=98
*/
三元运算符细节
1、表达式1和表达式2要为可以赋给接收变量的类型（或可以自动转换）。

2、三元运算符可以转换成if--else语句。

public class TernaryOperatorDetail{
	public static void main(String[] args) {
		int a = 3;
		int b = 8;
		int c = a > b ? a : b; //int c = a > b ? 1.1 : 2.2 错误，不符合自动类型转换。
		double d = a > b ? a : b + 3;
		System.out.println(c);
		System.out.println(d); //可以，满足自动类型转换。
	}
}
练习

//实现3个数的最大值
public class TernaryOperatorExercise{
	public static void main(String[] args) {
		int a = 100;
		int b = 555;
		int c = 1500;
		int result = a > b ? a : b;
		int result1 = result > c ? result : c;
		System.out.println(result1);
	}
}

//结果为：1500
运算符优先级
1、运算符有优先级，即表达式运算中的运算顺序。

2、只有单目运算符、赋值运算符是从右向左运算的。

标识符的命名规则和规范
概念

1、Java对各种变量、方法和类命名时使用的字符序列称为标识符。

2、凡是自己取名的地方都叫标识符。

规则

1、由字母大小写、数字、$、下划线组成。

2、数字不可开头。

3、不可以使用关键字、保留字，但可以包含关键字、保留字。

4、Java中严格区分大小写，长度无限制。

5、标识符不能包含空格。

规范

1、包名：多单词组成时所有字母都小写，aaa.bbb.ccc。

2、类名、接口名：多单词组成时，所有字母的首字母大写，AaaBbbCcc。（大驼峰）

3、变量名、方法名：多单词组成时，第一个单词字母小写，第二个单词开始每个单词首字母大写，xxxYyyZzz。（小驼峰）

4、常量名：所有字母都大写，多单词时每个单词用下划线连接，XXX_YYY_ZZZ。

键盘输入语句Scanner
介绍：在编程中，需要接收用户输入的数据，就可以用键盘输入语句来获取。需要一个扫描器（对象），就是Scanner。

步骤：

1、导入该类所在的包。

2、创建该类的对象。

3、调用里面的功能。

//表示将java.util下的Scanner类导入。
//Scanner类表示简单文本扫描器
import java.util.Scanner;

public class Input{
	public static void main(String[] args) {
		//演示接收用户的输入
		//引入scanner类所在的包
		//创建Scanner对象实例,new创建一个对象,即创建一支笔。
		Scanner scanner = new Scanner(System.in);

		System.out.println("请输入名字");
		//接收用户的输入的字符串。
		//当程序执行到next方法时会等待用户输入。不输入会一直等待。
		String name = scanner.next();

		System.out.println("请输入年龄");
		//接收用户输入int。
		int age = scanner.nextInt();

		System.out.println("请输入薪水");
		//接收用户输入double。
		double sal = scanner.nextDouble();

		System.out.println(name);
		System.out.println(age);
		System.out.println(sal);
	}
}
二进制、八进制、十进制、十六进制
1、二进制：用0、1表示一个数，满2进1，以0B或0b开头

2、十进制：用0-9表示一个数，满10进1。

3、八进制：用0-7表示一个数，满8进1。

4、十六进制：用0-9以及10-15（A-F）表示一个数，以0x或0X开头，此处A-F不区分大小写。

二进制、八进制、十六进制转十进制
1、二进制转十进制：从最低位（右边）开始，将每个位上的数提取出来，乘以2的（位数-1）次方，再求和。

ob1011 = 1 * 2的0次方 + 1 * 2的1次方 + 1 * 2的3次方 = 1 + 2 + 8 = 11

2、八进制转十进制：从最低位（右边）开始，将每个位上的数提取出来，乘以8的（位数-1）次方，再求和。

0234 = 4 * 8的0次方 + 3 * 8的1次方 + 2 * 8的2次方 = 4 + 24 + 128 = 156

3、十六进制转十进制：从最低位（右边）开始，将每个位上的数提取出来，乘以16的（位数-1）次方，再求和。

0x23A = 10 * 16的0次方 + 3 * 16的1次方 + 2 * 16的2次方 = 10 + 48 + 512 = 570

十进制转二进制、八进制、十六进制
1、十进制转二进制：将该数不断除以2，直到商为0为止，然后将每步得到的余数倒过来，即相应的二进制。

34 = 0b00100010

2、十进制转八进制：将该数不断除以8，直到商为0为止，然后将每步得到的余数倒过来，即相应的八进制。

131 = 0203

3、十进制转十六进制：将该数不断除以16，直到商为0为止，然后将每步得到的余数倒过来，即相应的十六进制。

237 = 0xED

二进制转八进制、十六进制
1、二进制转八进制：从低位开始，将二进制每3位一组，转成对应的八进制即可。

0b11010101 = 0325

2、二进制转十六进制：从低位开始，将二进制每4位一组，转成对应的八进制即可。

0b11010101 = 0xD5

八进制转二进制、十六进制转二进制
1、八进制转二进制：将八进制每1位转成对应的一个3位数二进制数即可。

0237 = ob10011111

2、十六进制转二进制：将十六进制每1位转成对应的一个4位数二进制数即可。

0x23B = 0b001000111011

原码、反码、补码
1、二进制的最高位是符号位，0表示正数，1表示负数。

2、正数的原码、反码、补码都一样。

3、负数的反码：原码符号位不变，其他位取反。负数的补码：反码 + 1。

4、0的反码、补码为0。

5、Java没有无符号数，即Java中的数都是有符号的。

6、计算机运算的时候都是以补码的方式运算的。

7、查看运算结果时，要查看他的原码。

位运算符
1、按位与&：两位全为1，结果为1，否则为0。

2、按位或|：两位有一个1，结果为1，否则为0。

3、按位异或^：两位一个为1，一个为0，结果为1，否则为0。

4、按位取反~

public class BitOperator{
	public static void main(String[] args) {

		//计算机运算都是以补码的方式运算
		//先得到2的补码
		//正数的原码、反码、补码一样，三码合一。
		//2的原码00000010 补码00000010
		//3的原码00000011 补码00000011
		//按位与后补码00000010 原码00000010，即2
		System.out.println(2&3);


		//-2原码10000010 反码11111101 补码11111110
		//按位取反后补码00000001 原码00000001，即1
		System.out.println(~-2);


		//2的原码00000010 补码00000010
		//按位取反后补码11111101，反码 = 补码 - 1 = 11111100，原码10000011，即-3
		System.out.println(~2);
	}
}

/*
输出结果：
2
1
-3
*/
5、>>:算术右移，低位溢出，符号位不变，并用符号位补溢出的高位。

6、<<：算术左移，符号位不变，低位补0。

7、>>>：逻辑右移，也叫无符号右移，运算规则：低位溢出，高位补0。

public class BitOperator02{
	public static void main(String[] args) {
		
		//算术右移，1的原码00000001 右移后00000000 本质1/2/2
		int a = 1 >> 2;


		//算术左移，1的原码00000001 左移后00000100 本质1*2*2
		int c = 1 << 2;

		System.out.println(a);
		System.out.println(c);
	}
}

/*
输出结果：
0
4
*/
Test

public class Test8{
	public static void main(String[] args) {
		System.out.println(10 / 3); //3
		System.out.println(10 / 5); //2
		System.out.println(10 % 2); //0
		System.out.println(-10.5 % 3); //-1.5,公式：a - (int)a / b * b，有小数时得到的结果是近似值。

		int i = 66;
		System.out.println(++i + i); //134

		String str = "18.8";
		double d1 = Double.parseDouble(str); //将String转换成double类型的语句。

		char = 'a';
		String str2 = c1 + ""; //将char类型转换成String类型的语句。
	}
}
1.1.4、控制结构
顺序控制
程序从上到下依次执行，中间没有任何判断和跳转。

public class control{
	public static void main(String[] args) {
		
		//顺序控制
		int num1 = 12;
		int num2 = num1 + 2;

		//错误形式，先申明再引用
		// int num2 = num1 + 2;
		// int num1 = 12;
	}
}
分支控制
让程序有选择地执行，分支控制有三种：单分支、双分支、多分支。

单分支：if(条件表达式){执行代码块}

当条件表达式为true时就执行{}内的代码，否则为false。

import java.util.Scanner;

public class BranchControl{
	public static void main(String[] args) {
		
		Scanner Scanner = new Scanner(System.in);
		System.out.println("请输入年龄");
		int age = Scanner.nextInt();

		if (age > 18) {
			System.out.println("送进监狱");
		}
		System.out.println("程序继续执行");

	}
}
双分支：if(条件表达式){执行代码块1}else{执行代码块2}

当条件表达式成立则执行代码块1，否则执行代码块2。

import java.util.Scanner;

public class BranchControl01{
	public static void main(String[] args) {
		
		Scanner Scanner = new Scanner(System.in);
		System.out.println("请输入年龄");
		int age = Scanner.nextInt();

		if (age > 18) {
			System.out.println("送进监狱");
		}else{
			System.out.println("侥幸逃过");
		}
	}
}
多分支：if(条件表达式1){执行代码块1}else if(条件表达式2){执行代码块2}else{执行代码块n}

当条件表达式1成立则执行代码块1

当条件表达式1不成立才判断条件表达式2是否成立

当条件表达式2成立则执行代码块2

如果所有的表达式都不成立则执行else代码块

特别说明：多分支可以没有else，如果所有的条件表达式都不成立，则没有执行入口。如果有else，所有的条件表达式都不成立，就默认执行else代码块。

import java.util.Scanner;

public class BranchControl02{
	public static void main(String[] args) {
		
		System.out.println("请输入芝麻分(1-100)");
		Scanner Scanner = new Scanner(System.in);
		int score = Scanner.nextInt();

		if (score == 100) {
			System.out.println("信用极好");
		}else if (score > 80 && score <= 99) {
			System.out.println("信用优秀");
		}else if (score >= 60 && score <= 80) {
			System.out.println("信用一般");
		}else{
			System.out.println("信用不及格");
		}
	}
}
Test
public class BranchControl03{
	public static void main(String[] args) {
		
		boolean b = true;
		if (b == false) {
			System.out.println("a");
		}else if (b) { // b = true，输出b。
			System.out.println("b");
		}else if (!b) {
			System.out.println("c");
		}else{
			System.out.println("d");
		}


		if (b = false) { //将false赋值给b。
			System.out.println("a");
		}else if (b) {
			System.out.println("b");
		}else if (!b) { //!b为true，输出c。
			System.out.println("c");
		}else{
			System.out.println("d");
		}
	}
}
循环控制
break
continue
return
1.1.5、数组、排序和查找
数组
排序
查找
Test
package net.wanhe.j2se.day05;

import java.util.Scanner;

public class Test01 {

    public static void main(String[] args) {
        run();
    }

    public static void run(){
        String[] stus = new String[20];
        String[] teas = new String[20];

        boolean falg = true;
        while(falg){

            //根据用户输入的选项执行对应的功能
            int chooise = PrintMenu();

            switch(chooise){
                case 1:
                    boolean StusFlag = true;
                    while(StusFlag){

                        //展示学生管理的菜单
                        int chooise1 = PrintStusMenu();

                        switch (chooise1){
                            case 1:
                                AllStus(stus);
                                break;
                            case 2:
                                AddStus(stus);
                                break;
                            case 3:
                                DelStus(stus);
                                break;
                            case 4:
                                StusFlag = false;
                                break;
                        }
                    }
                    //最后要加break，防止穿透到case 2。
                    break;
                case 2:
                    boolean TeasFlag = true;
                    while (TeasFlag){

                        //展示教师管理的菜单
                        int chooise2 = PrintTeasMenu();

                        switch(chooise2){
                            case 1:
                                AllTeas(teas);
                                break;
                            case 2:
                                AddTeas(teas);
                                break;
                            case 3:
                                DelTeas(teas);
                                break;
                            case 4:
                                TeasFlag = false;
                                break;
                        }
                    }
                    //最后要加break，防止穿透到case 3。
                    break;
                case 3:
                    falg = false;
                    break;
            }
        }
    }

    //输出首页菜单，返回用户输入的选项
    public static int PrintMenu(){
        System.out.println("--教育管理系统--");
        System.out.println("1、学生管理");
        System.out.println("2、教师管理");
        System.out.println("3、退出系统");
        System.out.println("请选择：");

        Scanner sc = new Scanner(System.in);
        int chooise = sc.nextInt();
        return chooise;
    }

    //输出学生菜单，返回用户输入的选项。
    public static int PrintStusMenu(){
        System.out.println("--学生管理系统--");
        System.out.println("1、学生信息");
        System.out.println("2、添加学生");
        System.out.println("3、删除学生");
        System.out.println("4、返回上级");
        System.out.println("请选择：");

        Scanner sc = new Scanner(System.in);
        int chooise1 = sc.nextInt();
        return chooise1;
    }

    //输出教师菜单，返回用户输入的选项。
    public static int PrintTeasMenu(){
        System.out.println("--教师管理系统--");
        System.out.println("1、教师信息");
        System.out.println("2、添加教师");
        System.out.println("3、删除教师");
        System.out.println("4、返回上级");
        System.out.println("请选择：");

        Scanner sc = new Scanner(System.in);
        int chooise2 = sc.nextInt();
        return chooise2;
    }

    //遍历数组，查看学生信息，将学生的信息在控制台输出打印
    public static void AllStus(String[] stus){
        for (int i =0;i < stus.length;i++){
            if (stus[i] != null){
                System.out.println((i + 1) + ":" + stus[i]);
            }
        }
    }

    //添加学生
    public static void AddStus(String[] stus){
        Scanner sc =new Scanner(System.in);
        System.out.println("输入学生学号");
        int num = sc.nextInt();
        System.out.println("输入学生姓名");
        String name = sc .next();

        if (num < 0 || num > 19){
            System.out.println("学号无效");
        }else if(stus[num] != null){
            System.out.println("学号无效");
        }else{
            System.out.println("添加成功");
            stus[num] = name;
        }
    }

    //删除学生
    public static void DelStus(String[] stus){
        Scanner sc =new Scanner(System.in);
        System.out.println("输入学生学号");
        int num = sc.nextInt();
        System.out.println("输入学生姓名");
        String name = sc .next();

        if (num < 0 || num > 19){
            System.out.println("学号无效");
        }else{
            System.out.println("删除成功");
            stus[num] = null;
        }
    }

    //遍历数组，查看教师信息，将教师的信息在控制台输出打印
    public static void AllTeas(String[] teas){
        for (int i =0;i < teas.length;i++){
            if (teas[i] != null){
                System.out.println((i + 1) + ":" + teas[i]);
            }
        }
    }

    //添加教师
    public static void AddTeas(String[] teas){
        Scanner sc =new Scanner(System.in);
        System.out.println("输入教师编号");
        int num = sc.nextInt();
        System.out.println("输入教师姓名");
        String name = sc .next();

        if (num < 0 || num > 19){
            System.out.println("编号无效");
        }else if(teas[num] != null){
            System.out.println("编号无效");
        }else{
            System.out.println("添加成功");
            teas[num] = name;
        }
    }

    //删除教师
    public static void DelTeas(String[] teas){
        Scanner sc =new Scanner(System.in);
        System.out.println("输入教师编号");
        int num = sc.nextInt();
        System.out.println("输入教师姓名");
        String name = sc .next();

        if (num < 0 || num > 19){
            System.out.println("编号无效");
        }else{
            System.out.println("删除成功");
            teas[num] = null;
        }
    }
}
1.1.6、面向对象编程（基础）
类与对象
类与对象引出：使用现有技术解决不利于数据的管理，效率低下。所以引出类与对象。

import java.util.Scanner;

public class Object{
	public static void main(String[] args) {
		//单独定义变量，不利于数据的管理。
		String cat_name = "小白";
		int cat_age = 3;
		char cat_color = "白";

		String cat1_name = "小花";
		int cat1_age = 5;
		char cat1_color = "黄";


		//数组，数据类型单一
		//只能通过下标获取信息，造成变量名字和内容对应关系不明确。
		//不能体现猫的行为
		String[] cat1 = {"小白","3","白"};
		String[] cat2 = {"小花","5","黄"};
	}
}
类和对象的联系：

1、类是抽象的，对象是具体的。

2、类是对象的模板，对象是类的实例。

3、类即数据类型。

属性/成员变量
1、从概念或叫法上：属性=成员变量

2、属性是类的一个组成部分，一般是基本数据类型，也可以是引用数据类型（对象、数组）。

属性注意事项和细节
1、属性定义语法：访问修饰符 属性数据类型 属性名。

2、属性的数据类型可以为基本或引用数据类型。

3、属性如果不赋值，有默认值，规则和数组一致。

public class PropertiesDetail{

	public static void main(String[] args) {
		//p1是对象名，new Person()创建的对象空间才是真正的对象。
		Person p1 = new Person();

		//对象的属性默认值遵守数组规则。
		System.out.println("age=" + p1.age + " " + "name=" + p1.name + 
			" " + "sal=" + p1.sal);
	}
}

class Person{
	int age;
	String name;
	double sal;
}
创建对象、访问属性
//先声明再创建
Cat cat;
cat = new Cat();

//直接创建
Cat cat = new Cat();
//对象名.属性名
cat.name;
cat.age;
cat color;
类和对象的内存分配机制
public class Object02{
	public static void main(String[] args) {
		Person p1 = new Person();
		p1.age = 10;
		p1.name = "小明";
		Person p2 = p1; //p1将地址赋值给p2。
		System.out.println(p2.age);
	}
}

class Person{
	String name;
	int age;
}
<img src="E:\Study\自学课程资料\Java\assets\类和对象的内存分配机制.PNG" alt="类和对象的内存分配机制"  />

成员方法
在某些情况下，我们需要定义成员方法。比如人类除了属性外，还有一些行为，这时就需要成员方法。

public class Method{
	public static void main(String[] args) {
		//1、方法写好需要调用，否则不会输出
		//先创建对象，再调用方法
		Person p1 = new Person();
		p1.speak();
	}	
}

class Person{

	String name;
	int age;


	//public 方法公开
	//void 无返回值
	//speak 方法名
	//() 形参列表
	//{} 方法体
	public void speak(){
		System.out.println("蒋兴树是帅哥");
	}
}

//输出结果：蒋兴树是帅哥
public class Method{
	public static void main(String[] args) {
		Person Person = new Person();
		//调用product方法并输入两个数。
		Person.product(4,5);
	}	
}

class Person{
	//定义一个方法，可以计算a的b次方
    //(int a,int b)形参列表，两个形参，可以接收用户输入的两个数。
	public void product(int a,int b){
		int rest = 1;
		for (int c = 0;c < b;c++) {
			rest = a * rest;
		}
		System.out.println(rest);
	}
}

//输出结果：1024
成员方法的定义
定义语法：public 返回数据类型 方法名(形参列表){方法体}

1、形参列表：成员方法的输入。

2、数据类型：成员方法输出的数据类型，void表示没有返回值。

3、方法体：实现功能的代码块。

4、return可有可无。

内存方法的调用机制
![image-20220907194115777](E:\Study\自学课程资料\Java\assets\jvm内存方法的调用机制.png)

jvm内存方法的调用机制注意事项：

1、当程序执行到方法时，会在栈中开辟一个独立的空间。

2、当方法执行结束时，或执行到return语句时会返回到调用方法的地方。

3、返回后继续执行方法后面的代码。

4、当main方法执行完毕，整个程序退出。

为什么需要成员方法
public class Method01{
	public static void main(String[] args) {
		int[][] map = {{0,0,1},{1,1,1},{1,1,3}};

		//传统遍历数组的方法
		for (int i =0;i < map.length;i++) {
			for (int j = 0;j < map[i].length;j++) {
				System.out.print(map[i][j] + "");	
			}
			System.out.println();
		}

        
        
		//创建一个MyTools对象，然后调用方法。提高代码的复用性。
		MyTools MyTools = new MyTools();	
		MyTools.printArr(map);
		MyTools.printArr(map);
		MyTools.printArr(map);
	}
}

class MyTools {
	//接收一个二维数组
	public void printArr(int[][] map){
		System.out.println("================");
		for (int i =0;i < map.length;i++) {
			for (int j = 0;j < map[i].length;j++) {
				System.out.print(map[i][j] + "");	
			}
			System.out.println();
		}
	}
}
1、提高代码复用性

2、可以将实现的细节封装起来，供其他用户使用。

成员方法的注意细节
修饰符注意细节：

1、访问修饰符，控制方法使用范围。（public、protected、默认、private）

返回类型注意细节：

1、一个方法最多有一个返回值。（返回数组可返回多个值）

public class MethodDetail{

	public static void main(String[] args) {
		data data = new data();
		int[] a = data.add_subtract(4,3);
		System.out.println(a[0]);
		System.out.println(a[1]);
	}
}

class data {

	public int[] add_subtract(int a,int b) {
		int[] array = new int[2];
		array[0] = a + b;
		array[1] = a - b;
		return array;
	}
}
2、返回类型可以为任意类型，包含基本数据类型和引用数据类型（数组、对象）。

3、如果方法要求有返回类型，则方法体最后的执行语句必须为return，而且返回值类型必须和return的值类型一致或兼容。

4、如果方法是void，则方法体中可以没有return语句，或者只有return。

5、方法名遵循驼峰命名法，见名知义。

形参列表注意细节：

1、一个方法可以有0个参数，也可以有多个参数，中间逗号隔开。

2、参数类型可以为任意类型，包含基本数据类型、引用数据类型。

3、调用带参数的方法时，一定要对应着参数列表传入相同的数据类型或兼容类型。

4、方法定义时的参数称为形式参数（形参），方法调用时的参数称为实际参数（实参）。形参和实参的类型要一致或兼容，个数、顺序必须一致。

方法体注意细节：

1、里面写完成功能的具体语法，可以为输入、输出、变量、运算、分支、循环、方法调用。

2、里面不可再定义方法。

细节又细节

1、同一个类中的方法可直接调用。

public class MethodDetail01{
	public static void main(String[] args) {
		A a = new A();
		a.say();
	}
}

class A{

	public void speak() {
		System.out.println("调用speak方法");
	}

    //直接调用speak方法
	public void say() {
		speak();
		System.out.println("继续执行");
	}
}
2、跨类中的方法A调用方法B，需要通过对象名调用。

public class MethodDetail02{

	public static void main(String[] args) {
		
		B b = new B();
		b.say();
	}
}

class A{
	public void speak() {
		System.out.println("调用speak方法");
	}
}

class B{
	public void say() {

		//跨类调用对象，需要通过对象名调用
		//创建A对象，再调用方法。
		A a = new A();
		a.speak();
		System.out.println("执行say方法");
	}
}
成员方法传参机制
1、基本数据类型的传参机制

public class MethodParameter{

	public static void main(String[] args) {
		int a = 10;
		int b = 20;

		//
		A num = new A();
		num.swap(a,b);

		System.out.println("main方法 a=" + a + " " + "b=" + b);
	}
}

class A{

	public void swap(int a,int b) {
		System.out.println("a和b交换前的值：\n" + "a=" + a + " " + "b=" + b + "\n");
		int temp = a;
		a = b;
		b = temp;
		System.out.println("a和b交换后的值：\n" + "a=" + a + " " + "b=" + b + "\n");
	} 
}

/*
输出结果：
a和b交换前的值：
a=10 b=20

a和b交换后的值：
a=20 b=10

main方法 a=10 b=20
*/
基本数据类型，传递的是值拷贝，形参的任何改变不影响实参。

2、引用数据类型的传参机制

public class MethodParameter01{

	public static void main(String[] args) {
		reference_transfer reference_transfer = new reference_transfer();
		int[] array = {1,2,3};
		reference_transfer.Test(array); 

		System.out.println("main的array数组：");
		for (int i = 0;i < array.length;i++) {
			System.out.println(array[i]);
		}
		System.out.println();

	}
}

//引用传参
class reference_transfer{

	public void Test(int[] array) {
		//修改数组中下表为0的数
		array[0] = 200;

		//遍历数组
		System.out.println("Test的array数组：");
		for (int i = 0;i < array.length;i++) {
			System.out.println(array[i]);
		}
		System.out.println();

	}
}

/*
输出结果：
Test的array数组：
200
2
3

main的array数组：
200
2
3
*/
![](E:\Study\自学课程资料\Java\assets\引用数据类型的传参机制.png)

引用类型传递的是地址，传递的也是值，但这个值是地址，可以通过形参影响实参。

克隆对象
public class MethodExercise01{

	public static void main(String[] args) {
		Person p = new Person();
		p.name = "蒋兴树";
		p.age = 21;

		MyTools mytools = new MyTools();
		Person p2 = mytools.copyPerson(p);

		//到此 p 和 p2 是Person对象，但是是两个独立的对象。
		
		System.out.println("p.name=" + p.name + " " + "p.age=" + p.age);
		System.out.println("p2.name=" + p2.name + " " + "p2.age=" + p2.age);
	}
}

class Person{
	String name;
	int age;
}

class MyTools{

	/* 编写一个方法copyPerson，可以复制一个Person对象，返回复制的对象。
	 * 访问修饰符 public
	 * 返回类型 Person
	 * 方法名 copyPerson
	 * 方法体
	*/
	public Person copyPerson(Person p) {
		Person p2 = new Person();
		//将传入的对象的值赋值给p2
		p2.name = p.name;
		p2.age = p.age;

		return p2;
	}
}
方法递归调用
打印问题

public class Recursion01{
	public static void main(String[] args) {
		RecursionTest RecursionTest = new RecursionTest();
		RecursionTest.test(4);
	}
}

class RecursionTest{
	public void test(int n) {
		if (n > 2) {
			test(n - 1);
		}
		System.out.println("n = " + " " + n);
	}
}

/*
输出结果：
n =  2
n =  3
n =  4
*/
![](E:\Study\自学课程资料\Java\assets\jvm的内存方法的递归调用（打印问题）.png)

阶乘问题

public class Recursion02{
	public static void main(String[] args) {
		RecursionTest recursionTest = new RecursionTest();
		int num = recursionTest.factorial(5);
		System.out.println(num);
	}
}

class RecursionTest{

	public int factorial(int n){
		if (n == 1) {
			return 1;
		}else {
			return factorial(n - 1) * n;
		}
	}
}

//输出结果：120
![](E:\Study\自学课程资料\Java\assets\jvm的内存方法的递归调用（阶乘问题）.png)

方法递归调用重要规则
1、执行一个方法时，就开辟一个受保护的栈空间。

2、方法的局部变量是独立的，不会相互影响。

3、如果方法中使用的是引用数据类型，就会共享该引用类型的数据。

4、递归必须向退出递归的条件逼近，否则就是无限递归。

5、当一个方法执行完毕或遇到return就会返回，遵守谁调用就将结果返回给谁。同时当方法体执行完毕或返回时，该方法也执行完毕。

重载（OverLoad）
介绍：同一个类中，允许多个同名方法存在，但形参列表不同

public class OverLoad01{

	public static void main(String[] args) {

		MyCalculator myCalculator = new MyCalculator();
		int n1 = myCalculator.calculate(1,2);
		double d1 = myCalculator.calculate(1,2.0);
		double d2 = myCalculator.calculate(1.0,2);
		int n2 = myCalculator.calculate(1,2,3);

		System.out.println(n1);
		System.out.println(d1);
		System.out.println(d2);
		System.out.println(n2);
	}
}

class MyCalculator {

	//calculate重载
	public int calculate(int n1,int n2) {
		return n1 + n2;
	}

	public double calculate(int n1,double n2) {
		return n1 + n2;
	}

	public double calculate(double n1,int n2) {
		return n1 + n2;
	}

	public int calculate(int n1,int n2,int n3) {
		return n1 + n2 + n3;
	}	
}

/*
输出结果：
3
3.0
3.0
6
*/
构成重载要求
1、方法名必须相同。

2、形参列表必须不同（形参类型、个数、顺序至少有一个不同）。

3、参数名、返回值不同不影响重载。

OverLoad Test
public class OverLoadExercise01{
	public static void main(String[] args) {
		Method method = new Method();
		System.out.println(method.max(1,2));
		System.out.println(method.max(1.0,2.0));
		System.out.println(method.max(3.0,3.5,4.5));
	}
}

class Method{

	public int max(int a,int b) {
		return a > b ? a : b;
	}

	public double max(double a,double b) {
		return a > b ? a : b;
	}

	public double max(double a,double b,double c) {
		double max = a > b ? a : b;
		return max > c ? max : c;
	}
}
可变参数
基本概念：将同一个类中多个同名同功能，参数不同的方法封装为一个方法。

public class VarParameter01{
	public static void main(String[] args) {
		HspMethod hspmethod = new HspMethod();
		System.out.println(hspmethod.sum(1,3,5));
		
		int[] array = {1,5,10};
		System.out.println(hspmethod.sum_1(array));
	}
}

class HspMethod{
	//int...表示接收的是可变参数，数据类型为int，即可接收多个int类型的数据。
	//使用可变参数时，可以当作数组使用，即nums可以当作数组。
	public int sum(int... nums) {
		int rest = 0;
		for (int i = 0;i < nums.length;i++) {
			rest += nums[i];
		}
		return rest;
	}


	//数组解决。
	public int sum_1(int[] array) {
		int rest = 0;
		for (int i = 0;i < array.length;i++) {
			rest += array[i];
		}
		return rest;
	}
}
可变参数细节
1、可变参数的实参可以为0或多个。

2、可变参数的实参可以为数组。

3、可变参数的本质就是数组。

4、可变参数可以和普通类型的参数一起出现在形参列表，但可变参数在最后。

5、一个形参列表只能有一个可变参数。

作用域
1、java编程中，主要变量为全局变量（属性）和局部变量。

2、局部变量一般指在成员方法中定义的变量。

3、全局变量作用域为整个类；局部变量作用域为定义它的代码块中。

4、全局变量有默认值，可以不赋值直接使用；局部变量没有默认值，必须赋值后使用。

public class Scope{
	public static void main(String[] args) {
	}
}

class Cat{

	double age; //默认值为0.0

	public void say(){
		int num;
        
        /*
         * Scope.java:14: 错误: 可能尚未初始化变量num
                System.out.println("num = " + num);
        */
		System.out.println("num = " + num);
		System.out.println("age = " + age);
	}
}
作用域细节
1、全局变量（属性）可以和局部变量重名，访问时遵循就近原则。

2、同一个作用域中，局部变量不能重名。

3、（全局变量）属性生命周期长，伴随着对象的创建销毁而创建销毁；局部变量随着代码块的执行而创建，随着代码块的结束而销毁。

4、（全局变量）可以被本类使用，或其它类通过对象调用；局部变量只能在本类中对应的方法中使用。

5、全局变量可以加修饰符；局部变量不可加修饰符。

构造器/构造器
基本语法：访问修饰符 方法名 （形参列表） {方法体}

1、构造器的访问修饰符可以默认，也可以是public、protected、private。

2、构造器没有返回值。

3、构造器方法名和类名必须相同。

4、参数列表和成员方法一样的规则。

5、构造器的调用由系统完成。

public class Constructor01{
	public static void main(String[] args) {
		//new 一个对象，直接通过构造器指定姓名、年龄。
		Person p = new Person("蒋兴树",21);
		System.out.println(p.name);	
		System.out.println(p.age);	
	}
}

class Person{
	String name;
	int age;

	public Person(String name,int age) {
		this.name = name;
		this.age = age;
	}
}
构造器细节
1、一个类可以定义多个不同的构造器，即构造器重载。

2、构造器名和类名要相同。

3、构造器无返回值。

4、构造器是完成对对象的初始化，并不是创建对象。

5、在创建对象时，系统自动调用该类的构造方法。

6、若没有定义构造方法，系统会自动生成一个无参构造方法。

7、若定义了构造方法，默认的构造器就被覆盖。就不能再使用默认的无参构造器，除非显式的定义一个。

public class ConstructorDetail{
	public static void main(String[] args) {
		Person p = new Person("蒋兴树",21);
		Person p1 = new Person("蒋兴树");
	}
}

class Person{
	String name;
	int age;

	//第一个构造器
	public Person(String name,int age){
		this.name = name;
		this.age = age;
	}

	//第二个构造器
	public Person(String name){
		this.name = name;
	}
}
构造器 对象创建流程
![](E:\Study\自学课程资料\Java\assets\构造器-对象创建流程.png)

this理解
![](E:\Study\自学课程资料\Java\assets\this理解.png)

this细节
1、this的调用必须在构造器中的第一个语句。

2、this关键字可以访问本类的属性、方法、构造器。

3、this用于区分当前类的全局变量（属性）和局部变量。

4、this访问成员方法的语法：this.方法名（参数列表）。

5、this访问构造器语法：this（参数列表），只能在构造器中访问另一个构造器。

6、this不能在类定义的外部使用，只能在类定义的方法中使用。

public class ThisDetail{
	public static void main(String[] args) {
		Test test = new Test();
		test.f2();
	}
}

class Test{
	public void f1() {
		System.out.println("调用f1方法");
	}

	//细节3
	public void f2() {
		f1();
		this.f1();//this就是指当前对象，this.f1 可以看作 Test.f1。
	}


	//细节4
	public Test(String name,int age) {
		System.out.println("Test(String name,int age)构造器");
	}
	public Test() {
		this("蒋兴树",21);//this的调用必须在构造器中的第一个语句。
		System.out.println("Test构造器");
	}
}
static
package net.wanhe.EduSystem;

public class Test {
    public static void main(String[] args) {

        EduSystem EduSystem = new EduSystem();
        EduSystem.run();
    }
}
package net.wanhe.EduSystem;

import java.util.Scanner;

public class EduSystem {

    //描述教育系统
    Scanner sc = new Scanner(System.in);

    //运行教育系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = PrintlnMenu();

            switch (chooise) {
                case 1:
                    StuSystem StuSystem = new StuSystem();
                    StuSystem.run();
                    break;
                case 2:
                    TeaSystem TeaSystem = new TeaSystem();
                    TeaSystem.run();
                    break;
                case 3:
                    flag = false;
                    System.out.println("谢谢使用");
                    break;
            }
        }
    }


    //展示系统菜单的方法
    public int PrintlnMenu() {
        System.out.println("--教育系统--");
        System.out.println("1、学生系统");
        System.out.println("2、教师系统");
        System.out.println("3、退出系统");
        System.out.println("请选择：");

        int chooise = sc.nextInt();
        return chooise;
    }
}
package net.wanhe.EduSystem;

import java.util.Scanner;

//描述学生系统
public class StuSystem {

    Scanner sc = new Scanner(System.in);

    static String[] Stus = new String[20];

    //运行学生系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = StuMenu();

            switch (chooise) {
                case 1:
                    FindAllStu();
                    break;
                case 2:
                    AddStu();
                    break;
                case 3:
                    DelStus();
                    break;
                case 4:
                    flag = false;
                    break;
            }
        }
    }


    //展示学生系统菜单的方法
    public int StuMenu() {
        System.out.println("--学生系统--");
        System.out.println("1、查看学生信息");
        System.out.println("2、添加学生");
        System.out.println("3、删除学生");
        System.out.println("4、返回上一级");
        System.out.println("请选择：");

        return sc.nextInt();
    }


    //查看学生信息
    public void FindAllStu() {
        for (int i = 0; i < Stus.length; i++) {
            if (Stus[i] != null) {
                System.out.println("学号:" + (i + 1) + "  " + "姓名:" + Stus[i]);
            }
        }
    }


    //添加学生
    public void AddStu() {
        System.out.println("输入学生学号");
        int num = sc.nextInt();
        System.out.println("输入学生姓名");
        String name = sc.next();

        if (num < 1 || num > Stus.length) {
            System.out.println("学号无效");
            return;
        }
        if (Stus[num] != null) {
            System.out.println("学号无效");
            return;
        }
        Stus[num - 1] = name;
        System.out.println("添加成功");
    }


    //删除学生
    public void DelStus() {
        System.out.println("输入学生学号");
        int num = sc.nextInt();

        if (num < 1 || num > Stus.length) {
            System.out.println("学号无效");
            return;
        }
        Stus[num] = null;
        System.out.println("删除成功");
    }
}
package net.wanhe.EduSystem;

import java.util.Scanner;

//描述教师系统
public class TeaSystem {

    Scanner sc = new Scanner(System.in);

    static String[] Teas = new String[20];

    //运行教师系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = TeaMenu();

            switch (chooise) {
                case 1:
                    FindAllTea();
                    break;
                case 2:
                    AddTea();
                    break;
                case 3:
                    DelTea();
                    break;
                case 4:
                    flag = false;
                    break;
            }
        }
    }


    //展示教师系统菜单的方法
    public int TeaMenu() {
        System.out.println("--教师系统--");
        System.out.println("1、查看教师信息");
        System.out.println("2、添加教师");
        System.out.println("3、删除教师");
        System.out.println("4、返回上一级");

        return sc.nextInt();
    }

    //查看教师信息
    public void FindAllTea() {
        for (int i = 0; i < Teas.length; i++) {
            if (Teas[i] != null) {
                System.out.println((i + 1) + ":" + Teas[i]);
            }
        }
    }


    //添加教师
    public void AddTea() {
        System.out.println("输入教师编号");
        int num = sc.nextInt();
        System.out.println("输入教师姓名");
        String name = sc.next();

        if (num < 1 || num > Teas.length) {
            System.out.println("编号无效");
            return;
        }
        if (Teas[num] != null) {
            System.out.println("编号无效");
            return;
        }
        Teas[num] = name;
        System.out.println("添加成功");
    }


    //删除教师
    public void DelTea() {
        System.out.println("输入教师编号");
        int num = sc.nextInt();

        if (num < 1 || num > Teas.length) {
            System.out.println("编号无效");
            return;
        }
        Teas[num] = null;
        System.out.println("删除成功");
    }
}
三层架构
![image-20220908103125923](E:\Study\自学课程资料\Java\assets\三层架构.png)

三层架构例
package net.wanhe.EduSystem.pojo;

public class Student {

    public String name;
    public int age;
    public char gender;
    public String number;
    public String address;
    public int num;

    public Student(int num,String name, int age, char gender, String number, String address) {
        this.num = num;
        this.name = name;
        this.age = age;
        this.gender = gender;
        this.number = number;
        this.address = address;
    }

    public Student(){

    }
}
package net.wanhe.EduSystem.pojo;

public class Teacher {

    public String name;
    public int age;
    public char gender;
    public String number;
    public String address;
    public int num;

    public Teacher(int num,String name, int age, char gender, String number, String address) {
        this.num = num;
        this.name = name;
        this.age = age;
        this.gender = gender;
        this.number = number;
        this.address = address;
    }

    public Teacher(){

    }
}
package net.wanhe.edusystem.controller;

import net.wanhe.edusystem.service.StuService;
import net.wanhe.edusystem.pojo.Student;

import java.util.Scanner;

/**
 * 模拟销售
 * 获取用户数据
 * 展示处理结果
 */
public class StuController {

    Scanner sc = new Scanner(System.in);

    StuService stuService = new StuService();

    /*
     * 展示菜单
     */
    public int printMenu(){
        System.out.println("--学生管理--");
        System.out.println("1.查看学生信息");
        System.out.println("2.添加学生");
        System.out.println("3.删除学生");
        System.out.println("4.返回上一级");
        System.out.println("请选择:");
        return sc.nextInt();
    }

    /*
     * 添加学生
     */
    public void addStu(){
        System.out.println("请输入学号:");
        int num = sc.nextInt();
        System.out.println("请输入姓名:");
        String name = sc.next();
        System.out.println("请输入年龄:");
        int age = sc.nextInt();
        System.out.println("请输入电话:");
        String phone = sc.next();
        System.out.println("请输入地址:");
        String address = sc.next();

        //将获取到的用户数据封装成学生对象
        Student stu = new Student(num,name,age,phone,address);
        //将数据交给service，由service继续完成

        stuService.addStu(stu);
    }

    /*
     * 删除学生
     */
    public void delStu(){
        System.out.println("请输入学号:");
        int num = sc.nextInt();
        stuService.delStu(num);
    }

    /*
     * 展示所有学生的信息
     */
    public void findAllStus(){
        Student[] stus = stuService.findAllStus();
        for(int i = 0;i < stus.length;i++){
            if(stus[i] != null){
                System.out.println("学号:" + stus[i].num
                        + "  姓名:" + stus[i].name
                        + "  年龄:" + stus[i].age
                        + "  手机号:" + stus[i].phone
                        + "  地址:" + stus[i].address
                );
            }
        }
    }
}
package net.wanhe.edusystem.service;

import net.wanhe.edusystem.dao.StuDao;
import net.wanhe.edusystem.pojo.Student;

/**
 * 模拟业务员
 * 处理业务逻辑
 */
public class StuService {

    StuDao stuDao = new StuDao();

    /*
     * 处理添加学生的业务逻辑
     */
    public void addStu(Student stu){
        //将学号给dao 获取该学号对应的信息
        Student s = stuDao.findByNum(stu.num);
        if(s != null){
            System.out.println("该学号以使用");
            return;
        }
        stuDao.addStu(stu);
        System.out.println("添加成功");
    }


    /*
     * 处理删除学生的业务逻辑
     */
    public void delStu(int num) {
        stuDao.delStu(num);
        System.out.println("删除成功");
    }

    /*
     * 查询所有的学生信息
     */
    public Student[] findAllStus() {
        Student[] stus = stuDao.findAllStus();
        return stus;
    }
}
package net.wanhe.edusystem.dao;

import net.wanhe.edusystem.pojo.Student;

/**
 * 模拟数据管理员
 * 管理数据
 */
public class StuDao {

    static Student[] stus = new Student[2];

    //记录了即将添加的数据的下标
    //记录了当前数组中存放的有效数据的数量
    static int index = 0;

    /*
     * 根据学号获取对应的学生信息
     */
    public Student findByNum(int num){
        for(int i = 0;i < index;i++){
            if(stus[i].num == num){
                return stus[i];
            }
        }
        return null;
    }

    /*
     * 添加学生
     * 动态数组
     */
    public void addStu(Student stu) {
        //当存放的数据和数组的容量相同时 进行 扩容 的操作
        if(index == stus.length){
            //创建一个新的数组
            Student[] newArray = new Student[stus.length + 2];
            //将旧数组stus中的数据存放到新数组newArray中
            for(int i = 0;i < stus.length;i++){
                newArray[i] = stus[i];
            }
            //将新数组的地址赋值给stus
            stus = newArray;
            System.err.println("测试代码 数组扩容");
        }
        stus[index++] = stu;
    }

    /*
     * 删除学生
     */
    public void delStu(int num) {
        //找到需要删除的下标
        for(int i = 0;i < index;i++){
            if(stus[i].num == num){
                //当前i的值就是要删除的下标
                //从i的值开始后面的数据都要向前移动
                for(int j = i;j < index - 1;j++){
                    stus[j] = stus[j+1];
                }
                stus[index - 1] = null;
                index--;
            }
        }
    }

    /*
     * 查询所有的学生信息
     */
    public Student[] findAllStus() {
        return stus;
    }
}
package net.wanhe.EduSystem.Controller;

import net.wanhe.EduSystem.Service.TeasService;
import net.wanhe.EduSystem.pojo.Teacher;

import java.util.Scanner;

//获取用户数据，展示处理结果。
public class TeasController {

    public int PrintMenu() {
        System.out.println("--教师系统--");
        System.out.println("1、查看教师信息");
        System.out.println("2、添加教师");
        System.out.println("3、删除教师");
        System.out.println("4、返回上一级");
        System.out.println("请选择：");

        Scanner scanner = new Scanner(System.in);
        int chooise = scanner.nextInt();
        return chooise;
    }


    //添加教师
    public void AddTeas() {
        Scanner scanner = new Scanner(System.in);

        System.out.println("输入教师编号");
        int num = scanner.nextInt();
        System.out.println("输入教师姓名");
        String name = scanner.next();
        System.out.println("输入教师年龄");
        int age = scanner.nextInt();
        System.out.println("输入教师性别");
        char gender = scanner.next().charAt(0);
        System.out.println("输入教师电话");
        String number = scanner.next();
        System.out.println("输入教师地址");
        String address = scanner.next();

        //将获取的数据封装为教师对象
        Teacher teacher = new Teacher(num,name,age,gender,number,address);
        //将数据交给Service处理，进行业务逻辑处理。
        TeasService TeasService = new TeasService();
        TeasService.AddTeas(teacher);
    }


    //删除教师
    public void DelTeas() {
        Scanner scanner = new Scanner(System.in);

        System.out.println("输入教师编号");
        int num = scanner.nextInt();

        //将获取的数据交给Service进行业务逻辑处理。
        TeasService TeasService = new TeasService();
        TeasService.DelTeas(num);
        System.out.println("删除成功");
    }


    public void FindAllTeas() {
        //查看所有数据，Controller不能直接去找Dao，只能先将数据交由Service，再由Service交给Dao。
        TeasService TeasService = new TeasService();
        Teacher[] teas = TeasService.FindAllTeas();

        for (int i = 0; i < teas.length; i++) {
            if (teas[i] != null) {
                System.out.println("学号:" + teas[i].num + "  " + "姓名:" + teas[i].name + "  " + "年龄:" +
                        teas[i].age + "  " + "性别:" + teas[i].gender + "  " + "电话:" + teas[i].number +
                        "  " + "地址:" + teas[i].address);
            }
        }
    }
}
package net.wanhe.EduSystem.Service;

import net.wanhe.EduSystem.Dao.TeasDao;
import net.wanhe.EduSystem.pojo.Teacher;

//业务逻辑处理
public class TeasService {

    //添加教师
    public void AddTeas(Teacher teacher) {

        //将编号给dao 获取该编号对应的信息。
        TeasDao TeaDao = new TeasDao();
        Teacher t = TeasDao.FindByNum(teacher.num);

        if (t != null) {
            System.out.println("编号无效");
        }
        TeasDao.AddTeas(teacher);
        System.out.println("添加成功");
    }

    //删除教师
    public void DelTeas(int num) {
        TeasDao TeasDao = new TeasDao();
        TeasDao.DelTeas(num);
    }

    //查询所有教师
    public Teacher[] FindAllTeas() {

        TeasDao TeasDao = new TeasDao();
        Teacher[] teas = TeasDao.FindAllTeas();
        return teas;
    }
}
package net.wanhe.EduSystem.Dao;

import net.wanhe.EduSystem.pojo.Teacher;

//管理数据
public class TeasDao {

    static Teacher[] teas = new Teacher[1];

    //记录了即将添加的数据的下标
    //记录了当前数组中存放的有效数据的数量
    static int index = 0;

    //根据编号获取对应的教师信息
    public static Teacher FindByNum(int num) {
        for (int i = 0;i < index;i++) {
            if (teas[i].num == num) {
                return teas[i];
            }
        }
        return null;
    }

    //添加教师，动态数组
    public static void AddTeas(Teacher teacher) {
        if (index == teas.length) {
            Teacher[] new_teas = new Teacher[teas.length + 1];
            for (int i = 0;i < teas.length;i++) {
                new_teas[i] = teas[i];
            }
            teas = new_teas;
            System.out.println("数组扩容");
        }
        teas[index++] = teacher;
    }

    //删除教师
    public void DelTeas(int num) {
        for (int i = 0;i < index;i++) {
            if (teas[i].num == num) {
                for (int j = i;j < index - 1;j++){
                    teas[j] = teas[j + 1];
                }
                teas[index - 1] = null;
                index--;
            }
        }
    }

    //查询所有教师信息
    public Teacher[] FindAllTeas() {
        return teas;
    }
}
package net.wanhe.EduSystem.System;

import java.util.Scanner;

public class EduSystem {

    //描述教育系统
    Scanner sc = new Scanner(System.in);

    StuSystem StuSystem = new StuSystem();

    TeaSystem TeaSystem = new TeaSystem();

    //运行教育系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = PrintlnMenu();

            switch (chooise) {
                case 1:
                    StuSystem StuSystem = new StuSystem();
                    StuSystem.run();
                    break;
                case 2:
                    TeaSystem TeaSystem = new TeaSystem();
                    TeaSystem.run();
                    break;
                case 3:
                    flag = false;
                    System.out.println("谢谢使用");
                    break;
            }
        }
    }


    //展示系统菜单的方法
    public int PrintlnMenu() {
        System.out.println("--教育系统--");
        System.out.println("1、学生系统");
        System.out.println("2、教师系统");
        System.out.println("3、退出系统");
        System.out.println("请选择：");

        int chooise = sc.nextInt();
        return chooise;
    }
}
package net.wanhe.EduSystem.System;

import net.wanhe.EduSystem.Controller.StusController;
import net.wanhe.EduSystem.pojo.Student;

import java.util.Scanner;

//描述学生系统
public class StuSystem {

    Scanner sc = new Scanner(System.in);

    static Student[] stus = new Student[20];

    StusController stusController = new StusController();

    //运行学生系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = StuMenu();

            switch (chooise) {
                case 1:
                    stusController.FindAllStus();
                    break;
                case 2:
                    stusController.AddStus();
                    break;
                case 3:
                    stusController.DelStus();
                    break;
                case 4:
                    flag = false;
                    break;
            }
        }
    }


    //展示学生系统菜单的方法
    public int StuMenu() {
        System.out.println("--学生系统--");
        System.out.println("1、查看学生信息");
        System.out.println("2、添加学生");
        System.out.println("3、删除学生");
        System.out.println("4、返回上一级");
        System.out.println("请选择：");

        return sc.nextInt();
    }
}
package net.wanhe.EduSystem.System;

import net.wanhe.EduSystem.Controller.TeasController;
import net.wanhe.EduSystem.pojo.Teacher;
import java.util.Scanner;

//描述教师系统
public class TeaSystem {

    Scanner sc = new Scanner(System.in);

    static Teacher[] Teas = new Teacher[20];

    TeasController teasController = new TeasController();

    //运行教师系统
    public void run() {

        boolean flag = true;

        while (flag) {

            int chooise = TeaMenu();

            switch (chooise) {
                case 1:
                    teasController.FindAllTeas();
                    break;
                case 2:
                    teasController.AddTeas();
                    break;
                case 3:
                    teasController.DelTeas();
                    break;
                case 4:
                    flag = false;
                    break;
            }
        }
    }


    //展示教师系统菜单的方法
    public int TeaMenu() {
        System.out.println("--教师系统--");
        System.out.println("1、查看教师信息");
        System.out.println("2、添加教师");
        System.out.println("3、删除教师");
        System.out.println("4、返回上一级");

        return sc.nextInt();
    }
}
package net.wanhe.EduSystem;

import net.wanhe.EduSystem.System.EduSystem;

public class Test {
    public static void main(String[] args) {

        EduSystem EduSystem = new EduSystem();
        EduSystem.run();
    }
}
1.1.7、面向对象编程（中级）
IDEA快捷键
1、Ctrl+D：复制行

2、Ctrl+Y：删除行

3、向上向下移动语句：Ctrl+Shift+⬆/⬇

4、补全代码：Alt+/

5、添加注释：Ctrl+/

6、快速格式化代码：Ctrl+Alt+L

7、运行代码：Shift+R

8、生成构造器：Alt+Ins

9、类型层次结构：Ctrl+H

10、定位方法：Ctrl+B

11、自动分配变量名：Alt+Enter

IDEA模板
1、main（public static void main(String[] args) {}）

2、sout（System.out.println();）

3、fori（for (int i = 0; i < ; i++) {}）

包
1、区分相同名字的类。

2、当类很多时，可以很好的管理类。

3、控制访问范围。

基本语法：package 包名

本质：创建不同的文件夹/目录来保存类文件。

包命名规则规范
规则：

1、只能包含数字、字母、圆点、下划线。

2、不能用数字开头。

3、不能是关键字或保留字。

规范：

1、一般是小写字母和圆点组成。

2、com.公司名.项目名.业务模块

新浪网 (sina.com.cn)

cn.com.sina.crm.user//用户模块

常用包
1、java.lang.*（基本包，默认引入）

2、java.util.*（系统提供的工具包）

3、java.net.*（网络包，网络开发）

4、java.awt.*（界面开发）

包使用细节
1、import java.util.Scanner;引入java.util包中的Scanner类

2、package的作用是声明当前类所在的包，需要放在类的最上面。

3、import指令位置在package下面，在类定义之前。

访问修饰符
作用：控制方法和属性的访问权限

1、公开级别public：对外公开。

2、受保护级别protected：对子类和同一个包中的类公开。

3、默认：对同一个包中的类公开。

4、私有级别private：类本身可以访问，不对外公开。

访问修饰符细节
1、同一个类中可以访问public、protected、默认、private修饰属性和方法。

2、同一个包中可以访问public、protected、默认修饰属性和方法。

3、不同包中可以访问public修饰属性和方法。

4、修饰符可以修饰类中的属性、方法以及类，只有public和默认的可以修饰类。

封装介绍
将抽象出的数据（属性）和对数据的操作（方法）封装在一起，数据被保护在内部，程序的其他部分只有通过被授权的操作（方法），才能对数据进行操作

封装优点
1、隐藏实现细节。

2、对数据进行验证，保证安全合理。

封装步骤
1、将属性私有化。

2、提供一个公共的set方法，用于对属性的判断并赋值。

3、提供一个公共的get方法，用于获取属性的值。

封装入门
package encapsulation.test01;

public class Person {
    public String name;
    private int age;
    private double salary;
    private String job;

    public Person(String name,int age,double salary,String job) {
        this.name = name;
        this.salary = salary;
        this.age = age;
        this.job = job;
    }

    public Person() {}

    public String getName() { return name; }

    public void setName(String name) {
        if (name.length() >= 2 && name.length() <= 6) {
            this.name = name;
        }else {
            System.out.println("名字不合理");
        }
    }

    public int getAge() { return age; }

    public void setAge(int age) {
        if (age >= 1 && age <= 120) {
            this.age = age;
        }else {
            System.out.println("年龄不合理");
        }
    }

    public double getSalary() { return salary; }

    public void setSalary(double salary) { this.salary = salary; }

    public String getJob() { return job; }

    public void setJob(String job) { this.job = job; }

    public String info() {
        return "name=" + name + " age=" + age + " salary=" + salary + " job=" + job;
    }
}

/*
 * 小程序
 * 不可随意查看人的年龄、工作、工资（封装）
 * 年龄必须在1-120之间
 * 姓名的长度在2-6字符之间
 */
class EncopExercise01 {
    public static void main(String[] args) {
        Person person = new Person();
        person.setName("蒋兴树儿 ohayo");
        person.setAge(30);
        person.setSalary(30000);
        person.setJob("工程师");

        String s = person.info();
        System.out.println(s);
    }
}
封装练习
package encapsulation.test01;

public class Account {
    private String name;
    private double salary;
    private String password;

    public Account() { }

    public Account(String name, double salary, String password) {
        this.name = name;
        this.salary = salary;
        this.password = password;
    }

    public String getName() { return name; }

    public void setName(String name) {
        if (name.length() == 2 || name.length() == 3 || name.length() == 4) {
            this.name = name;
        }else {
            System.out.println("名字不合理");
        }
    }

    public double getSalary() { return salary; }

    public void setSalary(double salary) {
        if (salary > 20) {
            this.salary = salary;
        }else {
            System.out.println("穷鬼");
        }
    }

    public String getPassword() { return password; }

    public void setPassword(String password) {
        if (password.length() == 6) {
            this.password = password;
        }else {
            System.out.println("密码错误");
            this.password = "123456";
        }
    }
}

class AccountTest {
    public static void main(String[] args) {
        Account account = new Account();
        account.setName("蒋兴树");
        account.setSalary(50000);
        account.setPassword("666666");
        System.out.println("====个人信息====");
        System.out.println("姓名：" + account.getName() + "  " + "薪资："
                + account.getSalary() + "  " + "密码：" + account.getPassword());
    }
}

/*
输出结果：
穷鬼
密码错误
====个人信息====
姓名：蒋兴树  薪资：0.0  密码：123456
*/
继承介绍
优点：提高代码复用性

基本语法：class 子类 extends 父类{}

继承示意图


1、子类会自动拥有父类定义的属性、方法。

2、父类又叫超类、基类；子类又叫派生类。

继承入门
package Extend;

public class Student {
    public String name;
    private int age;
    private double score;

    public void setScore(double score) {
        this.score = score;
    }

    public void showinfo() {
        System.out.println("学生名：" + name + " 年龄：" + age + " 分数：" + score);
    }
}

class Pupil extends Student{
    public void testing() {
        System.out.println("小学生" + name + "正在考小学数学");
    }
}

class Graduate extends Student{
    public void testing() {
        System.out.println("大学生" + name + "正在考大学数学");
    }
}

class Test{
    public static void main(String[] args) {
        Pupil pupil = new Pupil();
        pupil.name = "张林森";
        pupil.testing();
        System.out.println("=====================");
        Graduate graduate = new Graduate();
        graduate.name = "蒋兴树";
        graduate.testing();
    }
}

/*
输出结果：
小学生张林森正在考小学数学
=====================
大学生蒋兴树正在考大学数学
*/
继承细节
1、子类继承父类所有的属性和方法，可以直接访问父类非私有的属性和方法，父类的私有属性和方法要通过父类提供公共的方法访问。

package Extend;

public class ExtendsDetail {
    public static void main(String[] args) {
        Sub sub = new Sub();
        sub.say();
    }
}

class Base{
    public int n1 = 100;
    protected int n2 = 200;
    int n3 = 300;
    private int n4 = 400;

    public int getN4() { return n4; }//父类的私有属性要通过父类提供公共的方法访问。

    public Base() { System.out.println("Base()"); }//无参构造器
    public void test1() { System.out.println("test1"); }
    protected void test2() { System.out.println("test2"); }
    void test3() { System.out.println("test3"); }
    private void test4() { System.out.println("test4"); }

    public void callTest4() { test4(); }//父类的私有方法要通过父类提供公共的方法访问。
}

class Sub extends Base{
    public Sub() { System.out.println("Sub()"); }
    public void say() {
        //父类非私有属性和方法可以在子类直接访问
        System.out.println("n1=" + n1 + " n2=" + n2 + " n3=" + n3 + " n4=" + getN4());
        test1();
        test2();
        test3();
        callTest4();
    }
}

/*
输出结果：
Base()
Sub()
n1=100 n2=200 n3=300 n4=400
test1
test2
test3
test4
*/
2、子类必须调用父类的构造器，完成父类的初始化。

3、当创建子类对象时，不管使用子类的任意构造器，默认情况下总会去调用父类的无参构造器。如果父类没有提供无参构造器，则必须在子类的构造器中用super去指定使用父类的哪个构造器完成对父类的初始化工作，否则编译不通过。

package Extend;

public class ExtendsDetail {
    public static void main(String[] args) {
        System.out.println("====第一个对象====");
        Sub sub1 = new Sub();
        System.out.println("====第二个对象====");
        Sub sub2 = new Sub("jxs");
        System.out.println("====第三个对象====");
        Sub1 sub3 = new Sub1("jxs",21);
    }
}

class Base{
    public Base() { System.out.println("Base()构造器被调用"); }//父类无参构造器。
}

class Sub extends Base{
    public Sub() { System.out.println("Sub()构造器被调用"); }
    public Sub(String name) { System.out.println("Sub(String name)构造器被调用"); }
}




class Base1{
    public Base1(String name,int age) { System.out.println("Base1(String name,int age)构造器被调用"); }//父类有参构造器。
}

class Sub1 extends Base1{
    //如果父类没有提供无参构造器，则必须在子类的构造器中用super去指定使用父类的哪个构造器完成对父类的初始化工作
    public Sub1(String name, int age) {
        super(name, age);
    }
}

/*
输出结果：
====第一个对象====
Base()构造器被调用
Sub()构造器被调用
====第二个对象====
Base()构造器被调用
Sub(String name)构造器被调用
====第三个对象====
Base1(String name,int age)构造器被调用
*/
4、若想指定调用父类的某个构造器则显式的调用一下（super(参数列表)）；若没有指定构造器则默认调用父类的无参构造器。

package Extend;

public class ExtendsDetail {
    public static void main(String[] args) {
        System.out.println("====第一个对象====");
        Sub sub1 = new Sub();
        System.out.println("====第二个对象====");
        Sub sub2 = new Sub("jxs");
        System.out.println("====第三个对象====");
        Sub sub3 = new Sub("jxs",21);
    }
}

class Base{
    public Base() { System.out.println("Base()父类无参构造器被调用"); }//父类无参构造器。
    public Base(String name) { System.out.println("Base(String name)父类构造器被调用");}
    public Base(String name,int age) { System.out.println("Base(String name,int age)父类构造器被调用");}
}

class Sub extends Base{
    public Sub() { System.out.println("Sub()子类构造器被调用"); }
    public Sub(String name) { super("jxs"); }
    public Sub(String name,int age) { super("jxs",21); }
}

/*
输出结果：
====第一个对象====
Base()父类无参构造器被调用
Sub()子类构造器被调用
====第二个对象====
Base(String name)父类构造器被调用
====第三个对象====
Base(String name,int age)父类构造器被调用
*/
5、super在使用时必须放在构造器第一行。

6、super()、this()都只能放在构造器第一行，因此这两个方法不能共存在一个构造器。

7、java所有类都是Object类的子类。

8、父类构造器的调用不限于直接父类，将一直往上追溯到Object类（顶级父类）。

package Extend;

public class ExtendsDetail {
    public static void main(String[] args) {
        Sub sub = new Sub();
    }
}

class TopBase{
    public TopBase() { System.out.println("TopBase()构造器被调用"); }
}

class Base extends TopBase{
    public Base() { System.out.println("Base()构造器被调用"); }
}

class Sub extends Base{
    public Sub() { System.out.println("Sub()构造器被调用"); }
}

/*
输出结果：
TopBase()构造器被调用
Base()构造器被调用
Sub()构造器被调用
*/
9、java中是单继承机制，子类最多只能继承一个父类。

10、子类父类必须满足is a关系（cat is a animal）。

继承本质（重要）
package Extend;

public class ExtendsTheory {
    public static void main(String[] args) {
        Son son = new Son();
        /*
         * 按照查找关系返回信息
         * 1、若子类有该属性并可以访问，则返回信息
         * 2、若子类无该属性，就看父类是否有该属性，若父类有该属性并可以访问，则返回信息。
         * 3、。。。。。
         *
         */
        System.out.println(son.name);
        System.out.println(son.age);
        System.out.println(son.hobby);
    }
}

class GrandPa {
    String name = "老头爷爷";
    String hobby = "旅游";
}

class Father extends GrandPa {
    String name = "小头爸爸";
    int age = 40;
}

class Son extends Father {
    String name = "大头儿子";
}

/*
输出结果：
大头儿子
40
旅游
*/
![](E:\Study\自学课程资料\Java\assets\继承的内存布局.png)

继承Test
package Extend;

public class ExtendsExercise {
    public static void main(String[] args) {
        C c = new C("jxs");
    }
}

class A{
    public A() {
        System.out.println("A类无参构造");
    }
}

class B extends A{
    public B(String name) {
        //super() 自动调用父类的无参构造
        System.out.println("B类有参构造");
    }
}

class C extends B{
    public C(String name) {
        super("jxs");
        System.out.println("C类有参构造");
    }
}

/*
输出结果：
A类无参构造
B类有参构造
C类有参构造
*/
Super介绍
1、基本介绍：super代表对父类的引用，用于访问父类的属性、方法、构造器

2、基本语法：

访问父类的属性，但不能访问父类的private属性。（super.属性名）

访问父类的方法，但不能访问父类的private方法。（super.方法名(参数列表)）

访问父类的构造器。（super(参数列表)）

Super细节
1、当子类和父类中属性、方法重名时，访问父类的属性、方法必须使用super。

package Super;

public class SuperDetail {
    public static void main(String[] args) {
        B b = new B();
        b.sum();

        C c = new C();
        c.count();
    }
}

class A{
    public void count() { System.out.println("父类A count() 计算方法"); }
}

class B extends A{
    public void sum() {
        System.out.println("子类B sum() 求和方法");

        /*
         * 若想调用父类的count方法，有三种方式
         * 调用count方法顺序：1、若本类有则直接调用；2、若没有则找父类；3、若父类没有则找父类的父类
         * 若查找到但不能访问则报错
         * 若没查找到则提示方法不存在
         */
        count();
        this.count();
        super.count();
    }
}

class C extends A{
    public void count() {
        System.out.println("====================");
        System.out.println("子类C count() 计算方法");
        super.count();
    }
}

/*
输出结果：
子类B sum() 求和方法
父类A count() 计算方法
父类A count() 计算方法
父类A count() 计算方法
====================
子类C count() 计算方法
父类A count() 计算方法
*/
2、super的访问不局限于直接父类，super会一级一级往上寻找，遵循就近原则和访问权限。

super和this区别
1、super访问父类属性；this访问本类属性，若本类没有则从父类中继续查找。

2、super访问父类方法；this访问本类方法，若本类没有则从父类中继续查找。

3、super调用父类构造器，必须放在子类构造器首行；this调用本类构造器，必须放在构造器首行。

4、super表示子类中访问父类对象；this表示当前对象。

重写（Override）
1、基本介绍：子类和父类的方法的返回值、名称、参数列表相同，则子类的方法重写了父类的方法。

package Override;

public class Override01 {
    public static void main(String[] args) {
        
    }
}

class Animal {
    public void cry() {
        System.out.println("动物叫");
    }
}

class Dog extends Animal{
    public void cry() {
        /*
         * dog为animal子类
         * dog的cry方法和animal的cry方法形式一样
         * dog的cry方法重写了animal的cry方法
         */
        System.out.println("小狗汪汪叫");
    }
}
重写（Override）细节
1、子类方法的参数列表、名称和父类方法的参数列表、名称完全一致。

2、子类方法的返回值类型和父类的返回值类型一致或是父类的返回值类型的子类。

3、子类方法不能缩小父类方法的访问权限。

重载、重写区别
名称	发生范围	方法名	参数列表	返回值类型	修饰符
重载（overload）	本类	相同	不同	无要求	无要求
重写（override）	父子类	相同	相同	子类方法的返回值类型和父类的返回值类型一致或是父类的返回值类型的子类	子类方法不能缩小父类方法的访问权限
多态
基本介绍：方法或对象具有多种形态，多态建立在封装和继承基础之上。

多态的具体体现：

1、方法的多态：重载、重写

2、对象的多态：一个对象的编译类型和运行类型可以不一致或一致。

                             编译类型在定义对象时就已经确定；运行类型可以变化。

                             编译类型看定义时=左边；运行类型看定义时=右边。

package Poly.PolyObject;

public class PolyObject {
    public static void main(String[] args) {
        /*
         * 编译类型 animal
         * 运行类型 dog
         */
        Animal animal = new Dog();
        animal.cry();

        /*
         * 编译类型 animal
         * 运行类型 cat
         */
        animal = new Cat();
        animal.cry();
    }
}

class Animal{
    public void cry() {
        System.out.println("动物叫");
    }
}

class Dog extends Animal{
    @Override
    public void cry() {
        System.out.println("狗叫");
    }
}

class Cat extends Animal{
    @Override
    public void cry() {
        System.out.println("猫叫");
    }
}

/*
输出结果：
狗叫
猫叫
*/
多态向上转型细节
1、多态的前提：两个类之间存在继承关系。

2、本质：父类的引用指向了子类的对象，向上转型

3、语法：父类类型 引用名 = new 子类类型()

4、特点：编译类型看左边，运行类型看右边。

                  可以调用父类的所有成员，不可以调用子类的特有成员。

                  最终运行效果看子类的最终实现。

package Poly.PolyDetail;

public class PolyDeatil{
    public static void main(String[] args) {
        Animal animal = new Cat();
        animal.eat();
        animal.drink();
        animal.run();
        animal.sleep();
    }
}

class Animal {
    public void eat() {
        System.out.println("吃");
    }

    public void run() {
        System.out.println("跑");
    }

    public void drink() {
        System.out.println("喝");
    }

    public void sleep() {
        System.out.println("睡");
    }
}

class Cat extends Animal{
    public void eat() {
        System.out.println("吃~");
    }

    public void catchMouth() {
        System.out.println("抓老鼠");
    }
}

/*
输出结果：
吃~
喝
跑
睡
*/
多态向下转型细节
1、语法：子类类型 引用名 = （子类类型）父类引用

2、只能强转父类的引用，不能强转父类的对象

3、要求父类的引用必须指向当前目标类型的对象

4、当向下转型可以调用子类类型中所有的成员

多态细节
1、属性无重写之说，属性的值看编译类型。

2、instanceof比较操作符，用于判断对象的运行类型是否为XX类型或XX类型的子类型。

public class PolyDetail2 {
    public static void main(String[] args) {
        System.out.println("====细节1====");
        //属性无重写之说，属性的值看编译类型。
        Base base = new Bean();
        System.out.println(base.count);
        Bean bean = new Bean();
        System.out.println(bean.count);

        System.out.println("====细节2====");
        //instanceof比较操作符，用于判断对象的运行类型是否为XX类型或XX类型的子类型。
        System.out.println(bean instanceof Bean);
        System.out.println(bean instanceof Base);
    }
}

class Base{
    int count = 10;
}

class Bean extends Base{
    int count = 20;
}
多态Test
public class PolyDeatil03 {
    public static void main(String[] args) {
        Son son = new Son();
        System.out.println(son.age);
        son.test();

        System.out.println("========");

        Father father = son;
        System.out.println(father == son);
        System.out.println(father.age);
        father.test();
    }
}

class Father{
    int age = 10;

    public void test() {
        System.out.println(this.age);
    }
}

class Son extends Father{
    int age = 20;

    @Override
    public void test() {
        System.out.println(this.age);
    }
}

/*
输出结果：
20
20
========
true
10
20
*/
1、属性无法重写。属性看编译类型；方法看运行类型。

Java动态绑定机制
1、当调用对象方法时，该方法会和该对象的内存地址（运行类型）绑定

2、当调用对象属性时，无动态绑定机制，哪里声明哪里使用。

public class DynamicBinding {
    public static void main(String[] args) {
        Father father = new Son();
        System.out.println(father.sum());
        System.out.println(father.sum1());
    }
}

class Father{
    public int i = 10;
    public int getI() { return i; }
    public int sum() { return getI() + 10; }
    public int sum1() { return i + 10; }
}

class Son extends Father{
    public int i = 20;
    public int getI() { return i; }
}

/*
输出结果：
30
20
*/
多态数组
数组的定义类型为父类类型，数组保存的实际元素类型为子类类型

public class PolyArray {
    public static void main(String[] args) {
        Person[] person = new Person[3];
        person[0] = new Person("jxs",21);
        person[1] = new Student("jxs",21,100.0);
        person[2] = new Teacher("jxs",21,20000);

        for (int i = 0;i < person.length;i++) {
            System.out.println(person[i].say());//动态绑定
        }
    }
}

class Person{
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    public int getAge() { return age; }
    public void setAge(int age) { this.age = age; }

    public String say() { return name + "\t" + age; }
}

class Student extends Person{
    private double score;

    public Student(String name, int age, double score) {
        super(name, age);
        this.score = score;
    }

    public double getScore() { return score; }
    public void setScore(double score) { this.score = score; }

    @Override
    public String say() {
        return super.say() + "\t" + score;
    }
}

class Teacher extends Person{
    private int salary;

    public Teacher(String name, int age, int salary) {
        super(name, age);
        this.salary = salary;
    }

    public int getSalary() { return salary; }
    public void setSalary(int salary) { this.salary = salary; }

    @Override
    public String say() {
        return super.say() + "\t" + salary;
    }
}

/*
输出结果：
jxs	21
jxs	21	100.0
jxs	21	20000
*/
多态参数
方法定义的形参类型为父类类型，实参类型允许为子类类型

public class Test {
    public static void main(String[] args) {
        Worker worker = new Worker("tom",10000.0);
        Manager manager = new Manager("jxs",20000.0,200000.0);
        Test test = new Test();
        test.showEmpAnnual(worker);
        test.showEmpAnnual(manager);
        test.testWork(worker);
        test.testWork(manager);
    }

    public void showEmpAnnual(Employee e) {
        System.out.println(e.getAnnual());
    }

    public void testWork(Employee employee) {
        if (employee instanceof Worker) {
            ((Worker) employee).work();//向下转型
        }else if (employee instanceof Manager) {
//            Manager manager = (Manager) employee;
//            manager.manage();
            ((Manager) employee).manage();//向下转型
        }
    }
}

class Employee{
    private String name;
    private double salary;

    public Employee(String name, double salary) {
        this.name = name;
        this.salary = salary;
    }

    public String getName() { return name; }
    public void setName(String name) {
        this.name = name;
    }
    public double getSalary() {
        return salary;
    }
    public void setSalary(double salary) {
        this.salary = salary;
    }

    public double getAnnual() {
        return salary * 12;
    }
}

class Worker extends Employee{
    public Worker(String name, double salary) {
        super(name, salary);
    }

    @Override
    public double getAnnual() {
        return getSalary() * 12;
    }

    public void work() {
        System.out.println("我是工人");
    }

}

class Manager extends Employee {
    private double bonus;

    public double getBonus() {
        return bonus;
    }
    public void setBonus(double bonus) {
        this.bonus = bonus;
    }

    public Manager(String name, double salary, double bonus) {
        super(name, salary);
        this.bonus = bonus;
    }

    @Override
    public double getAnnual() {
        return getSalary() * 12 + bonus;
    }

    public void manage() {
        System.out.println("我是经理");
    }
}

/*
输出结果：
120000.0
440000.0
我是工人
我是经理
*/
Object类详解
1、概念：类层次结构的根类，每个类都使用Object作为超类，所有对象（包括数组）都实现这个类的方法。

Object类相关方法
equals和==
1、==既可判断基本类型也可判断引用类型。若判断基本类型，判断的是值是否相等；若判断引用类型，判断的是地址是否相等，即判定是不是同一个对象。

public class Test {
    public static void main(String[] args) {
        A a = new A();
        A a1 = new A();
        A a2 = a1;
        System.out.println(a == a1);
        System.out.println(a2 == a1);
    }
}

class A{

}
2、equals是Object类中的方法，只能判断引用类型

3、equals默认判断地址是否相等，子类中往往重写该方法，用于判断内容是否相等。

/*
Object类equals方法源码
*/
public boolean equals(Object obj) {
	return (this == obj);
}

/*
String类equals方法源码
*/
public boolean equals(Object anObject) {
	if (this == anObject) {
		return true;
	}
	if (anObject instanceof String) {
		String anotherString = (String)anObject;
		int n = value.length;
			if (n == anotherString.value.length) {
				char v1[] = value;
                char v2[] = anotherString.value;
                int i = 0;
                while (n-- != 0) {
                    if (v1[i] != v2[i])
                        return false;
                    i++;
                }
                return true;
            }
	}
	return false;
}

/*
Integer类equals方法源码
*/
public boolean equals(Object obj) {
	if (obj instanceof Integer) {
		return value == ((Integer)obj).intValue();
	}
	return false;
}
equals课堂练习
public class Test {
    public static void main(String[] args) {
        Person person1 = new Person("jxs",21,'男');
        Person person2 = new Person("dwy",21,'男');
        //Object类中equals默认判断地址是否相等。
        System.out.println(person1.equals(person2));
    }
}

class Person{
    private String name;
    private int age;
    private char gender;

    public Person(String name, int age, char gender) {
        this.name = name;
        this.age = age;
        this.gender = gender;
    }

    @Override
    public boolean equals(Object obj) {
        //判断比较的对象是同一个对象，则直接返回true
        if (this == obj) {
            return true;
        }
        if (obj instanceof Person) {
            //向下转型，因为需要得到obj的各个属性
            Person person = (Person) obj;
            return this.name.equals(person.name) && this.age == person.age && this.gender == person.gender;
        }
        return false;
    }
}

/*
输出结果：false
*/
public class Test {
    public static void main(String[] args) {
        Person person1 = new Person();
        person1.name = "jxs";
        Person person2 = new Person();
        person2.name = "jxs";

        System.out.println(person1 == person2);
        System.out.println(person1.name.equals(person2.name));
        System.out.println(person1.equals(person2));
        
        String s1 = new String("jxs");
        String s2 = new String("jxs");
        System.out.println(s1.equals(s2));
        System.out.println(s1 == s2);
    }
}

class Person {
    public String name;
}

/*
输出结果：
false
true
false
true
false
*/
public class Test {
    public static void main(String[] args) {
        int n = 65;
        float f = 65.0f;
        System.out.println(n == f);

        char c1 = 'A';
        char c2 = 12;
        System.out.println(c1 == n);
        System.out.println(12 == c2);

        String s1 = new String("hello");
        String s2 = new String("hello");
        System.out.println(s1 == s2);
        System.out.println(s1.equals(s2));  
    }
}

/*
输出结果：
true
true
true
false
true
*/
hashCode方法
1、提高具有哈希结构的容器的效率

2、两个引用，若指向的是同一对象则哈希值肯定一样。

3、两个引用，若指向的是不同对象则哈希值肯定不同。

4、哈希值主要根据地址号来计算的，不能完全将哈希值等价于地址

5、在集合中需要hashCode的话可以重写

public class HashCode {
    public static void main(String[] args) {
        Person person = new Person();
        Person person1 = new Person();
        Person person2 = person1;
        System.out.println("person.hashCode()=" + person.hashCode());
        System.out.println("person1.hashCode()=" + person1.hashCode());
        System.out.println("person2.hashCode()=" + person2.hashCode());
    }
}

class Person{ }

/*
输出结果：
person.hashCode()=835648992
person1.hashCode()=1134517053
person2.hashCode()=1134517053
*/
toString方法
1、默认返回：全类名 + @ + 哈希值的十六进制。

/*
Object类中toString方法源码：
1、getClass().getName() 类的全类名（包名+类名）
2、Integer.toHexString(hashCode() 将对象的hashCode值转成16进制字符串
*/
public String toString() {
	return getClass().getName() + "@" + Integer.toHexString(hashCode());
}
public class HashCode {
    public static void main(String[] args) {
        Monster monster = new Monster("smallmonster","巡山",10);
        System.out.println(monster.toString());
    }
}

class Monster{
    private String name;
    private String job;
    private double salary;

    public Monster(String name, String job, double salary) {
        this.name = name;
        this.job = job;
        this.salary = salary;
    }
}

/*
输出结果：net.wanhe.Monster@31cefde0
*/
2、子类往往重写toString方法，用于返回对象的属性信息。

public class HashCode {
    public static void main(String[] args) {
        Monster monster = new Monster("smallmonster","巡山",10);
        System.out.println(monster.toString());
    }
}

class Monster{
    private String name;
    private String job;
    private double salary;

    public Monster(String name, String job, double salary) {
        this.name = name;
        this.job = job;
        this.salary = salary;
    }

    @Override
    public String toString() {
        return "Monster{" +
                "name='" + name + '\'' +
                ", job='" + job + '\'' +
                ", salary=" + salary +
                '}';
    }
}

/*
输出结果：Monster{name='smallmonster', job='巡山', salary=10.0}
*/
3、当直接输出一个对象时，toString方法会被默认调用。

finalize方法
1、当对象被回收时，系统自动调用该对象的finalize方法。子类可以重写该方法，做一些释放资源的操作。

2、何时被回收：当某个对象没有任何引用时，则JVM就认为这个对象是一个垃圾对象，就会使用垃圾回收机制来销毁该对象，在销毁之前会先调用finalize方法。

3、垃圾回收机制的调用，由系统决定，也可以通过System.gc主动触发垃圾回收机制。

public class Finalize {
    public static void main(String[] args) {
        Car car = new Car("宝马");
        /*
        此时car对象无任何引用，垃圾回收器就会销毁此对象，销毁此对象前会调用该对象的finalize方法。
        程序员可以重写finalize方法，在finalize方法中输入自己的业务逻辑(如释放资源：数据库连接...)
        若程序员不重写finalize方法，则默认调用Object类的finalize方法
        */
        car = null;
        System.gc();//主动调用垃圾回收器
    }
}

class Car{
    private String name;

    public Car(String name) {
        this.name = name;
    }

    @Override
    protected void finalize() throws Throwable {
        System.out.println("销毁汽车对象，释放资源");
    }
}

/*
输出结果：销毁汽车对象，释放资源
*/
断点调试（debug）
1、实际需求：

（1）在开发中，程序员在查找错误时，可以用断点调试，一步一步查看源码执行的过程，从而发现错误所在。
（2）在断点调试过程中是运行状态，是以对象的运行类型来执行的。
2、介绍：

（1）断点调试指在程序的某一行设置一个断点，调试时，程序运行到这一行就会停止，然后可以一步一步往下调试，调试过程中可以看各个变量当前的值，调试到出错的代码即显示错误，停下。进行分析从而找到这个bug。
（2）断点调试是程序员必须掌握的技能
（3）断点调试可以帮助我们查看Java底层源代码的执行过程，提高程序员的Java水平。
3、断点调试快捷键：

F8：逐行执行代码
F7：跳入方法内，追溯源码
Alt+Shift+F7：强制跳入方法内，追溯源码
Shift+F8：跳出方法外
F9：resume，执行到下一个断点
断点调试案例
1、F8逐行执行

public class Debug01 {
    public static void main(String[] args) {
        //演示逐行执行
        int sum = 0;
        for (int i = 0; i < 5; i++) {
            sum += i;
            System.out.println("sum=" + sum);
            System.out.println("i=" + i);
        }
        System.out.println("退出for循环");
    }
}

/*
输出结果：
sum=0
i=0
sum=1
i=1
sum=3
i=2
sum=6
i=3
sum=10
i=4
退出for循环
*/
2、

public class Debug02 {
    public static void main(String[] args) {
        int[] array = {1,-10,-1};
        for (int i = 0; i <= array.length; i++) {
            System.out.println(array[i]);
        }
        System.out.println("退出for循环");
    }
}
/*
输出结果：
1
-10
-1
Exception in thread "main" java.lang.ArrayIndexOutOfBoundsException: 3
	at net.wanhe.Debug02.main(Debug02.java:7)
*/
3、追溯源码，提高编程思想

Debug如何F7进源码：
settings --> Build,Execution,Deployment --> Stepping --> Do not step into the classes --> 取消勾选java.*、javax.*
4、设置两个断点，在debug过程中，可以F9动态的执行到下一断点。

5、使用断点调试的方法，追踪下一个对象创建的过程。

public class DebugExercise {
    public static void main(String[] args) {
        Person person = new Person("jxs",21);
        System.out.println(person);
    }
}

class Person{
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public String toString() {
        return "Person{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}
6、使用断点调试的方法，查看动态绑定机制如何工作。

public class DynamicBinding {
    public static void main(String[] args) {
        Father father = new Son();
        System.out.println(father.sum());
    }
}

class Father{
    public int i = 10;
    public int getI() { return i; }
    public int sum() { return getI() + 10; }
}

class Son extends Father{
    public int i = 20;
    public int getI() { return i; }
}
1.1.8、学以致用
1.2、提升编程能力
1.2.1、面向对象编程（高级）
类变量提出
1、提出问题：一个游戏，不时有新小孩加入，请问如何知道现有多少小孩。

2、思路：main方法中定义一个变量count，当一个小孩加入游戏后count++

3、代码

public class Test {
    public static void main(String[] args) {
        //定义一个变量，统计有多少小孩
        int count = 0;
        
        Child child1 = new Child("jxs");
        child1.join(child1);
        count ++;

        Child child2 = new Child("dwy");
        child2.join(child2);
        count ++;

        Child child3 = new Child("zls");
        child3.join(child3);
        count ++;

        System.out.println(count);
    }
}

class Child{

    private String name;

    public Child(String name) {
        this.name = name;
    }

    public void join(Child child) {
        System.out.println(child.name + "加入了游戏");
    }
}
4、改进代码

public class Test {
    public static void main(String[] args) {
        Child child1 = new Child("jxs");
        child1.join(child1);
        child1.count++;

        Child child2 = new Child("dwy");
        child2.join(child2);
        child2.count++;

        Child child3 = new Child("zls");
        child3.join(child3);
        child3.count++;

        System.out.println(Child.count);
        System.out.println(child1.count);
        System.out.println(child2.count);
        System.out.println(child3.count);
    }
}

class Child{

    private String name;

    //定义一个变量 count , 是一个类变量（静态变量）。
    //该变量最大的特点就是会被 Child 类 所有的对象实例共享。
    public static int count = 0;

    public Child(String name) {
        this.name = name;
    }

    public void join(Child child) {
        System.out.println(child.name + "加入了游戏");
    }
}
类变量内存剖析
![](E:\Study\自学课程资料\Java\assets\类变量内存剖析.png)

类变量概念
1、类变量也叫静态变量/静态属性，是该类所有对象共享的变量，任何一个该类的对象去访问它时，取到的都是相同的值。

2、定义语句：访问修饰符 static 数据类型 变量名；

3、如何访问类变量：类名.类变量名

public class VisitStatic {
    public static void main(String[] args) {
        /*
         类名.类变量
         类变量随着类的加载而创建，无对象实例也可访问
         */
        System.out.println(Person.name);
        Person person = new Person();
        System.out.println(person.name);
    }
}

class Person{
    //类变量的访问必须遵循相关访问权限。
    public static String name = "jxs";
}
类变量使用细节
1、当某个类的所有对象都共享一个变量时，就可以考虑使用类变量

2、类变量与实例变量区别：类变量是该类所有对象共享；实例变量是每个对象独享

3、加上static称为类变量或静态变量，否则称为普通变量/实例变量/非静态变量。

4、类变量可以使用 类名.类变量名 或者 对象名.类变量名 访问

5、类变量在类加载时就进行初始化了

6、类变量的生命周期随着类的加载开始，随着类的消亡而销毁

类方法概念
1、形式：访问修饰符 static 数据返回类型 方法名(){}

2、类方法的调用：类名.类方法名 或者 对象名.类方法名

public class StaticMethod {
    public static void main(String[] args) {
        Student student = new Student("jxs");
        student.payFee(18500.0);
        student.payFee(10000.0);
        student.showFee();
    }
}

class Student{

    private String name;
    private static double fee = 0;

    public Student(String name) {
        this.name = name;
    }

    //当方法使用static修饰后，该方法就是静态方法
    //静态方法可以访问静态属性
    public static void payFee(double fee) {
        Student.fee += fee;
    }

    public static void showFee() {
        System.out.println(Student.fee);
    }
}
类方法经典使用场景
1、当方法中不涉及到任何和对象相关的成员，则可以将方法设计成静态方法，提高开发效率

2、在程序员实际开发时，往往会将一些通用的方法设计成静态方法，如此我们不需要创建对象就可使用。

类方法使用细节
1、类方法和普通方法都随着类的加载而加载，将结构信息存储在方法区

2、类方法无this参数；普通方法中隐含this参数

3、类方法可以通过类名调用，也可通过对象名调用；普通方法与对象有关，需通过对象名调用。

4、类方法中不可使用和对象有关的关键字，比如：this和super；普通方法可以。

5、类方法中只能访问静态变量或静态方法；普通成员方法既可访问普通变量，也可访问静态变量。

public class StaticMethod {
    public static void main(String[] args) {
        Student.test();
    }
}

class Student{
    private String name;
    private static double fee = 0;

    public static void testMath() {
        System.out.println("正在考数学");
    }

    public static void test() {
        //Non-static field 'name' cannot be referenced from a static context
        //System.out.println(name);

        testMath();
    }
}
public class StaticMethod {
    public static void main(String[] args) {
        Student student = new Student();
        student.test();
    }
}

class Student{
    private String name;
    private static double fee = 0;

    public static void testMath() {
        System.out.println("正在考数学");
    }

    public void test() {
        System.out.println(name);
        System.out.println(fee);
        testMath();
    }
}
理解main方法语法
public static void main(String[] args){}

1、java虚拟机需要调用类的main方法，即该方法的访问权限必须是public

2、java虚拟机在执行main方法时不必调用对象，所以该方法必须是静态方法

3、main方法接收String类型的数组参数，该数组中保存执行java命令时传递给所运行的类的参数。

main方法细节
1、在main方法中，我们可以直接调用main方法所在类的静态方法或静态属性。但不可直接访问该类中的非静态成员，必须创建该类的一个实例对象后才能通过这个对象去访问类中的非静态成员。

public class Main01 {
    
    private static String name = "jxs";
    private int age = 21;

    private static void test() { System.out.println("hello"); }
    private void test1() { System.out.println("hi"); }

    public static void main(String[] args) {
        //可直接调用 name
        //在main方法中，我们可以直接调用main方法所在类的静态方法或静态属性
        String name = Main01.name;
        System.out.println(name);
        Main01.test();

        //创建该类的一个实例对象后才能通过这个对象去访问类中的非静态成员
        Main01 main01 = new Main01();
        int age = main01.age;
        System.out.println(age);
        main01.test1();
    }
}
代码块
1、基本介绍：

		（1）代码块又称初始化块，属于类中的成员，类似于方法，将逻辑语句封装在方法体中，通过{}包围起来。		（2）和方法不同，代码块没有方法名，没有返回类型，没有参数，只有方法体，而且不用通过对象或类显示调用，而是加载类时或创建对象时隐式调用。

2、基本语法：[修饰符] {代码};

3、基本语法说明：

		（1）修饰符只可写static

		（2）被static修饰的为静态代码块，否则为普通代码块；

		（3）逻辑语句可以为任何逻辑语句

		（4）;可以省略

4、代码块好处：

		（1）相当于另一种形式的构造器（对构造器的补充），可以做初始化的操作

		（2）若多个构造器中都有重复语句，可以抽取到代码块中，提高代码复用性。

5、代码理解：

public class CodeBlock {
    public static void main(String[] args) {
        Movie movie = new Movie("你好李焕英");
        System.out.println("====================");
        Movie movie1 = new Movie("你好李焕英",100.0,"沈腾");
    }
}

class Movie{
    private String name;
    private double price;
    private String director;

    {
        System.out.println("人员入场");
        System.out.println("灯光熄灭");
        System.out.println("电影开始");
    }

    /*
     3个构造器 重载
     3个构造器都有相同的语句，代码冗余
     可以将相同的语句放入代码块中即可
     当我们不管调用哪个构造器创建对象，都会先调用代码块内容
     代码块调用的顺序优先于构造器
     */
    public Movie(String name) {
//        System.out.println("人员入场");
//        System.out.println("灯光熄灭");
//        System.out.println("电影开始");
        this.name = name;
        System.out.println("Movie(String name) 被调用");
    }

    public Movie(String name, double price) {
//        System.out.println("人员入场");
//        System.out.println("灯光熄灭");
//        System.out.println("电影开始");
        this.name = name;
        this.price = price;
        System.out.println("Movie(String name, double price) 被调用");
    }

    public Movie(String name, double price, String director) {
//        System.out.println("人员入场");
//        System.out.println("灯光熄灭");
//        System.out.println("电影开始");
        this.name = name;
        this.price = price;
        this.director = director;
        System.out.println("Movie(String name, double price, String director) 被调用");
    }
}

/*
输出结果：
人员入场
灯光熄灭
电影开始
Movie(String name) 被调用
====================
人员入场
灯光熄灭
电影开始
Movie(String name, double price, String director) 被调用
*/
代码块细节
1、static代码块也叫静态代码块，作用是对类进行初始化，随着类的加载而执行，并且只执行一次。若是普通代码块，每创建一个对象就执行一次

2、类何时被加载

		（1）创建对象实例时

		（2）创建子类对象实例，父类也会被加载

		（3）使用类的静态成员时。

public class CodeBlockDeatil {
    public static void main(String[] args) {
        //类何时被加载:创建对象实例时
        Block block = new Block();
        System.out.println("==================");
        //类何时被加载:创建子类对象实例，父类也会被加载
        Block01 block01 = new Block01();
        System.out.println("==================");
        //类何时被加载:使用类的静态成员时
        System.out.println(Block02.n1);
    }
}

class Block{
    static {
        System.out.println("Block父类的静态代码块被执行");
    }
}

class Block01 extends Block{
    static {
        System.out.println("Block01子类的静态代码块被执行");
    }
}

class Block02{
    public static int n1 = 100;
    static {
        System.out.println("Block02类的静态代码块被执行");
    }
}

/*
输出结果：
Block父类的静态代码块被执行
==================
Block01子类的静态代码块被执行
==================
Block02类的静态代码块被执行
100
*/
3、普通代码块，在创建对象实例时，会被隐式调用。被创建一次就会被调用一次。若只是使用类的静态成员时，普通代码块并不会执行

public class CodeClockDeail01 {
    public static void main(String[] args) {
        A a = new A();
        System.out.println("===============");
        //静态代码块随着类的加载而执行，并且只执行一次。
        A a1 = new A();
        System.out.println("===============");
        //若只是使用类的静态成员时，普通代码块并不会执行
        System.out.println(a1.n);
    }
}

class A{
    public static int n = 1000;

    static {
        System.out.println("A类的静态代码块被执行");
    }

    //普通代码块，创建1个对象实例就被调用1次，和类加载无关
    {
        System.out.println("A类的普通代码块被执行");
    }
}

/*
输出结果：
A类的静态代码块被执行
A类的普通代码块被执行
===============
A类的普通代码块被执行
===============
1000
*/
4、创建一个对象时，在一个类调用顺序是：

		（1）调用静态代码块和静态属性初始化（静态代码块和静态属性初始化调用的优先级一样，若有多个静态代码块和多个静态属性初始化，则按定义顺序调用）

		（2）调用普通代码块和普通属性初始化（普通代码块和普通属性初始化调用的优先级一样，若有多个普通代码块和多个普通属性初始化，则按定义顺序调用）

		（3）调用构造方法

public class CodeBlockDetail {
    public static void main(String[] args) {
        /*
         类调用顺序：
         1、多个静态代码块和多个静态属性初始化，则按定义顺序调用
         2、多个普通代码块和多个普通属性初始化，则按定义顺序调用
         3、调用构造方法
         */
        A a = new A(100);
    }
}

class A{
    //普通属性初始化
    private int n1 = getn1();

    //普通代码块
    {
        System.out.println("A类普通代码块");
    }

    //静态属性初始化
    private static int n = getn();

    //静态代码块
    static {
        System.out.println("A类静态代码块");
    }

    public static int getn() {
        System.out.println("getn方法被调用");
        return 100;
    }

    public int getn1() {
        System.out.println("getn1方法被调用");
        return 100;
    }

    //构造器
    public A(int n1) {
        this.n1 = n1;
        System.out.println("A类构造器被调用");
    }
}

/*
输出结果：
getn方法被调用
A类静态代码块
getn1方法被调用
A类普通代码块
A类构造器被调用
*/
5、构造器的最前面其实隐藏了super() 和 调用本类普通代码块

public class CodeBlockDetail {
    public static void main(String[] args) {
        B b = new B();
    }
}

class A{
    //A类普通代码块
    { System.out.println("A类普通代码块"); }

    //A类无参构造器
    public A() {
        //super()
        //调用本类普通代码块
        System.out.println("A类无参构造器"); 
    }
}

class B extends A{
    //B子类普通代码块
    { System.out.println("B子类普通代码块"); }

    //B子类无参构造器
    public B() {
        //super()
        //调用本类普通代码块
        System.out.println("B子类无参构造器");
    }
}

/*
输出结果：
A类普通代码块
A类无参构造器
B子类普通代码块
B子类无参构造器
*/
6、子类继承父类时，静态代码块、静态属性初始化、普通代码块、普通属性初始化，构造器调用顺序

		（1）父类的静态代码块、静态属性（优先级一样，按定义顺序执行）

		（2）子类的静态代码块、静态属性（优先级一样，按定义顺序执行）

		（3）父类的普通代码块、普通属性（优先级一样，按定义顺序执行）

		（4）父类构造器

		（5）子类的普通代码块、普通属性（优先级一样，按定义顺序执行）

		（6）子类构造器

public class CodeBlockDetail {
    public static void main(String[] args) {
        /*
         1、类加载
            （1）先加载父类 A类
            （2）再加载子类 B类
         2、创建对象
            （1）子类构造器
         */
        B b = new B();
    }
}

class A{
    static { System.out.println("A父类静态代码块"); }
    { System.out.println("A父类普通代码块"); }
    public A() {
        /*
         1、super()
         2、调用本类普通代码块
         */
        System.out.println("A父类无参构造器");
    }
}

class B extends A{
    static { System.out.println("B子类静态代码块"); }
    { System.out.println("B子类普通代码块"); }
    public B() {
        /*
         1、super()
         2、调用本类普通代码块
         */
        System.out.println("B子类无参构造器"); }
}

/*
输出结果：
A父类静态代码块
B子类静态代码块
A父类普通代码块
A父类无参构造器
B子类普通代码块
B子类无参构造器
*/
7、静态代码块只能调用静态属性、静态方法；普通代码块可以调用任意成员。

单例设计模式
1、设计模式是静态方法和静态属性的经典使用

2、设计模式是在大量的实践中总结和理论化后优选的代码结构、编程风格以及解决问题的思考方式。

3、何为单例设计模式：采取一定的方法保证在整个软件中，对某个类只能存在一个对象实例，并且该类只提供1个取得其对象实例的方法。

4、单例模式有两种方式：（1）饿汉式、（2）懒汉式

饿汉式
步骤：

1、构造器私有化

2、类内部创建对象

3、创建一个向外暴露一个静态的公共方法

4、代码实现

public class Single01 {
    public static void main(String[] args) {
        GirlFriend instance = GirlFriend.getInstance();
        System.out.println(instance);
    }
}

class GirlFriend{
    private String name;

    /*
     1、类加载后创建一个girlfriend对象
     2、静态方法中只能调用静态属性和静态方法
     3、为能够在静态方法中返回girlfriend对象，需将其修饰为static
     */
    private static GirlFriend girlfriend = new GirlFriend("dwy");
    /*
     如何保证只能创建一个GirlFriend对象：
     1、私有化构造器
     2、在类内部创建一个GirlFriend对象
     3、提供一个公共的static方法，返回GirlFriend对象
     */
    private GirlFriend(String name) {
        this.name = name;
    }

    public static GirlFriend getInstance() {
        return girlfriend;
    }
}

/*
输出结果：
net.wanhe.single.GirlFriend@31cefde0
*/
懒汉式
public class Single02 {
    public static void main(String[] args) {
        BoyFriend instance = BoyFriend.getInstance();
        System.out.println(instance);
    }
}

class BoyFriend{
    private String name;
    private static BoyFriend boyFriend;

    /*
     懒汉式步骤
     1、构造器私有化
     2、定义1个static静态属性对象
     3、提供一个公共的static方法，可以返回1个boyfriend对象
     */
    private BoyFriend(String name) {
        this.name = name;
    }

    //懒汉式：只有当用户使用getInstance方法时才会返回boyFriend对象，再次调用getInstance方法时会返回上次创建的boyFriend对象。
    public static BoyFriend getInstance() {
        if (boyFriend == null) {
            boyFriend = new BoyFriend("jxs");
        }
        return boyFriend;
    }
}

/*
输出结果：
net.wanhe.single.BoyFriend@31cefde0
*/
饿汉式、懒汉式区别
1、创建对象的时机不同：

		（1）饿汉式在类加载时就创建了对象实例

		（2）懒汉式在调用方法后才创建对象实例

2、饿汉式不存在线程安全问题；懒汉式存在线程安全问题。

3、饿汉式存在浪费资源问题；懒汉式不存在浪费资源问题。

final关键字
1、基本介绍：

		（1）final中文意思：最终的

		（2）final可以修饰类、属性、方法、局部变量

2、使用场景

		（1）不希望类被继承，可用final修饰

		（2）不希望父类的某个方法被子类重写时，可用final修饰（访问修饰符 final 返回值类型 方法名）

		（3）不希望类的某个属性被修改时，可用final修饰

		（4）不希望某个局部变量被修改时，可用final修饰

final细节
1、final修饰的属性又叫常量，一般用XX_XX_XX

2、final修饰的属性在定义时必须赋值且不能修改，赋值可以在如下位置之一：

		（1）定义时

		（2）构造器中

		（3）代码块中

public class Final01 {
    public static void main(String[] args) {
        A a = new A();
        System.out.println(a.TAX_RATE);
        System.out.println(a.TAX_RATE1);
        System.out.println(a.TAX_RATE2);
    }
}

class A{
    /*
     final修饰的属性在定义时必须赋值且不能修改，赋值可以在如下位置之一：
    （1）定义时
    （2）构造器中
    （3）代码块中
     */
    //（1）定义时
    public final double TAX_RATE = 0.8;

    public final double TAX_RATE1;
    public final double TAX_RATE2;

    //（2）构造器中
    public A() { TAX_RATE1 = 0.9; }

    //（3）代码块中
    { TAX_RATE2 = 0.1; }
}

/*
输出结果：
0.8
0.9
0.1
*/
3、若final修饰的属性是静态的，则初始化位置只能是：

		（1）定义时

		（2）静态代码块

public class Final01 {
    public static void main(String[] args) {
        System.out.println(A.TAX_RATE);
        System.out.println(A.TAX_RATE1);
    }
}

class A{
    public static final double TAX_RATE = 0.8;
    public static final double TAX_RATE1;

    static {
        TAX_RATE1 = 0.9;
    }
}

/*
输出结果：
0.8
0.9
*/
4、final类不能继承，但可以实例化对象

5、若类不是final类，但含有final方法。则方法不能被重写，但类可以被继承。

6、若一个类已经是final类，就无需将方法修饰为final方法。

7、final不能修饰构造器

8、final往往和static一起使用，效率更高，不会导致类加载，底层编译器做了优化处理。

public class Final01 {
    public static void main(String[] args) {
        System.out.println(A.n1);
    }
}

class A{
    //final往往和static一起使用，效率更高，不会导致类加载，底层编译器做了优化处理。
    public static final int n1 = 1000;
    static { System.out.println("A类的静态代码块"); }
}

/*
输出结果：1000
*/
9、包装类（Integer、Double、Float、Boolean等都是final），String也是final类。

final练习
1、求圆的面积

public class FinalExercise {
    public static void main(String[] args) {
        System.out.println(Circle.area(10.0));
    }
}

class Circle{
    private double radius;
    private static final double PI = 3.14;

    /**
     * 需求：求圆的面积
     * test方法求圆面积，求面积方法固定，方法不可被重写
     * @param radius
     * @return
     */
    public static final double area(double radius) {
        return PI * radius * radius;
    }
}
2、

class A{
    public static int addOne(final int n) {
        //不可修改，可以返回
        //++n;
        return n + 1;
    }
}
抽象类
1、父类的某些方法，需要声明但不明确如何实现，可以将其声明为抽象方法，那么这个类就是抽象类。

2、抽象类快速入门：当父类的一些方法无法确定时，可以用abstract关键字来修饰此方法，这个方法就是抽象方法，当一个类中存在抽象方法时，需要将该类声明为抽象类。

public class Abstract01 {
    public static void main(String[] args) {

    }
}

abstract class Animal{
    private String name;

    public Animal(String name) {
        this.name = name;
    }

    /**
     * 1、eat方法实现了也没有意义
     * 2、即 父类方法不确定性的问题
     * 3、因此将该方法设计为抽象方法
     * 4、所谓抽象方法，就是没有实现的方法
     * 5、所谓没有实现，就是没有方法体
     * 6、当一个类中存在抽象方法时，需要将该类声明为抽象类
     * 7、抽象类会被继承，由子类来实现抽象方法。
     */
    public abstract void eat() ;
}
抽象类细节
1、用abstract关键字来修饰一个类时，这个类就叫抽象类（访问修饰符 abstract 类名{}）

2、用abstract关键字来修饰一个方法时，这个方法就叫抽象方法（访问修饰符 abstract 返回值类型 方法名(参数列表);）

3、抽象类的价值更多作用是在于设计，设计者设计好父类后，子类继承并实现抽象类。

4、抽象类，是考官比较爱问的知识点，在框架和设计模式使用较多。

5、抽象类不能被实例化

public class Abstract01 {
    public static void main(String[] args) {
        //'Animal' is abstract; cannot be instantiated
        //new Animal();
    }
}

abstract class Animal{
    /**
     * 1、eat方法实现了也没有意义
     * 2、即 父类方法不确定性的问题
     * 3、因此将该方法设计为抽象方法
     * 4、所谓抽象方法，就是没有实现的方法
     * 5、所谓没有实现，就是没有方法体
     * 6、当一个类中存在抽象方法时，需要将该类声明为抽象类
     * 7、抽象类会被继承，由子类来实现抽象方法。
     */
    public abstract void eat() ;
}
6、抽象类不一定包含抽象方法；当一个类中存在抽象方法时，需要将该类声明为抽象类。

7、abstract只能修饰类和方法。

8、抽象类可以有任意成员（抽象类的本质还是类）。

abstract class Animal{
    public int n1 = 100;
    public static int n2 = 200;
    public void eat() {}
    public static void drink() {}
    public abstract void run();
}
9、抽象方法不可有方法体。

10、一个类若继承了抽象类，则它必须实现抽象类的所有抽象方法，除非它自己也声明为抽象类。

abstract class Animal{
    public abstract void eat();
}

//类“狗”必须声明为抽象或在“动物”中实现抽象方法“eat（）”
abstract class Dog extends Animal{

}

class Pastoral_Dog extends Dog{
    /*
     实现了父类Animal的抽象方法
     所谓实现，就是有方法体
     */
    @Override
    public void eat() {
        
    }
}
11、抽象方法不可使用private、final、static来修饰，因为这些关键字都与重写相违背。

抽象类练习
abstract public class Employee {
    private String name;
    private int id;
    private double salary;

    public Employee(String name, int id, double salary) {
        this.name = name;
        this.id = id;
        this.salary = salary;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getId() {
        return id;
    }
    public void setId(int id) {
        this.id = id;
    }
    public double getSalary() {
        return salary;
    }
    public void setSalary(double salary) {
        this.salary = salary;
    }

    //抽象方法
    public abstract void work();

    public static void main(String[] args) {
        Manager manager = new Manager("jxs",1,10000.0,100000.0);
        CommonEmployee commonEmployee = new CommonEmployee("zls",1,1.0);
        manager.work();
        commonEmployee.work();
    }
}

class Manager extends Employee{
    private double bonus;

    public double getBonus() {
        return bonus;
    }
    public void setBonus(double bonus) {
        this.bonus = bonus;
    }

    public Manager(String name, int id, double salary, double bonus) {
        super(name, id, salary);
        this.bonus = bonus;
    }

    @Override
    public void work() {
        System.out.println("经理" + getName() + "工作中");
    }
}

class CommonEmployee extends Employee{

    public CommonEmployee(String name, int id, double salary) {
        super(name, id, salary);
    }

    @Override
    public void work() {
        System.out.println("普通员工" + getName() + "工作中");
    }
}

/*
输出结果：
经理jxs工作中
普通员工zls工作中
*/
抽象类实践
1、需求

		（1）现有多个类，完成不同的任务

		（2）统计各自完成任务的时间

		（3）编程实现

public class TestTemplate {
    public static void main(String[] args) {
        A a = new A();
        B b = new B();
        a.job();
        b.job();
    }
}

class A{
    //计算任务 从1+...+800000000
    public void job() {
        //得到开始时间
        long start = System.currentTimeMillis();

        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i;
        }

        //得到结束时间
        long stop = System.currentTimeMillis();
        System.out.println("A类job方法执行时间=" + (stop - start) + "毫秒");
    }
}

class B{
    public void job() {
        //得到开始时间
        long start = System.currentTimeMillis();

        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i * 2;
        }

        //得到结束时间
        long stop = System.currentTimeMillis();
        System.out.println("B类job方法执行时间=" + (stop - start) + "毫秒");
    }
}

/*
输出结果：
A类job方法执行时间=314毫秒
B类job方法执行时间=377毫秒
*/
改进后：

public class TestTemplate {
    public static void main(String[] args) {
        A a = new A();
        B b = new B();
        a.calculateTime();
        b.calculateTime();
    }
}

class A{
    public void calculateTime() {
        //得到开始时间
        long start = System.currentTimeMillis();
        job();
        //得到结束时间
        long stop = System.currentTimeMillis();
        System.out.println("A类job方法执行时间=" + (stop - start) + "毫秒");
    }

    //计算任务 从1+...+800000000
    public void job() {
        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i;
        }
    }
}

class B{
    public void calculateTime() {
        //得到开始时间
        long start = System.currentTimeMillis();
        job();
        //得到结束时间
        long stop = System.currentTimeMillis();
        System.out.println("B类job方法执行时间=" + (stop - start) + "毫秒");
    }

    public void job() {
        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i * 2;
        }
    }
}
再改进：

public class TestTemplate {
    public static void main(String[] args) {
        A a = new A();
        B b = new B();
        a.calculateTime();
        b.calculateTime();
    }
}

//抽象类，模板设计模式
abstract class C {
    public abstract void job();
    public void calculateTime() {
        //得到开始时间
        long start = System.currentTimeMillis();
        job();
        //得到结束时间
        long stop = System.currentTimeMillis();
        System.out.println("job方法执行时间=" + (stop - start) + "毫秒");
    }
}

class A extends C {
    /*
     * 计算任务 从1+...+800000000
     * 实现了父类的job方法
     */
    @Override
    public void job() {
        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i;
        }
    }
}

class B extends C {
    @Override
    public void job() {
        long sum = 0;
        for (long i = 0; i < 800000000; i++) {
            sum += i * 2;
        }
    }
}
接口
//接口
public interface UsbInterface {
    //规定接口的相关方法
    public void start();
    public void stop();
}

class Computer{
    //编写一个方法，计算机工作
    public void work(UsbInterface usbInterface) {
        //通过接口调用方法
        usbInterface.start();
        usbInterface.stop();
    }

    public static void main(String[] args) {
        iPhone iPhone = new iPhone();
        Computer computer = new Computer();
        //将手机接入到电脑
        computer.work(iPhone);
    }
}

/*
 类 iPhone 实现 UsbInterface 接口
 类 iPhone 需要实现 UsbInterface 接口 规定的方法
 */
class iPhone implements UsbInterface{

    @Override
    public void start() {
        System.out.println("手机开始工作");
    }

    @Override
    public void stop() {
        System.out.println("手机停止工作");
    }
}

/*
输出结果：
手机开始工作
手机停止工作
*/
接口基本介绍
1、接口就是给出一些没有实现的方法，封装到一起，某个类要使用时，再根据具体情况将方法写出来。

2、语法：

interface 接口名{
    //属性
    //方法（1、抽象方法；2、默认实现方法；3、静态方法）
}

class 类名 implements 接口{
    //自己属性
    //自己方法
    //必须实现接口的抽象方法
}
3、JDK7.0前，接口里的所有方法都没有方法体，即都是抽象方法。

4、JDK8.0后，接口可以有默认实现方法，需要用default关键字修饰；JDK8.0后可以有静态方法

接口应用场景
/**
 * 项目经理提供1个接口
 */
interface DBInterface {
    public void connect();
    public void close();
}

/**
 * A程序员实现项目经理提供的接口去连接MySQL数据库
 */
class MySql implements DBInterface{
    @Override
    public void connect() { }

    @Override
    public void close() { }
}

/**
 * B程序员实现项目经理提供的接口去连接Oracle数据库
 */
class Oracle implements DBInterface{
    @Override
    public void connect() { }

    @Override
    public void close() { }
}
接口细节
1、接口不可被实例化

2、接口中所有方法都是public方法

3、接口中的方法可以不用abstract修饰

4、一个普通的类实现接口，就必须将该接口的所有方法都实现

5、抽象类实现接口，可以不实现接口的方法。

6、一个类可以同时实现多个接口

7、接口中的属性只可为final的，而且是public static final修饰符。

8、接口中属性的访问形式：接口名.属性名

9、一个接口不可继承其他类，但是可以继承多个别的接口。

10、接口的修饰符只能是public、默认，这点和类修饰符是一样的。

public interface IA {
    //细节2、3：接口中的方法默认用public、abstract修饰
    abstract public void eat();
    abstract public void drink();
}

interface ID{
    //细节7：默认为public static final int n = 10;
    int n = 10;
    //细节2、3：接口中的方法默认用public、abstract修饰
    void run();
}

//细节9：一个接口不可继承其他类，但是可以继承多个别的接口。
interface IE extends IA , ID{ }

//细节4：一个普通的类实现接口，就必须将该接口的所有方法都实现
class Cat implements IA{
    @Override
    public void eat() { }

    @Override
    public void drink() { }
}

//细节5：抽象类实现接口，可以不实现接口的方法。
abstract class Dog implements IA{
}

//细节6：一个类可以同时实现多个接口
class Pig implements IA , ID{

    @Override
    public void eat() { }

    @Override
    public void drink() { }

    @Override
    public void run() { }
}
接口练习题
public interface A {
    //默认为public static final int n = 1;
    int n = 1;
}

class B implements A{
    public static void main(String[] args) {
        B b = new B();
        System.out.println(b.n);
        System.out.println(A.n);
        System.out.println(B.n);
    }
}

/*
输出结果：
1
1
1
*/
继承类和实现接口
1、继承类和实现接口的区别是 is a 和 has a 

2、继承是先天具备；实现是后天学习。

3、继承解决代码的复用性和可维护性；接口是设计好各种规范，让其它类去实现这些方法。

4、接口在一定程度上实现了代码解耦

public class ExendsVsInterface {
    public static void main(String[] args) {
        LittleMonkey littleMonkey = new LittleMonkey("悟空");
        littleMonkey.climb();
        littleMonkey.swim();
        littleMonkey.fly();
    }
}

class Monkey{
    private String name;

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    public Monkey(String name) {
        this.name = name;
    }

    public void climb() {
        System.out.println(name + "爬树");
    }
}

//接口
interface Fish{
    void swim();
}

//接口
interface Bird{
    void fly();
}

/**
 * 当子类继承父类，即拥有父类的能力
 * 当子类需要扩展能力时，可以通过实现接口的方式扩展
 * 可以理解为实现接口是对java单继承机制的补充
 */
class LittleMonkey extends Monkey implements Fish , Bird{
    public LittleMonkey(String name) {
        super(name);
    }

    @Override
    public void swim() {
        System.out.println(getName() + "游泳");
    }

    @Override
    public void fly() {
        System.out.println(getName() + "飞翔");
    }
}

/*
输出结果：
悟空爬树
悟空游泳
悟空飞翔
*/
接口多态特性
1、多态参数

		（1）父类类型的变量 可以指向 继承父类类型的类的对象实例

		（2）接口的类型变量 可以指向 实现IF接口的类的对象实例

public class Interface_PolyParameter {
    public static void main(String[] args) {
        /*
         1、接口的多态实现
         2、接口的类型变量 可以指向 实现IF接口的类的对象实例
         */
        IF anIf = new Monster();
        IF anIf1 = new Car();

        /*
         1、继承的多态实现
         2、父类类型的变量 可以指向 继承父类类型的类的对象实例
         */
        Person person = new Student();
        Person person1 = new Teacher();
    }
}

interface IF{}
class Monster implements IF { }
class Car implements IF { }

class Person{}
class Student extends Person {}
class Teacher extends Person {}
class Computer{
    /*
     编写一个方法，计算机工作
     1、UsbInterface usbInterface形参是接口类型
     2、接收 实现了UsbInterface接口 的类的对象实例
     */
    public void work(Usb usb) {
        //通过接口调用方法
        usb.start();
        usb.stop();
    }

    public static void main(String[] args) {
        iPhone iPhone = new iPhone();
        Computer computer = new Computer();
        //将手机接入到电脑
        computer.work(iPhone);
    }
}

interface Usb {
    //规定接口的相关方法
    void start();
    void stop();
}

/*
 类 iPhone 实现 UsbInterface 接口
 类 iPhone 需要实现 UsbInterface 接口 规定的方法
 */
class iPhone implements Usb{
    @Override
    public void start() {
        System.out.println("手机开始工作");
    }

    @Override
    public void stop() {
        System.out.println("手机停止工作");
    }
}

/*
输出结果：
手机开始工作
手机停止工作
*/
2、多态数组

public class Interface_Array {
    public static void main(String[] args) {
        //接口类型的多态数组
        Usb[] usbs = new Usb[2];
        usbs[0] = new iPhone();
        usbs[1] = new Cimera();

        for (int i = 0; i < usbs.length; i++) {
            if (usbs[i] instanceof iPhone) {
                //向下转型
                ((iPhone) usbs[i]).call();
                usbs[i].connect();
            } else {
                usbs[i].connect();
            }
        }
    }
}

interface Usb {
    void connect();
}

class iPhone implements Usb {
    public void call() { System.out.println("打电话");}

    @Override
    public void connect() {
        System.out.println("手机连接Usb");
    }
}

class Cimera implements Usb {
    @Override
    public void connect() {
        System.out.println("相机连接Usb");
    }
}

/*
输出结果：
打电话
手机连接Usb
相机连接Usb
*/
3、接口的动态传递

public class Interface_PolyPass {
    public static void main(String[] args) {
        //接口类型的变量 指向 实现了该接口的类的对象实例
        Canidae canidae = new Dog();
        /*
         多态传递：
         若Canidae接口 继承了 Animal接口 ， Dog类 实现了 Canidae接口 ， 则相当于 Dog类 也实现了 Animal接口。
         */
        Animal animal = new Dog();

        Flower Flower = new SunFlower();
        Plant plant = new SunFlower();

    }
}

interface Animal { }
interface Canidae extends Animal{ }
class Dog implements Canidae { }

class Plant { }
class Flower extends Plant { }
class SunFlower extends Flower { }
接口练习
public class A extends C implements B {
    public void test() {
        /*
         System.out.println(n);
         Reference to 'n' is ambiguous, both 'C.n' and 'B.n' match(对“n”的引用是模棱两可的，“C.n”和“B.n”都匹配)
         */
        System.out.println(super.n);
        System.out.println(new C().n);
        System.out.println(B.n);
    }

    public static void main(String[] args) {
        A a = new A();
        a.test();
    }
}

interface B {
    //public static final int n = 1;
    int n = 1;
}

class C {
    int n = 2;
}

/*
输出结果：
2
2
1
*/
内部类
1、类的五大成员：属性、方法、构造器、代码块、内部类

2、基本介绍：一个类的内部完整的嵌套了另一个类结构。被嵌套的类称为内部类。

3、特点：可以直接访问内部类的私有属性，体现类与类之间的包含关系

//外部其他类
public class InnerClass {
    public static void main(String[] args) {
    }
}

//外部类
class Outer {
    private int n1 = 100;
    public void m1() { System.out.println("m1方法"); }
    public Outer(int n1) {
        this.n1 = n1;
    }
    { System.out.println("代码块"); }
    
    //内部类
    class Inner { }
}
4、内部类分类：

1、定义在外部类局部位置上
	（1）局部内部类(有类名)
	（2）匿名内部类(无类名)

2、定义在外部类的成员位置上
	（1）成员内部类(用static修饰)
	（2）静态内部类(无static修饰)
局部内部类
1、局部内部类是定义在外部类的局部位置上，并且有类名。

2、局部内部类可以直接访问外部类的所有成员，包含私有成员。

3、局部内部类不可添加访问修饰符，但可用final修饰。局部内部类好比局部变量。

4、局部内部类作用域：仅在定义它的方法或代码块中

5、外部类在方法中可以创建局部内部类的对象实例，然后调用方法即可。

6、外部其他类不可访问局部内部类

7、若外部类和局部内部类的成员重名时，默认遵循就近原则

//外部其他类
public class InnerClass {
    public static void main(String[] args) {
        Outer outer = new Outer();
        outer.m1();
    }
}

//外部类
class Outer {
    private int n1 = 100;
    private void m2() { System.out.println("Outer类m2方法"); }

    public void m1() {
        /*
         局部内部类:
         细节1:局部内部类是定义在外部类的局部位置上，比如方法中，并且有类名。
         细节3:局部内部类不可添加访问修饰符，但可用final修饰。
         细节4:局部内部类作用域：仅在定义它的方法或代码块中。
         */
        final class Inner {
            private int n1 = 100;
            public void tset() {
                /*
                 细节2:局部内部类可以访问外部类的所有成员，包含私有成员。
                 细节7:若外部类和局部内部类的成员重名时，默认遵循就近原则
                 Outer.this.n1解析:
                    (1)Outer.this:本质就是外部类的对象
                 */
                System.out.println("局部内部类n1=" + n1 + "\n" + "外部类n1=" + Outer.this.n1);
                m2();
            }
        }

        //细节6:外部类在方法中可以创建局部内部类的对象实例，然后调用方法即可。
        Inner inner = new Inner();
        inner.tset();
    }
}

/*
输出结果：
局部内部类n1=100
外部类n1=100
Outer类m2方法
*/
匿名内部类
1、匿名内部类本质是类、是内部类、是一个对象、无类名。

2、匿名内部类定义在外部类的局部位置，并且没有类名。

3、基本语法：new 类或接口(参数列表){类体};

/**
 * 演示匿名内部类
 */
public class AnonymousInnerClass {
    public static void main(String[] args) {
        Outer outer = new Outer();
        outer.test();
    }
}

//外部类
class Outer {
    public void test() {
        /*
         1、基于接口的匿名内部类:
            (1)传统方式:写一个类实现此接口，创建该类的一个对象实例
            但写一个类只使用一次，后续不再使用，因此可以使用匿名内部类来简化开发。
            (2)匿名内部类:new 接口(参数列表){类体}
         2、编译类型、运行类型
            (1)tiger编译类型:Animal
            (2)tiger运行类型:匿名内部类 Outer$1
         3、底层源码
            (1)System.out.println(tiger.getclass()); 得到tiger的运行类型 --> class net.wanhe.Inner.Outer$1
            (2)系统自动分配类名
             class Outer$1 implements Animal {
                 @Override
                 public void cry() {
                     System.out.println("老虎叫唤");
                 }
             };
            (3)JDK底层在创建匿名内部类 Outer$1 后，立即创建了 Outer$1类 的对象实例，并且把地址返回给 tiger。
         4、匿名内部类使用一次后就不再使用。
         */
        Animal tiger = new Animal() {
            @Override
            public void cry() {
                System.out.println("老虎叫唤");
            }
        };
        tiger.cry();


        /*
         1、基于类的匿名内部类
         2、编译类型、运行类型
            (1)father编译类型:Father
            (2)father运行类型:匿名内部类 Outer$2
         3、底层源码
            (1)System.out.println(father.getClass()); 得到father的运行类型 --> class net.wanhe.Inner.Outer$2
            (2)系统自动分配类名
             class Outer$2 extends Father {
             }
            (3)JDK底层在创建匿名内部类 Outer$2 后，立即创建了 Outer$2类 的对象实例，并且把地址返回给 father。
         4、参数列表会传递给构造器
         */
        Father father = new Father("jack") {
            @Override
            public void test() {
                System.out.println("匿名内部类重写了test()方法");
            }
        };
        father.test();

        
        /*
         1、基于抽象类的匿名内部类
         */
        Flower flower = new Flower() {
            @Override
            void grow() {
                System.out.println("花生长");
            }
        };
        flower.grow();
    }
}


interface Animal { void cry();}

class Father {
    private String name;
    public Father(String name) {
        this.name = name;
    }
    public void test() {}
}

abstract class Flower {
    abstract void grow ();
}

/*
输出结果：
老虎叫唤
匿名内部类重写了test()方法
花生长
*/
匿名内部类使用细节
1、匿名内部类语法奇特，匿名内部类既是一个类的定义，同时本身也是一个对象。因此语法上看，匿名内部类既有定义类的特征，也有创建对象的特征。因此调用匿名内部类方法如下：

public class AnonymousInnerClassDetail {
    public static void main(String[] args) {
        Outer01 outer01 = new Outer01();
        outer01.test();
    }
}

class Outer01 {
    private int n = 100;
    public void test() {

        /*
         调用test()方法
         */
        //方式一:
        Person person = new Person() {
            @Override
            public void test() {
                System.out.println("匿名内部类重写了test()方法");
            }
        };
        person.test();
        //方式二:
        new Person() {
            @Override
            public void test() {
                System.out.println("匿名内部类重写了test()方法");
            }

            @Override
            public void test1(String str) {
                super.test1(str);
            }
        }.test1("jxs");
    }
}

class Person {
    public void test() {
        System.out.println("Person类中的test()方法");
    }
    public void test1(String str) {
        System.out.println(str);
    }
}

/*
输出结果：
匿名内部类重写了test()方法
jxs
*/
2、匿名内部类可以直接访问外部类的所有成员，包括私有成员。

3、匿名内部类不可添加访问修饰符，因为匿名内部类的地位如同一个局部变量。

4、匿名内部类作用域：仅在定义它的方法或代码块中。

5、外部其他类不可访问匿名内部类

6、若外部类和匿名内部类的成员重名时，匿名内部类访问的话遵循就近原则。若想访问外部类的重名成员，则使用 外部类名.this.成员。

匿名内部类练习
1、

public class InnerClassExercise {
    //静态方法，形参为接口类型
    public static void test(Show show) {
        show.show_picture();
    }

    public static void main(String[] args) {
        //当作实参直接传递，简洁高效
        test(new Show() {
            @Override
            public void show_picture() {
                System.out.println("展示图片");
            }
        });


        /*
         传统方式:
         1、写一个类实现Show接口
         2、创建类的一个对象实例
         */
        Picture picture = new Picture();
        picture.show_picture();
    }
}


interface Show {
    void show_picture();
}

class Picture implements Show {
    //一个普通的类实现接口，就必须将该接口的所有方法都实现
    @Override
    public void show_picture() {
        System.out.println("展示图片");
    }
}

/*
输出结果：
展示图片
展示图片
*/
2、

public class Cellphone {
    public static void alarmClock(Bell bell) {
        bell.ring();
    }

    public static void main(String[] args) {
        /*
         1、传递了一个实现了 Bell接口 的匿名内部类Cellphone$1，立即创建 Cellphone$1类 的对象实例，并将地址返回给 bell。
         2、重写ring方法
         */
        alarmClock(new Bell() {
            @Override
            public void ring() {
                System.out.println("懒猪起床了");
            }
        });

        alarmClock(new Bell() {
            @Override
            public void ring() {
                System.out.println("小伙伴上课了");
            }
        });
    }
}

interface Bell {
    //默认为public abstract void ring();
    void ring();
}

/*
输出结果：
懒猪起床了
小伙伴上课了
*/
成员内部类
1、成员内部类是定义在外部类的成员位置，并且没有static修饰

2、成员内部类可以直接访问外部类的所有成员，包含私有的成员。

3、成员内部类可以添加任意访问修饰符，因为成员内部类的地位就相当于成员。

4、成员内部类作用域和外部类的其他成员一样。

5、外部类访问成员内部类的访问方式：创建对象实例再访问。

6、外部其他类访问成员内部类的访问方式如下：

7、外部类和成员内部类的成员重名时，成员内部类访问的话遵循就近原则。若想访问外部类的成员时则使用（外部类名.this.成员）访问。

//外部其他类
public class MemberInnerClass01 {
    public static void main(String[] args) {
        System.out.println("外部其他类使用成员内部类方式：");
        System.out.println("====方式一====");
        Outer.Inner inner = new Outer().new Inner();
        inner.test();
        System.out.println("====方式二====");
        Outer outer = new Outer();
        outer.getInnerInstance().test();
    }
}

//外部类
class Outer {
    private int n = 100;
    private String name = "jxs";
    private void test2() { System.out.println("外部类的test2()私有方法"); }

    /*
     成员内部类:
     1、成员内部类是定义在外部类的成员位置，并且没有static修饰
     2、定义在外部类的成员位置上，可以添加任意访问修饰符。
     3、成员内部类作用域和外部类的其他成员一样。
     */
    public class Inner {
        private int n = 200;
        public void test() {
            //成员内部类可以直接访问外部类的所有成员，包含私有的成员。
            System.out.println("n=" + n + '\n' + "name=" + name);
            test2();
            //外部类和成员内部类的成员重名时，成员内部类访问的话遵循就近原则。若想访问外部类的成员时则使用（外部类名.this.成员）访问。
            System.out.println("n=" + Outer.this.n);
        }
    }

    //定义一个方法:返回一个成员内部类Inner的对象实例。
    public Inner getInnerInstance() { return new Inner(); }

    public void test1() {
        /*
         使用成员内部类:
         外部类访问成员内部类的访问方式：创建对象实例再访问。
         */
        Inner inner = new Inner();
        inner.test();
        System.out.println(inner.n);
    }
}

/*
输出结果：
外部其他类使用成员内部类方式：
====方式一====
n=200
name=jxs
外部类的test2()私有方法
n=100
====方式二====
n=200
name=jxs
外部类的test2()私有方法
n=100
*/
静态内部类
1、静态内部类是定义在外部类的成员位置，并且有static修饰

2、静态内部类可以直接访问外部类的所有静态成员，包括私有的静态成员。

3、静态内部类不可以直接访问非静态成员。

4、静态内部类可以添加任意访问修饰符，因为它的地位就好比一个成员。

5、静态内部类的作用域和外部类的其他成员一样。

6、外部类访问静态内部类的访问方式：创建对象实例再访问。

7、外部其他类访问静态内部类的方式如下：

8、若外部类和静态内部类的成员重名时，静态内部类访问时默认遵循就近原则。若想访问外部类的成员，则可以使用（外部类名.成员）去访问。

public class StaticInnerClass {
    public static void main(String[] args) {
        System.out.println("外部其他类访问静态内部类的方式:");
        System.out.println("====方式一====");
        //静态内部类可以通过类名直接访问(遵循访问权限)
        Outer.Inner inner = new Outer.Inner();
        inner.test();
        System.out.println("====方式二====");
        //编写一个方法，可以返回静态内部类对象实例
        Outer.getInner().test();
    }
}

class Outer {
    private int n = 10;
    private static String name = "jxs";
    private static void test1() { System.out.println("外部类Outer的test1()方法"); }
    /*
     1、静态内部类是定义在外部类的成员位置，并且有static修饰
     3、静态内部类可以添加任意访问修饰符，因为它的地位就好比一个成员。
     */
    public static class Inner {
        private int n = 20;
        private static String name = "dwy";
        public void test() {
            /*
             2、静态内部类可以直接访问外部类的所有静态成员，包括私有的静态成员。
             8、若外部类和静态内部类的成员重名时，静态内部类访问时默认遵循就近原则。若想访问外部类的成员，则可以使用（外部类名.成员）去访问。
             */
            System.out.println("静态内部类name=" + name);
            System.out.println("静态内部类n=" + n);

            System.out.println("外部类name=" + Outer.name);
            test1();
        }
    }

    //6、外部类访问静态内部类的访问方式：创建对象实例再访问。
    public void test2() {
        Inner inner = new Inner();
        inner.test();
    }

    public static Inner getInner() {
        return new Inner();
    }
}

/*
输出结果：
外部其他类访问静态内部类的方式:
====方式一====
静态内部类name=dwy
静态内部类n=20
外部类name=jxs
外部类Outer的test1()方法
====方式二====
静态内部类name=dwy
静态内部类n=20
外部类name=jxs
外部类Outer的test1()方法
*/
1.2.2、枚举和注解
枚举
1、枚举是一组常量的集合

2、枚举为一种特殊的类，其中只包含一组有限的特定的对象

3、枚举的2种实现方式：

		（1）自定义类实现枚举

		（2）enum关键字实现枚举

自定义类实现枚举
1、不需要提供set方法，因为枚举类对象值通常为只读

2、对枚举类对象/属性提供final+static共同修饰，实现底层优化

3、枚举类对象名通常使用全部大写，常量的命名规范

4、枚举对象根据需要，也可以有多个属性

public class Eunumeration02 {
    public static void main(String[] args) {
        /*
         1、将构造器私有化，不可创建对象实例
         2、去除set相关方法，只可读不可修改
         3、在该类内部直接创建固定的对象
         4、重写父类Object类的toString方法，返回对象的属性信息。
         5、优化:为固定对象加入final修饰符
         */
        System.out.println(Season.SPRING);
    }
}

class Season{
    private String name;
    private String desc;

    public static Season SPRING = new Season("春","温暖");
    public static Season SUMMER = new Season("夏", "炎热");
    public static Season AUTUMN = new Season("秋", "凉爽");
    public static Season WINTER = new Season("冬", "寒冷");

    private Season(String name, String desc) {
        this.name = name;
        this.desc = desc;
    }

    public String getDesc() {
        return desc;
    }
    public void setDesc(String desc) {
        this.desc = desc;
    }

    @Override
    public String toString() {
        return "Season{" +
                "name='" + name + '\'' +
                ", desc='" + desc + '\'' +
                '}';
    }
}

/*
输出结果：Season{name='春', desc='温暖'}
*/
enum关键字实现枚举
public class Eunumeration03 {
    public static void main(String[] args) {
        System.out.println(Season.SPRING);
        System.out.println(Season.SUMMER);
        System.out.println(Season.AUTUMN);
        System.out.println(Season.WINTER);
    }
}

/*
 演示使用enum关键字来实现枚举类:
 1、使用关键字enum替代class
 2、常量名(实参列表)
 3、若有多个常量，使用 , 间隔
 4、若使用enum来实现枚举，要求将定义的常量对象写在前面
 */
enum Season {

    SPRING("春", "温暖"),
    SUMMER("夏", "炎热"),
    AUTUMN("秋", "凉爽"),
    WINTER("冬", "寒冷");
    private String name;
    private String desc;


    private Season(String name, String desc) {
        this.name = name;
        this.desc = desc;
    }

    public String getDesc() {
        return desc;
    }

    public void setDesc(String desc) {
        this.desc = desc;
    }

    @Override
    public String toString() {
        return "Season{" +
                "name='" + name + '\'' +
                ", desc='" + desc + '\'' +
                '}';
    }
}

/*
输出结果：
Season{name='春', desc='温暖'}
Season{name='夏', desc='炎热'}
Season{name='秋', desc='凉爽'}
Season{name='冬', desc='寒冷'}
*/
enum关键字实现枚举注意事项
1、当我们使用 enum 关键字开发一个枚举类时，默认会继承Enum类

1、E:\Software Development Kit\Maven\workspace\ZooKeeper\src\main\java\net\wanhe\enum_test目录下进入命令行模式

2、编译javac Eunumeration03.java

3、反编译javap Season.class得到:
Compiled from "Eunumeration03.java"
final class net.wanhe.enum_test.Season extends java.lang.Enum<net.wanhe.enum_test.Season> {
  public static final net.wanhe.enum_test.Season SPRING;
  public static final net.wanhe.enum_test.Season SUMMER;
  public static final net.wanhe.enum_test.Season AUTUMN;
  public static final net.wanhe.enum_test.Season WINTER;
  public static net.wanhe.enum_test.Season[] values();
  public static net.wanhe.enum_test.Season valueOf(java.lang.String);
  public java.lang.String getDesc();
  public void setDesc(java.lang.String);
  public java.lang.String toString();
  static {};
}
2、传统的public static final Season SPRING = new Season("春天","温暖");简化成SPRING("春天","温暖"),这里必须知道，它调用的是哪个构造器

3、如果使用无参构造器创建枚举对象，则实参列表和小括号都可以省略

4、若有多个常量，使用 , 间隔

5、枚举对象必须放在枚举类的行首

枚举类练习
1、

public class Eunumeration04 {
    public static void main(String[] args) {
        Gender boy = Gender.BOY;
        Gender boy1 = Gender.BOY;
        Gender gril = Gender.GRIL;
        /*
         本质调用了Gender的父类Enum的toSrting方法
         Enum的toString方法:
         public String toString() {
            return name;
         }
         */
        System.out.println(boy);
        System.out.println(boy == boy1);
        System.out.println(boy == gril);

    }
}

enum Gender{
    BOY,GRIL;

    Gender() { }
}

/*
输出结果：
BOY
true
false
*/
Enum常用方法
使用enum关键字时，会隐式的继承Enum类，因此我们就可以使用Enum类的相关方法。

public class EnumMethod {
    public static void main(String[] args) {
        Season spring = Season.SPRING;
        /*
         1、name:得到当前枚举常量的名称
         2、ordinal:得到当前枚举常量的次序，从0开始编号
         3、values:返回Season[]，含有定义的所有枚举对象。
         4、valueOf:传递枚举类型的Class对象和枚举常量名称给静态方法valueOf，会得到与参数匹配的枚举常量。
         5、compareTo:枚举类型实现了Comparable接口,比较两个枚举常量的大小（按照声明的顺序排列）。
         */
        System.out.println("name方法:");
        System.out.println(spring.name());
        
        System.out.println("ordinal方法:");
        System.out.println(spring.ordinal());
        
        System.out.println("values方法:");
        Season[] values = Season.values();
        //依次从Season数组中取出数据，赋值给season。取出完毕后，退出for循环
        for (Season season : values) {
            System.out.println(season);
        }
        
        System.out.println("valueOf方法:");
        //根据输入的内容到Season的枚举对象中去查找。查找到就返回这个枚举对象；反之报错
        System.out.println(Season.valueOf("SPRING"));
        
        System.out.println("compareTo方法:");
        /*
         1、将 Season.SPRING 枚举对象的编号和 Season.SUMMER 枚举对象的编号比较
         2、返回的是 Season.SPRING 枚举对象的编号 - Season.SUMMER 枚举对象的编号
         */
        System.out.println(Season.SPRING.compareTo(Season.SUMMER));
    }
}

enum Season {
    SPRING("春", "温暖"),
    SUMMER("夏", "炎热"),
    AUTUMN("秋", "凉爽"),
    WINTER("冬", "寒冷");
    private String name;
    private String desc;

    private Season(String name, String desc) {
        this.name = name;
        this.desc = desc;
    }

    public String getDesc() {
        return desc;
    }
    public void setDesc(String desc) {
        this.desc = desc;
    }

    @Override
    public String toString() {
        return "Season{" +
                "name='" + name + '\'' +
                ", desc='" + desc + '\'' +
                '}';
    }
}

/*
输出结果：
name方法:
SPRING
ordinal方法:
0
values方法:
Season{name='春', desc='温暖'}
Season{name='夏', desc='炎热'}
Season{name='秋', desc='凉爽'}
Season{name='冬', desc='寒冷'}
valueOf方法:
Season{name='春', desc='温暖'}
compareTo方法:
-1
*/
Enum练习
public class Test {
    public static void main(String[] args) {
        Week[] values = Week.values();
        System.out.println("所有的星期信息如下:");
        for (Week week : values) {
            System.out.println(week);
        }
    }
}

enum Week{
    MONDAY("星期一"),
    TUESDAY("星期二"),
    WEDNESDAY("星期三"),
    THURSDAY("星期四"),
    FRIDAY("星期五"),
    SATURDAY("星期六"),
    SUNDAY("星期天");
    private String name;

    private Week(String name) {
        this.name = name;
    }

    @Override
    public String toString() {
        return name;
    }
}

/*
输出结果：
所有的星期信息如下:
星期一
星期二
星期三
星期四
星期五
星期六
星期天
*/
Enum实现接口
1、使用enum关键字后，就不可以继承其他类，因为enum会隐式继承Enum。

2、枚举类和普通类一样，可以实现接口，格式如下：

enum 类名 implements 接口1,接口2 {}
注解理解
1、注解也被称为元数据，用于修饰解释 包、类、方法、属性、构造器、局部变量等数据信息。

2、注解和注释一样，注解不影响程序逻辑，但注解可以被编译或运行，相当于嵌入在代码中的补充信息。

3、在JavaSE中，注解的使用目的比较简单。例如：标记过时的功能，忽略警报等。

4、在JavaEE中，注解占据了更重要的角色。例如：用来配置应用程序的任何切面，代替JavaEE旧版中所遗留的繁冗代码和XML配置等。

JDK内置的基本注解类型
1、使用Annotation时要在其前面增加@符号，并将Annotation当成一个修饰符使用，用于修饰它支持的程序元素。

2、三个基本的Annotation：

		（1）@Override：限定某个方法，是重写父类方法，该注解只能用于方法。

		（2）@Deprecated：用于表示某个程序元素（类、方法等）已过时

		（3）@SuppressWarnings：抑制编译器警告

class Father {
    public void fly() { }
}

class Student extends Father {
    /*
     1、@Override，注解放在fly上，表示子类的fly方法重写了父类的fly方法
     2、若没有 @Override 注解，还是会重写父类的fly方法
     3、若写了 @Override 注解，编译器就会去检查是否真的重写了父类的fly方法
        若的确重写了则编译通过，反之则编译错误
     4、@Override源码
        @Target(ElementType.METHOD)
        @Retention(RetentionPolicy.SOURCE)
        public @interface Override {
        }
     5、解读:
        @interface表示一个注解类
        @Target(ElementType.METHOD) --> @Override只能修饰方法
        @Target --> 修饰注解的注解，称为元注解
     */
    @Override
    public void fly() {
        super.fly();
    }
    
    //@Override --> Method does not override method from its superclass
    public void say() {}
}
public class Deprecated_test {
    public static void main(String[] args) {
        A a = new A();
        System.out.println(a.n);
        a.test();
    }
}

/*
 解读：
 1、@Deprecated修饰某个元素，表示该元素已过时
 2、即不推荐使用，但是仍可以使用
 3、@Deprecated源码:
    @Documented
    @Retention(RetentionPolicy.RUNTIME)
    @Target(value={CONSTRUCTOR, FIELD, LOCAL_VARIABLE, METHOD, PACKAGE, PARAMETER, TYPE})
    public @interface Deprecated {
    }
 4、@Deprecated可以修饰方法、类、字段、包、参数 等等
 5、@Deprecated可以做版本升级过渡使用
 */
@Deprecated
class A {
    @Deprecated
    public int n = 10;
    @Deprecated
    public void test() {}
}
public class SuppressWarnings_test {
    /*
     @SuppressWarnings({""})解读:
     1、@SuppressWarnings抑制警告信息（不显示），在{""}中写入抑制信息
     2、@SuppressWarnings作用范围和你放置的位置相关
     3、@SuppressWarnings源码:
        @Target({TYPE, FIELD, METHOD, PARAMETER, CONSTRUCTOR, LOCAL_VARIABLE})
        @Retention(RetentionPolicy.SOURCE)
        public @interface SuppressWarnings {
            String[] value();
        }
     4、@SuppressWarnings注解类设置了一个数组来传递抑制信息
     */
    @SuppressWarnings({})
    public static void main(String[] args) {
        List list = new ArrayList();
        list.add("jxs");
    }
}
元注解：对注解进行注解
1、JDK的元Annotation用于修饰其他Annotation

2、元注解种类：

		（1）@Retention(指定注解的作用范围，三种SOURCE、CLASS、RUNTIME)

		（2）@Target(指定注解可以在哪些地方使用)

		（3）@Documented(指定该注解是否会在javadoc体现)

		（4）@Inherited(子类会继承父类注解)

3、@Retention注解：

只能用于修饰一个Annotation定义，用于指定该Annotation可以保留多长时间，@Retention包含一个RetentionPolicy类型的成员变量，使用@Retention时必须为该value成员变量指定值：

		（1）RetentionPolicy.SOURCE：编译器使用后直接丢弃这种策略的注释

		（2）RetentionPolicy.CLASS：编译器将注解记录在class文件中，当运行Java程序时，JVM不会保留注解。															  这是默认值。

		（3）RetentionPolicy.RUNTIME：编译器将注解记录在class文件中，当运行Java程序时，JVM会保留注解。

																	程序可以通过反射获取该注释。

4、@Target注解：

用于修饰Annotation定义，用于指定被修饰的Annotation能用于修饰哪些程序元素。

		（1）value

5、@Documented注解：

用于指定被该元Annotation修饰的Annotation类将被javadoc工具提取成文档，即生成文档时，可以看到该注解。定义为Documented的注解必须设置Retention值为RUNTIME。

6、@Inherited注解：

被该元Annotation修饰的Annotation类将具有继承性，其子类将自动拥有该注解。

1.2.3、Exception
try-catch快速入门
public class ExceptionTest {
    public static void main(String[] args) {
        /*
         1、执行到int result = n1 / n2会抛出ArithmeticException异常
         2、程序出现1个不致命问题就导致整个系统崩溃，因此Java设计者提供了异常处理机制来解决该问题
         3、若程序员认为一段代码可能出现异常问题，可以使用try-catch异常处理机制来解决，从而保证程序的健壮性
         4、选中代码块，Ctrl+Alt+T选中try/catch
         5、若进行异常处理，即使出现了异常，程序可以继续执行。
         */
        int n1 = 10;
        int n2 = 0;
        try {
            int result = n1 / n2;
        } catch (Exception e) {
            //输出异常信息
            System.out.println(e.getMessage());
        }
        System.out.println("程序继续运行");
    }
}
异常的概念
1、Java语言中，将程序执行中发生的不正常情况称为"异常"。

2、执行过程中所发生的异常事件可以分为两类：

		（1）Error（错误）：Java虚拟机无法解决的严重问题。如JVM系统内部错误、资源耗尽等严重情况

		（2）Exception（异常）：其他因编程原因错误或偶然的外在因素导致的一般性问题，可以使用针对性的代码进行处理。Exception分为两大类：运行时异常、编译时异常。

异常体系图
![](E:\Study\自学课程资料\Java\assets\异常体系图.png)

1、异常分为运行时异常、编译时异常

2、运行时异常，编译器检查不出。一般指编程时的逻辑错误，是程序员应该避免其出现的异常

3、运行时异常因为很普遍可以不做处理，若全处理可能会对程序的可读性和运行效率产生影响。

4、编译时异常，是编译器要求必须处理的异常。

常见运行时异常
1、NullPointerException（空指针异常）：当应用程序试图在需要对象的地方使用Null时抛出该异常

2、ArithmeticException（数学运算异常）：当出现异常的运算条件时，抛出此异常。

3、ArrayIndexOutOfBoundsException（数组下标越界异常）：用非法索引访问数组时抛出的异常。

4、ClassCastException（类型转换异常）：当试图将对象强制转换为不是实例的子类时抛出该异常。

5、NumberFormatException（数字格式不正确异常）：当应用程序试图将字符串转换成一种数值类型，但该字符串不能转换为适当格式时抛出该异常。

常见编译时异常
1、SQLException：操作数据库时查询表可能发生异常。

2、IOException：操作文件时发生的异常。

3、FileNotFoundException：当操作一个不存在的文件时发生的异常。

4、ClassNotFoundException：加载类但类不存在时发生的异常。

5、EOFException：操作文件时，到文件末尾发生异常。

异常处理机制
![](E:\Study\自学课程资料\Java\assets\异常处理机制图.png)

1、try-catch-finally

程序员在代码中捕获发生的异常，自行处理
try {
	//可能有异常的代码
} catch (Exception exception) {
	/*
	1、捕获到异常
	2、系统将异常封装成Exception对象exception，传递给catch
	3、得到异常对象后，程序员可以自己处理
	4、try代码块无异常发生，则catch代码块不执行
	*/
} finally {
	//不管try代码块是否有异常发生，始终要执行finally
}
2、throws

将发生的异常抛出，交给调用者处理，最顶级的处理者就是JVM
try-catch细节
1、Java提供try-catch块来处理异常。try块中用于包含可能出错的代码，catch块用于处理try块中发生的异常。

try {
	//可能有异常的代码
} catch (Exception exception) {
	//对异常的处理
}
2、若异常发生，则异常发生后面的代码不会执行，直接进入到catch块。

3、若异常没有发生，则顺序执行try代码块，不会进入到catch块。

4、若希望不管有无异常发生，都执行某段代码，则使用finally代码块。

public class ExceptionDetail {
    public static void main(String[] args) {
        //try-catch快捷键:Ctrl+Alt+T
        try {
            /*
             细节2:若异常发生，则异常发生后面的代码不会执行，直接进入到catch块;
             细节3:若异常没有发生，则顺序执行try代码块，不会进入到catch块。
             */
            String str = "蒋兴树";
            int i = Integer.parseInt(str);
            System.out.println("字符串转数字" + i);
        } catch (Exception exception) {
            System.out.println("异常信息" + exception.getMessage());
        } finally {
            //细节4:若希望不管有无异常发生，都执行某段代码，则使用finally代码块。
            System.out.println("finally代码块执行");
        }
    }
}

/*
输出结果：
异常信息For input string: "蒋兴树"
finally代码块执行
*/
5、可以有多个catch语句，捕获不同的异常，要求父类异常在后，子类异常在前，如果发生异常，只会匹配1个catch。

public class ExceptionDetail01 {
    public static void main(String[] args) {
        try {
            Person person = new Person();
            person = null;
            System.out.println(person.getName());//NullPointerException
            int n1 = 10;
            int n2 = 0;
            int result = n1 / n2;//ArithmeticException
            //细节5:可以有多个catch语句，捕获不同的异常，要求父类异常在后，子类异常在前，如果发生异常，只会匹配1个catch。
        } catch (NullPointerException e){
            System.out.println("空指针异常" + e.getMessage());
        } catch (ArithmeticException e){
            System.out.println("算术运算异常" + e.getMessage());
        }catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            System.out.println("执行finally代码块");
        }
    }
}

class Person {
    private String name = "jxs";

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
}

/*
输出结果：
空指针异常null
执行finally代码块
*/
6、可以进行try-finally配合使用，相当于没有捕获异常，因此程序会直接退出。应用场景：一段代码，不管是否发生异常，都必须执行某个业务逻辑。

try-catch练习
1、

public class ExceptionTest02 {
    public static void main(String[] args) {
        System.out.println(method());
    }

    public static int method() {
        try {
            String[] strings = new String[3];
            if (strings[1].equals("jxs")) {
                System.out.println(strings[1]);
            } else {
                strings[3] = "dwy";
            } return 1;
        } catch (ArrayIndexOutOfBoundsException e) {
            return 2;
        } catch (NullPointerException e) {
            return 3;
        } finally {
            return 4;
        }
    }
}

/*
输出结果：4
*/
2、

public class ExceptionTest02 {
    public static void main(String[] args) {
        System.out.println(method());
    }

    public static int method() {
        int i = 1;
        try {
            i++;
            String[] strings = new String[3];
            if (strings[1].equals("jxs")) {
                System.out.println(strings[1]);
            } else {
                strings[3] = "dwy";
            } return 1;
        } catch (ArrayIndexOutOfBoundsException e) {
            return 2;
        } catch (NullPointerException e) {
            return ++i;
        } finally {
            return ++i;
        }
    }
}

/*
输出结果：4
*/
3、

public class ExceptionTest02 {
    public static void main(String[] args) {
        System.out.println(method());
    }

    public static int method() {
        int i = 1;
        try {
            i++;
            String[] strings = new String[3];
            if (strings[1].equals("jxs")) {
                System.out.println(strings[1]);
            } else {
                strings[3] = "dwy";
            } return 1;
        } catch (ArrayIndexOutOfBoundsException e) {
            return 2;
        } catch (NullPointerException e) {
            return ++i;//i=3,保存临时变量temp=3
        } finally {
            ++i;
            System.out.println("i=" + i);
        }
    }
}

/*
输出结果：
i=4
3
*/
try-catch最佳实践
public class ExceptionTest02 {
    public static void main(String[] args) {
        method();
    }

    public static void method() {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            System.out.println("请输入一个整数");
            try {
                Integer.parseInt(scanner.next());
                break;
            } catch (NumberFormatException e) {
                System.out.println("输入的不是整数");
            }
        }
        System.out.println("循环结束");
    }
}
throws快速入门
1、若一个方法中可能生成某种异常，但是并不能确定如何处理这种异常，则此方法显示的声明抛出异常，表明该方法将不对这些异常进行处理，而由该方法的调用者进行处理。

2、在方法声明中用throws语句可以声明抛出异常的列表，throws后面的异常类型可以是方法中产生的异常类型，也可以是它的父类。

3、throws后面可以是异常列表，即可以抛出多个异常。

public class Thorws {
    public static void main(String[] args) {
        
    }

    /*
     1、创建文件流对象
     2、FileNotFoundException编译异常
     3、可以使用try-catch-finally解决或者throws抛出异常
     4、throws后面的异常类型可以是方法中产生的异常类型，也可以是它的父类。
     5、throws后面可以是异常列表，即可以抛出多个异常
     */
    public void method() throws FileNotFoundException,Exception{
        FileInputStream fileInputStream = new FileInputStream("E:\\Study\\自学课程资料\\Java\\java.md");
    }
}
throws使用细节
1、对于编译时异常，程序中必须采用try-catch-finally或throws处理

2、对于运行时异常，程序中若没有进行处理则默认以throws方式处理

3、子类重写父类的方法时，对抛出异常的规定：子类重写父类的方法抛出的异常和父类抛出的异常一致或是父类抛出的异常类型的子类型

4、在throws过程中，若有方法try-catch（相当于处理异常），则不必throws。

public class ThrowsDetail {
    /*
     1、method()方法不处理异常，选择将异常抛出
     2、main方法调用method()方法，选择不处理异常，将异常抛出
     3、JVM暴力处理异常信息:输出异常信息，退出程序。
     */
    public static void main(String[] args) throws ArithmeticException{
        method();
    }

    public static void method() throws ArithmeticException{
        /*
         细节1:对于编译时异常，程序中必须采用try-catch-finally或throws处理
         细节2:对于运行时异常，程序中若没有进行处理则默认以throws方式处理
         */
        int n1 = 1;
        int n2 = 0;
        int result = n1 / n2;
    }

    public static void f1() throws FileNotFoundException { }
    public static void f2() throws FileNotFoundException {
        //对于编译时异常，程序中必须采用try-catch-finally或throws处理
        f1();
    }

    public static void f3() throws ArithmeticException { }
    public static void f4() {
        //对于运行时异常，程序中若没有进行处理则默认以throws方式处理
        f3();
    }
}

class Father {
    public void method1() throws RuntimeException{}
}

class Son extends Father {
    /*
     细节3:子类重写父类的方法时，对抛出异常的规定：子类重写父类的方法抛出的异常和父类抛出的异常一致或是父类抛出的异常类型的子类型。
     细节4：在throws过程中，若有方法try-catch（相当于处理异常），则不必throws
     */
    @Override
    public void method1() throws NullPointerException { }
}
自定义异常
1、基本概念：当程序中出现某些错误，但错误信息没有在throwable子类中描述处理，这时可以自己设计异常类用于描述该错误信息。

2、自定义异常步骤：

定义类：自定义异常类名。若继承Exception则属于编译时异常；若继承RuntimeException则属于运行时异常。
public class CustomException {
    public static void main(String[] args) {
        Person01 person01 = new Person01("jxs",16);
        //要求年龄范围在18-120之间，否则抛出自定义异常
        if (person01.getAge() >= 18 && person01.getAge() <= 120) {
            System.out.println("年龄正常");
        } else {
            //通过自定义异常的构造器设置信息
            throw new AgeException("年龄需要在18-120之间");
        }
    }
}

class Person01 {
    private String name;
    private int age;

    public Person01(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}

/*
 自定义异常:
 1、一般情况下，我们自定义异常是继承RuntimeException
 2、好处:可以使用默认的处理机制
 */
class AgeException extends RuntimeException {
    //构造器
    public AgeException(String message) {
        super(message);
    }
}

/*
输出结果：
Exception in thread "main" net.wanhe.exception.AgeException: 年龄需要在18-120之间
	at net.wanhe.exception.CustomException.main(CustomException.java:11)
*/
throw和throws的对比
关键字	意义	位置	后面跟的内容
throws	异常处理的一种方式	方法声明处	异常类型
throw	手动生成异常对象的关键字	方法体中	异常对象
public class ThrowException {
    public static void main(String[] args) {
        try {
            ReturnException.methodA();
        } catch (RuntimeException e) {
            System.out.println(e.getMessage());
        }
        ReturnException.methodB();
    }
}

class ReturnException {
    static void methodA() {
        try {
            System.out.println("进入方法A");
            throw new RuntimeException("制造运行时异常");
        } finally {
            System.out.println("methodA方法的finally");
        }
    }

    static void methodB() {
        try {
            System.out.println("进入方法B");
            return;
        } finally {
            System.out.println("methodB方法的finally");
        }
    }
}

/*
输出结果：
进入方法A
methodA方法的finally
制造运行时异常
进入方法B
methodB方法的finally
*/
异常练习
1、

public class EcmDef {
    /*
     1、编写EcmDef程序，接收命令行两个参数，计算两数相除
     2、使用cal方法计算两数相除
     3、对数据格式不正确(NumberFormatException)、
     缺少命令行参数(ArrayIndexOutOfBoundsException)、
     算术运算(ArithmeticException)进行异常处理
     */
    public static void main(String[] args) {

        try {
            if (args.length != 2) {
                throw new ArrayIndexOutOfBoundsException("参数个数不符");
            }

            int n1 = Integer.parseInt(args[0]);
            int n2 = Integer.parseInt(args[1]);

            double result = cal(n1, n2);
            System.out.println("计算结果=" + result);

        } catch (ArrayIndexOutOfBoundsException arrayIndexOutOfBoundsException) {
            System.out.println(arrayIndexOutOfBoundsException.getMessage());
        } catch (NumberFormatException numberFormatException) {
            System.out.println("参数格式不正确，请输入整数");
        } catch (ArithmeticException arithmeticException) {
            System.out.println("算术运算异常");
        }
    }

    public static double cal(int n1, int n2) {
        return n1 / n2;
    }
}
2、

public class Homework {
    public static void main(String[] args) {
        try {
            method();
            System.out.println("A");
        } catch (Exception e) {
            System.out.println("C");
        }
        System.out.println("D");
    }

    public static void method() {
        try {
            throw new RuntimeException();
        } finally {
            System.out.println("B");
        }
    }
}

/*
输出结果：
B
C
D
*/
1.2.4、常用类
包装类
包装类概念：针对8种基本数据类型相应的引用类型

基本数据类型	包装类
byte	Byte
short	Short
int	Integer
long	Long
float	Float
double	Double
char	Character
boolean	Boolean
包装类	解析
Byte	Byte 类将基本类型 byte 的值包装在一个对象中。
Short	Short 类在对象中包装基本类型 short 的值。
Integer	Integer 类在对象中包装了一个基本类型 int 的值。
Long	Long 类在对象中包装了基本类型 long 的值。
Float	Float 类在对象中包装一个基本类型 float 的值。
Double	Double 类在对象中包装一个基本类型 double 的值。
Character	Character 类在对象中包装一个基本类型 char 的值。
Boolean	Boolean 类将基本类型为 boolean 的值包装在一个对象中。
1、Boolean包装类体系图

![](E:\Study\自学课程资料\Java\assets\Boolean包装类体系图.png)

2、  Character包装类体系图

![](E:\Study\自学课程资料\Java\assets\Character包装类体系图.png)

3、Byte、Short、Integer、Long、Float、Double包装类体系图

![](E:\Study\自学课程资料\Java\assets\Byte、Short、Integer、Long、Float、Double包装类体系图.png)

包装类与基本数据类型的转换
1、JDK5之前手动装箱和拆箱方式。装箱：基本类型类型 --> 包装类；拆箱：包装类 --> 基本类型类型。

2、JDK5之后自动装箱和拆箱方式。

3、自动装箱拆箱底层调用的是valueOf方法。

public class Integer01 {
    public static void main(String[] args) {
        //JDK5之前手动装箱和拆箱方式:
        int n1 = 100;
        //装箱
        Integer integer = new Integer(n1);
        //拆箱
        int i = integer.intValue();


        //JDK5之后自动装箱和拆箱方式:
        int n2 = 200;
        //装箱,底层使用的是Integer valueOf(int n2),
        //valueOf(int i):返回一个表示指定的 int 值的 Integer 实例。
        Integer integer1 = n2;
        //拆箱,底层使用的是intValue()
        int n3 = integer1;
    }
}
包装类练习
public class WrapperExercise01 {
    public static void main(String[] args) {
        //三元运算符是一个整体
        Object object = true ? new Integer(1) : new Double(2.0);
        System.out.println(object);

        Object object02;
        if (true) {
            object02 = new Integer(1);
        } else {
            object02 = new Double(2.0);
        }
        System.out.println(object02);
    }
}

/*
输出结果：
1.0
1
*/
包装类与String类型的转换
public class Wrapper_String {
    //包装类转换为String
    Integer i = 100;//自动装箱
    //方式1:
    String str = i + "";
    //方式2:
    String str1 = i.toString();
    //方式3:
    String str2 = String.valueOf(i);
    
    //String转换为包装类
    String str3 = "12345";
    //方式1:
    Integer i2 = Integer.parseInt(str3);//自动装箱
    //方式2:
    Integer i3 = new Integer(str3);
}

/*
输出结果：
100
100
100
12345
12345
*/
Integer创建机制
public class WrapperExercise02 {
    public static void main(String[] args) {
        Integer integer = new Integer(1);
        Integer integer1 = new Integer(2);
        System.out.println(integer == integer1);

        /*
         1、Integer包装类valueOf:返回一个表示指定的int值的Integer实例。
         2、Integer包装类valueOf源码:
         public static Integer valueOf(int i) {
            if (i >= IntegerCache.low && i <= IntegerCache.high)
                return IntegerCache.cache[i + (-IntegerCache.low)];
            return new Integer(i);
         }
         3、源代码解析:在-128~127范围内直接从数组返回,在-128~127范围外则创建一个Integer对象实例
         */
        Integer m = 1;
        Integer n = 1;
        System.out.println(m == n);

        Integer a = 128;
        Integer b = 128;
        System.out.println(a == b);
    }
}

/*
输出结果：
false
true
false
*/
Integer面试题
public class WrapperExercise03 {
    public static void main(String[] args) {
        Integer integer = new Integer(127);
        Integer integer1 = new Integer(127);
        System.out.println(integer == integer1);

        Integer integer2 = new Integer(128);
        Integer integer3 = new Integer(128);
        System.out.println(integer2 == integer3);

        //将已经创建好的Integer对象地址赋给integer4、integer5
        Integer integer4 = 127;
        Integer integer5 = 127;
        System.out.println(integer4 == integer5);

        //在-128~127范围外则创建一个Integer对象实例
        Integer integer6 = 128;
        Integer integer7 = 128;
        System.out.println(integer6 == integer7);

        Integer integer8 = 127;
        Integer integer9 = new Integer(128);
        System.out.println(integer8 == integer9);

        //只要存在基本数据类型，则判断的是值是否相等
        Integer integer10 = 127;
        int integer11 = 127;
        System.out.println(integer10 == integer11);

        Integer integer12 = 128;
        int integer13 = 128;
        System.out.println(integer12 == integer13);
    }
}

/*
输出结果：
false
false
true
false
false
true
true
*/
String结构剖析
<img src="E:\Study\自学课程资料\Java\assets\String类体系图.png" style="zoom:80%;" />

1、String对象用于保存字符串，也就是一组字符序列

2、字符串常量对象是用双引号括起来的字符序列。

3、字符串的字符使用Unicode字符编码，一个字符（不区分字母、汉字）占两个字节。

4、String类存在很多构造器，即构成构造器重载，String类较常用的构造方法：

		（1）String str = new String();

		（2）String str = new String(String original);

		（3）String str = new String(char[] a);

		（4）String str = new String(char[] a,int startIndex,int count);

5、String类实现了Serializable、Comparable接口，可以串行化（网络传输）、String对象可以比较。

6、String是final类，不可被其它类继承

7、String中有属性private final char value[];用于存放字符串内容。

8、value[] 是一个final类型，地址不可以修改。value[]不可指向新的地址，但是单个字符内容是可以变化的。

public class String01 {
    public static void main(String[] args) {
        final char value[] = {'a','b','c'};
        char value1[] = {'d','e','f'};
        value[0] = 'H';
        //value = value1;不可修改value地址
    }
}
String创建方式剖析
1、创建String对象的两种方式

		方式一：直接赋值 String s = "jxs";

		方式二：调用构造器 String s = new String("jxs");

2、区别

		方式一：先从常量池中查看是否有"jxs"数据空间，若有则直接指向；若没有则重新创建，然后指向。s最终指向的是常量池的空间地址。

		方式二：先在堆中创建空间，里面维护了value属性，指向常量池的jxs空间，若常量池中没有"jxs"则重新创建；若有，则直接通过value指向。s最终指向的是堆中的空间地址。

3、String创建方式内存图

<img src="E:\Study\自学课程资料\Java\assets\String创建方式内存图.png" style="zoom:80%;" />

String练习
public class StringExercise {
    public static void main(String[] args) {
        String a = "jxs"; //a指向常量池的"jxs"
        String b = new String("jxs"); //b指向堆中的对象
        System.out.println(a.equals(b));
        System.out.println(a == b);
        /*
         当调用intern方法时
         若常量池中已经包含一个等于此String对象的字符串(用equals(Object)方法确定)则返回池中的字符串
         否则将此String对象添加到池中，并返回此String对象的引用。
         总而言之即intern()方法最终返回的是常量池的地址(对象)。
         */
        System.out.println(a == b.intern());
        //b指向堆中对象的地址，b.intern()指向的是常量池"jxs"的地址
        System.out.println(b == b.intern());
    }
}

/*
输出结果：
true
false
true
false
*/
public class StringExercise01 {
    public static void main(String[] args) {
        Person person1 = new Person();
        person1.name = "jxs";
        Person person2 = new Person();
        person2.name = "jxs";
        System.out.println(person1.name.equals(person2.name));
        System.out.println(person1.name == person2.name);
        System.out.println(person1.name == "jxs");

        String s1 = new String("abcd");
        String s2 = new String("abcd");
        System.out.println(s1 == s2);
    }
}

class Person {
    public String name;
}

/*
输出结果：
true
true
true
false
*/
String对象特性
public class StringExercise02 {
    public static void main(String[] args) {
        //创建了两个对象
        String s1 = "jxs";
        s1 = "dwy";

        //创建了一个对象。编译器优化String s2 = "jxsdwy"
        String s2 = "zls" + "wgw";

        String s3 = "lxz";
        String s4 = "yj";
        /*
         1、创建一个StringBuilder sb = StringBuilder()
         2、执行sb.append("lxz")
         3、执行sb.append("yj")
         4、String s5 = sb.toString()
         5、重要规则:常量相加看常量池;变量相加看堆
         */
        String s5 = s3 + s4;
        String s6 = "lxz" + "yj";
        String s7 = "lxzyj";
        System.out.println(s5 == s7);
        System.out.println(s6 == s7);
    }
}

/*
输出结果：
false
true
*/
public class StringExercise03 {
    public static void main(String[] args) {
        String s1 = "jxs";//指向常量池"jxs"
        String s2 = "dwy";//指向常量池"dwy"
        String s3 = "jxsdwy";//指向常量池"jxsdwy"

        String s4 = (s1 + s2).intern();//指向常量池"jxsdwy"
        System.out.println(s3 == s4);
        System.out.println(s3.equals(s4));
    }
}

/*
输出结果：
true
true
*/
String对象特性难题
public class String02 {

    String s = new String("jxs");
    final char[] chars = {'d','w','y'};

    public void change(String s,char[] chars) {
        s = "java";
        chars[0] = 'h';
    }

    public static void main(String[] args) {
        String02 string02 = new String02();
        string02.change(string02.s, string02.chars);
        System.out.println(string02.s + "and");
        System.out.println(string02.chars);
    }
}

/*
输出结果：
jxsand
hwy
*/
![](E:\Study\自学课程资料\Java\assets\String对象特性内存图.png)

String常用方法
public class StringMethod {

    public static void main(String[] args) {
        //charAt(int index) 返回指定索引处的 char 值
          
        //equals 区分大小写，判断内容是否相等
        String s1 = "jxs";
        String s2 = "Jxs";
        System.out.println(s1.equals(s2));

        //equalslgnoreCase 不区分大小写，判断内容是否相等
        System.out.println(s1.equalsIgnoreCase(s2));

        //length 获取字符个数，字符串长度
        System.out.println(s1.length());

        //indexOf 获取字符在字符串中第一次出现的索引，索引从0开始，若找寻不到返回-1
        String s3 = "@123@123";
        System.out.println(s3.indexOf('@'));
        System.out.println(s3.indexOf('4'));
        System.out.println(s3.indexOf("@123"));

        //lastIndexOf 获取字符在字符串中最后一次出现的索引，索引从0开始，若找寻不到返回-1
        System.out.println(s3.lastIndexOf('@'));
        System.out.println(s3.lastIndexOf('4'));
        System.out.println(s3.lastIndexOf("@123"));

        //substring 截取指定范围的子串，左闭右开
        String name = "jxsdwy666";
        //从索引6开始截取后面的内容
        System.out.println(name.substring(6));
        //截取索引0-5的字符
        System.out.println(name.substring(0, 5));

        //toUpperCase 转换成大写
        String s4 = "jxsJXS";
        System.out.println(s4.toUpperCase());

        //toLowerCase 转换成小写
        System.out.println(s4.toLowerCase());

        //concat 拼接字符串
        String name1 = "张林森";
        String name2 = "王国伟";
        String play = "在一起";
        String test = name1.concat(name2).concat(play);
        System.out.println(test);

        //replace 替换字符串中的字符。将字符串中所有的 在 替换为 不在
        System.out.println(test.replace("在", "不在"));

        //split 分割字符串
        String poem = "锄禾日当午,汗滴禾下土,谁之盘中餐,粒粒皆辛苦";
        String[] split = poem.split(",");
        for (int i = 0; i < split.length; i++) {
            System.out.println(split[i]);
        }
        //在对字符串进行分割时，若有特殊字符需加入转义字符\
        String field = "E:\\java笔记\\java.md";
        String[] split1 = field.split("\\\\");
        for (int i = 0; i < split1.length; i++) {
            System.out.println(split1[i]);
        }

        //toCharArray 将字符串转换为字符数组
        String s5 = "happy";
        char[] chars = s5.toCharArray();
        for (int i = 0; i < chars.length; i++) {
            System.out.println(chars[i]);
        }

        //compareTo 比较两个字符串的字典顺序。若前者大返回正数;若前者小返回负数;相等返回0
        String s6 = "jack";
        String s7 = "tom";
        String s8 = "simo";
        System.out.println(s6.compareTo(s7));
        System.out.println(s7.compareTo(s8));
        System.out.println(s6.compareTo(s8));

        /*
         1、format 格式字符串
         2、占位符:%s(字符串) %c(字符) %d(整型) %.2f(浮点型)
         */
        String name3 = "蒋兴树";
        int age = 21;
        double score = 100.0;
        char gender = '男';
        String info = "姓名" + name3 + "\n"
                + "年龄" + age + "\n"
                + "分数" + score + "\n"
                + "性别" + gender;
        System.out.println(info);

        /*
         1、这些占位符用后面的变量来替换
         2、%s 表示后面用 字符串 来替换
         3、%d 用 整数 来替换
         4、%.2f 用 小数 来替换，替换后只会保留小数点两位(四舍五入)
         5、%c 用 char 类型替换
         */
        String formatstr = "我的姓名是%s 年龄是%d 分数是%.2f 性别是%c";
        String format = String.format(formatstr, name3, age, score, gender);
        System.out.println(format);
    }
}

/*
输出结果：
false
true
3
0
-1
0
4
-1
4
666
jxsdw
JXSJXS
jxsjxs
张林森王国伟在一起
张林森王国伟不在一起
锄禾日当午
汗滴禾下土
谁之盘中餐
粒粒皆辛苦
E:
java笔记
java.md
h
a
p
p
y
-10
1
-9
姓名蒋兴树
年龄21
分数100.0
性别男
我的姓名是蒋兴树 年龄是21 分数是100.00 性别是男
*/
StringBuffer
1、可变的字符序列，可以对字符串内容进行增删

2、很多方法与String相同

3、StringBuffer是一个容器

![](E:\Study\自学课程资料\Java\assets\StringBuffer体系图.png)

4、String VS StringBuffer

		（1）String保存的是字符串常量，字符串内容不可修改，每次String的更新实际为更改地址。String字符串内容存放在private final char value[]。

		（2）StringBuffer保存的是字符串变量，字符串内容可以修改，每次StringBuffer的更新实际为更新内容，不需每次更新地址。StringBuffer字符串内容存放在char[] value。

		（3）StringBuffer效率高于String

public class StringBuffer01 {
    public static void main(String[] args) {
        /*
         1、StringBuffer 的直接父类为 AbstractStringBuilder
         2、StringBuffer 实现了 Serializable 接口，即StringBuffer对象可以串行化
         3、在父类 AbstractStringBuilder 中有属性 char[] value ，不为final类型
         4、char[] value 存放字符串内容，存放在堆中
         5、StringBuffer 是一个 final 类，不可被继承
         6、因为StringBuffer字符串内容存放在 char[] value，删除时不需要每次都更新地址（创建新对象）
         */
        StringBuffer stringBuffer = new StringBuffer();
    }
}
StringBuffer构造器
public class StringBuffer02 {
    public static void main(String[] args) {

        /*
         StringBuffer构造器:
         1、创建一个大小为 16 的 char[] , 用于存在字符串内容
         */
        StringBuffer stringBuffer = new StringBuffer();

        //2、通过构造器指定 char[] 大小
        StringBuffer stringBuffer1 = new StringBuffer(16);

        //3、通过给一个 字符串 创建 StringBuffer，char[]大小是 "jxs".length + 16
        StringBuffer stringBuffer2 = new StringBuffer("jxs");
    }
}
String和StringBuffer转换
public class StringBuffer03 {
    public static void main(String[] args) {

        /*
         String --> StringBuffer
         1、返回的 stringBuffer 才是 StringBuffer类 的对象，对 str 本身无影响
         2、方式一:使用构造器
         */
        String str = "hello jxs";
        StringBuffer stringBuffer = new StringBuffer(str);

        //方式二:使用append方法
        StringBuffer stringBuffer1 = new StringBuffer().append(str);


        /*
         StringBuffer --> String
         方式一:使用StringBuffer提供的toString方法
         */
        String s = new StringBuffer().toString();

        //方式二:使用构造器
        String s1 = new String(new StringBuffer());
    }
}
StringBuffer常用方法
public class StringBufferMethod {
    public static void main(String[] args) {
        StringBuffer stringBuffer = new StringBuffer("hello");
        stringBuffer.append(',');
        stringBuffer.append("蒋兴树");
        stringBuffer.append("丁维一").append(100).append(true).append(10.5);
        System.out.println(stringBuffer);
        
        //删除 11<=索引<14 处的字符
        stringBuffer.delete(10,14);
        System.out.println(stringBuffer);

        //使用字符串 森宝宝 替换 10<=索引<14 处的字符
        stringBuffer.replace(10,14,"森宝宝");
        System.out.println(stringBuffer);

        //查找指定子字符串第一次出现的索引
        System.out.println(stringBuffer.indexOf("森宝宝"));

        //在索引为10的位置插入字符串"帅哥",原索引为10的内容自动后移
        System.out.println(stringBuffer.insert(10,"帅哥"));

        //长度
        System.out.println(stringBuffer.length());
    }
}

/*
输出结果：
hello,蒋兴树丁维一100true10.5
hello,蒋兴树丁0true10.5
hello,蒋兴树丁森宝宝e10.5
10
hello,蒋兴树丁帅哥森宝宝e10.5
20
*/
StringBuffer练习
public class StringBufferExercise01 {
    public static void main(String[] args) {
        String str = null;
        StringBuffer stringBuffer = new StringBuffer();
        //底层调用AbstractStringBuilder 的 appendNull()方法
        System.out.println(stringBuffer.append(str));
        System.out.println(stringBuffer.length());

        StringBuffer stringBuffer1 = new StringBuffer(stringBuffer);
        System.out.println(stringBuffer1);
    }
}

/*
输出结果：
null
4
null
*/
public class StringBufferExercise02 {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("请输入商品名称");
        String name = scanner.next();
        System.out.println("请输入商品价格");
        String price = scanner.next();
        StringBuffer stringBuffer = new StringBuffer(price);

        //2000 stringBuffer.length()=4 索引3 2,000
        for (int i = stringBuffer.length() - 3; i > 0; i -= 3) {
            stringBuffer.insert(i,",");
        }
        System.out.println("商品名称:" + name + "\n"
                + "商品价格:" + stringBuffer);
    }
}

/*
输出结果：
请输入商品名称
手机
请输入商品价格
888888888888888
商品名称:手机
商品价格:888,888,888,888,888
*/
StringBuilder
1、一个可变的字符序列。此类提供一个与StringBuffer兼容的API，但不保证同步（StringBuilder不是线程安全）。该类被设计用作StringBuffer的简易替换，用在字符串缓冲区被单个线程使用的时候。建议优先使用该类，因大多数实现中，StringBuilder比StringBuffer更快。

2、在StringBuilder上主要操作的是append和insert方法，可重载这些方法以接受任意类型的数据。

public class StringBuilder01 {
    public static void main(String[] args) {
        /*
        1、StringBuilder 继承 AbstractStringBuilder 类
        2、StringBuilder 实现了 Serializable 接口，即StringBuilder对象可以串行化
        3、StringBuilder 是一个 final 类，不可被继承
        4、StringBuilder字符串内容存放在 父类 AbstractStringBuilder类 的 char[] value 中。
        5、StringBuilder的方法没有做互斥处理，即没有 synchronized关键字，因此在单线程时使用
         */
        StringBuilder stringBuilder = new StringBuilder();
    }
}
String、StringBuffer、StringBuilder区别
1、StringBuffer和StringBuilder类似，代表可变字符序列，且方法一样

2、String：不可变字符序列，效率低，复用性高

3、StringBuffer：可变字符序列，效率较高，线程安全

4、StringBuilder：可变字符序列，效率最高，线程不安全

5、若我们要对String做大量修改，不要使用String。

public class StringVSStringBufferVSStringBuilder {
    public static void main(String[] args) {
        String s = "";
        StringBuffer stringBuffer = new StringBuffer("");
        StringBuilder stringBuilder = new StringBuilder("");
        long startTime = System.currentTimeMillis();
        for (int i = 0; i < 50000; i++) {
            stringBuffer.append(String.valueOf(i));
        }
        long endTime = System.currentTimeMillis();
        System.out.println("StringBuffer执行时间：" + (endTime - startTime));

        
        long startTime01 = System.currentTimeMillis();
        for (int i = 0; i < 50000; i++) {
            stringBuilder.append(String.valueOf(i));
        }
        long endTime01 = System.currentTimeMillis();
        System.out.println("StringBuilder执行时间：" + (endTime01 - startTime01));

        
        long startTime02 = System.currentTimeMillis();
        for (int i = 0; i < 50000; i++) {
            s = s + i;
        }
        long endTime02 = System.currentTimeMillis();
        System.out.println("String执行时间：" + (endTime02 - startTime02));
    }
}
结论：

（1）若字符串存在大量修改操作，一般使用StringBuffer、StringBuilder

（2）若字符串存在大量修改操作，并在单线程情况下，使用StringBuilder

（3）若字符串存在大量修改操作，并在多线程情况下，使用StringBuilder

（4）若字符串存在少量修改操作，并被多个对象引用，使用String。

Math
public class MathMethod {
    public static void main(String[] args) {
        //abs 绝对值
        System.out.println(Math.abs(-9));

        //pow 求幂
        System.out.println(Math.pow(3.5,4));

        //ceil 向上取整，返回大于等于该参数的最小整数
        System.out.println(Math.ceil(4.4));
        System.out.println(Math.ceil(-3.4));

        //floor 向下取整，返回小于等于该参数的最大整数
        System.out.println(Math.floor(-3.4));
        System.out.println(Math.floor(4.4));

        //round 四舍五入
        System.out.println(Math.round(-4.45));

        //sqrt 求开方
        System.out.println(Math.sqrt(16.0));

        //random 求随机数，返回的是[0,1)之间的一个随机小数
        System.out.println((int)(Math.random() * 5 + 2));

        //max min 返回最大值、最小值
        System.out.println(Math.max(500,300));
        System.out.println(Math.min(400,300));
    }
}

/*
输出结果：
9
150.0625
5.0
-3.0
-4.0
4.0
-4
4.0
3
500
300
*/
Arrays常用方法（重要）
public class ArrayMethod {
    public static void main(String[] args) {
        /*
         1、toString 返回数组的字符串形式
            (1)老办法 for循环遍历数组
            (2)新办法 Arrays类toString方法
         */
        Integer[] integers = {10, 20, 30};
        //for循环遍历数组
        for (int i = 0; i < integers.length; i++) {
            System.out.println(integers[i]);
        }
        //Arrays类toString方法
        System.out.println(Arrays.toString(integers));


        
        /*
         2、sort排序(自然排序、定制排序)
            (1)老办法 冒泡排序
            (2)新办法 Arrays类sort方法
         */
        //冒泡排序
        int[] array = {1,3,2,5,4,8,7,9,6};
        ArrayMethod.bubbleSort(array);

        //Arrays类sort方法默认排序
        Integer[] integers1 = {1,3,2,5,4,8,7,9,6};
        Arrays.sort(integers1);
        System.out.println("\n" + Arrays.toString(integers1));

        /*
         Arrays类sort方法定制排序，通过传入Comparator实现定制排序，实现了Comparator接口的匿名内部类
         1、体现接口编程的方式
         2、追溯源码
            采用二叉排序(binarySort)，在binarySort方法底层，通过匿名内部类的compare方法决定排序顺序
                while (left < right) {
                    int mid = (left + right) >>> 1;
                    if (c.compare(pivot, a[mid]) < 0)
                        right = mid;
                    else
                        left = mid + 1;
                }
                assert left == right;
         3、源码分析
            (1)Arrays.sort(integers2, new Comparator()
            (2)private static <T> void binarySort(T[] a, int lo, int hi, int start,
                                       Comparator<? super T> c) {
            (3)执行到binarySort方法的代码，会根据动态绑定执行c.compare()执行我们传入的
               匿名内部类的compare()方法
                while (left < right) {
                    int mid = (left + right) >>> 1;
                    if (c.compare(pivot, a[mid]) < 0)
                        right = mid;
                    else
                        left = mid + 1;
                }
                assert left == right;
            (4) public int compare(Object o1, Object o2) {
                    Integer n1 = (Integer) o1;
                    Integer n2 = (Integer) o2;
                    return n1 - n2;
                }
            (5)该方法public int compare(Object o1, Object o2) {} 返回值>0、<0会影响整个排序结果。
         */
        Integer[] integers2 = {1,3,2,5,4,8,7,9,6};
        /*
         1、基于接口的匿名内部类:匿名内部类:new 接口(参数列表){类体}
         2、编译类型 Comparator、运行类型 ArrayMethod$1
         3、JDK底层在创建匿名内部类 ArrayMethod$1 后
            立即创建了 ArrayMethod$1 的对象实例，并将地址返回
         4、匿名内部类使用一次后就不再使用。
         5、自己总结:基于接口的匿名内部类，一个类实现了一个接口，创建了一个对象实例
                   并将对象实例的地址返回给匿名内部类，不显示类名。这就是匿名内部类
         */
        Arrays.sort(integers2, new Comparator() {
                    @Override
                    public int compare(Object o1, Object o2) {
                        Integer n1 = (Integer) o1;
                        Integer n2 = (Integer) o2;
                        return n1 - n2;
                    }
                });
        System.out.println(Arrays.toString(integers2));
    }

    
    
    //冒泡排序方法
    public static void bubbleSort ( int[] array){
        //控制比较轮次，一共 n-1 轮
        for (int i = 0; i < array.length - 1; i++) {
            //控制两个挨着的元素进行比较
            for (int j = 0; j < array.length - 1 - i; j++) {
                if (array[j] > array[j + 1]) {
                    int temp = array[j];
                    array[j] = array[j + 1];
                    array[j + 1] = temp;
                }
            }
        }
        for (int i = 0; i < array.length; i++) {
            System.out.print(array[i]);
        }
    }
}

/*
输出结果：
10
20
30
[10, 20, 30]
123456789
[1, 2, 3, 4, 5, 6, 7, 8, 9]
[1, 2, 3, 4, 5, 6, 7, 8, 9]
*/
Arrays模拟排序
public class ArraySortCustom {
    public static void main(String[] args) {
        int[] arr = {1, -1, 8, 0, 20};
        bubble(arr);

        bubble01(arr, new Comparator() {
            @Override
            public int compare(Object o1, Object o2) {
                /*
                 1、向下转型 Integer integer = (Integer) o1
                 2、拆箱 int n1 = integer
                 */
                int n1 = (Integer) o1;
                int n2 = (Integer) o2;
                return n2 - n1;
            }
        });
    }

    //冒泡排序
    public static void bubble(int[] array) {
        for (int i = 0; i < array.length - 1; i++) {
            for (int j = 0; j < array.length - 1 - i; j++) {
                if (array[j] > array[j + 1]) {
                    int temp = array[j];
                    array[j] = array[j + 1];
                    array[j + 1] = temp;
                }
            }
        }
        System.out.println(Arrays.toString(array));
    }

    //综合冒泡+定制排序
    public static void bubble01(int[] array, Comparator c) {
        for (int i = 0; i < array.length - 1; i++) {
            for (int j = 0; j < array.length - 1 - i; j++) {
                //数组的排序由compare(array[j], array[j + 1])返回的值决定
                if (c.compare(array[j], array[j + 1]) > 0) {
                    int temp = array[j];
                    array[j] = array[j + 1];
                    array[j + 1] = temp;
                }
            }
        }
        System.out.println(Arrays.toString(array));
    }
}

/*
输出结果：
[-1, 0, 1, 8, 20]
[20, 8, 1, 0, -1]
*/
Arrays其他方法
public class ArrayMethod01 {
    public static void main(String[] args) {
        /*
         binarySearch 通过二分搜索法进行查找，要求必须排好序
         1、使用 binarySearch 二叉查找要求该数组是有序的，若数组无序则不可使用 binarySearch。
         2、若数组中不存在该元素则返回 return -(low + 1)
         */
        Integer[] integers = {1, 3, 5, 7, 9, 11, 13, 15};
        System.out.println(Arrays.binarySearch(integers, 8));
        System.out.println(Arrays.binarySearch(integers, 2));

        /*
         copyOf 数组元素的复制
         1、从 integers数组 中拷贝 20个元素 到 integers1数组中
         2、若拷贝的长度大于 integers.length ,则在新数组后用 null 补齐
         3、若拷贝的长度小于 0 ,则返回异常
         */
        Integer[] integers1 = Arrays.copyOf(integers, 20);
        System.out.println(Arrays.toString(integers1));

        /*
         fill 数组填充
         1、使用 100 去填充 integers2数组 , 替换所有元素
         */
        Integer[] integers2 = {9, 10, 2};
        Arrays.fill(integers2, 100);
        System.out.println(Arrays.toString(integers2));

        /*
         equals 比较两个数组元素内容是否完全一致
         1、若两个数组元素内容完全一致,返回true;反之false
         */
        Integer[] integers3 = {1, 2, 3};
        Integer[] integers4 = {1, 2, 3};
        boolean equals = Arrays.equals(integers3, integers4);
        System.out.println(equals);

        /*
         asList 将一组值，转换成list
         1、将(1, 3, 5, 6, 7, 8, 9)这组数据转换成一个List集合
         2、编译类型 List接口 , 运行类型 class java.util.Arrays$ArrayList
         */
        List<Integer> asList = Arrays.asList(1, 3, 5, 6, 7, 8, 9);
        System.out.println(asList);
    }
}

/*
输出结果：
-5
-2
[1, 3, 5, 7, 9, 11, 13, 15, null, null, null, null, null, null, null, null, null, null, null, null]
[100, 100, 100]
true
[1, 3, 5, 6, 7, 8, 9]
*/
Arrays练习
自定义Book类，包含name、price属性。

使用定制排序按照price从小到大、书名从短到长排序

1、自己写的版本

public class ArrayExercise {
    public static void main(String[] args) {
        Book[] books = new Book[4];
        books[0] = new Book("红楼梦",50);
        books[1] = new Book("三国演义",60);
        books[2] = new Book("假如给我三天光明",70);
        books[3] = new Book("三体",80);

        Book.test(books, new Comparator() {
            @Override
            public int compare(Object o1, Object o2) {
                int d1 = (int) o1;
                int d2 = (int) o2;
                return d1 - d2;
            }
        });
        for (int i = 0; i < books.length; i++) {
            System.out.println(books[i].price);
        }

        Book.test1(books, new Comparator() {
            @Override
            public int compare(Object o1, Object o2) {
                int d1 = (int) o1;
                int d2 = (int) o2;
                return d1 - d2;
            }
        });
        for (int i = 0; i < books.length; i++) {
            System.out.println(books[i].name);
        }
    }
}

class Book {
    String name;
    int price;

    public Book(String name, int price) {
        this.name = name;
        this.price = price;
    }

    public static void test(Book[] books, Comparator comparator) {
        for (int i = 0; i < books.length - 1; i++) {
            for (int j = 0; j < books.length - 1 - i; j++) {
                if (books[j].price > books[j + 1].price) {
                    int temp = books[j].price;
                    books[j].price = books[j + 1].price;
                    books[j + 1].price = temp;
                }
            }
        }
    }

    public static void test1(Book[] books, Comparator comparator) {
        for (int i = 0; i < books.length - 1; i++) {
            for (int j = 0; j < books.length - 1 - i; j++) {
                if ((books[j].name).length() > (books[j + 1].name).length()) {
                    String temp = books[j].name;
                    books[j].name = books[j + 1].name;
                    books[j + 1].name = temp;
                }
            }
        }
    }
}

/*
输出结果：
50
60
70
80
三体
红楼梦
三国演义
假如给我三天光明
*/
2、老师写的版本

public class ArrayExercise {
    public static void main(String[] args) {
        Book[] books = new Book[4];
        books[0] = new Book("红楼梦", 60);
        books[1] = new Book("三国演义", 50);
        books[2] = new Book("假如给我三天光明", 80);
        books[3] = new Book("三体", 70);

        //price从低到高
        Arrays.sort(books, new Comparator() {
            //对books数组进行排序，因此 o1、o2 就是 Book对象
            @Override
            public int compare(Object o1, Object o2) {
                Book b1 = (Book) o1;
                Book b2 = (Book) o2;
                return (int) (b1.getPrice() - b2.getPrice());
            }
        });
        System.out.println(Arrays.toString(books));

        //price从高到低
        Arrays.sort(books, new Comparator() {
            //对books数组进行排序，因此 o1、o2 就是 Book对象
            @Override
            public int compare(Object o1, Object o2) {
                Book b1 = (Book) o1;
                Book b2 = (Book) o2;
                return (int) (b2.getPrice() - b1.getPrice());
            }
        });
        System.out.println(Arrays.toString(books));

        //书名从短到长
        Arrays.sort(books, new Comparator() {
            //对books数组进行排序，因此 o1、o2 就是 Book对象
            @Override
            public int compare(Object o1, Object o2) {
                Book b1 = (Book) o1;
                Book b2 = (Book) o2;
                return (b2.getName()).length() - (b1.getName()).length();
            }
        });
        System.out.println(Arrays.toString(books));
    }
}

class Book {
    private String name;
    private double price;

    public Book(String name, int price) {
        this.name = name;
        this.price = price;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public double getPrice() {
        return price;
    }

    public void setPrice(int price) {
        this.price = price;
    }

    @Override
    public String toString() {
        return "Book{" +
                "name='" + name + '\'' +
                ", price=" + price +
                '}';
    }
}

/*
输出结果：
[Book{name='三国演义', price=50.0}, Book{name='红楼梦', price=60.0}, Book{name='三体', price=70.0}, Book{name='假如给我三天光明', price=80.0}]
[Book{name='假如给我三天光明', price=80.0}, Book{name='三体', price=70.0}, Book{name='红楼梦', price=60.0}, Book{name='三国演义', price=50.0}]
[Book{name='假如给我三天光明', price=80.0}, Book{name='三国演义', price=50.0}, Book{name='红楼梦', price=60.0}, Book{name='三体', price=70.0}]
*/
System常用方法
1、exit：退出当前程序

2、arraycopy：复制数组元素，适合底层调用

3、currentTimeMillens：返回当前时间距离 1970-1-1 的毫秒数

4、gc：运行垃圾回收机制

public class SystemMethod {
    public static void main(String[] args) {
        /*
         exit(0) 表示程序退出，0表示一个正常状态
         */
        System.out.println("lalala");
        //System.exit(0);
        System.out.println("hahaha");

        /*
         arraycopy 复制数组元素，适合底层调用
         1、参数含义
         src:源数组
         srcPos:从源数组的哪个索引开始拷贝
         dest:目标数组
         destPos:将源数组的数据拷贝到目标数组的哪个索引
         length:从源数组拷贝多少元素到目标数组
         */
        int[] src = {1, 2, 3};
        int[] dest = new int[3];
        System.arraycopy(src, 0, dest, 0, 3);
        System.out.println(Arrays.toString(dest));

        /*
         currentTimeMillens 返回当前时间距离 1970-1-1 的毫秒数
         */
        System.out.println(System.currentTimeMillis());
    }
}

/*
输出结果：
lalala
hahaha
[1, 2, 3]
1667465891397
*/
Biglnteger BigDecimal
1、应用场景

		（1）BigInteger适合保存比较大的整型

		（2）BigDecimal适合保存精度更高的浮点型

public class BigInteger01 {
    public static void main(String[] args) {
        /*
         BigInteger适合保存比较大的整型
         1、对 BigInteger 进行加减乘除时需要使用对应方法
         2、可以创建一个要操作的 BigInteger, 再进行相应操作
         */
        BigInteger bigInteger = new BigInteger("8888888888888888888888888");
        BigInteger bigInteger1 = new BigInteger("9999999999999999");
        System.out.println(bigInteger);
        System.out.println(bigInteger.add(bigInteger1));
        System.out.println(bigInteger.subtract(bigInteger1));
        System.out.println(bigInteger.multiply(bigInteger1));
        System.out.println(bigInteger.divide(bigInteger1));
    }
}
public class BigDecimal01 {
    public static void main(String[] args) {
        /*
         BigDecimal 适合保存精度更高的浮点型
         1、对 BigDecimal 进行加减乘除时需要使用对应方法
         2、可以创建一个要操作的 BigDecimal, 再进行相应操作
         */
        BigDecimal bigDecimal = new BigDecimal("99.99999999999999999");
        System.out.println(bigDecimal);
        BigDecimal bigDecimal1 = new BigDecimal("99.999999999999");
        System.out.println(bigDecimal.add(bigDecimal1));
        System.out.println(bigDecimal.subtract(bigDecimal1));
        System.out.println(bigDecimal.multiply(bigDecimal1));
        /*
         1、可能会抛出ArithmeticException算术运算异常
         2、解决方案:调用divide方法时指定精度即可
         */
        System.out.println(bigDecimal.divide(bigDecimal1,BigDecimal.ROUND_CEILING));
    }
}
Date、Calendar、LocalDate
1、Date

public class Date01 {
    public static void main(String[] args) {
        //第一代日期类Date 精确到毫秒
        //Date date = new Date(); 无参构造器获取当前系统时间,默认输出日期为国外方式,因此要对输出日期进行格式转换
        Date date = new Date();
        System.out.println(date);

        //SimpleDateFormat 格式和解析日期的类
        SimpleDateFormat dateFormat = new SimpleDateFormat("yyyy年MM月dd日 hh:mm:ss EE");
        System.out.println(dateFormat.format(date));

        //Date date = new Date(long); 有参构造通过指定的毫秒得到时间
        Date date1 = new Date(123456789);
        System.out.println(dateFormat.format(date1));

        /*
         将一个格式化的 String 转换成对应的 Date
         1.得到的Date输出后仍是国外格式,若想指定格式输出,需要转换
         2.将String --> Date,String的格式和dataFormat格式一致,否则会抛出转换异常
         */
        String s = "1999年12月1日 10:20:30 星期一";
        try {
            System.out.println(dateFormat.parse(s));
        } catch (ParseException e) {
            System.out.println(e.getMessage());
        }
    }
}

/*
输出结果：
Fri Nov 04 10:47:47 CST 2022
2022年11月04日 10:47:47 星期五
1970年01月02日 06:17:36 星期五
Wed Dec 01 10:20:30 CST 1999
*/
2、Calendar

public class Calendar01 {
    public static void main(String[] args) {
        /*
         第二代日期类Calendar
         1.抽象类,为特定瞬间与一组诸如YEAR、MONTH、DAY_OF_MONTH、HOUR等日历字段之间的转换提供方法
         2.通过 getInstance() 来获取实例
         */
        Calendar calendar = Calendar.getInstance();
        System.out.println(calendar.get(Calendar.YEAR));
        //Calendar返回月的时候按照0开始编号
        System.out.println(calendar.get(Calendar.MONTH) + 1);
        System.out.println(calendar.get(Calendar.DAY_OF_MONTH));
        System.out.println(calendar.get(Calendar.HOUR));
        System.out.println(calendar.get(Calendar.MINUTE));
        System.out.println(calendar.get(Calendar.SECOND));

        //Calendar没有专门的格式化方法
        System.out.println(calendar.get(Calendar.YEAR) + "年"
                + (calendar.get(Calendar.DAY_OF_MONTH) + 1) + "月"
                + calendar.get(Calendar.HOUR) + "号");
    }
}

/*
输出结果：
2022
11
4
11
15
46
2022年5月11号
*/
3、LocalDate

public class LocalDate01 {
    public static void main(String[] args) {
        /*
         第三代日期类 LocalDate、LocalTime、LocalDateTime
         1.LocalDate 只包含日期
         2.LocalTime 只包含时间
         3.LocalDateTime 包含日期时间
         */
        LocalDateTime timenow = LocalDateTime.now();
        System.out.println(timenow);
        System.out.println(timenow.getYear());
        System.out.println(timenow.getMonth());
        System.out.println(timenow.getDayOfMonth());
        System.out.println(timenow.getHour());
        System.out.println(timenow.getMinute());
        System.out.println(timenow.getSecond());

        /*
         DateTimeFormatter类 对 LocalDateTime对象 进行格式化
         */
        DateTimeFormatter formatter = DateTimeFormatter.ofPattern("yyyy年MM月dd日 hh:mm:ss EE");
        System.out.println(formatter.format(timenow));

        /*
         Instant类 提供一系列和Date类转换的方式
         1.通过 静态方法now() 获取当前时间戳的对象
         2.通过 from 可以把 Instant 转成 Date
         3.通过 date toInstant()方法将 date 转换成 Instant对象
         */
        Instant now = Instant.now();
        System.out.println(now);
        Date date = Date.from(now);
        Instant instant = date.toInstant();

        /*
         plus、minus方法 对当前时间进行加减
         */
        System.out.println(timenow.plusDays(890));
        System.out.println(timenow.minusDays(1000));
    }
}

/*
输出结果：
2022-11-04T15:15:32.426
2022
NOVEMBER
4
15
15
32
2022年11月04日 03:15:32 星期五
2022-11-04T07:15:32.469Z
2025-04-12T15:15:32.426
2020-02-08T15:15:32.426
*/
IDEA Diagrams说明
1、Fields 域

2、Constructors 构造器

3、Methods 方法

4、Properties 属性

5、Inner Classes 内部类

课后习题
String翻转
/**
 * 将字符串中指定部分进行翻转
 */
public class Test {
    public static void main(String[] args) {
        String str = "aaaaabbbbb";
        try {
            String reverse = Test.reverse(str, 0, 10);
            System.out.println(reverse);
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        }
    }

    public static String reverse(String str, int start, int end) throws Exception {

        if (str != null
                && start >= 0
                && start < end
                && end < str.length()) {
            char[] chars = str.toCharArray();

            for (int i = start, j = end; i < j; i++, j--) {
                char temp = chars[i];
                chars[i] = chars[j];
                chars[j] = temp;
            }
            return Arrays.toString(chars);
        } else {
            throw new Exception("参数不正确");
        }
    }
}
注册
public class Test01 {
    public static void main(String[] args) {
        try {
            Test01.login();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        }
    }

    public static void login() throws Exception {

        Scanner scanner = new Scanner(System.in);
        System.out.println("请输入用户名：");
        String loginname = scanner.next();
        System.out.println("请输入密码：");
        String loginpassword = scanner.next();
        System.out.println("请输入邮箱：");
        String loginmailbox = scanner.next();

        if (!(loginname.length() == 2
                || loginname.length() == 3
                || loginname.length() == 4)) {
            throw new Exception("用户名长度不规范");
        } if (isDigital(loginpassword) == false || loginpassword.length() != 6) {
            throw new Exception("密码格式不正确");
        } if (!(loginmailbox.contains("@")
                && loginmailbox.contains(".")
                && loginmailbox.indexOf("@") < loginmailbox.indexOf("."))) {
            throw new Exception("邮箱格式不正确");
        }
        System.out.println("注册成功");
    }

    //判断密码是否全部为数字
    public static boolean isDigital(String str) {
        char[] chars = str.toCharArray();
        for (int i = 0; i < chars.length; i++) {
            if (chars[i] < '0' || chars[i] > '9') {
                return false;
            }
        }
        return true;
    }
}
字符串统计
public class Test02 {
    public static void main(String[] args) {
        Test02.statistics("Jiang Xing Shu");
    }

    public static void statistics(String name) {
        String[] s = name.split(" ");

        if (name == null) {
            System.out.println("name不能为空");
        }
        if (s.length != 3) {
            System.out.println("输入的字符串格式不正确");
        }
        String substring = s[1].substring(0, 1);
        System.out.println(s[2].concat(",").concat(substring).concat(",").concat(s[0]));
    }
}
判断字符串内容
public class Test03 {
    public static void main(String[] args) {
        Test03.judge("11111JJJJJjjjjjXXXXX");
    }

    /**
     * 输入字符串，判断字符串内大写字母、小写字母、数字数量
     * 遍历字符串
     * char在'0'~'9'之间为数字
     * char在'a'~'z'之间为小写字母
     * char在'A'~'Z'之间为大写字母
     */
    public static void judge(String str) {
        if (str == null) {
            System.out.println("字符串不可为空");
        }
        int character = 0;
        int lowercase = 0;
        int capital = 0;
        char[] chars = str.toCharArray();
        for (int i = 0; i < chars.length; i++) {
            if (chars[i] >= '0' && chars[i] <= '9') {
                character++;
            }
            if (chars[i] >= 'a' && chars[i] <= 'z') {
                lowercase++;
            }
            if (chars[i] >= 'A' && chars[i] <= 'Z') {
                capital++;
            }
        }
        System.out.println("数字数量：" + character + "\n"
                + "小写字母数量：" + lowercase + "\n"
                + "大写字母数量：" + capital);
    }
}

/*
输出结果：
数字数量：5
小写字母数量：5
大写字母数量：10
*/
String内存布局
public class Test04 {
    public static void main(String[] args) {
        String s1 = "hspedu";//指向常量池hspedu
        //创建一个Animal类的对象实例，对象实例的name指向常量池的hspedu
        Animal a = new Animal(s1);
        //创建一个Animal类的对象实例，对象实例的name指向常量池的hspedu
        Animal b = new Animal(s1);
        //==判断引用类型，判断的是地址是否相等
        System.out.println(a == b);
        //Animal没有重写父类的equals方法,则使用父类的equals方法(默认判断地址是否相等)
        System.out.println(a.equals(b));
        System.out.println(a.name == b.name);
        //s2指向的是堆中的空间地址
        String s2 = new String("hspedu");
        String s3 = "hspedu";//指向常量池hspedu
        System.out.println(s1 == s2);
        System.out.println(s2 == s3);
        String s4 = "hello" + s1;//指向常量池的hellohspedu
        String s5 = "hellohspedu";//指向常量池的hellohspedu
        //s4.intern()指向常量池的hellohspedu
        System.out.println(s4.intern() == s5);
    }
}

class Animal {
    String name;

    public Animal(String name) {
        this.name = name;
}

/*
输出结果：
false
false
true
false
false
true
*/
1.2.5、集合
集合快速入门
集合：
1、动态的保存任意多个对象
2、提供一系列方便的操作对象的方法：add、remove、set、get
3、增删元素简洁
public class ArrayTest {
    public static void main(String[] args) {
        /*
         数组：长度固定、保存同一类型元素、增删元素繁琐
         */
        Person[] person1 = new Person[1];

        //数组扩容
        Person[] person2 = new Person[person1.length + 1];
        for (int i = 0; i < person1.length; i++) {
            person2[i] = person1[i];
        }
        
        /*
         集合：
         1、动态的保存任意多个对象
         2、提供一系列方便的操作对象的方法：add、remove、set、get
         3、增删元素简洁
         */
    }
}

class Person {
}
集合框架体系
1、集合分两组(单列集合、双列集合)。
2、Collection接口有两个重要的子接口List、Set，它们的实现子类都为单列集合。
3、Map接口的实现子类是双列集合。
1、Collection
	1.1、List
		1.1.1、ArrayList
		1.1.2、LinkedList
		1.1.3、Vector
	1.2、Set
		1.2.1、HashSet
		1.2.2、TreeSet

2、Map
	2.1、HashMap
	2.2、Hashtable
	2.3、LinkedHashMap
	2.4、TreeMap
	2.5、Properties




Collection接口实现类特点
1、Collection接口实现子类可以存放多个元素，每个元素可以是Object

2、有些Collection的实现类可以存放重复元素，有些不可以

3、Collection的实现类有些是有序的（List），有些是无序的（Set）

4、Collection接口没有直接的实现子类，是通过它的子接口List、Set来实现。

Collection方法
public class CollectionMethod {
    public static void main(String[] args) {
        List list = new ArrayList();
        System.out.println("add:添加单个元素");
        list.add("jack");
        list.add(1);//list.add(new Integer(1))
        list.add(true);
        System.out.println("list=" + list);

        System.out.println("remove:删除指定元素");
        System.out.println(list.remove(0));//删除指定索引的元素
        System.out.println(list.remove(true));//删除指定的某个元素
        System.out.println("list=" + list);

        System.out.println("contains:查找元素是否存在");
        System.out.println(list.contains(1));
        System.out.println(list.contains("jack"));

        System.out.println("size:获取元素个数");
        System.out.println(list.size());

        System.out.println("isEmpty:判断是否为空");
        System.out.println(list.isEmpty());

        System.out.println("clear:清空");
        list.clear();
        System.out.println(list);

        System.out.println("addAll:添加多个元素");
        ArrayList list1 = new ArrayList();
        list1.add("三国演义");
        list1.add("红楼梦");
        list.addAll(list1);
        System.out.println(list);

        System.out.println("containsAll:查找多个元素是否存在");
        System.out.println(list.containsAll(list1));

        System.out.println("removeAll:删除多个元素");
        list.removeAll(list1);
        System.out.println(list);
    }
}

/*
输出结果：
add:添加单个元素
list=[jack, 1, true]
remove:删除指定元素
jack
true
list=[1]
contains:查找元素是否存在
true
false
size:获取元素个数
1
isEmpty:判断是否为空
false
clear:清空
[]
addAll:添加多个元素
[三国演义, 红楼梦]
containsAll:查找多个元素是否存在
true
removeAll:删除多个元素
[]
*/
Collection接口遍历元素方式
方式一：迭代器
1、Iterator对象称为迭代器，主要用于遍历Collection集合中的元素

2、实现了Collection接口的集合类都有一个iterator()方法，用于返回一个实现了Iterator接口的对象，即可以返回一个迭代器

3、Iterator仅用于遍历集合，Ietrator本身并不存放对象。

迭代器 iterator 的三个基本操作是 next 、hasNext 和 remove。
调用 iterator.next() 会返回迭代器的下一个元素，并且更新迭代器的状态。
调用 iterator.hasNext() 用于检测集合中是否还有元素。
调用 iterator.remove() 将迭代器返回的元素删除。

在调用iterator.next()方法之前必须要调用iterator.hasNext()方法进行检测。
若不调用并且下一条记录无效，直接调用iterator.next()方法会抛出NoSuchElementException异常。
public class Collection_Iterator {
    public static void main(String[] args) {
        ArrayList list = new ArrayList();
        list.add(new Book("三国演义","罗贯中",50.0));
        list.add(new Book("红楼梦","曹雪芹",60.0));
        list.add(new Book("西游记","吴承恩",70.0));
        list.add(new Book("水浒传","施耐庵",80.0));
        System.out.println(list);

        /*
         遍历集合
         1.实现了Collection接口的集合类都有一个iterator()方法，
           用于返回一个实现了Iterator接口的对象，即可以返回一个迭代器
         2.得到list的迭代器
         */
        Iterator iterator = list.iterator();
        /*
         3.使用while循环
         快速生成while循环快捷键 itit
         显示所有快捷指令的快捷键 ctrl + j
         */
        while(iterator.hasNext()) {
            //4.返回下一个元素，类型为Object
            Object next = iterator.next();
            System.out.println(next);
        }
        /*
         5.退出while循环后,iterator迭代器指向最后的元素,再向后取元素会抛出NoSuchElementException异常
         6.若希望再次遍历集合,需要重置迭代器
         */
        iterator = list.iterator();
        while (iterator.hasNext()) {
            Object next = iterator.next();
            System.out.println(next);
        }
    }
}

class Book {
    private String name;
    private String author;
    private double price;

    public Book(String name, String author, double price) {
        this.name = name;
        this.author = author;
        this.price = price;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public String getAuthor() {
        return author;
    }
    public void setAuthor(String author) {
        this.author = author;
    }
    public double getPrice() {
        return price;
    }
    public void setPrice(double price) {
        this.price = price;
    }

    @Override
    public String toString() {
        return "Book{" +
                "name='" + name + '\'' +
                ", author='" + author + '\'' +
                ", price=" + price +
                '}';
    }
}

/*
输出结果：
[Book{name='三国演义', author='罗贯中', price=50.0}, Book{name='红楼梦', author='曹雪芹', price=60.0}, Book{name='西游记', author='吴承恩', price=70.0}, Book{name='水浒传', author='施耐庵', price=80.0}]
Book{name='三国演义', author='罗贯中', price=50.0}
Book{name='红楼梦', author='曹雪芹', price=60.0}
Book{name='西游记', author='吴承恩', price=70.0}
Book{name='水浒传', author='施耐庵', price=80.0}
Book{name='三国演义', author='罗贯中', price=50.0}
Book{name='红楼梦', author='曹雪芹', price=60.0}
Book{name='西游记', author='吴承恩', price=70.0}
Book{name='水浒传', author='施耐庵', price=80.0}
*/
方式二：增强for循环
1、增强for循环，可以替代iterator迭代器

2、增强for循环特点：简化版iterator，本质一样。可以用来遍历集合或数组

3、基本语法：

for(元素类型 元素名 : 集合名或数组名) {
    访问元素
}
public class Collection_Iterator {
    public static void main(String[] args) {
        ArrayList list = new ArrayList();
        list.add(new Book("三国演义", "罗贯中", 50.0));
        list.add(new Book("红楼梦", "曹雪芹", 60.0));
        list.add(new Book("西游记", "吴承恩", 70.0));
        list.add(new Book("水浒传", "施耐庵", 80.0));
        System.out.println(list);

        /*
         1.增强for循环可以遍历集合或数组
         2.增强for循环底层是迭代器
         3.增强for循环可以理解为简化版的迭代器
         4.增强for循环快捷键 iter
         */
        for (Object book : list) {
            System.out.println(book);
        }

        int[] arrays = {1,10,100};
        for (Object array : arrays) {
            System.out.println(array);
        }
    }
}

class Book {
    private String name;
    private String author;
    private double price;

    public Book(String name, String author, double price) {
        this.name = name;
        this.author = author;
        this.price = price;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public String getAuthor() {
        return author;
    }
    public void setAuthor(String author) {
        this.author = author;
    }
    public double getPrice() {
        return price;
    }
    public void setPrice(double price) {
        this.price = price;
    }

    @Override
    public String toString() {
        return "Book{" +
                "name='" + name + '\'' +
                ", author='" + author + '\'' +
                ", price=" + price +
                '}';
    }
}

/*
输出结果：
[Book{name='三国演义', author='罗贯中', price=50.0}, Book{name='红楼梦', author='曹雪芹', price=60.0}, Book{name='西游记', author='吴承恩', price=70.0}, Book{name='水浒传', author='施耐庵', price=80.0}]
Book{name='三国演义', author='罗贯中', price=50.0}
Book{name='红楼梦', author='曹雪芹', price=60.0}
Book{name='西游记', author='吴承恩', price=70.0}
Book{name='水浒传', author='施耐庵', price=80.0}
1
10
100
*/
Collection练习
public class CollectionExercise01 {
    public static void main(String[] args) {
        ArrayList list = new ArrayList();
        list.add(new Dog("小花",5));
        list.add(new Dog("小白",6));
        list.add(new Dog("小黑",7));

        Iterator iterator = list.iterator();
        while(iterator.hasNext()) {
            Object next = iterator.next();
            System.out.println(next);
        }

        for (Object dog : list) {
            System.out.println(dog);
        }
    }
}

class Dog {
    private String name;
    private int age;

    public Dog(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "Dog{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}

/*
输出结果：
Dog{name='小花', age=5}
Dog{name='小白', age=6}
Dog{name='小黑', age=7}
Dog{name='小花', age=5}
Dog{name='小白', age=6}
Dog{name='小黑', age=7}
*/
List接口基本介绍
1、List接口是Collection接口的子接口

2、List集合类中元素排列有序（添加取出顺序一致）、元素可重复

3、List集合类中每个元素都有其对应的顺序索引，即支持索引

4、List容器中的元素都对应一个整数型的序号记载其在容器中的位置，可以根据序号存取容器中的元素

5、JDK API中List接口的实现类很多，常用的有ArrayList、LinkedList、Vector

public class List01 {
    public static void main(String[] args) {
        List list = new ArrayList();//向上转型
        list.add("jxs");
        list.add("dwy");
        list.add("tyh");
        //1.List集合类中元素排列有序、元素可重复
        list.add("jxs");
        System.out.println(list);
        //2.List集合类中每个元素都有其对应的顺序索引，即支持索引
        System.out.println(list.get(0));
    }
}

/*
输出结果：
[jxs, dwy, tyh, jxs]
jxs
*/
List接口方法
public class ListMethod {
    public static void main(String[] args) {
        List list1 = new ArrayList();
        list1.add("jxs");
        list1.add("dwy");
        System.out.println("add(int index, Object element):在index索引位置插入element元素");
        list1.add(1,"小丑");
        System.out.println(list1);

        System.out.println("addAll(int index, Collection c):在index索引位置将集合c的所有元素添加进来");
        List list2 = new ArrayList();
        list2.add("zls");
        list2.add("lxz");
        list2.add("wgw");
        list1.addAll(1,list2);
        System.out.println(list1);

        System.out.println("get(int index):获取index索引位置的元素");
        System.out.println(list1.get(5));

        System.out.println("indexOf(Object o):返回o在集合中首次出现的位置");
        System.out.println(list1.indexOf("jxs"));

        System.out.println("lastIndexOf(Object o):返回o在集合中最后一次出现的位置");
        System.out.println(list1.lastIndexOf("dwy"));

        System.out.println("remove(int index):移除index索引位置的元素,并返回该元素");
        System.out.println(list1.remove(1));
        System.out.println(list1);

        System.out.println("set(int index, Object element):将index索引位置的元素替换为element元素");
        list1.set(1,"dwy");
        System.out.println(list1);

        System.out.println("subList(int fromIndex, int toIndex):返回fromIndex到toIndex索引位置的子集合,左闭右开");
        System.out.println(list1.subList(1,3));
    }
}

/*
输出结果：
add(int index, Object element):在index索引位置插入element元素
[jxs, 小丑, dwy]
addAll(int index, Collection c):在index索引位置将集合c的所有元素添加进来
[jxs, zls, lxz, wgw, 小丑, dwy]
get(int index):获取index索引位置的元素
dwy
indexOf(Object o):返回o在集合中首次出现的位置
0
lastIndexOf(Object o):返回o在集合中最后一次出现的位置
5
remove(int index):移除index索引位置的元素,并返回该元素
zls
[jxs, lxz, wgw, 小丑, dwy]
set(int index, Object element):将index索引位置的元素替换为element元素
[jxs, dwy, wgw, 小丑, dwy]
subList(int fromIndex, int toIndex):返回fromIndex到toIndex索引位置的子集合,左闭右开
[dwy, wgw]
*/
List三种遍历方式
1、迭代器

2、增强for循环

3、普通for循环

public class ListExercise01 {
    public static void main(String[] args) {
        List list = new ArrayList();
        list.add("jxs");
        list.add("dwy");
        list.add("tom");

        //1.迭代器
        Iterator iterator = list.iterator();
        while (iterator.hasNext()) {
            Object next = iterator.next();
            System.out.println(next);
        }

        //2.增强for循环
        for (Object o : list) {
            System.out.println(o);
        }

        //3.普通for循环
        for (int i = 0; i < list.size(); i++) {
            Object o = list.get(i);
            System.out.println(o);
        }
    }
}

/*
输出结果：
jxs
dwy
tom
jxs
dwy
tom
jxs
dwy
tom
*/
List练习
public class ListExercise02 {
    public static void main(String[] args) {
        List list = new ArrayList();

        list.add(new Books("三国演义", 50.0, "罗贯中"));
        list.add(new Books("红楼梦", 40.0, "曹雪芹"));
        list.add(new Books("西游记", 60.0, "吴承恩"));

        ListExercise02.sort(list);
    }

    //冒泡排序
    public static void sort(List list) {
        for (int i = 0; i < list.size() - 1; i++) {
            for (int j = 0; j < list.size() - 1 - i; j++) {
                /*
                 取出Books类对象
                 1、取出的对象为Object类对象,因属性看编译类型;方法看运行类型。
                 2、Object类对象无法调用Books类的get、set方法
                 3、向下转型取出Books类对象
                 */
                Books book1 = (Books) list.get(j);
                Books book2 = (Books) list.get(j + 1);

                if (book1.getPrice() < book2.getPrice()) {
                    //交换j、j+1索引处的Books类对象
                    list.set(j, book2);
                    list.set(j + 1, book1);
                }
            }
        }
        //增强for循环遍历list集合
        for (Object o : list) {
            System.out.println(o);
        }
    }
}

class Books {
    private String name;
    private double price;
    private String author;

    public Books(String name, double price, String author) {
        this.name = name;
        this.price = price;
        this.author = author;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public double getPrice() {
        return price;
    }
    public void setPrice(double price) {
        this.price = price;
    }
    public String getAuthor() {
        return author;
    }
    public void setAuthor(String author) {
        this.author = author;
    }

    /*
     1、重写父类 Object类 的toString方法
     2、Object类的 toString方法 默认输出地址
     */
    @Override
    public String toString() {
        return "书名：" + name + "\t"
                + "价格：" + price + "\t"
                + "作者：" + author;
    }
}

/*
输出结果：
书名：西游记	价格：60.0	作者：吴承恩
书名：三国演义	价格：50.0	作者：罗贯中
书名：红楼梦	价格：40.0	作者：曹雪芹
*/
ArrayList注意事项
1、ArrayList可以放入所有元素，包括null

2、ArrayList是由数组来实现数据存储的

3、ArrayList基本等同于Vector

4、ArrayList是线程不安全的，多线程情况下，不建议使用ArrayList

ArrayList底层结构和源码分析（重要！）
1、ArrayList中维护了一个Object类型的数组elementData

	  transient Object[] elementData（被transient修饰的属性不会被序列化）

2、当创建ArrayList对象时，若使用的是无参构造器，则初始elementData容量为0

	  第一次添加，则扩容elementData为10

	  若需再次扩容，则扩容elementData为1.5倍。

3、当创建ArrayList对象时，若使用的是指定大小的构造器，则初始elementData容量为指定大小

	  若需扩容，则扩容elementData为1.5倍

	  若需再次扩容，也扩容elementData为1.5倍

ArrayList底层结构和源码分析（代码+图解）
使用无参构造器
public class ArrayListSource {
    public static void main(String[] args) {
        /*
         1、使用无参构造器创建ArrayList对象
         2、使用for循环为 arrayList1集合 添加 1-10 数据
         3、使用for循环为 arrayList1集合 添加 11-15 数据
         */
        ArrayList arrayList1 = new ArrayList();

        for (int i = 1; i <= 10; i++) {
            arrayList1.add(i);
        }

        for (int i = 11; i < 15; i++) {
            arrayList1.add(i);
        }

        for (Object o : arrayList1) {
            System.out.println(o);
        }
    }
}
ArrayList底层源码步骤1：



ArrayList底层源码步骤2：

![](E:\Study\自学课程资料\Java\assets\ArrayList底层源码步骤2.png)

ArrayList底层源码步骤3：

![](E:\Study\自学课程资料\Java\assets\ArrayList底层源码步骤3.png)

ArrayList底层源码步骤4：

![](E:\Study\自学课程资料\Java\assets\ArrayList底层源码步骤4.png)

ArrayList底层源码步骤5：

![](E:\Study\自学课程资料\Java\assets\ArrayList底层源码步骤5.png)

使用有参构造器
public class ArrayListSource {
    public static void main(String[] args) {
        
        ArrayList arrayList = new ArrayList(8);

        for (int i = 1; i <= 10; i++) {
            arrayList.add(i);
        }

        for (int i = 11; i < 15; i++) {
            arrayList.add(i);
        }

        for (Object o : arrayList) {
            System.out.println(o);
        }
    }
}
ArrayList使用有参构造底层源码步骤1：

![](E:\Study\自学课程资料\Java\assets\ArrayList使用有参构造底层源码步骤1.png)

ArrayList使用有参构造底层源码步骤2：

![](E:\Study\自学课程资料\Java\assets\ArrayList使用有参构造底层源码步骤2.png)

Vector注意事项
1、Vector底层也是一个对象数组，protected Object[] elementData

2、Vector是线程同步的，Vector类的操作方法带有synchronized

3、在开发中，需要线程安全时，可以考虑Vector

Vector底层结构和源码分析（重要）
底层结构	版本	线程安全(同步)效率	扩容倍数
ArrayList	可变数组	JDK1.2	不安全，效率高	有参构造1.5倍；无参构造第一次10，之后1.5倍扩容
Vector	可变数组	JDK1.0	安全，效率不高	有参构造2倍；无参构造第一次10，之后2倍扩容
public class VectorSource {
    public static void main(String[] args) {
        Vector vector = new Vector();
        /*
         源码解读
         1、public Vector() {
                this(10);
            }

            public Vector(int initialCapacity) {
                this(initialCapacity, 0);
            }

         2、添加数据到集合
            public synchronized boolean add(E e) {
                modCount++;
                ensureCapacityHelper(elementCount + 1);
                elementData[elementCount++] = e;
                return true;
            }

         3、进入 ensureCapacityHelper方法，确认是否需要扩容
            private void ensureCapacityHelper(int minCapacity) {
                // overflow-conscious code
                if (minCapacity - elementData.length > 0)
                    grow(minCapacity);
            }

         4、
         (1)将 elementData数组长度 赋值给 oldCapacity
         (2)capacityIncrement = 0
         (3)若 capacityIncrement > 0，则 oldCapacity + capacityIncrement 赋值给 newCapacity
         (4)否则 oldCapacity + oldCapacity 赋值给 newCapacity
         (5)newCapacity - minCapacity > 0
         (6)newCapacity - MAX_ARRAY_SIZE < 0
         (7)elementData = Arrays.copyOf(elementData, newCapacity);
            private void grow(int minCapacity) {
                // overflow-conscious code
                int oldCapacity = elementData.length;
                int newCapacity = oldCapacity + ((capacityIncrement > 0) ?
                                         capacityIncrement : oldCapacity);
                if (newCapacity - minCapacity < 0)
                    newCapacity = minCapacity;
                if (newCapacity - MAX_ARRAY_SIZE > 0)
                    newCapacity = hugeCapacity(minCapacity);
                elementData = Arrays.copyOf(elementData, newCapacity);
            }
         */

        for (int i = 0; i < 10; i++) {
            vector.add(i);
        }

        vector.add(100);
    }
}
LinkedList注意事项
1、LinkedList底层实现了双向链表、双端队列特点

2、可以添加任意元素，包括null

3、线程不安全，没有实现同步

4、	LinkedList中维护了两个属性first、last，分别指向首节点和尾节点

5、每个节点（Node对象）中维护了prev、next、item三个属性，prev指向前一个节点，next指向后一个节点，最终实现双向链表

6、LinkedList的元素添加和删除，不是通过数组来完成的，相对来说效率较高

双向链表模拟
/**
 * 模拟双向链表
 */
public class LinkedList {
    public static void main(String[] args) {
        Node node1 = new Node("jxs");
        Node node2 = new Node("dwy");
        Node node3 = new Node("tyh");

        /*
         连接3个节点
         node1 --> node2 --> node3
         node3 --> node2 --> node1
         first 指向 node1,即双向链表的头节点
         last 指向 node3,即双向链表的尾节点
         */
        node1.next = node2;
        node2.next = node3;

        node3.prev = node2;
        node2.prev = node1;

        Node first = node1;
        Node last = node3;

        /*
         遍历
         1、从头到尾遍历
         2、从尾到头遍历
         */
        while (true) {
            if (first == null) {
                break;
            }
            System.out.println(first);
            first = first.next;
        }

        while (true) {
            if (last == null) {
                break;
            }
            System.out.println(last);
            last = last.prev;
        }

        /*
         插入数据
         */
        Node node4 = new Node("zls");
        node2.next = node4;
        node4.prev = node2;
        node4.next = node3;
        node3.prev = node4;

        //first 再次指向第一个节点,last 再次指向最后一个节点
        first = node1;

        while (true) {
            if (first == null) {
                break;
            }
            System.out.println(first);
            first = first.next;
        }
    }
}

/**
 * 定义一个Node类，Node对象表示双向链表的一个节点
 * item 存放数据
 * next 指向下一个节点
 * prev 指向上一个节点
 */
class Node {
    public Object item;
    public Node next;
    public Node prev;

    //构造器
    public Node(Object name) {
        this.item = name;
    }

    @Override
    public String toString() {
        return "Node_Name = " + item;
    }
}

/*
输出结果：
Node_Name = jxs
Node_Name = dwy
Node_Name = tyh
Node_Name = tyh
Node_Name = dwy
Node_Name = jxs
Node_Name = jxs
Node_Name = dwy
Node_Name = zls
Node_Name = tyh
*/
LinkedList底层结构和源码分析（重要！）
public class LinkedListCRUD {
    public static void main(String[] args) {
        LinkedList linkedList = new LinkedList();
        linkedList.add(1);
        System.out.println(linkedList);
        linkedList.add(2);
        System.out.println(linkedList);
        linkedList.remove();//默认删除第一个节点
        System.out.println(linkedList);
    }
}
LinkedList底层源码步骤1

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤1.png)

LinkedList底层源码步骤2

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤2.png)

LinkedList底层源码步骤3

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤3.png)

LinkedList底层源码步骤4

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤4.png)

LinkedList底层源码步骤5

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤5.png)

LinkedList底层源码步骤6

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤6.png)

LinkedList底层源码步骤7

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤7.png)

LinkedList底层源码步骤8

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤8.png)

LinkedList底层源码步骤9

![](E:\Study\自学课程资料\Java\assets\LinkedList底层源码步骤9.png)

ArrayList和LinkedList比较
底层结构	增删效率	改查效率
ArrayList	可变数组	较低，通过数组扩容	较高
LinkedList	双向链表	较高，通过链表追加	较低
1、改查操作多时，选择ArrayList

2、增删操作多时，选择LinkedList

3、程序中80%~90%为查询，选择ArrayList

4、在项目中，根据业务灵活选择，也可一个模块为ArrayList，一个模块为LinkedList

Set接口基本介绍
1、无序（添加、取出顺序不一致），无索引

2、不允许重复元素，即最多包含一个null

3、JDK API中Set接口的实现类有:HashSet、TreeSet

Set接口方法及遍历方式
1、Set接口的常用方法：和List接口一样，Set接口也是Collection的子接口，因此，常用方法和Collection接口一样。

2、Set接口的遍历方式：

		（1）迭代器

		（2）增强for循环

		（3）无索引，不可使用索引的方式

public class SetMethod {
    public static void main(String[] args) {
        /*
         1、以Set接口的实现类HashSet讲解Set接口的方法
         2、实现Set接口的类的对象,不能存放重复元素
         3、可以添加null
         4、实现Set接口的类的对象是无序的，即添加和取出的顺序不一致
         5、取出的顺序虽不是添加的顺序，但是是固定的
         6、遍历方式:迭代器、增强for循环
         7、实现Set接口的类的对象不可用索引来获取
         */
        Set set = new HashSet();
        set.add("jack");
        set.add("lucy");
        set.add("john");
        set.add("jack");
        set.add(null);
        set.add(null);
        System.out.println(set);
        set.add("jxs");
        System.out.println(set);

        Iterator iterator = set.iterator();
        while (iterator.hasNext()) {
            Object next = iterator.next();
            System.out.println(next);
        }

        for (Object o : set) {
            System.out.println(o);
        }
    }
}

/*
输出结果：
[null, john, lucy, jack]
[null, jxs, john, lucy, jack]
null
jxs
john
lucy
jack
null
jxs
john
lucy
jack
*/
HashSet全面说明
1、HashSet实现了Set接口

2、HashSet实际上是HashMap

public HashSet() {
	map = new HashMap<>();
}
3、可以存放null值，但只能存放一个null，即元素不能重复

4、HashSet不保证存放元素和取出元素的顺序一致，取决于hash后，再确定索引的结果

数组链表模拟
public class HashSetStructure {
    public static void main(String[] args) {
        /*
         HashSet的底层结构即HashMap的底层结构
         1、创建一个数组,数组的数据类型为Node[]
         2、Node[]又称table
         */
        Node[] table = new Node[16];
        Node node1 = new Node("jxs",null);
        //将node1放到table表的索引为2的位置
        table[2] = node1;

        Node node2 = new Node("dwy",null);
        //将node2挂载到node1
        node1.next = node2;

        Node node3 = new Node("jjz",null);
        //将node3挂载到node2
        node2.next = node3;

        Node node4 = new Node("zls",null);
        //将node4放到table表的索引为3的位置
        table[3] = node4;
    }
}

/*
 1、节点,存储数据
 2、可以指向下一节点,形成链表
 */
class Node {
    Object item;
    Node next;

    public Node(Object item, Node next) {
        this.item = item;
        this.next = next;
    }
}
HashSet源码解读(重要重要重要！！！)
public class HashSetSource {
    public static void main(String[] args) {
        /*
         1.HashSet底层为HashMap
         2.添加一个元素时,先得到hash值,hash值->索引值
         3.找到存储数据表,若索引位置没有存放元素则直接加入
         4.若索引位置已经存放元素则调用equals比较(equals方法可以重写)。若相同则放弃添加;若不相同则添加到最后
         5.在JDK8中,若链表的元素个数到达TREEIFY_THRESHOLD(树化阈值,默认值为8),
           并且table的大小大于等于MIN_TREEIFY_CAPACITY(最小树化容量,默认为64),则进行树化(红黑树)
         */
        HashSet hashSet = new HashSet();
        hashSet.add("java");
        hashSet.add("jxs");
        hashSet.add("java");
        System.out.println(hashSet);
    }
}
1、执行HashSet()构造器
    
public HashSet() {
    map = new HashMap<>();
}
2、执行add()方法
(1)传入的e = "java"
(2)调用put(e, PRESENT)方法
(3)PRESENT:private static final Object PRESENT = new Object();
PRESENT:HashSet类中final类型的Object类对象,占位作用
    
public boolean add(E e) {
    return map.put(e, PRESENT)==null;
}
3、执行put()方法
(1)传入的key = "java"
(2)传入的value = PRESENT
(3)执行hash(key)方法
(4)执行putVal(hash(key), key, value, false, true)方法

public V put(K key, V value) {
	return putVal(hash(key), key, value, false, true);
}
4、执行hash()方法
(1)传入的key = "java"
(2)定义int类型的变量h
(3)若key == null则返回0
(4)若key != null则返回 hashcode和无符号右移16位的hashcode后得到的值做异或运算
    
static final int hash(Object key) {
    int h;
    return (key == null) ? 0 : (h = key.hashCode()) ^ (h >>> 16);
}
5、执行putVal()方法
(1)定义辅助变量HashMap.Node<K,V>[] tab; HashMap.Node<K,V> p; int n, i
(2)执行if判断:if ((tab = table) == null || (n = tab.length) == 0)
(3)执行resize()方法
(4)执行n = (tab = resize()).length,将newTab.length赋值给n
(5)执行if判断:if ((p = tab[i = (n - 1) & hash]) == null)
(6)++modCount;记录修改次数
(7)if (++size > threshold)
   	resize();
若++size > threshold(阈值)则执行resize()方法。

final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
               boolean evict) {
    HashMap.Node<K,V>[] tab; HashMap.Node<K,V> p; int n, i;
    /*
    HashMap类的一个属性:Node类型的数组
    transient Node<K,V>[] table;
    */
    if ((tab = table) == null || (n = tab.length) == 0)
        n = (tab = resize()).length;
    /*
    1.i = (n - 1) & hash(根据K key对应的hash值来计算存放在table表哪个索引位置)
    2.将这个位置的对象赋给p
    3.若p为null,表示还未存放元素,则在(n - 1) & hash索引处创建一个newNode(hash, key, value, null)
    */
    if ((p = tab[i = (n - 1) & hash]) == null)
        tab[i] = newNode(hash, key, value, null);
    else {
        HashMap.Node<K,V> e; K k;
        if (p.hash == hash &&
                ((k = p.key) == key || (key != null && key.equals(k))))
            e = p;
        else if (p instanceof HashMap.TreeNode)
            e = ((HashMap.TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
        else {
            for (int binCount = 0; ; ++binCount) {
                if ((e = p.next) == null) {
                    p.next = newNode(hash, key, value, null);
                    if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
                        treeifyBin(tab, hash);
                    break;
                }
                if (e.hash == hash &&
                        ((k = e.key) == key || (key != null && key.equals(k))))
                    break;
                p = e;
            }
        }
        if (e != null) { // existing mapping for key
            V oldValue = e.value;
            if (!onlyIfAbsent || oldValue == null)
                e.value = value;
            afterNodeAccess(e);
            return oldValue;
        }
    }
    ++modCount;
    if (++size > threshold)
        resize();
    afterNodeInsertion(evict);
    return null;
}
6、执行resize()方法
(1)将table赋值给oldTab
    
(2)三元运算符判断int oldCap = (oldTab == null) ? 0 : oldTab.length;

(3)将阈值threshold = 0赋值给oldThr
    
(4)定义int类型的newCap, newThr,并将0赋值给newCap, newThr
    
(5)执行newCap = DEFAULT_INITIAL_CAPACITY;
DEFAULT_INITIAL_CAPACITY:默认初始容量
static final int DEFAULT_INITIAL_CAPACITY = 1 << 4;(左移4位,乘以4次2)

(6)执行newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
DEFAULT_LOAD_FACTOR:默认负载系数0.75
    
(7)threshold = newThr;将 newThr 赋值给 threshold
    
(8)Node<K,V>[] newTab = (Node<K,V>[])new Node[newCap];定义一个长度为newCap的Node类型的数组newTab
    
(9)table = newTab;将newTab赋值给table
    
(10)return newTab;返回newTab

final HashMap.Node<K,V>[] resize() {
    HashMap.Node<K,V>[] oldTab = table;
    int oldCap = (oldTab == null) ? 0 : oldTab.length;
    int oldThr = threshold;
    int newCap, newThr = 0;
    if (oldCap > 0) {
        if (oldCap >= MAXIMUM_CAPACITY) {
            threshold = Integer.MAX_VALUE;
            return oldTab;
        }
        else if ((newCap = oldCap << 1) < MAXIMUM_CAPACITY &&
                oldCap >= DEFAULT_INITIAL_CAPACITY)
            newThr = oldThr << 1; // double threshold
    }
    else if (oldThr > 0) // initial capacity was placed in threshold
        newCap = oldThr;
    else {               // zero initial threshold signifies using defaults
        newCap = DEFAULT_INITIAL_CAPACITY;
        newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
    }
    if (newThr == 0) {
        float ft = (float)newCap * loadFactor;
        newThr = (newCap < MAXIMUM_CAPACITY && ft < (float)MAXIMUM_CAPACITY ?
                (int)ft : Integer.MAX_VALUE);
    }
    threshold = newThr;
    @SuppressWarnings({"rawtypes","unchecked"})
    HashMap.Node<K,V>[] newTab = (HashMap.Node<K,V>[])new HashMap.Node[newCap];
    table = newTab;
    if (oldTab != null) {
        for (int j = 0; j < oldCap; ++j) {
            HashMap.Node<K,V> e;
            if ((e = oldTab[j]) != null) {
                oldTab[j] = null;
                if (e.next == null)
                    newTab[e.hash & (newCap - 1)] = e;
                else if (e instanceof HashMap.TreeNode)
                    ((HashMap.TreeNode<K,V>)e).split(this, newTab, j, oldCap);
                else { // preserve order
                    HashMap.Node<K,V> loHead = null, loTail = null;
                    HashMap.Node<K,V> hiHead = null, hiTail = null;
                    HashMap.Node<K,V> next;
                    do {
                        next = e.next;
                        if ((e.hash & oldCap) == 0) {
                            if (loTail == null)
                                loHead = e;
                            else
                                loTail.next = e;
                            loTail = e;
                        }
                        else {
                            if (hiTail == null)
                                hiHead = e;
                            else
                                hiTail.next = e;
                            hiTail = e;
                        }
                    } while ((e = next) != null);
                    if (loTail != null) {
                        loTail.next = null;
                        newTab[j] = loHead;
                    }
                    if (hiTail != null) {
                        hiTail.next = null;
                        newTab[j + oldCap] = hiHead;
                    }
                }
            }
        }
    }
    return newTab;
}
7、添加重复元素时
(1)执行if判断:if ((tab = table) == null || (n = tab.length) == 0) 
   表不为空,跳过此if判断代码块
(2)执行if判断:if ((p = tab[i = (n - 1) & hash]) == null)
   添加重复元素,hash值相同,将(n - 1) & hash赋值给i,tab[i] != null,跳过此if判断代码块
(3)进入else代码块

final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
               boolean evict) {
    HashMap.Node<K,V>[] tab; HashMap.Node<K,V> p; int n, i;
    if ((tab = table) == null || (n = tab.length) == 0)
        n = (tab = resize()).length;
    if ((p = tab[i = (n - 1) & hash]) == null)
        tab[i] = newNode(hash, key, value, null);
    else {
        //定义局部辅助变量
        HashMap.Node<K,V> e; K k;
        /*
        执行if代码块满足条件
        p = tab[i]
        1.当前索引位置对应的链表的第一个元素和准备添加的key的hash值一样
        2.准备添加的 key 和 p指向Node节点的key为同一对象,或准备添加的 key != null 且 准备添加           的 key的内容 和 p指向Node节点的key的内容 一致时执行此if判断代码块
        
        注:比较hash的作用:
        首先我们了解一个逻辑式即:key相等->hash值相同（需要我们自己重写hashcode实现）
        若满足hash值相等的条件后,我们无法确定key值是否相等,因为hash相等只是一个必要条件,接着判断key值相等就行,这样就极大的提高性能。
        类比生活:班长从班干部中选，所以先判断他是否为班干部，而不是一按照班长的所有符合条件去判断班里         每个人
        */
        if (p.hash == hash &&
                ((k = p.key) == key || (key != null && key.equals(k))))
            e = p;
        /*
        执行else if代码块满足条件
        1.判断p是否为一颗红黑树
        2.若为一棵红黑树则调用putTreeVal方法
        */
        else if (p instanceof HashMap.TreeNode)
            e = ((HashMap.TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
        /*
        若table表对应的索引位置为一个链表,则使用for循环比较
        (1)依次和该链表的每一个元素比较后,若都不相同,则加入到此链表最后
        (2)依次和该链表的每一个元素比较时,若binCount >= 树化阈值 - 1时,执行treeifyBin(tab, hash)方法
        (3)依次和该链表的每一个元素比较过程中,若有相同元素情况则直接break
        */
        else {
            for (int binCount = 0; ; ++binCount) {
                if ((e = p.next) == null) {
                    p.next = newNode(hash, key, value, null);
                    if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
                        treeifyBin(tab, hash);
                    break;
                }
                /*
                1.e = p.next
                2.e.hash即p.next.hash
                */
                if (e.hash == hash &&
                        ((k = e.key) == key || (key != null && key.equals(k))))
                    break;
                /*
                例:
                一个链表第一个元素jxs,第二个元素dwy,第三个元素tyh,添加第四个元素
                (1)p = tab[i],将p.next 赋值给 e,此时e指向第二个元素
                (2)将e赋值给p(点睛之笔)
                (3)将p.next 赋值给 e,此时e指向第三个元素
                */
                p = e;
            }
        }
        if (e != null) { // existing mapping for key
            V oldValue = e.value;
            if (!onlyIfAbsent || oldValue == null)
                e.value = value;
            afterNodeAccess(e);
            return oldValue;
        }
    }
    ++modCount;
    if (++size > threshold)
        resize();
    afterNodeInsertion(evict);
    return null;
}
8、HashSet扩容机制以及转红黑树机制
(1)HashSet底层为HashMap,第一次添加时table数组扩容到16,临界值(THRESHOLD)为16 * 加载因子(LOADFACTOR) = 12
(2)若table数组使用到临界值12,则扩容到16 * 2 = 32,新的临界值为 32 * 0.75 = 24
(3)每加入一个节点Node(hash,key,value,next),就会++size,当++size > THRESHOLD时,则调用resize()方法进行扩容
(4)在JDK8中,若一条链表的元素个数达到 TREEIFY_THRESHOLD,并且table数组大小 >= MIN_TREEIFY_CAPACITY,则会进化为红黑树,否则继续采用数组扩容机制
    
public class HashSetIncrement {
    public static void main(String[] args) {
        /*
         (1)HashSet底层为HashMap,
            第一次添加时table数组扩容到16,临界值(THRESHOLD)为16 * 加载因子(LOADFACTOR) = 12
         (2)若table数组使用到临界值12,则扩容到16 * 2 = 32,新的临界值为 32 * 0.75 = 24
         (3)依次类推
         (4)数组长度和阈值(临界值)依次扩容两倍!!!!!!
         */
        HashSet hashSet = new HashSet();
        //断点调试查看
        for (int i = 0; i < 100; i++) {
            hashSet.add(i);
        }

        /*
         (1)将hashSet置空
         (2)在JDK8中,若一条链表的元素个数达到 TREEIFY_THRESHOLD(默认为8)
         并且table数组大小 >= MIN_TREEIFY_CAPACITY(默认为64),
         则会进化为红黑树,否则继续采用数组扩容机制
         */
        hashSet = new HashSet();
        /*
         断点调试查看
         (1)元素个数达到 TREEIFY_THRESHOLD(默认为8)时,执行treeifyBin(tab, hash)方法
         (2)若table数组大小未达到64则进行扩容操作
         (3)若table数组大小达到64则进化为红黑树
         */
        for (int i = 0; i < 11; i++) {
            hashSet.add(new Person(i));
        }

        /*
         if (++size > threshold)
            resize();
         (1)++size:每加入一个节点Node(hash,key,value,next),进行一次++size操作
         (2)在table数组索引处或在table数组索引处的链表上加入节点时,都进行++size操作
         */
        //在table数组某一索引处的一条链表上添加了7个Person对象
        hashSet = new HashSet();
        for (int i = 0; i <= 7; i++) {
            hashSet.add(new Person(i));
        }
        //在table数组某一索引处的一条链表上添加了7个Student对象
        for (int i = 0; i <= 7; i++) {
            hashSet.add(new Student(i));
        }
    }
}

class Person {
    private int number;

    public Person(int number) {
        this.number = number;
    }

    /*
     重写hashCode()方法
     (1)演示进化为红黑树过程
     (2)若将数据保存在table数组同一索引处的一条链表上,则需要保证hash值相同
     */
    @Override
    public int hashCode() {
        return 100;
    }
}

class Student {
    private int number;

    public Student(int number) {
        this.number = number;
    }

    @Override
    public int hashCode() {
        return 200;
    }
}
HashSet练习题1（重要！！！）
public class HashSetExercise {
    public static void main(String[] args) {
        HashSet hashSet = new HashSet();
        /*
        若不对hashCode()方法进行重写,则table数组中加入两个元素
        hashSet.add(new Employee("jxs",21));
        hashSet.add(new Employee("jxs",21));
        */

        hashSet.add(new Employee("jxs",21));
        hashSet.add(new Employee("jxs",21));
        hashSet.add(new Employee("dwy",22));
        System.out.println(hashSet);
    }
}

class Employee {
    private String name;
    private int age;

    public Employee(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Employee employee = (Employee) o;
        return age == employee.age && Objects.equals(name, employee.name);
    }

    @Override
    public int hashCode() {
        return Objects.hash(name, age);
    }

    @Override
    public String toString() {
        return "Employee{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }
}
![](E:\Study\自学课程资料\Java\assets\重写equals、hashCode方法步骤1.png)

![](E:\Study\自学课程资料\Java\assets\重写equals、hashCode方法步骤2.png)

![](E:\Study\自学课程资料\Java\assets\重写equals、hashCode方法步骤3.png)

HashSet练习题2（重要重要重要！！！）
public class HashSetExercise {
    public static void main(String[] args) {
        HashSet hashSet = new HashSet();
        hashSet.add(new Employee("jxs",10000.00,new MyDate("2001","2","10")));
        hashSet.add(new Employee("jxs",10000.00,new MyDate("2001","2","10")));
        System.out.println(hashSet);
    }
}

class Employee {
    private String name;
    private double salary;
    private MyDate birthday;

    public Employee(String name, double salary, MyDate birthday) {
        this.name = name;
        this.salary = salary;
        this.birthday = birthday;
    }
    
    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Employee employee = (Employee) o;
        return Objects.equals(name, employee.name) && Objects.equals(birthday, employee.birthday);
    }

    @Override
    public int hashCode() {
        return Objects.hash(name, birthday);
    }

    @Override
    public String toString() {
        return "Employee{" +
                "name='" + name + '\'' +
                ", salary=" + salary +
                ", birthday=" + birthday +
                '}';
    }
}

class MyDate {
    private String year;
    private String month;
    private String day;

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        MyDate myDate = (MyDate) o;
        return Objects.equals(year, myDate.year) && Objects.equals(month, myDate.month) && Objects.equals(day, myDate.day);
    }

    @Override
    public int hashCode() {
        return Objects.hash(year, month, day);
    }

    public MyDate(String year, String month, String day) {
        this.year = year;
        this.month = month;
        this.day = day;
    }

    @Override
    public String toString() {
        return year + "年" + month + "月" + day + "日";
    }
}
为何重写equals方法必须重写hashcode方法
1、equals在Object类中默认判断地址是否相同,重写equals方法,不同对象,属性的值相同时返回true
2、但属性相同,地址不同的对象hash值不同,造成相同的对象散列到不同的位置而造成对象的不能覆盖的问题,所以重写hashCode方法
3、不同对象,属性的值相同时返回相同hash值
LinkedHashSet介绍
1、LinkedHashSet是HashSet的子类

2、LinkedHashSet底层为LinkedHashMap，底层维护了一个数组+双向链表

3、LinkedHashSet根据元素的hashCode值来决定元素的存储位置，同时使用链表维护元素的次序，这使得元素看起来是以插入顺序保存的

4、LinkedHashSet不允许添加重复元素

LinkedHashSet底层机制示意图
1、LinkedHashSet中维护了一个hash表和双向链表（LinkedHashSet有head和tail）

2、每一个节点有before和after属性，即形成双向链表

3、在添加一个元素时，先求得这个元素的hash值，由hash值求得索引值，确定该元素在hashtable数组的位置，然后将添加的元素加入到双向链表（若元素已经存在则不添加）

4、遍历LinkedHashSet能确保插入顺序和遍历顺序一致

![](E:\Study\自学课程资料\Java\assets\LinkedHashSet底层机制示意图.png)

LinkedHashSet源码解读（重要重要！！！）
public class LinkedHashSetSource {
    public static void main(String[] args) {
        Set set = new LinkedHashSet();
        set.add(new String("123"));
        set.add(234);
        set.add(234);
        set.add(new Teacher("jxs",1));
        /*
         1.LinkedHashSet添加元素顺序和取出元素顺序一致
         2.LinkedHashSet底层维护的是LinkedHashMap(HashMap子类)
         3.table数组为HashMap$Node类型
         4.LinkedHashSet存放的节点类型为LinkedHashMap$Entry
         */
        System.out.println(set);
    }
}

class Teacher {
    private String name;
    private int number;

    public Teacher(String name, int number) {
        this.name = name;
        this.number = number;
    }

    @Override
    public String toString() {
        return "Teacher{" +
                "name='" + name + '\'' +
                ", number=" + number +
                '}';
    }
}
table数组为HashMap$Node类型
LinkedHashSet存放的节点类型为LinkedHashMap$Entry

static class Entry<K,V> extends HashMap.Node<K,V> {
    Entry<K,V> before, after;
    Entry(int hash, K key, V value, Node<K,V> next) {
        super(hash, key, value, next);
    }
}
具体源码和HashSet源码解读一样！！！！
LinkedHashSet练习题
public class LinkedHashSetExercise {
    public static void main(String[] args) {
        LinkedHashSet linkedHashSet = new LinkedHashSet();
        linkedHashSet.add(new Car("宝马",1000000.0));
        linkedHashSet.add(new Car("宝马",1000000.0));
        linkedHashSet.add(new Car("奔驰",800000.0));
        System.out.println(linkedHashSet);
    }
}

class Car{
    private String name;
    private double price;

    public Car(String name, double price) {
        this.name = name;
        this.price = price;
    }

    /*
     重写equals、hashCode方法
     1.重写hashCode方法,当name、price相同时返回相同的hashCode值
     2.重写equals方法,当name、price相同时返回true
     */
    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Car car = (Car) o;
        return Double.compare(car.price, price) == 0 && Objects.equals(name, car.name);
    }

    @Override
    public int hashCode() {
        return Objects.hash(name, price);
    }

    @Override
    public String toString() {
        return "Car{" +
                "name='" + name + '\'' +
                ", price=" + price +
                '}';
    }
}
Map接口特点（重点看第7点！！！！）
1、Map与Collection并列存在，用于保存具有映射关系的数据：key-value（双列元素）

2、Map中的key和value可以是任何引用类型的数据，会封装到HashMap$Node对象（table数组）中

3、Map中的key不允许重复，Map中的value允许重复

4、Map中的key可以为null，value也可以为null，key只可有一个null；value可有多个null

5、常用String类作为Map的key

6、key与value之间存在单向一对一关系，即通过指定的key总能找到对应的value

public class Map01 {
    public static void main(String[] args) {
        /*
         Map接口实现类的特点
         */
        Map map = new HashMap();
        /*
        特点1.Map与Collection并列存在
             用于保存具有映射关系的数据：key-value（双列元素）
        特点2.Map中的key和value可以是任何引用类型的数据
             会封装到HashMap$Node对象(table数组)中
         */
        map.put("number1", "jxs");
        map.put("number2", "dwy");
        map.put("number3", "tyh");

        /*
        特点3.Map中的key不允许重复，Map中的value允许重复
             当出现相同的key,会替换原有的key-value
         */
        map.put("number1", "zls");
        map.put("number4", "zls");
        map.put("number5", "zls");

        /*
        特点4.Map中的key可以为null,value也可以为null
             key只可有一个null,value可有多个null
         */
        map.put(null,null);
        map.put(null,"abc");//替换

        /*
        特点5.常用String类作为Map的key
         */
        map.put(1,1);
        map.put(new Object(),new Object());

        /*
        特点6.key与value之间存在单向一对一关系，即通过指定的key总能找到对应的value
        1.通过get()方法,传入一个key,会返回一个对应的value
         */
        System.out.println(map.get(1));
    }
}
7、

一对key-value是存放在一个HashMap$Node节点中的。

因为Node实现了Entry接口，有些书上也说一对key-value就是一个Entry。

public class MapSource {
    public static void main(String[] args) {
        Map map = new HashMap();
        map.put(new Cat("wgw", 1), 1);
        map.put(new Cat("lxz", 2), 2);
        System.out.println(map.getClass());

        /*
         解读:
         1.key-value最后存放在HashSet$Node node = newNode(hash, key, value, null)中
         2.key-value为方便程序员的遍历,会在底层创建EntrySet集合,该集合存放的元素的类型Entry
           一个Entry对象就包含key-value,即EntrySet<Entry<key,value>>
         3.EntrySet中定义的类型是Map.Entry,但实际上存放的还是HashMap$Node
           因为static class Node<K,V> implements Map.Entry<K,V>
           (实现接口的类的对象赋值给接口)
         4.当把HashSet$Node对象存放到entrySet时方便遍历,因为Map.Entry提供了两个重要方法
           K getKey(),V getValue()
         */
        Set set = map.entrySet();
        System.out.println(set.getClass()); // HashMap$EntrySet

        //增强for遍历set集合
        for (Object entry : set) {
            System.out.println(entry.getClass()); // HashMap$Node
            //为了从HashMap$Node中取出key-value,先向下转型,Object类型转为Map.Entry类型
            Map.Entry map_entry = (Map.Entry) entry;
            //取出key-value
            Object key = map_entry.getKey();
            Object value = map_entry.getValue();

            //将map集合中的所有的key封装到set1集合中,将map集合中所有的value封装到collection集合中
            Set set1 = map.keySet();
            Collection collection = map.values();
            System.out.println(set1.getClass()); // HashMap$KeySet
            System.out.println(collection.getClass()); // HashMap$Values
        }
    }
}

class Cat {
    private String name;
    private int age;

    public Cat(String name, int age) {
        this.name = name;
        this.age = age;
    }
}
(白话通俗讲解)Java实现接口的类的对象赋值给接口的理解

废话不多说，先来看一段代码:
//接口
public interface JustInterface {
    void justMethod(Object object);
}

//类实现接口
public class JustInterfaceImpl implements JustInterface{
    @Override
	public void justMethod(Object object) {
		do something…
	}
}

// 在Main.class里可以这样声明和初始化：
public static void main( String[] args ) {
    //实现接口的类的对象赋值给接口
    JustInterface justInterface = new JustInterfaceImpl();
	justInterface.justMethod;
}


对于这段挺正经的面向接口编程的代码，包括我自己，也一直处于似懂非懂的状态，但是具体为什么会出现这种方式，我一定要想清楚才会安心。接下来请允许我用一个很俗的故事来说明这种方式。

故事是这样的，双手受伤的独居宅男，想吃放在面前饭桌上的青椒炒牛肉。我们需要一种方法，最好是人机接口，可以帮助这位宅男不用手轻松吃到青椒炒牛肉。

市面上有一种机械臂，他对外提供了一个人机接口。而接口里面有一个方法，这个方法听起来很符合宅男的要求：夹起机械臂面前的物体-移动到指定坐标点-然后松开。看来只需要把这个机械臂放在饭桌上就行了。

于是双手受伤的独居宅男买了一个机械臂，想通过这个机械臂来吃青椒炒牛肉。整个欢喜的过程如下：

// 在机械臂公司里的组装线是这样的：
public interface 人机接口 {
    void 传递物体(宅男嘴里的位置);	
} 

public class 机械臂 implements 人机接口 {
    @Override
	public void 传递物体(宅男嘴里的位置) {
		夹起机械臂面前的物体；
		移动到 宅男嘴里的位置；
		松开物体；
	}
}

main 函数 {
	人机接口 = new 机械臂;  //宅男准备开始使用带有人机接口的实现了传递物体方法的机械臂
	机械臂.传递物体(宅男嘴里的位置); //机械臂夹起了放在面前的青椒炒牛肉，移动到宅男嘴里的位置，然后松开了青椒炒牛肉。
1、基于接口的匿名内部类:匿名内部类:new 接口(参数列表){类体}
2、编译类型、运行类型
	(1)编译类型:Entry
	(2)运行类型:匿名内部类HashSet$Node
3、底层源码
	(1)系统自动分配类名
	class HashSet$Node implements Map.Entry<K,V> {
    }
	(2)JDK底层在创建匿名内部类 HashSet$Node 后，立即创建了 HashSet$Node类 的对象实例，并且把地址返回给 node。
    HashSet$Node node = newNode(hash, key, value, null)
4、匿名内部类使用一次后就不再使用。
底层源码:
(1)
tab[i] = newNode(hash, key, value, null)

(2)
Node<K,V> newNode(int hash, K key, V value, Node<K,V> next) {
    return new Node<>(hash, key, value, next);
}

(3)
static class Node<K,V> implements Map.Entry<K,V> {
    final int hash;
    final K key;
    V value;
    Node<K,V> next;
    
    Node(int hash, K key, V value, Node<K,V> next) {
        this.hash = hash;
        this.key = key;
        this.value = value;
        this.next = next;
    }
总结:
(1)EntrySet集合中存放的元素类型为Map.Entry
(2)HashMap$Node实现了Map.Entry接口,即可以将实现接口的类的对象赋值给接口
(3)EntrySet中定义的类型是Map.Entry,实际上存放的还是HashMap$Node
(4)Map.Entry提供了两个重要方法K getKey(),V getValue()
(5)所有的key封装在Set集合中,所有的value封装在Collection集合中,key、value实际存储在HashMap$Node节点中,这里只是指向
Map接口方法
public class MapMethod {
    public static void main(String[] args) {
        //添加
        Map map = new HashMap();
        map.put("jxs",new Book("钢铁是怎么炼成的",100));
        map.put("jxs","dwy"); // 替换
        map.put("zls","wgw");
        map.put(null,"lxz");
        System.out.println(map);

        //删除
        map.remove(null);
        System.out.println(map);

        //根据key获取value
        System.out.println(map.get("jxs"));

        //获取元素个数
        System.out.println(map.size());

        //判断集合是否为空
        System.out.println(map.isEmpty());

        //清除集合
        map.clear();
        System.out.println(map);

        //查找key是否存在
        System.out.println(map.containsKey("jxs"));
    }
}

class Book {
    private String name;
    private double price;

    public Book(String name, double price) {
        this.name = name;
        this.price = price;
    }
}
Map六大遍历方式
public class MapFor {
    public static void main(String[] args) {
        Map map = new HashMap();
        map.put("jxs", "dwy");
        map.put("zls", "wgw");

        //取出map集合中所有的key
        Set set = map.keySet();
        //方式1.增强for
        for (Object key : set) {
            System.out.println(key + " " + map.get(key));
        }
        //方式2.迭代器
        Iterator iterator1 = set.iterator();
        while (iterator1.hasNext()) {
            Object next = iterator1.next();
            System.out.println(next + " " + map.get(next));
        }

        Collection collection = map.values();
        //方式3.迭代器取出collection集合中的value
        Iterator iterator2 = collection.iterator();
        while (iterator2.hasNext()) {
            System.out.println(iterator2.next());
        }
        //方式4.增强for取出collection集合中的value
        for (Object value : collection) {
            System.out.println(value);
        }

        //方式5.通过EntrySet获取key-value
        Set entrySet = map.entrySet();
        for (Object entry : entrySet) {
            Map.Entry map_entry = (Map.Entry) entry;
            System.out.println(map_entry.getKey() + " " + map_entry.getValue());
        }

        //方式6.迭代器
        Iterator iterator = entrySet.iterator();
        while (iterator.hasNext()) {
            // next为 Object类,向下转型为Map.Entry,执行getKey、getValue()方法
            Object next = iterator.next();
            Map.Entry map_entry = (Map.Entry) next;
            System.out.println(map_entry.getKey() + " " + map_entry.getValue());
        }
    }
}

/*
输出结果：
zls wgw
jxs dwy
zls wgw
jxs dwy
wgw
dwy
wgw
dwy
zls wgw
jxs dwy
zls wgw
jxs dwy
*/
Map接口课堂练习
public class MapExercise {
    public static void main(String[] args) {
        Staff staff1 = new Staff("jxs", 30000.0, 1);
        Staff staff2 = new Staff("dwy", 20000.0, 2);
        Staff staff3 = new Staff("zls", 1.0, 3);
        HashMap hashMap = new HashMap();
        hashMap.put(staff1.getId(), staff1);
        hashMap.put(staff2.getId(), staff2);
        hashMap.put(staff3.getId(), staff3);
        System.out.println(hashMap);

        //取出hashMap中所有的key
        Set set = hashMap.keySet();
        //迭代器遍历set集合
        Iterator iterator = set.iterator();
        while (iterator.hasNext()) {
            //取出每个key
            Object key = iterator.next();
            Object value = hashMap.get(key);
            Staff value1 = (Staff) value;
            if (value1.getSalary() > 18000) {
                System.out.println(value1);
            }else {

            }
        }

        /*
         比较难的一点
         1.将key-value包装到node节点
         2.将node节点对象赋值给接口entry
         3.entry最后包装到entrySet中
         */
        Set set1 = hashMap.entrySet();
        Iterator iterator1 = set1.iterator();
        while (iterator1.hasNext()) {
            Object entry = iterator1.next();
            //将Object类的entry对象向下转型为Map.Entry类型的对象,从而使用getValue()方法
            Map.Entry map_entry = (Map.Entry) entry;
            Staff value = (Staff) map_entry.getValue();
            if (value.getSalary() > 18000) {
                System.out.println(value);
            }else {

            }
        }
    }
}

class Staff {
    private String name;
    private double salary;
    private int id;

    public Staff(String name, double salary, int id) {
        this.name = name;
        this.salary = salary;
        this.id = id;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public double getSalary() {
        return salary;
    }

    public void setSalary(double salary) {
        this.salary = salary;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    @Override
    public String toString() {
        return "Staff{" +
                "name='" + name + '\'' +
                ", salary=" + salary +
                ", id=" + id +
                '}';
    }
}

/*
输出结果：
{1=Staff{name='jxs', salary=30000.0, id=1}, 2=Staff{name='dwy', salary=20000.0, id=2}, 3=Staff{name='zls', salary=1.0, id=3}}
Staff{name='jxs', salary=30000.0, id=1}
Staff{name='dwy', salary=20000.0, id=2}
Staff{name='jxs', salary=30000.0, id=1}
Staff{name='dwy', salary=20000.0, id=2}
*/
HashMap阶段小结
1、Map接口最常用的3个实现类HashMap、HashTable、Properties

2、HashMap是Map接口使用频率最高的实现类

3、HashMap是以key-value的形式来存储数据的

4、key不可重复，value可重复

5、若添加相同的key，会覆盖原有的key-value

6、与HashSet一样，不保证映射的顺序

7、HashMap没有实现同步，因此线程不安全

HashMap源码解读（重中之重！！！）
1、HashMap底层维护了Node类型的数组table

2、当创建对象时，将加载因子LOADFACTOR初始化为0.75

3、当添加key-value时，通过key的hash值得到在table数组的索引。若索引处没有元素则直接添加；若索引处有元素，则判断将要添加的key和索引处的key是否相等，若相等则直接替换value。若不相等则需要判断是树结构还是链表结构做出相应处理。若添加时发现容量不足则需要扩容

4、第一次扩容，table数组容量为16，临界值THRESHOLD为12

5、再次扩容，则需要扩容table数组容量为原先的2倍，临界值为原先的2倍

6、在JDK8中，若一条链表的元素个数超过TREEIFY_THRESHOLD（树化阈值，默认为8），并且table数组的大小 >= MIN_TREEIFY_CAPACITY（默认为64），就会进行树化（进化为红黑树）。

public class HashMapSource {
    public static void main(String[] args) {
        HashMap hashMap = new HashMap();
        hashMap.put("jxs",10);
        hashMap.put("dwy",10);
        hashMap.put("jxs",20);
        System.out.println(hashMap);
    }
}
1、
(1)初始化加载因子LOADFACTOR=0.75
(2)HashMap$Node[] table = null

public HashMap() {
    this.loadFactor = DEFAULT_LOAD_FACTOR; // all other fields defaulted
}
2、对基本数据类型进行装箱

public static Integer valueOf(int i) {
    if (i >= IntegerCache.low && i <= IntegerCache.high)
        return IntegerCache.cache[i + (-IntegerCache.low)];
    return new Integer(i);
}
3、执行put方法
(1)执行hash(key)方法
(2)执行putVal(hash(key), key, value, false, true)方法

public V put(K key, V value) {
    return putVal(hash(key), key, value, false, true);
}
4、执行hash(key)方法
(1)将key的hashCode值和key的hashCode值无符号右移16位得到的值进行异或运算

static final int hash(Object key) {
int h;
    return (key == null) ? 0 : (h = key.hashCode()) ^ (h >>> 16);
}
5、执行执行putVal(hash(key), key, value, false, true)方法
(1)判断tab数组是否为空,为空则执行resize()方法
(2)由hash值判断对应的table数组的索引位置是否为空,若为空则创建Node节点,将hash-key-value放入此节点
(3)++modCount;记录修改次数
(4)if (++size > threshold)
   	resize();
每在链表或table数组某一索引处加入Node节点,都进行一次++size操作
(5)return null;

final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
               boolean evict) {
    HashMap.Node<K,V>[] tab; HashMap.Node<K,V> p; int n, i;
    if ((tab = table) == null || (n = tab.length) == 0)
        n = (tab = resize()).length;
    if ((p = tab[i = (n - 1) & hash]) == null)
        tab[i] = newNode(hash, key, value, null);
    else {
        HashMap.Node<K,V> e; K k;
        if (p.hash == hash &&
                ((k = p.key) == key || (key != null && key.equals(k))))
            e = p;
        else if (p instanceof TreeNode)
            e = ((HashMap.TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
        else {
            for (int binCount = 0; ; ++binCount) {
                if ((e = p.next) == null) {
                    p.next = newNode(hash, key, value, null);
                    if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
                        treeifyBin(tab, hash);
                    break;
                }
                if (e.hash == hash &&
                        ((k = e.key) == key || (key != null && key.equals(k))))
                    break;
                p = e;
            }
        }
        if (e != null) { // existing mapping for key
            V oldValue = e.value;
            if (!onlyIfAbsent || oldValue == null)
                e.value = value;
            afterNodeAccess(e);
            return oldValue;
        }
    }
    ++modCount;
    if (++size > threshold)
        resize();
    afterNodeInsertion(evict);
    return null;
}
6、执行resize()方法
(1)将table数组赋给oldTab
(2)若oldTab为null则返回0,并将oldTab赋给oldCap
(3)将threshold(临界值,这里为0)赋给oldThr
(4)定义int newCap, newThr = 0;
(5)此时oldCap,oldThr,newCap,newThr = 0
(6)newCap = DEFAULT_INITIAL_CAPACITY;(将默认初始容量16赋给newCap)
(7)newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);(将默认加载因子0.75*默认初始容量16赋给newThr)
(8)threshold = newThr;将newThr赋给threshold(将12赋给临界值)
(9)HashMap.Node<K,V>[] newTab = (HashMap.Node<K,V>[])new HashMap.Node[newCap];(创建一个Node类型的数组,容量为16)
(10)table = newTab;将newTab赋给table
    

final HashMap.Node<K,V>[] resize() {
    HashMap.Node<K,V>[] oldTab = table;
    int oldCap = (oldTab == null) ? 0 : oldTab.length;
    int oldThr = threshold;
    int newCap, newThr = 0;
    if (oldCap > 0) {
        if (oldCap >= MAXIMUM_CAPACITY) {
            threshold = Integer.MAX_VALUE;
            return oldTab;
        }
        else if ((newCap = oldCap << 1) < MAXIMUM_CAPACITY &&
                oldCap >= DEFAULT_INITIAL_CAPACITY)
            newThr = oldThr << 1; // double threshold
    }
    else if (oldThr > 0) // initial capacity was placed in threshold
        newCap = oldThr;
    else {               // zero initial threshold signifies using defaults
        newCap = DEFAULT_INITIAL_CAPACITY;
        newThr = (int)(DEFAULT_LOAD_FACTOR * DEFAULT_INITIAL_CAPACITY);
    }
    if (newThr == 0) {
        float ft = (float)newCap * loadFactor;
        newThr = (newCap < MAXIMUM_CAPACITY && ft < (float)MAXIMUM_CAPACITY ?
                (int)ft : Integer.MAX_VALUE);
    }
    threshold = newThr;
    @SuppressWarnings({"rawtypes","unchecked"})
    HashMap.Node<K,V>[] newTab = (HashMap.Node<K,V>[])new HashMap.Node[newCap];
    table = newTab;
    if (oldTab != null) {
        for (int j = 0; j < oldCap; ++j) {
            HashMap.Node<K,V> e;
            if ((e = oldTab[j]) != null) {
                oldTab[j] = null;
                if (e.next == null)
                    newTab[e.hash & (newCap - 1)] = e;
                else if (e instanceof HashMap.TreeNode)
                    ((HashMap.TreeNode<K,V>)e).split(this, newTab, j, oldCap);
                else { // preserve order
                    HashMap.Node<K,V> loHead = null, loTail = null;
                    HashMap.Node<K,V> hiHead = null, hiTail = null;
                    HashMap.Node<K,V> next;
                    do {
                        next = e.next;
                        if ((e.hash & oldCap) == 0) {
                            if (loTail == null)
                                loHead = e;
                            else
                                loTail.next = e;
                            loTail = e;
                        }
                        else {
                            if (hiTail == null)
                                hiHead = e;
                            else
                                hiTail.next = e;
                            hiTail = e;
                        }
                    } while ((e = next) != null);
                    if (loTail != null) {
                        loTail.next = null;
                        newTab[j] = loHead;
                    }
                    if (hiTail != null) {
                        hiTail.next = null;
                        newTab[j + oldCap] = hiHead;
                    }
                }
            }
        }
    }
    return newTab;
}
7、添加重复元素
(1)进入else代码块
(2)若将要添加的 key的hash值 和 table数组中p索引位置的Node节点的hash值相同 且 将要添加的key 和 table数组中p索引位置的Node节点的key相同 或者 将要添加的key!=null 且 将要添加的key 和 table数组中p索引位置的Node节点的key 内容相同 则将 table数组中p索引位置的Node节点 赋给 辅助变量e
(3)else if、else代码块看HashSet源码解析！！
(4)若e != null,则将 e索引位置的Node节点的value 赋给 oldValue ,将 将要添加的value 赋给 e索引位置Node节点的value
(5)return oldValue;返回oldValue;

final V putVal(int hash, K key, V value, boolean onlyIfAbsent,
               boolean evict) {
    HashMap.Node<K,V>[] tab; HashMap.Node<K,V> p; int n, i;
    if ((tab = table) == null || (n = tab.length) == 0)
        n = (tab = resize()).length;
    if ((p = tab[i = (n - 1) & hash]) == null)
        tab[i] = newNode(hash, key, value, null);
    else {
        HashMap.Node<K,V> e; K k;
        if (p.hash == hash &&
                ((k = p.key) == key || (key != null && key.equals(k))))
            e = p;
        else if (p instanceof TreeNode)
            e = ((HashMap.TreeNode<K,V>)p).putTreeVal(this, tab, hash, key, value);
        else {
            for (int binCount = 0; ; ++binCount) {
                if ((e = p.next) == null) {
                    p.next = newNode(hash, key, value, null);
                    if (binCount >= TREEIFY_THRESHOLD - 1) // -1 for 1st
                        treeifyBin(tab, hash);
                    break;
                }
                if (e.hash == hash &&
                        ((k = e.key) == key || (key != null && key.equals(k))))
                    break;
                p = e;
            }
        }
        if (e != null) { // existing mapping for key
            V oldValue = e.value;
            if (!onlyIfAbsent || oldValue == null)
                e.value = value;
            afterNodeAccess(e);
            return oldValue;
        }
    }
    ++modCount;
    if (++size > threshold)
        resize();
    afterNodeInsertion(evict);
    return null;
}
HashMap底层扩容机制、树化机制
树化机制:table数组容量为64且table数组任意索引处一条链表长度为8时进化为红黑树

扩容机制:
table数组初始容量为16,临界值为12,当数组元素达到临界值时进行扩容
table数组容量扩容为32,临界值为24,以此类推。

注:当一条链表Node节点为8个时,但table数组容量为16时,再次在这条链表加入第9个Node节点时,底层判断机制：(e.hash & oldCap) == 0,即在原来位置的屁股后面直接加入该节点
HashTable基本介绍
1、HashTable存放的元素为key-value

2、HashTable的键和值都不可为null

3、HashTable使用方法基本和HashMap一致

4、HashTable是线程安全的（synchronized），HashMap是线程不安全的

5、HashTable底层为HashTable$Entry数组，初始化大小为11

6、THRESHOLD为8（临界值），LOADFACTOR * 11得到的

7、扩容机制：达到临界值8时，table数组扩容为23（11 * 2 + 1），临界值扩容为17（8 * 2 + 1）

public class HashTableExercise {
    public static void main(String[] args) {
        Hashtable hashtable = new Hashtable();
        hashtable.put("jxs",10);
        hashtable.put("jxs",20);//替换
        //hashtable.put(null,1);//抛出异常NullPointerException
        //hashtable.put(1,null);//抛出异常NullPointerException
        System.out.println(hashtable);
    }
}
HashTable扩容机制
public class HashTableExercise {
    public static void main(String[] args) {
        Hashtable hashtable = new Hashtable();
        hashtable.put("hello1",1);
        hashtable.put("hello2",1);
        hashtable.put("hello3",1);
        hashtable.put("hello4",1);
        hashtable.put("hello5",1);
        hashtable.put("hello6",1);
        hashtable.put("hello7",1);
        hashtable.put("hello8",1);
        hashtable.put("hello9",1);
        hashtable.put("hello10",1);
        System.out.println(hashtable);
    }
}
1、装箱

public static Integer valueOf(int i) {
    if (i >= IntegerCache.low && i <= IntegerCache.high)
        return IntegerCache.cache[i + (-IntegerCache.low)];
    return new Integer(i);
}
2、
(1)进行if判断:if (value == null)则抛出空指针异常
(2)执行addEntry(hash, key, value, index)方法,将key-value封装到Entry
    
public synchronized V put(K key, V value) {
    // Make sure the value is not null
    if (value == null) {
        throw new NullPointerException();
    }

    // Makes sure the key is not already in the hashtable.
    Entry<?,?> tab[] = table;
    int hash = key.hashCode();
    int index = (hash & 0x7FFFFFFF) % tab.length;
    @SuppressWarnings("unchecked")
    Entry<K,V> entry = (Entry<K,V>)tab[index];
    for(; entry != null ; entry = entry.next) {
        if ((entry.hash == hash) && entry.key.equals(key)) {
            V old = entry.value;
            entry.value = value;
            return old;
        }
    }

    addEntry(hash, key, value, index);
    return null;
}
3、执行执行addEntry(hash, key, value, index)方法
(1)执行if判断:if (count >= threshold)
(2)执行rehash()方法

private void addEntry(int hash, K key, V value, int index) {
    modCount++;

    Hashtable.Entry<?,?> tab[] = table;
    if (count >= threshold) {
        // Rehash the table if the threshold is exceeded
        rehash();

        tab = table;
        hash = key.hashCode();
        index = (hash & 0x7FFFFFFF) % tab.length;
    }

    // Creates the new entry.
    @SuppressWarnings("unchecked")
    Hashtable.Entry<K,V> e = (Hashtable.Entry<K,V>) tab[index];
    tab[index] = new Hashtable.Entry<>(hash, key, value, e);
    count++;
}
4、执行rehash()方法
(1)将table数组的长度赋给oldCapacity
(2)将table数组赋给Hashtable.Entry<?,?>[] oldMap
(3)将(oldCapacity << 1) + 1(向右位移几位就乘以2的几次方) 赋给 newCapacity
(4)Hashtable.Entry<?,?>[] newMap = new Hashtable.Entry<?,?>[newCapacity];
(5)modCount++;记录修改次数
(6)threshold = (int)Math.min(newCapacity * loadFactor, MAX_ARRAY_SIZE + 1);
将(newCapacity * loadFactor、MAX_ARRAY_SIZE + 1中小的值赋给threshold(临界值)
(7)table = newMap;将newMap赋给table
    
protected void rehash() {
    int oldCapacity = table.length;
    Hashtable.Entry<?,?>[] oldMap = table;

    // overflow-conscious code
    int newCapacity = (oldCapacity << 1) + 1;
    if (newCapacity - MAX_ARRAY_SIZE > 0) {
        if (oldCapacity == MAX_ARRAY_SIZE)
            // Keep running with MAX_ARRAY_SIZE buckets
            return;
        newCapacity = MAX_ARRAY_SIZE;
    }
    Hashtable.Entry<?,?>[] newMap = new Hashtable.Entry<?,?>[newCapacity];

    modCount++;
    threshold = (int)Math.min(newCapacity * loadFactor, MAX_ARRAY_SIZE + 1);
    table = newMap;

    for (int i = oldCapacity ; i-- > 0 ;) {
        for (Hashtable.Entry<K,V> old = (Hashtable.Entry<K,V>)oldMap[i]; old != null ; ) {
            Hashtable.Entry<K,V> e = old;
            old = old.next;

            int index = (e.hash & 0x7FFFFFFF) % newCapacity;
            e.next = (Hashtable.Entry<K,V>)newMap[index];
            newMap[index] = e;
        }
    }
}
HashTable和HashMap对比
版本	线程安全	效率	允许null键null值
HashMap	1.2	不安全	高	可以
HashTable	1.0	安全	低	不可以
Properties基本介绍
1、Properties类继承自HashTable类并实现了Map接口，也使用键值对的形式保存数据

2、使用特点和HashTable类似

3、Properties可以用于从xxx.properties文件中加载数据到Properties类对象中，并进行读取和修改

4、说明：工作后 xxx.properties文件通常作为配置文件，这个知识点在IO流举例。

public class PropertiesExercise {
    public static void main(String[] args) {
        /*
         1.Properties 继承自 HashTable,实现了 Map接口
         2.可以通过key-value的形式存放数据
         3.key和value不可为null,为空则抛出NullPointerException空指针异常
         */
        Properties properties = new Properties();
        //properties.put(null,1);
        //properties.put(1,null);
        properties.put("jxs",1);
        properties.put("jxs",2);
        properties.put("dwy",1);
        System.out.println(properties);

        //通过key获取对应的value值
        System.out.println(properties.get("jxs"));

        //删
        properties.remove("jxs");
        System.out.println(properties);

        //改
        properties.put("dwy",2);
        System.out.println(properties);
    }
}
集合选型规则
1、判断存储类型（一组对象或一组键值对）

2、若存储类型是一组对象

		（1）List：元素排列有序且元素可重复

				增删操作多：LinkedList（底层维护了数组+双向链表结构）

				改查操作多：ArrayList（底层维护了Object类型的可变数组）

		（2）Set：元素排列无需且元素不可重复

				无序：HashSet（底层维护了数组+链表+红黑树结构）

				排序：TreeSet

				插入元素和取出元素顺序一致：LinkedHashSet（底层维护了数组+双向链表结构）

3、若存储类型是一组键值对

		键无序：HashMap（底层维护了数组+链表+红黑树结构）

		键排序：TreeMap

		键插入和取出顺序一致：LinkedHashMap

		读取文件：Properties

TreeSet源码解读（重要重要重要！！！！！）
public class TreeSetSource {
    public static void main(String[] args) {
        /*
         解读:
         1.当使用无参构造创建TreeSet时进行自然排序
           若添加的元素的所属类实现了Comparable接口则执行compareTo()方法
           若添加的元素的所属类没有实现Comparable接口则抛出类转换异常
         2.当使用有参构造创建TreeSet时可以传入一个比较器对象,进行自定义排序
         */
        TreeSet treeSet = new TreeSet(new Comparator() {
            @Override
            /*
            o1:要比较的第一个对象。
            o2:要比较的第二个对象。

            返回:负整数、零、正整数
                 第一个参数小于、等于、大于第二个参数。

            抛出:
            NullPointerException – 如果参数为空并且此比较器不允许空参数
            ClassCastException – 如果参数的类型阻止它们被此比较器进行比较。
             */
            public int compare(Object o1, Object o2) {
                return ((String) o1).length() - ((String) o2).length();
            }
        });

        treeSet.add("1");
        treeSet.add("12");
        treeSet.add("123");
        treeSet.add("1234");
        treeSet.add("12345");
        
        /*
        1.若User类没有实现Comparable接口
        2.treeSet.add(new User("jxs",21)) 抛出类转换异常
        3.使用treeSet的无参构造时,添加元素会进行自然排序
        4.User类没有实现Comparable接口,无法将类的对象实例赋给Comparable接口,无法进行比较
        5.treeSet.add("aa") 不抛出异常
        6.String类默认实现Comparable接口,可以进行排序
        7.让User类实现Comparable接口,重写compareTo()方法
        8.让调用compareTo()方法的对象和compareTo()方法中传入的形参进行自定义排序比较
         */
        //treeSet.add(new User("jxs",21))
        treeSet.add("aa");

        System.out.println(treeSet);
    }
}

class User implements Comparable {
    private String name;
    private int age;

    public User(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }

    @Override
    public int compareTo(Object o) {
        return this.age - ((User) o).getAge();
    }
}
1、compareTo()方法
(1)String中有属性private final char value[];用于存放字符串内容。
(2)将第一个字符数组的长度赋给len1
(3)将第二个字符数组的长度赋给len2
(4)用Math类的min方法返回len1、len2之间的最小值
(5)将第一个字符数组value赋给char v1[],将第二个字符数组赋给char v2[]
(6)while循环,将字符数组中的值一个个字符取出比较
(7)若有字符不相等,则返回c1 - c2(ASCII码差值)
(8)根据返回的值再进行排序

public int compareTo(String anotherString) {
    int len1 = value.length;
    int len2 = anotherString.value.length;
    int lim = Math.min(len1, len2);
    char v1[] = value;
    char v2[] = anotherString.value;

    int k = 0;
    while (k < lim) {
        char c1 = v1[k];
        char c2 = v2[k];
        if (c1 != c2) {
            return c1 - c2;
        }
        k++;
    }
    return len1 - len2;
}
2、构造器
(1)传入一个实现Comparator接口的匿名对象
(2)调用TreeMap构造器
(3)将传入的实现Comparator接口的匿名对象赋给TreeMap的一个属性comparator

public TreeSet(Comparator<? super E> comparator) {
    this(new TreeMap<>(comparator));
}
    
public TreeMap(Comparator<? super K> comparator) {
    this.comparator = comparator;
}
3、执行put()方法

public boolean add(E e) {
    return m.put(e, PRESENT)==null;
}
4、执行put()方法
(1)将传入的实现Comparator接口的匿名对象赋给Comparator<? super K> cpr
(2)执行if判断:if (cpr != null)
(3)执行cmp = cpr.compare(key, t.key);会动态绑定到我们传入的实现Comparator接口的匿名对象的compare()方法
(4)cmp = cpr.compare(key, t.key);将调用compare()方法得到的值赋给cmp
(5)若cmp < 0则执行t = t.left,反之执行t = t.right
    
public V put(K key, V value) {
    TreeMap.Entry<K,V> t = root;
    if (t == null) {
        compare(key, key); // type (and possibly null) check

        root = new TreeMap.Entry<>(key, value, null);
        size = 1;
        modCount++;
        return null;
    }
    int cmp;
    TreeMap.Entry<K,V> parent;
    // split comparator and comparable paths
    Comparator<? super K> cpr = comparator;
    if (cpr != null) {
        do {
            parent = t;
            cmp = cpr.compare(key, t.key);
            if (cmp < 0)
                t = t.left;
            else if (cmp > 0)
                t = t.right;
            else
                return t.setValue(value);
        } while (t != null);
    }
    else {
        if (key == null)
            throw new NullPointerException();
        @SuppressWarnings("unchecked")
        Comparable<? super K> k = (Comparable<? super K>) key;
        do {
            parent = t;
            cmp = k.compareTo(t.key);
            if (cmp < 0)
                t = t.left;
            else if (cmp > 0)
                t = t.right;
            else
                return t.setValue(value);
        } while (t != null);
    }
    TreeMap.Entry<K,V> e = new TreeMap.Entry<>(key, value, parent);
    if (cmp < 0)
        parent.left = e;
    else
        parent.right = e;
    fixAfterInsertion(e);
    size++;
    modCount++;
    return null;
}
TreeMap源码解读
public class TreeMapSource {
    public static void main(String[] args) {
        /*
        1.当使用无参构造器的时候，TreeMap默认按照key值进行自然排序
          若添加的元素的所属类没有实现Comparable接口,则抛出类转换异常
          若添加的元素的所属类实现了Comparable接口则执行compareTo()方法进行排序
        2.当使用有参构造器的时候，TreeMap可以传入一个比较器对象,进行自定义排序
          使用有参构造器的场景:元素的key支持Comparable但自然排序不满足调用者要求，需要自定义
        3.基于接口的匿名内部类
          系统自动分配类名TreeMapSource$1后立即创建TreeMapSource$1对象
          并将TreeMapSource$1对象赋给匿名对象
         */
        
        TreeMap treeMap = new TreeMap(new Comparator() {
            @Override
            public int compare(Object o1, Object o2) {
                //使用String类的compareTo()方法比较两个字符串之间的大小
                return ((String) o1).compareTo((String) o2);
            }
        });
        
        treeMap.put("aaa", "123");
        treeMap.put("ccc", "123");
        treeMap.put("bbb", "123");
        treeMap.put("ddd", "123");
        System.out.println(treeMap);
    }
}
1、执行TreeMap构造器
(1)将传入的实现Comparator接口的匿名对象赋给TreeMap的一个属性comparator

public TreeMap(Comparator<? super K> comparator) {
    this.comparator = comparator;
}
2、执行put()方法
(1)加入第一个元素时,root默认为null
static final class Entry<K,V> implements Map.Entry<K,V>{...}
private transient Entry<K,V> root;
(2)执行if判断:if (t == null),执行if代码块,compare(key, key)会动态绑定到匿名对象的compare()方法
(3)加入第二个元素时,root默认为上一个元素,将root赋给TreeMap.Entry<K,V> t
(4)定义辅助变量int cmp;TreeMap.Entry<K,V> parent;
(5)将传入的实现Comparator接口的匿名对象赋给cpr
(6)执行if判断:if (cpr != null)
(7)将t赋给parent,因为root默认为上一个元素,将root赋给TreeMap.Entry<K,V> t,因此t指向上一个元素
(8)cmp = cpr.compare(key, t.key);将第二个元素的key和上一个元素的key进行比较,这时compare会进行动态绑定,绑定到匿名对象的compare()方法,将输出的结果赋给cmp
(9)最后执行if判断:若cmp < 0则执行t = t.left;若cmp > 0则执行t = t.right;若cmp = 0则返回t.setValue(value)

public V put(K key, V value) {
    TreeMap.Entry<K,V> t = root;
    if (t == null) {
        compare(key, key); // type (and possibly null) check

        root = new TreeMap.Entry<>(key, value, null);
        size = 1;
        modCount++;
        return null;
    }
    int cmp;
    TreeMap.Entry<K,V> parent;
    // split comparator and comparable paths
    Comparator<? super K> cpr = comparator;
    if (cpr != null) {
        do {
            parent = t;
            cmp = cpr.compare(key, t.key);
            if (cmp < 0)
                t = t.left;
            else if (cmp > 0)
                t = t.right;
            else
                return t.setValue(value);
        } while (t != null);
    }
    else {
        if (key == null)
            throw new NullPointerException();
        @SuppressWarnings("unchecked")
        Comparable<? super K> k = (Comparable<? super K>) key;
        do {
            parent = t;
            cmp = k.compareTo(t.key);
            if (cmp < 0)
                t = t.left;
            else if (cmp > 0)
                t = t.right;
            else
                return t.setValue(value);
        } while (t != null);
    }
    TreeMap.Entry<K,V> e = new TreeMap.Entry<>(key, value, parent);
    if (cmp < 0)
        parent.left = e;
    else
        parent.right = e;
    fixAfterInsertion(e);
    size++;
    modCount++;
    return null;
}
Comparator和Comparable区别
Comparable接口
(1)Comparable接口依附于实体类
(2)若一个类实现了Comparable接口,该类支持排序,需重写compareTo()方法
(3)实现Comparable接口的类的对象的列表或数组可以通过Collections.sort或Arrays.sort进行自动排序。(重要！！！)
(4)实现此接口的对象可以用作有序映射中的键或有序集合中的集合,无需指定比较器。

Comparator接口
(1)Comparator接口一般匿名内部类来实现,实现业务逻辑的比较,且只比较1次
(2)传入两个参数,第一个参数大于、等于、小于第二个参数则分别返回正整数、0、负整数
Collections工具类
1、Collections是操作Set、List、Map等集合的工具类

2、Collections中提供了一系列静态的方法对集合元素进行排序、查询和修改等操作

public class Collections01 {
    public static void main(String[] args) {
        ArrayList arrayList = new ArrayList();
        arrayList.add("tom");
        arrayList.add("smith");
        arrayList.add("king");
        arrayList.add("milan");
        arrayList.add("tom");

        //反转List中元素的顺序
        Collections.reverse(arrayList);
        System.out.println(arrayList);

        //集合元素进行随机排序
        Collections.shuffle(arrayList);
        System.out.println(arrayList);

        //根据自然排序(按字符串首字母从小到大排序)对指定的List进行升序排序
        Collections.sort(arrayList);
        System.out.println(arrayList);

        //自定义排序(重写匿名内部类),按照字符串长度进行排序
        Collections.sort(arrayList, new Comparator<Object>() {
            @Override
            public int compare(Object o1, Object o2) {
                return ((String) o1).length() - ((String) o2).length();
            }
        });
        System.out.println(arrayList);

        //将指定List集合中i处元素和j处元素进行交换
        Collections.swap(arrayList, 1, 2);
        System.out.println(arrayList);

        //根据元素的自然排序返回指定集合中的最大值
        System.out.println(Collections.max(arrayList));

        //返回集合中长度最大的元素
        Object max = Collections.max(arrayList, new Comparator() {
            @Override
            public int compare(Object o1, Object o2) {
                return ((String) o1).length() - ((String) o2).length();
            }
        });
        System.out.println(max);

        //根据元素的自然排序返回指定集合中的最小值
        System.out.println(Collections.min(arrayList));

        //返回指定集合中长度最小的元素
        Object min = Collections.min(arrayList, new Comparator<Object>() {
            @Override
            public int compare(Object o1, Object o2) {
                return ((String) o1).length() - ((String) o2).length();
            }
        });
        System.out.println(min);

        //返回指定集合中指定元素出现的次数
        System.out.println(Collections.frequency(arrayList, "tom"));

        //将src集合的元素拷贝到到dest集合
        ArrayList src = new ArrayList();
        src.add("jxs");
        src.add("dwy");
        ArrayList dest = new ArrayList();
        /*
         1.若源集合的长度大于目标集合的长度则抛出数组越界异常
         2.为完成一个完整的拷贝,需要先给dest目标集合赋值,让目标集合的长度和源集合的长度一致
         */
        for (int i = 0; i < src.size(); i++) {
            dest.add("");
        }
        Collections.copy(dest, src);
        System.out.println(dest);

        //使用新值替换指定集合中的所有的旧值
        Collections.replaceAll(arrayList,"tom","蒋兴树");
        System.out.println(arrayList);
    }
}
集合总练习（每条都是重点！！！）
第一题
1.封装一个新闻类，包含标题和内容属性，提供get、set方法，重写toString方法，打印对象时只打印标题
2.只提供一个带参数的构造器，实例化对象时，只初始化标题
3.实例化两个对象:
新闻一:新冠确诊病例超千万，数百万印度教信徒赴恒河“圣浴”引民众担忧
新闻二:男子突然想起2个月前钓的鱼还在网兜里，捞起一看赶紧放生
4.将新闻对象添加到ArrayList集合中，并且进行倒序遍历;
5.在遍历集合过程中，对新闻标题进行处理，超过15字的只保留前15个，然后在后边加“…"
6.在控制台打印遍历出经过处理的新闻标题;
public class Homework01 {
    public static void main(String[] args) {
        News news1 = new News("新冠确诊病例超千万，数百万印度教信徒赴恒河“圣浴”引民众担忧");
        News news2 = new News("男子突然想起2个月前钓的鱼还在网兜里，捞起一看赶紧放生");
        ArrayList arrayList = new ArrayList();
        arrayList.add(news1);
        arrayList.add(news2);
        Collections.reverse(arrayList);
        for (Object o : arrayList) {
            News n = (News) o;
            if (n.getTopic().length() >= 15) {
                n.setTopic(n.getTopic().substring(0,15) + "...");
            }
            System.out.println(n.getTopic());
        }

    }
}

class News {
    private String topic;
    private String content;

    public News(String topic) {
        this.topic = topic;
    }

    public String getTopic() {
        return topic;
    }

    public void setTopic(String topic) {
        this.topic = topic;
    }

    public String getContent() {
        return content;
    }

    public void setContent(String content) {
        this.content = content;
    }

    @Override
    public String toString() {
        return "News{" +
                "topic='" + topic + '\'' +
                '}';
    }
}
第二题
使用ArrayList完成对对象Car{name, price}的各种操作
1.add:添加单个元素
2.remove:删除指定元素
3.contains:查找元素是否存在
4.size:获取元素个数
5.isEmpty:判断是否为空
6.clear:清空
7.addAll:添加多个元素
8.containsAll:查找多个元素是否都存在
9.removeAll:删除多个元素
10.使用增强for和迭代器来遍历所有的car，需要重写Car 的toString方法
public class Homework02 {
    public static void main(String[] args) {
        Car car1 = new Car("宝马",200000.0);
        Car car2 = new Car("奔驰",300000.0);
        ArrayList arrayList = new ArrayList();
        //增
        arrayList.add(car1);
        arrayList.add(car2);
        //删
        arrayList.remove(car1);
        //集合是否包含某个元素
        System.out.println(arrayList.contains(car1));
        //集合大小
        System.out.println(arrayList.size());
        //集合是否为空
        System.out.println(arrayList.isEmpty());
        //清空集合
        arrayList.clear();
        //添加多个元素
        ArrayList arrayList1 = new ArrayList();
        arrayList1.add(new Car("梅赛德斯",2000000.0));
        arrayList.addAll(arrayList1);
        System.out.println(arrayList);
        //删除多个元素
        arrayList.removeAll(arrayList1);
        System.out.println(arrayList);

        arrayList.add(car1);
        arrayList.add(car2);
        System.out.println("====迭代器====");
        Iterator iterator = arrayList.iterator();
        while (iterator.hasNext()) {
            System.out.println(iterator.next());
        }

        System.out.println("====增强for====");
        for (Object o : arrayList) {
            System.out.println(o);
        }
    }
}

class Car {
    private String name;
    private double price;

    public Car(String name, double price) {
        this.name = name;
        this.price = price;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public double getPrice() {
        return price;
    }

    public void setPrice(double price) {
        this.price = price;
    }

    @Override
    public String toString() {
        return "Car{" +
                "name='" + name + '\'' +
                ", price=" + price +
                '}';
    }
}
第三题
按要求完成下列任务
1.使用HashMap类实例化一个Map类型的对象m
键(String）和值(int)分别用于存储员工的姓名和工资
存入数据如下:jack—650元; tom—1200元; smith——2900元;
2.将jack的工资更改为2600元
3.为所有员工工资加薪100元
4.遍历集合中所有的员工
5.遍历集合中所有的工资
public class Homework03 {
    public static void main(String[] args) {
        HashMap hashMap = new HashMap();
        //注意:int会自动装箱为Integer
        hashMap.put("jack", 650);
        hashMap.put("tom", 1200);
        hashMap.put("smith", 2900);
        System.out.println(hashMap);

        //改
        hashMap.put("jack", 2600);

        //为所有员工加薪100
        Set set2 = hashMap.keySet();
        for (Object key : set2) {
            hashMap.put(key, (Integer) hashMap.get(key) + 100);
        }

        //遍历所有员工
        Set set = hashMap.keySet();
        Iterator iterator = set.iterator();
        while (iterator.hasNext()) {
            Object key = iterator.next();
            Object value = hashMap.get(key);
            System.out.println(key + " " + value);
        }

        for (Object o : set) {
            Object value = hashMap.get(o);
            System.out.println(o + " " + value);
        }

        /*
         1.entry存放在entrySet中
         2.遍历entrySet取出entry
         3.key-value实际存储在node节点中
         4.key-value的引用存放在entry中
         5.遍历entrySet取出的entry为Object类型,向下转型为Map.Entry
         6.调用entry的方法getKey、getValue获取键和值
         */
        Set set1 = hashMap.entrySet();
        for (Object o : set1) {
            Map.Entry keyValue = (Map.Entry) o;
            Object key = keyValue.getKey();
            Object value = keyValue.getValue();
            System.out.println(key + " " + value);
        }

        Iterator iterator1 = set1.iterator();
        while (iterator1.hasNext()) {
            Object next = iterator1.next();
            Map.Entry keyValue = (Map.Entry) next;
            Object key = keyValue.getKey();
            Object value = keyValue.getValue();
            System.out.println(key + " " + value);
        }
    }
}
第四题（重点！！）
HashSet实现去重:
(1)HashSet会根据传入的key得到hash值,再由hash值得到存放在table数组的哪个索引处
(2)若将要添加的元素的hash值和索引处node节点的hash值相同,且将要添加的元素的key和索引处node节点的key相同则直接覆盖
(3)若将要添加的元素的hash值和索引处node节点的hash值相同,且将要添加的元素的key.equals(索引处node节点的key)为true则直接覆盖
TreeSet实现去重:
(1)若传入了一个实现了Comparator接口的匿名对象,则将实现了Comparator接口的匿名对象赋给TreeMap的一个属性comparator
(2)传入第一个元素时,执行compare(key, key)方法,compare(key, key)方法会动态绑定到匿名对象的compare()方法
(3)传入第二个元素时,执行compare(key, t.key),也会动态绑定到匿名对象的compare()方法,将将要添加的key和之前添加的元素的key一一比较,若compare()方法返回0,则认为是相同的元素,就不进行添加。
(4)若没有传入匿名对象,则以你传入的对象实现的Compareable接口的compareTo()方法去重
public int compareTo(String anotherString) {
    int len1 = value.length;
    int len2 = anotherString.value.length;
    int lim = Math.min(len1, len2);
    char v1[] = value;
    char v2[] = anotherString.value;

    int k = 0;
    while (k < lim) {
        char c1 = v1[k];
        char c2 = v2[k];
        if (c1 != c2) {
            return c1 - c2;
        }
        k++;
    }
    return len1 - len2;
}
第五题
public class Homework04 {
    public static void main(String[] args) {
        /*
         会抛异常吗？
         会！
         1.Person类没有实现Comparable接口
         2.没有传入实现Comparator接口的匿名对象
         */
        TreeSet treeSet = new TreeSet();
        treeSet.add(new Person());
    }
}

class Person {
}
第六题（重点！！！）
已知:Student类按照number和name重写了hashCode和equals方法,问下面代码输出什么?
解析:
(1)最关键的地方:hashSet.remove(student1)
(2)无法删除student1对象
(3)修改了student1对象的属性name,hash值也随之改变
(4)重写的hashCode()方法源码:
@Override
public int hashCode() {
    return Objects.hash(number, name);
}

public static int hash(Object... values) {
    return Arrays.hashCode(values);
}

public static int hashCode(Object a[]) {
    if (a == null)
        return 0;
    
    int result = 1;
    for (Object element : a)
        result = 31 * result + (element == null ? 0 : element.hashCode());
    return result;
}
(5)
当第一次添加student1对象时,假设将student1对象添加到索引为1的位置
随后修改了student1对象的属性name
重写的hashCode是根据student1对象的key和value计算出的值,所以更改value后,student1索引位置改变,即删除失败
public class Homework05 {
    public static void main(String[] args) {
        HashSet hashSet = new HashSet();
        Student student1 = new Student(1001,"jxs");
        Student student2 = new Student(1002,"dwy");
        hashSet.add(student1);
        hashSet.add(student2);

        student1.name = "j";
        hashSet.remove(student1);
        /*
        此时集合中已有的元素(1001,"j")、(1002,"dwy")
        */
        hashSet.add(new Student(1001,"tyh"));
        
        hashSet.add(new Student(1001,"jxs"));
        System.out.println(hashSet);
    }
}

class Student {
    public int number;
    public String name;

    public Student(int number, String name) {
        this.number = number;
        this.name = name;
    }

    @Override
    public String toString() {
        return "Student{" +
                "number=" + number +
                ", name='" + name + '\'' +
                '}';
    }

    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Student student = (Student) o;
        return number == student.number && Objects.equals(name, student.name);
    }

    @Override
    public int hashCode() {
        return Objects.hash(number, name);
    }
}

/*
输出结果：
[Student{number=1001, name='tyh'}, Student{number=1001, name='j'}, Student{number=1002, name='dwy'}, Student{number=1001, name='jxs'}]
*/
1.2.6、泛型
泛型引入
传统方法
public class generic {
    public static void main(String[] args) {
        ArrayList arrayList = new ArrayList();
        arrayList.add(new Dog("hua", 1));
        arrayList.add(new Dog("bai", 2));
        arrayList.add(new Dog("hei", 3));

        arrayList.add(new Cat("hong",4));
        for (Object dogs : arrayList) {
            /*
             1.为调用Dog类的getName()方法需向下转型 Object -> Dog
             2.极端情况下:若程序员不小心在arrayList集合中添加了Cat类对象
             3.Dog dog = (Dog) dogs则会抛出类型转换异常

             4.从而引出泛型
                (1)不能对加入到集合中的数据类型进行约束
                (2)遍历集合时,需要进行类型转换,若集合中数据量较大,对效率有影响
             */
            Dog dog = (Dog) dogs;
            System.out.println(dog.getName());
        }
    }
}

class Dog {
    private String name;
    private int age;

    public Dog(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}

class Cat {
    private String name;
    private int age;

    public Cat(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}
引入泛型
public class generic01 {
    public static void main(String[] args) {
        ArrayList<Dog> dogs = new ArrayList<Dog>();
        dogs.add(new Dog("bai",1));
        dogs.add(new Dog("hei",2));
        dogs.add(new Dog("hong",3));

        /*
        dogs.add(new Cat("hong",3));
        1.ArrayList<Dog>表示我们存放到集合中的元素是Dog类型
        2.若编译器发现添加的类型不满足要求则会报错(约束数据类型)
        3.遍历集合时可以直接取出数据类型
         */
        for (Dog dog : dogs) {
            System.out.println(dog.getName());
        }

    }
}

class Dog {
    private String name;
    private int age;

    public Dog(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}

class Cat {
    private String name;
    private int age;

    public Cat(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}
总结:
(1)若不使用泛型,假设在集合中添加Dog类型的对象,使用迭代器、增强for循环遍历集合后返回的为Object类型的对象,需要向下转型为Dog类型,才能调用Dog类型对象的方法
(2)使用泛型对集合进行数据类型的约束,让其只能添加Dog类型的对象,使用迭代器、增强for循环遍历集合后返回的为Dog类型的对象,不必进行向下转型就可调用Dog类型对象的方法

泛型的好处
(1)编译时,检查添加元素的类型,提高了安全性
(2)减少了数据类型转换的次数,提高效率
(3)不再提示编译警告
泛型介绍
1、泛型即可以表示数据类型的数据类型

2、泛型又称参数化类型，是JDK5.0出现的新特性

3、泛型解决数据类型的安全性问题

4、在类声明或实例化时只要指定好需要的具体的类型即可

5、Java泛型可以保证若程序在编译时没有发出警告，运行时就不会产生ClassCastException异常。代码也更加简洁、健壮

6、泛型作用：可以在类声明时通过一个标识表示类中某个属性的类型，或者是某个方法的返回值的类型，或者是参数类型

public class Generic02 {
    public static void main(String[] args) {

        //1.定义Person对象时指定泛型具体是什么数据类型
        Person<String> person1 = new Person<>("jxs");
        person1.method2();
        Person<Integer> person2 = new Person<>(100);
        person2.method2();
        Person<Double> person3 = new Person<>(100.0);
        person3.method2();
    }
}

/*
1.声明一个类时,通过一个标识来表示类中某个属性的数据类型
2.声明一个类时,通过一个标识来表示参数类型
3.声明一个类时,通过一个标识来表示某个方法的返回值的类型
 */
class Person<E> {
    //E表示一个数据类型,是定义Person对象时指定的,即在编译期间确定E是什么类型
    E datatype;

    public Person(E datatype) {
        this.datatype = datatype;
    }

    public E method1() {
        return datatype;
    }

    public void method2() {
        System.out.println(datatype.getClass());
    }
}

/*
输出结果：
class java.lang.String
class java.lang.Integer
class java.lang.Double
*/
总结:
泛型所谓即在声明一个类时,通过一个标识来指定类中某个属性的数据类型,或者参数的数据类型,或者返回值的数据类型。在创建这个类的对象实例时才确定泛型具体是什么数据类型。
泛型的语法
1、泛型的声明
interface 接口<T> {}
class 类<K,V> {}
说明:T、K、V不代表值,代表数据类型
泛型语法理解练习（看总结！！！）
1、创建3个学生对象
2、将学生对象放入到HashSet集合中,使用使用两种方式遍历
3、将学生对象放入到HashMap集合中,Key为String name,Value为学生对象,使用使用两种方式遍历
public class GenericExercise {
    public static void main(String[] args) {
        Student<String, Integer> jxs = new Student<>("jxs", 21);
        Student<String, Integer> dwy = new Student<>("dwy", 21);
        Student<String, Integer> tyh = new Student<>("tyh", 21);

        HashSet<Student> students = new HashSet<>();
        students.add(jxs);
        students.add(dwy);
        students.add(tyh);

        System.out.println("====迭代器====");
        Iterator<Student> iterator = students.iterator();
        while (iterator.hasNext()) {
            System.out.println(iterator.next());
        }
        System.out.println("====增强for====");
        for (Student student : students) {
            System.out.println(student);
        }


        HashMap<String, Student> hashMap = new HashMap<>();
        hashMap.put("jxs",jxs);
        hashMap.put("dwy",dwy);
        hashMap.put("tyh",tyh);

        System.out.println("====entrySet====");
        Set<Map.Entry<String, Student>> entries = hashMap.entrySet();
        Iterator<Map.Entry<String, Student>> iterator1 = entries.iterator();
        while(iterator1.hasNext()) {
            Map.Entry<String, Student> next = iterator1.next();
            String key = next.getKey();
            Student value = next.getValue();
            System.out.println(key + " " + value);
        }
    }
}

class Student<K, V> {
    private K name;
    private V age;

    public Student(K name, V age) {
        this.name = name;
        this.age = age;
    }

    public K getName() {
        return name;
    }
    public void setName(K name) {
        this.name = name;
    }
    public V getAge() {
        return age;
    }
    public void setAge(V age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "Student{" +
                "name=" + name +
                ", age=" + age +
                '}';
    }
}

/*
输出结果：
====迭代器====
Student{name=tyh, age=21}
Student{name=dwy, age=21}
Student{name=jxs, age=21}
====增强for====
Student{name=tyh, age=21}
Student{name=dwy, age=21}
Student{name=jxs, age=21}
====entrySet====
tyh Student{name=tyh, age=21}
jxs Student{name=jxs, age=21}
dwy Student{name=dwy, age=21}
*/
总结:
(1)声明一个类,class Student<K,V> {}
(2)将这个类的属性的数据类型分为定义为K,V
(3)创建这个类的对象实例时确定泛型的具体数据类型
Student<String, Integer> jxs = new Student<>("jxs", 21);
(4)创建一个泛型为<Student>的集合hashSet,集合中只可存放Student数据类型的元素
(5)利用迭代器或增强for循环取出hashSet集合中的元素,因为hashSet集合指定了泛型,所以取出的元素数据类型不为Object类型,而为Student类

(6)创建一个泛型为<String,Student>的集合hashMap
(7)key的数据类型为String,value的数据类型为Student
(8)key-value实际保存在table数组的Node节点中,Map.entry中存放key-value的引用,Map.entry存放在entrySet中
(9)Set<Map.Entry<String, Student>> entries = hashMap.entrySet()
(10)利用增强for循环或迭代器遍历entries,取出一个个Map.Entry
(11)再利用Map.Entry的getKey()、getValue()方法得到键值对
泛型细节
1、泛型只能为引用类型

2、在指定泛型的具体类型后，可以传入该类型或者该类型的子类类型

public class GenericDetail {
    public static void main(String[] args) {
        Test<Animal> animalTest1 = new Test<Animal>(new Animal());
        Test<Animal> animalTest2 = new Test<Animal>(new Dog());
    }
}

class Test<E> {
    E name;

    public Test(E name) {
        this.name = name;
    }
}

class Animal {
}

class Dog extends Animal{
}
(1)定义了一个Test类
(2)创建Test类实例对象时,指定泛型为Animal类型,即属性name为Animal类型,传入的参数为Animal类型
(3)Dog类继承了Animal类,所以传入的参数也可以为Dog类型
3、泛型的使用形式

//编译器会进行类型推断,推荐第一种写法
(1)ArrayList<Integer> arrayList1 = new ArrayList<>();
(2)ArrayList<Integer> arrayList2 = new ArrayList<Integer>();
4、若不指定泛型的具体类型，则默认为Tiger<Object> Tiger = new Tiger<Object>()

public class GenericDetail01 {
    public static void main(String[] args) {
        Tiger tiger = new Tiger();
    }
}

class Tiger<E>{
    E name;

    public Tiger() { }
}
ArrayList arrayList1 = new ArrayList();
默认为:ArrayList<Object> arrayList2 = new ArrayList<Object>();
泛型课堂练习（看总结！！！）
1、定义Employee类,该类包含:private成员变量name,sal,birthday,其中birthday为MyDate类的对象
2、为每一个属性定义getter,setter方法
3、重写toString方法输出name,sal,birthday
4、MyDate类包含:private成员变量month,day,year
5、为每一个属性定义getter,setter方法;
5、创建该类的3个对象,并把这些对象放入ArrayList集合中(ArrayList需使用泛型来定义),对集合中的元素进行排序,并遍历输出:
排序方式:调用ArrayList的sort方法,传入 Comparator对象[使用泛型],先按照name排序,如果name相同,则按生日日期的先后排序。[即:定制排序]
总结:
(1)调用ArrayList的sort方法,传入实现Comparator接口的匿名对象
(2)o1.getName().compareTo(o2.getName()),调用compareTo()方法对o1的name和o2的name进行比较
(3)将生日日期的排序的方法封装到MyDate类中
(4)MyDate类实现Comparable<MyDate>接口,指定泛型为MyDate类型,即传入的参数也为MyDate类型
(5)MyDate类中重写compareTo()方法

Comparable 自然排序(实体类实现)
Comparator 定制排序(无法修改实体类时，直接在方法中创建实现该接口的匿名对象)
public class GenericExercise {
    public static void main(String[] args) {

        Employee dagy = new Employee("dagy", 10000.0, new MyDate(2001, 2, 10));
        Employee jxs = new Employee("jxs", 10000.0, new MyDate(2001, 2, 10));
        Employee dwy = new Employee("dwy", 10000.0, new MyDate(2000, 7, 13));

        ArrayList<Employee> employees = new ArrayList<>();

        employees.add(jxs);
        employees.add(dwy);
        employees.add(dagy);


        employees.sort(new Comparator<Employee>() {
            @Override
            public int compare(Employee o1, Employee o2) {

                int i = o1.getName().compareTo(o2.getName());
                if (i != 0) {
                    return i;
                }
                return o1.getBirthday().compareTo(o2.getBirthday());
            }
        });


        System.out.println(employees);
    }
}

class Employee {
    private String name;
    private double salary;
    private MyDate birthday;

    public Employee(String name, double salary, MyDate birthday) {
        this.name = name;
        this.salary = salary;
        this.birthday = birthday;
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public double getSalary() {
        return salary;
    }
    public void setSalary(double salary) {
        this.salary = salary;
    }
    public MyDate getBirthday() {
        return birthday;
    }
    public void setBirthday(MyDate birthday) {
        this.birthday = birthday;
    }

    @Override
    public String toString() {
        return "\nEmployee{" +
                "name='" + name + '\'' +
                ", salary=" + salary +
                ", birthday=" + birthday +
                '}';
    }
}

class MyDate implements Comparable<MyDate> {
    private int year;
    private int month;
    private int day;

    public MyDate(int year, int month, int day) {
        this.year = year;
        this.month = month;
        this.day = day;
    }

    public int getYear() {
        return year;
    }
    public void setYear(int year) {
        this.year = year;
    }
    public int getMonth() {
        return month;
    }
    public void setMonth(int month) {
        this.month = month;
    }
    public int getDay() {
        return day;
    }
    public void setDay(int day) {
        this.day = day;
    }

    @Override
    public String toString() {
        return "MyDate{" +
                "year=" + year +
                ", month=" + month +
                ", day=" + day +
                '}';
    }

    @Override
    public int compareTo(MyDate o) {
        int i1 = year - o.getYear();
        if (i1 != 0) {
            return i1;
        }

        int i2 = month - o.getMonth();
        if (i2 != 0) {
            return i2;
        }

        return day - o.getDay();
    }
}

/*
输出结果：
[
Employee{name='dagy', salary=10000.0, birthday=MyDate{year=2001, month=2, day=10}}, 
Employee{name='dwy', salary=10000.0, birthday=MyDate{year=2000, month=7, day=13}}, 
Employee{name='jxs', salary=10000.0, birthday=MyDate{year=2001, month=2, day=10}}]
*/
重点代码:
employees.sort(new Comparator<Employee>() {
    @Override
    public int compare(Employee o1, Employee o2) {

        int i = o1.getName().compareTo(o2.getName());
        if (i != 0) {
            return i;
        }
        return o1.getBirthday().compareTo(o2.getBirthday());
    }
});

@Override
public int compareTo(MyDate o) {
    int i1 = year - o.getYear();
    if (i1 != 0) {
        return i1;
    }

    int i2 = month - o.getMonth();
    if (i2 != 0) {
        return i2;
    }

    return day - o.getDay();
}
自定义泛型类
1、基本语法

class 类名<T,R...> {}
2、注意细节

(1)普通成员可以使用泛型(属性、方法)
(2)使用泛型的数组,不能初始化
(3)静态方法中不能使用泛型
(4)泛型的类型,是在创建类的对象实例时确定的
(5)若创建对象时,没有指定泛型的类型,默认为Object类型
public class CustomGeneric01 {
    public static void main(String[] args) {

    }
}

/*
1.T,R,M:泛型标识符
2.泛型的标识符可以有多个,一般为大写字母
3.普通成员可以使用泛型
4.使用泛型的数组,不能初始化,因为泛型的类型无法确定
5.被static修饰的属性和方法不能使用泛型,静态方法在类加载时被加载,而泛型需要创建类的对象实例时才能指定类型
 */
class Tiger<T, R, M> {
    T name;
    R age;
    M height;

    T[] ts;

    public Tiger(T name, R age, M height) {
        this.name = name;
        this.age = age;
        this.height = height;
    }

    public void method(T name) {
    }
}
自定义泛型接口
1、基本语法

interface 接口<T,R...> {}
2、注意细节

(1)接口中,静态成员也不可使用泛型
(2)泛型接口的类型在继承接口或者实现接口时确定
(3)没有指定泛型接口的类型,默认为Object类型
public class CustomInterfaceGeneric {
    public static void main(String[] args) {

    }
}

/**
 * 泛型接口使用的说明
 * 1.接口中,静态成员不可使用泛型
 * 2.泛型接口的类型在继承接口或实现接口时指定
 *
 * @param <U>
 * @param <R>
 */
interface Usb<U, R> {
    R get(U u);

    void hi(R r);

    void run(R r1, R r2, U u1, U u2);
}

interface IA extends Usb<String, Double> {
}

/*
1.IA接口在实现Usb接口时指定了泛型的类型
2.当一个类去实现IA接口,使用String、Double替换U、R
 */
class Test01 implements IA {

    @Override
    public Double get(String s) {
        return null;
    }

    @Override
    public void hi(Double aDouble) {
    }

    @Override
    public void run(Double r1, Double r2, String u1, String u2) {
    }
}

/*
1.没有指定泛型接口的类型,默认为Object类型
2.建议直接写成class Test02 implements Usb<Object,Object> {}
 */
class Test02 implements Usb {

    @Override
    public Object get(Object o) {
        return null;
    }

    @Override
    public void hi(Object o) {
    }

    @Override
    public void run(Object r1, Object r2, Object u1, Object u2) {
    }
}
自定义泛型方法
1、基本语法

修饰符 <T,R...> 返回类型 方法名(参数列表) {}
2、注意细节

(1)泛型方法可以定义在普通类中,也可以定义在泛型类中
(2)当泛型方法被调用时,泛型的类型会被确定
(3)public void eat(E e) {},不为泛型方法,修饰符后没有<T,R...>,所以eat()方法不是泛型方法,而是使用了泛型
/**
 * 泛型方法的使用
 */
public class CustomMethodGeneric {
    public static void main(String[] args) {
        Car car = new Car();
        /*
         1.当调用泛型方法时,编译器会自动确定类型
         2.当调用泛型方法时,若是基本数据类型会进行自动装箱为包装类
         */
        car.fly("宝马", 1000000);

        Fish<String, ArrayList> fish = new Fish<>();
        fish.play(1000,"1000");
    }
}

class Car {
    public void run() {//普通方法
    }

    /*
     泛型方法
     1.<T,R>就是泛型
     2.提供给fly()方法使用
     */
    public <T, R> void fly(T t, R r) {//泛型方法
        System.out.println(t.getClass());
        System.out.println(r.getClass());
    }
}

class Fish<T, R> {//泛型类

    public void run() {//普通方法
    }

    public <U, M> void eat(U u, M m) {//泛型方法
    }

    /*
     1.下面方法不为泛型方法
     2.drink()方法使用了类声明的泛型
     */
    public void drink(T t) {
    }

    /*
     1.泛型方法可以使用类声明的泛型,也可以使用自己声明的泛型
     2.K即play()方法自己声明的泛型,T即Fish类声明的泛型
     */
    public <K> void play(K k, T t) {
        System.out.println(k.getClass());
        System.out.println(t.getClass());
    }
}
泛型继承和通配符
1、泛型不具备继承性

public class GenericExtends {
    public static void main(String[] args) {
        Object o = new String("jxs");
        
        //ArrayList<Object> list = new ArrayList<String>();错误,泛型不具备继承性
    }
}
2、<?>:支持任意泛型类型

3、<? extends A>：泛型的类型只支持A类以及A类的子类，规定了泛型的上限

4、<? super A>：支持A类以及A类的父类，不限于直接父类，规定了泛型的下限

public class GenericExtends {
    public static void main(String[] args) {
        ArrayList<Object> list1 = new ArrayList<>();
        ArrayList<String> list2 = new ArrayList<>();
        ArrayList<AA> list3 = new ArrayList<>();
        ArrayList<BB> list4 = new ArrayList<>();
        ArrayList<CC> list5 = new ArrayList<>();

        printCollection1(list1);
        printCollection1(list2);
        printCollection1(list3);
        printCollection1(list4);
        printCollection1(list5);

        printCollection2(list3);
        printCollection2(list4);
        printCollection2(list5);

        printCollection3(list3);
        printCollection3(list1);
    }

    //<?>:表示实现List接口的集合的泛型类型支持任意类型
    public static void printCollection1(List<?> c) {
        for (Object object : c) {
            System.out.println(object);
        }
    }

    //<? extends AA>:表示实现List接口的集合的泛型类型只能为AA类或AA的子类
    public static void printCollection2(List<? extends AA> c) {
        for (Object object : c) {
            System.out.println(object);
        }
    }

    //<? super AA>:表示实现List接口的集合的泛型只能为AA类或AA类的父类,不只限于直接父类
    public static void printCollection3(List<? super AA> c) {
        for (Object object : c) {
            System.out.println(object);
        }
    }
}

class AA {
}

class BB extends AA {
}

class CC extends BB {
}
JUnit
1、一个类有很多功能代码需要测试，为了测试即需要写入到main()方法中

2、若有多个功能代码测试则需要来回注销，切换很麻烦

3、若可以直接运行一个功能代码则方便很多，并可以给出相关信息，由此引出JUnit

4、JUnit基本介绍

(1)JUnit是一个Java语言的单元测试框架
(2)多数Java的开发环境都已经集成了JUnit作为单元测试的工具
(3)加入@Test则可以直接运行一个功能代码
(4)输入@Test,Alt+Enter选择JUnit5.4依赖包导入
泛型总练习
定义个泛型类DAO<T>,在其中定义一个Map成员变量,Map的键为String类型,值为T类型,分别创建以下方法:
(1)public void save(String id,T entity):保存T类型的对象到Map成员变量中
(2)public T get(String id):从map中获取id对应的对象
(3)public void update(String id,T entity):替换map中key为id的内容,改为entity对象
(4)public List<T> list():返回map中存放的所有T对象
(5)public void delete(String id):删除指定id对象

定义一个User类:
该类包含:private成员变量(int类型)id,age,(String类型)name

创建DAO类的对象,分别调用其save、get、update、list、delete方法来操作User对象，使用Junit单元测试类进行测试。
public class Homework01 {
    public static void main(String[] args) {
    }

    @Test
    public void test() {
        /*
         1.创建一个Dao类对象
         2.指定Dao类泛型的类型为User类
         */
        Dao<User> dao = new Dao<>();

        dao.save("001",new User(1,10,"jxs"));
        dao.save("002",new User(2,20,"dwy"));
        dao.save("003",new User(3,30,"tyh"));

        List<User> list = dao.list();
        System.out.println(list);

        dao.update("003",new User(4,40,"milan"));
        list = dao.list();
        System.out.println(list);

        dao.delete("003");
        list = dao.list();
        System.out.println(list);

        System.out.println(dao.get("003"));
    }
}

class User {
    private int id;
    private int age;
    private String name;

    public User(int id, int age, String name) {
        this.id = id;
        this.age = age;
        this.name = name;
    }

    public int getId() {
        return id;
    }
    public void setId(int id) {
        this.id = id;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }

    @Override
    public String toString() {
        return "User{" +
                "id=" + id +
                ", age=" + age +
                ", name='" + name + '\'' +
                '}';
    }
}

class Dao<T> {
    private HashMap<String, T> hashMap = new HashMap<>();

    //方法一:
    public void save(String id, T entity) {
        hashMap.put(id, entity);
    }

    //方法二:
    public T get(String id) {
        return hashMap.get(id);
    }

    //方法三:
    public void update(String id, T entity) {
        hashMap.put(id, entity);
    }

    //方法四:
    public List<T> list() {
        /*
         1.遍历hashMap取出value
         2.将所有value封装到arrayList
         */
        ArrayList<T> arrayList = new ArrayList<>();

        Set<String> strings = hashMap.keySet();
        for (String string : strings) {
            arrayList.add(hashMap.get(string));
        }
        return arrayList;
    }

    //方法五:
    public void delete(String id) {
        hashMap.remove(id);
    }
}

/*
输出结果：
[User{id=1, age=10, name='jxs'}, User{id=2, age=20, name='dwy'}, User{id=3, age=30, name='tyh'}]
[User{id=1, age=10, name='jxs'}, User{id=2, age=20, name='dwy'}, User{id=4, age=40, name='milan'}]
[User{id=1, age=10, name='jxs'}, User{id=2, age=20, name='dwy'}]
null
*/
1.2.7、线程（基础）
线程介绍
1、程序：为完成特定任务，用某种语言编写的一组指令的集合

2、进程：进程是指运行中的程序，比如我们使用QQ，就启动了一个进程，操作系统就会为进程分配内存空间。当我们使用迅雷，又启动了一个进程，操作系统将为迅雷分配新的内存空间。

3、进程是程序的一次执行过程，或是正在运行的一个程序，是动态过程，进程有它自身的产生、存在和消亡的过程。

4、线程由进程创建，是进程的一个实体，一个进程可以拥有多个线程

5、单线程：同一时刻，只允许执行一个线程；多线程：同一时刻，可以执行多个线程。比如一个QQ进程，可以同时打开多个聊天窗口。一个迅雷进程，可以同时下载多个文件

6、并发：同一时刻，多个任务交替执行。单核CPU实现的多任务就是并发

7、并行：同一时刻，多个任务同时执行。多核CPU可以实现并行。并行中也可以存在并发。

8、Java程序查看当前电脑的CPU数量

public class CpuNumber {
    public static void main(String[] args) {
        Runtime runtime = Runtime.getRuntime();
        int cupNumber = runtime.availableProcessors();
        System.out.println(cupNumber);
    }
}
进程、线程区别
(1)根本区别:进程是操作系统资源分配的基本单位;线程是处理器任务调度和执行的基本单位

(2)资源开销:每个进程都有独立的代码和数据空间(程序上下文),程序之间的切换会有较大的开销;线程可以看做轻量级的进程,同一类线程共享代码和数据空间,每个线程都有自己独立的运行栈和程序计数器(PC),线程之间切换的开销小。

(3)包含关系:线程是进程的一部分,若进程内有多个线程,则执行过程为多条线（线程）共同完成的

(4)内存分配:同一进程的线程共享本进程的地址空间和资源,而进程之间的地址空间和资源是相互独立的

(5)影响关系:一个进程崩溃后,在保护模式下不会对其他进程产生影响,但是一个线程崩溃整个进程都死掉。所以多进程要比多线程健壮。

(6)执行过程:每个独立的进程有程序运行的入口、顺序执行序列和程序出口。但是线程不能独立执行，必须依存在应用程序中，由应用程序提供多个线程执行控制，两者均可并发执行
线程使用
![](E:\Study\自学课程资料\Java\assets\创建线程方式.png)

1、继承Thread类，重写run方法

2、实现Runnable接口，重写run方法

继承Thread类创建线程
/**
 * 演示通过继承Thread类创建线程
 */
public class Thread01 {
    public static void main(String[] args) {
        //创建Cat对象,因为Cat类继承了Thread类,Cat类可以当作线程使用
        Cat cat = new Cat();
        cat.start();
    }
}

/*
1.当一个类继承了Thread类,该类就可以当作线程使用
2.重写run方法,加入自己的业务逻辑
3.Thread类实现了Runnable接口,重写了run方法
 */
class Cat extends Thread {
    @Override
    //重写run方法,
    public void run() {
        int times = 0;

        while (true) {
            //该线程每隔一秒在控制台输出"喵喵"
            System.out.println("第" + times + "秒输出" + "喵喵");
            times++;
            try {
                //让该线程休眠1秒
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
            if (times == 80) {
                //当times达到80,while循环结束,线程退出
                break;
            }
        }
    }
}
多线程机制
/**
 * 演示通过继承Thread类创建线程
 */
public class Thread01 {
    public static void main(String[] args) throws InterruptedException {
        //创建Cat对象,因为Cat类继承了Thread类,Cat类可以当作线程使用
        Cat cat = new Cat();
        /*
         底层源码:
         1.public synchronized void start() {
            start0();
         }
         2.start0()为本地方法,是JVM调用,底层是c/c++实现
         3.真的实现多线程的效率不是run方法,而是start0()方法
         */
        cat.start();

        /*
        1.当main线程启动时,会启动一个子线程Thread-0
        2.主线程不会阻塞,会继续执行
        3.主线程休眠1秒
        4.主线程、子线程交替执行
         */
        for (int i = 0; i < 60; i++) {
            System.out.println("主线程" + i);
            Thread.sleep(1000);
        }
    }
}

/*
1.当一个类继承了Thread类,该类就可以当作线程使用
2.重写run方法,加入自己的业务逻辑
3.Thread类实现了Runnable接口,重写了run方法
 */
class Cat extends Thread {
    @Override
    //重写run方法,
    public void run() {
        int times = 0;

        while (true) {
            //该线程每隔一秒在控制台输出"喵喵"
            System.out.println("第" + times + "秒输出" + "喵喵");
            times++;
            try {
                //让该线程休眠1秒
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
            if (times == 80) {
                //当times达到80,while循环结束,线程退出
                break;
            }
        }
    }
}
总结:
(1)Cat类继承了Thread类,即Cat类可以当做线程使用
(2)执行程序时,启动main线程,若创建一个Cat类的对象并启动线程(cat.start()),最终去执行run方法
(3)main线程会创建一个子线程:Thread-0
(4)若直接调用run方法,run方法只是一个普通的方法,线程并没有真正执行,并且会阻塞main线程
(5)跟步骤3:main线程不会被阻塞,会继续执行,main线程和子线程交替执行
(6)Cat类继承了Thread类,该类可以当作线程使用,重写run方法实现自己的逻辑,cat.start(),线程启动后,真正实现多线程的不是run方法,而是底层的start0()方法,start0为本地方法,被JVM虚拟机调用。
实现Runnable接口创建线程
(1)Java为单继承,若一个类已经继承了父类,则不可再继承Thread实现创建线程
(2)则使用另一种方式来创建线程,即通过实现Runnable接口来创建线程
public class Thread02 implements Runnable{
    public static void main(String[] args) {
        Thread02 thread02 = new Thread02();
        /*
        1.Runnable接口中只有run()方法,没有start()方法来启动线程
        2.创建Thread类对象,传入thread02参数
        3.底层使用设计模式[代理模式]
        4.将thread02传送给代理类Thread
          代理类的target属性负责接收
          然后使用代理类的对象去调用start()方法
          start()方法去调用本地的start0()方法
          由此完成多线程
         */
        Thread thread = new Thread(thread02);
        thread.start();

        Tiger tiger = new Tiger();
        ThreadProxy threadProxy = new ThreadProxy(tiger);
        threadProxy.start();
    }

    @Override
    public void run() {
        int times = 0;
        while (true) {
            System.out.println("hi" + times);
            times ++;
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }

            if (times == 10) {
                break;
            }
        }
    }
}

/**
 * 代码演示代理模式,模拟极简的Thread
 * 1.代理类:ThreadProxy
 * 2.何为代理? 举例:外卖(外卖员代理你拿外卖)
 * 3.代理类中有Runnable类型的属性target
 */
class ThreadProxy implements Runnable{
    private Runnable target = null;

    @Override
    public void run() {
        if (target != null) {
            target.run();
        }
    }

    public void start() {
        start0();
    }

    public void start0() {
        run();
    }

    public ThreadProxy(Runnable target) {
        this.target = target;
    }
}

class Animal {}
class Tiger extends Animal implements Runnable{

    @Override
    public void run() {
        System.out.println("嗷嗷");
    }
}
多个子线程案例
public class Thread03 {
    public static void main(String[] args) {
        Test1 test1 = new Test1();
        test1.start();

        Test2 test2 = new Test2();
        Thread thread = new Thread(test2);
        thread.start();
    }
}

class Test1 extends Thread{
    @Override
    public void run() {
        //每隔1秒输出"hello word",输出10次
        int number = 0;

        while(true) {
            System.out.println("子线程1执行" + number);
            number ++;
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }

            if (number ==  10) {
                break;
            }
        }
    }
}

class Test2 implements Runnable {
    @Override
    public void run() {
        int number = 0;

        while(true) {
            System.out.println("子线程2执行" + number);
            number ++;
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }

            if (number ==  5) {
                break;
            }
        }
    }
}
继承Thread和实现Runnable接口的区别
1、从Java的设计来看，通过继承Thread或者实现Runnable接口来创建线程本质上没有区别，从JDK帮助文档可以看到Thread类本身就实现了Runnable接口

2、实现Runnable接口方式更加适合多个线程共享一个资源的情况，并且避免单继承的限制。

线程终止
1、线程完成任务后自动退出

2、通过变量控制run方法退出的方式停止线程

public class ThreadExit {
    public static void main(String[] args) {
        T t = new T();
        t.start();
        /*
         1.使用main线程控制t线程的终止,通过修改loop的值让t退出while循环,从而终止t线程
         2.通知方式
         3.主线程休眠10秒再通知t线程退出
         */
        try {
            Thread.sleep(10000);
        } catch (InterruptedException e) {
            System.out.println(e.getMessage());
        }
        t.setLoop(false);
    }
}

class T extends Thread {
    private boolean loop = true;

    public void setLoop(boolean loop) {
        this.loop = loop;
    }

    int num = 0;

    @Override
    public void run() {
        while (loop) {
            System.out.println(num++);
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
总结:
(1)T类继承Thread类,T类可被作为线程
(2)在T类中重写run()方法
(3)定义辅助变量int num = 0,while循环输出num,输出一次进行一次num++,线程休眠1秒
(4)创建T类的对象实例t,启动线程t.start()
(5)run()方法只是普通方法,若执行run()方法,没有真正启动线程
(6)若在main线程中控制t线程终止,则在T类中通过设置变量控制线程run()方法退出
(7)private boolean loop = true
(8)t.setLoop(false)即可
线程常用方法即注意事项和细节
1、start底层会创建新的线程，调用run()方法，run()方法本身不会启动线程，而是底层start0()方法启动线程

2、线程优先级的范围

public final static int MIN_PRIORITY = 1;
public final static int NORM_PRIORITY = 5;
public final static int MAX_PRIORITY = 10;
3、interrupt：中断线程，但没有真正结束线程。所以一般用于正在休眠的线程

4、sleep：线程的静态方法，使当前进程休眠

5、yield：线程的礼让，让出CPU，让其他线程执行，但礼让的时间不确定，所以不一定礼让成功

6、join：线程的插队，插队的线程一旦插队成功，则先执行完插入的线程的所有的任务

public class ThreadMethod01 {
    public static void main(String[] args) {
        Test3 test3 = new Test3();
        test3.start();

        /*
         1.main线程创建一个子线程,每隔1秒吃1个包子,一共吃20次
         2.主线程每隔1秒吃1个包子,一共吃20次
         3.当主线程吃5个包子后,让子线程运行完毕后,主线程再继续执行
         */
        for (int i = 0; i < 20; i++) {
            //for循环,每次输出吃了i个包子,再休眠1秒,继续for循环
            System.out.println("主线程吃了" + i + "个包子");
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
            //当主线程执行完第5次后,test3.join,让子线程test3任务全部执行完毕后再执行主线程
            if (i == 4) {
                try {
                    test3.join();
                } catch (InterruptedException e) {
                    System.out.println(e.getMessage());
                }
            }
        }
    }
}

class Test3 extends Thread{
    @Override
    public void run() {
        for (int i = 0; i < 20; i++) {
            System.out.println("子线程吃了" + i + "个包子");
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
用户线程和守护线程
1、用户线程：也叫工作线程，当线程的任务执行完毕或以通知方式结束

2、守护线程：一般为工作线程服务，当所有的用户线程结束，守护线程自动结束

3、常见的守护线程：垃圾回收机制

public class ThreadMethod02 {
    public static void main(String[] args) {
        MyDaemonThread myDaemonThread = new MyDaemonThread();
        myDaemonThread.setDaemon(true);
        myDaemonThread.start();

        /*
        1.main线程结束后,子线程自动结束
        2.将子线程设置为守护进程myDaemonThread.setDaemon(true)
         */
        for (int i = 0; i < 5; i++) {
            System.out.println("jxs辛勤学习");
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}

class MyDaemonThread extends Thread{
    @Override
    public void run() {
        while (true) {
            int num = 0;
            System.out.println("dwy嘻嘻哈哈");
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
总结:
(1)设置为守护线程 setDaemon(true)
线程生命周期7大状态
![](E:\Study\自学课程资料\Java\assets\线程状态转换图.png)

1.初始(NEW)：刚被创建，还没运行(未执行线程的start()方法)

2.就绪状态(READY)：线程在可运行线程池中，但未获得CPU执行权，和RUNNING并称运行

3.运行中状态(RUNNING)：线程执行并获得CPU执行权，和READY并称运行

4.阻塞(BLOCK)：等待其他线程释放锁的状态

5.等待(WAITING)：需要其他线程做出一些约定好的动作,或被唤醒(通知或中断)

6.超时等待(TIME_WAITING)：和等待的不同点在于可以在指定的时间自行醒来

7.终止(TERMINATED)：线程已经执行完毕

public class ThreadState {
    public static void main(String[] args) {
        Test4 test4 = new Test4();
        System.out.println(test4.getState());

        test4.start();

        while (test4.getState() != Thread.State.TERMINATED) {
            System.out.println(test4.getState());
            try {
                Thread.sleep(500);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
        System.out.println(test4.getState());
    }
}

class Test4 extends Thread{
    @Override
    public void run() {
        while(true) {
            for (int i = 0; i < 10; i++) {
                System.out.println("hi" + i);
                try {
                    Thread.sleep(1000);
                } catch (InterruptedException e) {
                    System.out.println(e.getMessage());
                }
            }
        }
    }
}
线程同步Synchronized（重点看总结！！！）
1、线程同步机制

多线程编程，一些敏感的数据不允许被多个线程同时访问，此时就使用同步访问技术，保证数据在同一时刻，最多有一个线程访问，以保证数据的完整性

也可以这样理解:线程同步,当有一个线程在对内存进行操作时,其他线程都不可对这个内存地址进行操作,直到该线程完成操作,其他线程才能对该内存地址进行操作。
2、线程同步具体方法

(1)同步代码块
synchronized(对象) {//得到对象实例的锁,才能操作同步代码
    //需要被同步的代码
}

synchronized(类.class) {//得到当前类的锁,才能操作同步代码
    //需要被同步的代码
}

(2)同步方法
public synchronized void method1() {
    //需要被同步的代码
}

public static synchronized void method2() {
    //需要被同步的代码
}
3、线程同步理解

某位小伙伴上厕所要将门锁上,完事儿后将门解锁,其他小伙伴才可使用厕所
4、线程同步案例（售票问题）

/**
 * 使用多线程模拟3个窗口同时售100张票
 */
public class SellTicketExercise {
    public static void main(String[] args) {
        CellTicket cellTicket = new CellTicket();
        new Thread(cellTicket).start();//第1个线程 窗口1
        new Thread(cellTicket).start();//第2个线程 窗口2
        new Thread(cellTicket).start();//第3个线程 窗口3
    }
}

class CellTicket implements Runnable{
    private int ticketNum = 100;
    private boolean loop = true;

    /*
    同步方法
    1.同一时刻,只能有一个线程来执行method()方法
     */
    public synchronized void method() {
        if (ticketNum <= 0) {
            System.out.println("售票结束");
            loop = false;
            return;
        }

        System.out.println(
                Thread.currentThread().getName()
                        + "售出一张票"
                        + "剩余票数" + (--ticketNum));
        try {
            Thread.sleep(500);
        } catch (InterruptedException e) {
            System.out.println(e.getMessage());
        }
    }

    @Override
    public void run() {
        while (loop) {
            method();
        }
    }
}
5、线程同步原理

(1)线程1、线程2、线程3去争夺实例对象锁(同一对象实例)
(2)争夺到对象锁的线程执行run()方法,执行完run()方法后返回对象锁
(3)线程1、线程2、线程3继续争夺对象锁
6、总结

静态 synchronized 方法占用的锁是当前类的锁
非静态 synchronized 方法占用的锁是当前实例对象锁
synchronized(this|object) {} 进入同步代码块前获得实例对象的锁
synchronized(类.class) {} 进入同步代码块前要获得当前类的锁  
互斥锁（重点看总结！！！）
1、基本介绍

(1)Java语言中,引入了对象互斥锁的概念,来保证共享数据的完整性
(2)每个对象实例都对应于一个可称为"互斥锁"的标记,这个标记用来保证在任意时刻,只能有一个线程访问该对象
(3)关键字synchronized来与对象的互斥锁联系。当某个对象用synchronized修饰时,表明该对象在任意时刻只能由一个线程访问
(4)同步的局限性:程序执行效率降低
(5)同步非静态方法的锁可以是this,也可以是其他对象
(6)同步静态方法的锁为当前类本身
2、互斥锁案例

/**
 * 使用多线程模拟3个窗口同时售100张票
 */
public class SellTicketExercise {
    public static void main(String[] args) {
        CellTicket cellTicket = new CellTicket();
        new Thread(cellTicket).start();//第1个线程 窗口1
        new Thread(cellTicket).start();//第2个线程 窗口2
        new Thread(cellTicket).start();//第3个线程 窗口3
    }
}

class CellTicket implements Runnable{
    private int ticketNum = 100;
    private boolean loop = true;

    /*
    同步静态方法
    1.同步静态方法的锁为当前类本身
    2.静态方法中实现同步代码块,锁在类本身
     */
    public static synchronized void method1() {
    }

    public static void method2() {
        synchronized (CellTicket.class) {
        }
    }

    /*
    同步方法
    1.同一时刻,只能有一个线程来执行method()方法
    2.这时锁在this对象上
    3.在method()方法中加入同步代码块,这时锁还在this对象上
     */
    public /*synchronized*/ void method() {
        synchronized (this) {
            if (ticketNum <= 0) {
                System.out.println("售票结束");
                loop = false;
                return;
            }

            System.out.println(
                    Thread.currentThread().getName()
                            + "售出一张票"
                            + "剩余票数" + (--ticketNum));
            try {
                Thread.sleep(500);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }

    @Override
    public void run() {
        while (loop) {
            method();
        }
    }
}
3、总结

(1)非静态方法和非静态代码块锁在this对象上
(2)静态方法和静态代码块锁为当前类本身
(3)实现同步落地方式:
分析上锁代码块
选择同步代码块和同步方法
要求多线程的锁对象为同一个
/*
1.CellTicket01继承Thread类,CellTicket01可以被当作线程使用
2.同步代码块,锁在对象实例上,并且要求多线程的锁对象为同一个
3.CellTicket01启动线程必须要创建一个对象实例,再启动线程
4.导致多线程不为同一个锁对象
 */
class CellTicket01 extends Thread {
    public void method() {
        synchronized (this) {
            System.out.println("hello");
        }
    }
}
死锁
1、基本介绍

多个线程都占用对方的锁资源,双方都不相让,导致死锁,编程时一定避免死锁的发生
2、应用案例

妈妈:写完作业再玩手机
小明:先玩手机再写作业
3、死锁案例

public class DeadLock {
    public static void main(String[] args) {
        DeadLockDemo deadLockDemo1 = new DeadLockDemo(true);
        DeadLockDemo deadLockDemo2 = new DeadLockDemo(false);
        deadLockDemo1.setName("A线程");
        deadLockDemo2.setName("B线程");
        deadLockDemo1.start();
        deadLockDemo2.start();
    }
}

class DeadLockDemo extends Thread {
    static Object o1 = new Object();
    static Object o2 = new Object();
    boolean flag;

    public DeadLockDemo(boolean flag) {
        this.flag = flag;
    }

    @Override
    public void run() {
        /*
        业务逻辑分析
        1.若flag为true,假设线程A得到o1对象锁,执行同步代码块
        2.线程A会尝试获取o2对象锁,若得不到o2对象锁则会Blocked
        3.若flag为false,假设线程B得到o2对象锁,执行同步代码块
        4.线程B会尝试获取o1对象锁,若得不到o1对象锁则会Blocked
        5.线程A得到o1对象锁,线程B得到o2对象锁,线程A、线程B无法释放锁,即会导致死锁
         */
        if (flag) {
            synchronized (o1) {
                System.out.println(Thread.currentThread().getName() + "进入同步代码块1");
                synchronized (o2) {
                    System.out.println(Thread.currentThread().getName() + "进入同步代码块2");
                }
            }
        } else {
            synchronized (o2) {
                System.out.println(Thread.currentThread().getName() + "进入同步代码块3");
                synchronized (o1) {
                    System.out.println(Thread.currentThread().getName() + "进入同步代码块4");
                }
            }
        }
    }
}
释放锁
1、释放锁的4种情况

(1)当前线程的同步方法、同步代码块执行结束
(2)当前线程在同步方法、同步代码块中遇到break、return
(3)当前线程在同步方法、同步代码块中出现未处理的Error或Exception,导致异常结束
(4)当前线程在同步方法、同步代码块中执行线程对象的wait()方法,当前线程暂停,并释放锁
2、不释放锁的2种情况

(1)当前线程执行同步方法、同步代码块时,程序调用Thread.sleep()、Thread.yield()方法暂停当前线程的执行,不会释放锁
(2)当前线程执行同步代码块时,其他线程调用该线程的suspend()方法将该线程挂起,该线程不会释放锁
线程练习
练习1

(1)在main方法中启动两个线程
(2)第1个线程循环随机打印100以内的整数
(3)直到第2个线程从键盘读取了“Q”命令
public class Homework01 {
    public static void main(String[] args) {
        A a = new A();
        a.start();
        B b = new B(a);
        b.start();
    }
}

class A extends Thread {
    private boolean flag = true;
    public void setFlag(boolean flag) {
        this.flag = flag;
    }

    @Override
    public void run() {
        while (flag) {
            Random random = new Random();
            int i = random.nextInt(100);
            System.out.println(i);

            try {
                Thread.sleep(2000);
            } catch (InterruptedException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}

class B extends Thread {
    private A a;
    Scanner scanner = new Scanner(System.in);

    public B(A a) {
        this.a = a;
    }

    @Override
    public void run() {
        while (true) {
            char c = scanner.next().toUpperCase().charAt(0);
            if (c == 'Q') {
                a.setFlag(false);
                break;
            }
        }
    }
}
练习2

(1)有2个用户分别从同一个卡上取钱(总额:10000)
(2)每次都取1000,当余额不足时,就不能取款了
(3)不能出现超取现象 -> 线程同步问题
public class Homework02 {
    public static void main(String[] args) {
        GetMoney getMoney = new GetMoney();
        Thread thread1 = new Thread(getMoney);
        thread1.setName("A线程");
        Thread thread2 = new Thread(getMoney);
        thread2.setName("B线程");

        thread1.start();
        thread2.start();
    }
}

class GetMoney implements Runnable {
    private double money = 10000.0;

    @Override
    public void run() {
        while (true) {
            /*
            /*
            1.synchronized关键字实现线程同步
            2.当3个线程执行到同步代码块时,争夺this对象锁
            3.争夺到的执行run()方法;争夺不到的阻塞在此,等待下次争夺
            4.执行完run()方法后,释放this对象锁
            5.3个线程继续争夺this对象锁
             */
            synchronized (this) {
                //判断余额是否足够
                if (money < 1000) {
                    System.out.println("余额不足");
                    break;
                }

                money -= 1000.0;
                System.out.println(
                        Thread.currentThread().getName() + "取款1000.0元 "
                                + "当前余额" + money);

                try {
                    Thread.sleep(1000);
                } catch (InterruptedException e) {
                    System.out.println(e.getMessage());
                }
            }
        }
    }
}
1.2.8、IO流
文件
1、基本概念

文件是保存数据的地方(word文档、txt文件、excel文件)
2、文件流

文件在程序中是以流的形式来操作的
文件(磁盘) --> java程序 输入流:数据从数据源到程序的路径
java程序 --> 文件(磁盘) 输出流:数据从程序到数据源的路径
创建文件
1、创建文件对象相关构造器和方法

new File(String pathname)//根据路径构建文件对象
new File(File parent,String child)//根据父目录文件+子路径构建文件对象
new File(String parent,String child)//根据父目录+子路径构建文件对象

createNewFile:创建新文件
/**
 * 演示创建文件
 */
public class FileCreate01 {
    public static void main(String[] args) {
    }

    @Test
    public void createFile01() {
        /*
        1.File file = new File() 在内存中创建文件对象
        2.file.createNewFile() 将文件对象输入到磁盘对应位置
         */
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\newFile01.txt");
        try {
            file.createNewFile();
            System.out.println("文件创建成功");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }

    @Test
    public void createFile02() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream"
                , "newFile02.txt");
        try {
            file.createNewFile();
            System.out.println("文件创建成功");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }

    @Test
    public void createFile03() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream","newFile03.txt");
        try {
            file.createNewFile();
            System.out.println("文件创建成功");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }
}
总结:
(1)File file = new File() 在内存中创建文件对象
(2)file.createNewFile 将文件对象输入到磁盘对应位置
获取文件信息
public class FileInformation {
    public static void main(String[] args) {
    }

    @Test
    public void getInformation() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\newFile01.txt");
        //文件名
        System.out.println(file.getName());
        //文件绝对路径
        System.out.println(file.getAbsoluteFile());
        //文件父路径
        System.out.println(file.getParent());
        //文件大小(字节)
        System.out.println(file.length());
        //文件是否存在
        System.out.println(file.exists());
        //判断是否为文件
        System.out.println(file.isFile());
        //判断是否为目录
        System.out.println(file.isDirectory());
    }
}

/*
输出结果：
newFile01.txt
E:\application\IntelliJ IDEA 2021.1\IOStream\newFile01.txt
E:\application\IntelliJ IDEA 2021.1\IOStream
14
true
true
false
*/
目录操作
public class directory01 {
    public static void main(String[] args) {
    }

    /**
     * 删除文件
     */
    @Test
    public void directory01() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\directory\\directoryTest.txt");
        if (file.exists()) {
            if (file.delete()) ;
            System.out.println("文件删除成功");
        } else {
            System.out.println("文件删除失败");
        }
    }

    /**
     * 删除目录
     * java编程中,目录也被当作文件
     */
    @Test
    public void directory02() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\directory");
        if (file.exists()) {
            if (file.delete()) {
                System.out.println("目录删除成功");
            } else {
                System.out.println("目录删除失败");
            }
        }
    }

    /**
     * 创建目录
     */
    @Test
    public void directory03() {
        File file = new File("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\directory");
        if (file.exists()) {
            System.out.println("目录已存在");
        } else {
            /*
            1.创建一级目录使用mkdir()
            2.创建多级目录使用mkdirs()
             */
            if (file.mkdir()) {
                System.out.println("目录创建成功");
            } else {
                System.out.println("目录创建失败");
            }
        }
    }
}
总结:
删除文件:
(1)file.exists(判断文件是否存在),存在返回true;不存在返回false
(2)file.delete(删除文件),删除成功返回true;删除失败返回false

删除目录:
(1)在Java编程中,目录也被当作文件
(2)file.exists(判断目录是否存在)
(2)file.delete(删除目录)

创建目录:
(1)file.exists(判断目录是否存在)
(2)file.mkdirs(创建多级目录),创建成功返回true,创建失败返回false
IO流的原理及流的分类
1、IO流原理

(1)I/O是Input/Output的缩写,I/O技术是非常实用的技术,用于处理数据传输。如读/写文件,网络通讯等
(2)Java程序中,对于数据的输入输出采用"流"的方式进行
(3)java.io包下提供了各种"流"类和接口,用以获取不同种类的数据,并通过方法输入或输出数据。
(4)输入input:读取外部数据(磁盘、光盘等存储设备数据)到程序(内存)中
(5)输出output:将程序(内存)数据输出到(磁盘、光盘等存储设备)中
2、流的分类

(1)按操作数据单位不同分为:字节流(8 bit,适合二进制文件,比如图片、视频、音乐)、字符流(按字符,纯文本文件)
(2)按数据流的流向不同分为:输入流、输出流
(3)按流的角色的不同分为:节点流、处理流/包装流
抽象基类	字节流	字符流
输入流	InputStream	Reader
输出流	OutputStream	Writer
3、字节输入流抽象基类类图

![](E:\Study\自学课程资料\Java\assets\InputStream字节输入流抽象类类图.png)

4、字节输出流抽象基类类图

![](E:\Study\自学课程资料\Java\assets\OutputStream字节输出流抽象类类图.png)

5、字符输入流抽象基类类图

![](E:\Study\自学课程资料\Java\assets\字符输入流抽象类类图.png)

6、字符输出流抽象基类类图

![](E:\Study\自学课程资料\Java\assets\字符输出流抽象类类图.png)

7、总结

(1)Java的IO流共涉及40多个类,非常规则,都是从4个抽象基类派生的
(2)由这4个抽象基类派生出的子类名称都是以其父类名作为子类名的后缀
8、文件和流

流是文件的传输形式
FileInputStream字节输入流（重要！！！！）
![](E:\Study\自学课程资料\Java\assets\InputStream字节输入流抽象基类继承类类图.png)

/**
 * 演示FileInputStream的使用
 */
public class FileInputStream01 {
    public static void main(String[] args) {

    }

    @Test
    public void readFile01() {
        FileInputStream fileInputStream = null;
        try {
            //创建FileInputStream对象,用于读取文件
            fileInputStream = new FileInputStream("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\newFile01.txt");
            /*
            从此输入流中读取一个数据字节。如果没有输入可用,则此方法将阻塞。
            指定者:类 InputStream 中的 read
            返回:下一个数据字节;若读取完毕则返回 -1
             */
            int readData;
            //当未达到文件末尾,则循环输出下一个字节数据
            while ((readData = fileInputStream.read()) != -1) {
                System.out.print((char) readData);
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                //关闭文件流
                fileInputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }

    @Test
    public void readFile02() {
        FileInputStream fileInputStream = null;
        byte[] buf = new byte[8];
        try {
            fileInputStream = new FileInputStream("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\newFile01.txt");
            /*
            从此输入流中将最多 buf.length 个字节的数据读入一个 byte 数组中,在某些输入可用之前，此方法将阻塞。
            1.覆盖:类 InputStream 中的 read
            2.参数:buf - 存储读取数据的缓冲区。
            3.返回:若读取完毕则返回 -1;若读取正常则返回实际读取的字节数
             */
            int readLength;
            while ((readLength = fileInputStream.read(buf)) != -1) {
                System.out.print(new String(buf,0,readLength));
            }
        }  catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileInputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
总结:
(1)创建流对象(FileInputStream fileInputStream = new FileInputStream)
    
(2)读取流对象内部数据
    read():返回下一个数据字节并转换为int形式,读取完毕返回-1
    read(byte[] buffer):buffer(存储数据的缓冲区),读取正常则返回实际读取的字节数,读取完毕则返回-1)
    
(3)关闭流对象fileInputStream.close()
FileOutputStream字节输出流
![](E:\Study\自学课程资料\Java\assets\OutputStream字节输出流抽象基类继承类类图.png)

public class FileOutputStream01 {
    public static void main(String[] args) {

    }

    @Test
    public void writeFile01() {
        FileOutputStream fileOutputStream = null;
        try {
            /*
            1.获取文件输出流对象
            2.FileOutputStream fileOutputStream = new FileOutputStream(filePath)创建方法,写入内容时会覆盖原有内容
            3.FileOutputStream fileOutputStream = new FileOutputStream(filePath,true)创建方法,写入内容时会追加到文件末尾
             */
            fileOutputStream = new FileOutputStream("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\FileOutputStream\\fileOutputStream.txt",true);
            /*
            1.write(int b) 将指定字节写入文件输出流
            2.向流对象写入一个字节,char类型会自动转换为int类型
             */
            fileOutputStream.write('a');

            /*
            1.write(byte[] b) 将b.length个字节从指定byte[]数组写入到文件输出流
            2.向流对象写入一个字符串,利用字符串get.Bytes()方法将字符串->字节数组
             */
            String str = "hello,jxs";
            fileOutputStream.write(str.getBytes());

            /*
            1.write(byte[] b,int off,int len) 将byte[]数组中从索引off到索引len处的字节写入到文件输出流
            2.向流对象写入一个字符串,利用字符串的get.Bytes()方法将字符串->字节数组
             */
            fileOutputStream.write(str.getBytes(),0,4);

        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
总结:
(1)获取文件输出流对象
	FileOutputStream fileOutputStream = new FileOutputStream(filePath)
	写入数据时会覆盖原有内容
	
	FileOutputStream fileOutputStream = new FileOutputStream(filePath,true)
	写入数据时会追加到文件末尾
	
(2)向文件输出流中写入数据
	write(int b):写入一个字节到文件输出流,传入的字符会自动转换为int类型
	
	write(byte[] b):写入一个字符串,利用字符串的get.Bytes()方法将字符串->字符数组
	
	write(byte[] b,int off,int len):写入一个字符串,利用字符串的get.Bytes()方法将字符串->字符数组,将字符数组中索引off到索引len的位置的字节传入到文件输出流中
	
(3)关闭文件输出流
	fileOutputStream.close()
文件拷贝
/**
 * 文件拷贝
 * 1.创建文件输入流对象
 * 2.创建文件输出流对象
 * 3.文件通过文件输入流的方式将数据输入到java程序
 * java程序通过文件输出流的方式将数据输出到文件
 * 4.使用while循环,读取部分数据就写入部分数据
 */
public class FileCopy {
    public static void main(String[] args) {
        FileInputStream fileInputStream = null;
        FileOutputStream fileOutputStream = null;
        String srcPath = "E:\\Study\\自学课程资料\\Java\\assets\\ArrayList底层源码步骤1.png";
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\ArrayList.png";

        //定义字节数组提高读取效率
        byte[] buf = new byte[1024];

        int readLength = 0;

        try {
            //1.创建文件输入流,文件以文件输入流的形式将数据输入到java程序
            fileInputStream = new FileInputStream(srcPath);
            /*
            2.
              fileInputStream.read(buf)
              1.正常读取成功则返回buf.length长度的字节数组
              2.当字节数不足buf.length则返回实际读取的字节数
              3.正常读取完毕则返回-1
             */
           while ((readLength = fileInputStream.read(buf)) != -1) {
                //边读取边写入
                fileOutputStream = new FileOutputStream(destPath, true);
                /*
                1.第一次读取1024字节,则将字节数组索引0~readLength处的字节输出到文件
                2.第二次读取不足1024字节的话,readLength返回的是实际读取的字节数
                 */
                fileOutputStream.write(buf);
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileInputStream.close();
                fileOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
总结:
文件拷贝
(1)文件通过文件输入流的形式将数据传入到java程序中
(2)定义字节数组提高读取效率
(3)边读取边写入
(4)java程序通过文件输出流的形式将数据输出到文件中
FileReader字符输入流
![](E:\Study\自学课程资料\Java\assets\Reader字符输入流抽象基类继承类类图.png)

public class FileReader01 {
    public static void main(String[] args) {
    }

    @Test
    public void fileReader01() {
        FileReader fileReader = null;
        String srcPath = "D:\\HDFS_Downloads\\data\\phone_data.txt";
        int data = 0;
        try {
            //定义字符输入流对象
            fileReader = new FileReader(srcPath);
            /*
             1.文件以字符输入流的形式传入到java程序中
             2.read返回的是读取的内容,返回int只是读取到的内容的表示方式
             3.将read读取到的内容强转为char输出
             */
            while((data = fileReader.read()) != -1){
                System.out.print((char) data);
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileReader.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }

    @Test
    public void fileReader02() {
        String srcPath = "D:\\HDFS_Downloads\\data\\phone_data.txt";
        FileReader fileReader = null;
        //定义字符数组,提高读取效率,每次读取8个字符
        char[] chars = new char[8];
        int readLength = 0;

        try {
            //定义字符输入流对象,将文件以字符输入流的形式输入到java程序
            fileReader = new FileReader(srcPath);
            /*
             1.循环读取,返回的是实际读取到的字符,若返回值为-1,说明读取到文件结尾
             2.read返回的是读取的内容,返int就是读取到的内容的表示方式
               以二进制形式表现的，然后再把它转换为字符串输出
             */
            while ((readLength = fileReader.read(chars)) != -1) {
                System.out.print(new String(chars,0,readLength));
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileReader.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
FileWriter字符输出流
![](E:\Study\自学课程资料\Java\assets\Writer字符输出流抽象基类继承类类图.png)

public class FileWriter01 {
    public static void main(String[] args) {
        FileWriter fileWriter = null;
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\FileWriter\\fileWriter.txt";
        char[] chars = {'a', 'b', 'c'};

        try {
            fileWriter = new FileWriter(destPath);
            fileWriter.write('H');

            fileWriter.write(65);

            fileWriter.write(chars);

            fileWriter.write("jxsdwy".toCharArray(), 0, 3);

            fileWriter.write("dwy");

            fileWriter.write("南京欢迎你", 0, 4);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileWriter.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
节点流和处理流（重要！！！！）
1、基本介绍

(1)节点流可以从一个特定的数据源读写数据
文件节点流:FileInputStream、FileOutputStream、FileReader、FileWriter
数组节点流:ByteArrayInputStream、ByteArrayOutputStream、CharArrayReader、CharArrayWriter
管道节点流:PipedInputStream、PipedOutputStream、PipedReader、PipedWriter
字符串节点流:StringReader、StringWriter
(2)处理流(也叫包装流),是"连接"在已存在的流(节点流或处理流)之上,为程序提供更为强大的读写功能,也更加灵活,如BufferedReader、BufferedWriter。
(3)处理流BufferedReader类中有属性Reader,即可以封装一个Reader的子类;处理流BufferedWriter类中有属性Writer,即可以封装一个Writer的子类
public class BufferedWriter extends Writer {
    private Writer out;
}
2、节点流、处理流一览图

![](E:\Study\自学课程资料\Java\assets\节点流、处理流一览图.png)

处理流设计模式（重要！！！！）
1、节点流和处理流的区别和联系

(1)节点流是底层流/低级流，直接跟数据源相接
(2)处理流(包装节点流,既可以消除不同节点流的实现差异,也可以提供更方便的方法来完成输入输出)
(3)处理流(也叫包装流),对节点流进行包装,使用了修饰器设计模式,不会直接与数据源相连
2、处理流的功能主要体现在以下两个方面

(1)性能的提高:主要以增加缓冲的方式来提高输入输出的效率
(2)操作的便捷:处理流可能提供了一系列便捷的方法来一次输入输出大批量的数据,使用更加灵活方便
3、代码理解

/*
1.自定义抽象类Reader_,就好比字符输入流抽象基类Reader
2.自定义抽象方法readFile()、readString()
 */
public abstract class Reader_ {
    public abstract void readFile();

    public abstract void readString();
}

/*
1.FileReader_继承抽象类Reader_
2.实现Reader_抽象类所有抽象方法
 */
class FileReader_ extends Reader_ {
    public void readFile() {
        System.out.println("传入一个文件");
    }

    @Override
    public void readString() {
    }
}

/*
1.StringReader_类继承抽象类Reader_
2.实现Reader_抽象类所有抽象方法
 */
class StringReader_ extends Reader_ {
    @Override
    public void readFile() {
    }

    public void readString() {
        System.out.println("传入一个字符串");
    }
}

/*
处理流(包装流)
1.BufferedReader_类继承Reader_抽象类
2.实现Reader_抽象类所有抽象方法
3.BufferedReader_类有属性Reader_
4.提供构造器
5.创建一个BufferedReader_类实例对象,实参可以传入Reader_类或Reader_类的子类的实例对象
 */
class BufferedReader_ extends Reader_ {
    private Reader_ reader_;

    public BufferedReader_(Reader_ reader) {
        this.reader_ = reader;
    }

    /*
    1.扩展readFile()方法,扩展readString()方法
    2.创建一个BufferedReader_实例对象时
      实参传入一个Reader_类或Reader_类的子类的实例对象
    3.执行readFiles()、readStrings()方法时
      会动态绑定到实参传入的实例对象的readFile()、readString()方法
     */
    public void readFiles(int num) {
        for (int i = 0; i < num; i++) {
            reader_.readFile();
        }
    }

    public void readStrings(int num) {
        for (int i = 0; i < num; i++) {
            reader_.readString();
        }
    }


    @Override
    public void readFile() {

    }

    @Override
    public void readString() {

    }
}

class Test {
    public static void main(String[] args) {
        BufferedReader_ bufferedReader_ = new BufferedReader_(new FileReader_());
        bufferedReader_.readFiles(10);

        BufferedReader_ bufferedReader_1 = new BufferedReader_(new StringReader_());
        bufferedReader_.readStrings(10);
    }
}
BufferedReader
![](E:\Study\自学课程资料\Java\assets\BufferedReader类图.png)

1、基本介绍

(1)BufferedReader和BufferedWriter属于字符流,是按照字符来读取数据的
(2)关闭处理流时,只需关闭外层流即可
2、代码演示

public class BufferedReader01 {
    public static void main(String[] args) {
        BufferedReader bufferedReader = null;
        String srcPath = "D:\\HDFS_Downloads\\data\\phone_data.txt";
        String line;
        try {
            //创建bufferedReader对象,实参中传入fileReader对象
            bufferedReader = new BufferedReader(new FileReader(srcPath));
            /*
            按行读取文件,当返回null时表示文件读取完毕
            1.读取一个文本行。通过下列字符之一即可认为某行已终止:
              换行 ('\n')、回车 ('\r') 或回车后直接跟着换行。
            2.返回:包含该行内容的字符串,不包含任何行终止符
              如果已到达流末尾，则返回 null
             */
            while ((line = bufferedReader.readLine()) != null) {
                System.out.println(line);
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                /*
                关闭处理流
                1.只需关闭BufferedReader,底层会自动关闭节点流
                 */
                bufferedReader.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
BufferedWriter
public class BufferedWriter01 {
    public static void main(String[] args) {
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\BufferedWriter\\test.txt";
        BufferedWriter bufferedWriter = null;
        char[] chars = {'a', 'b', 'c', 'd', 'e'};
        try {
            /*
            new BufferedWriter(new FileWriter(destPath,true))
            添加的内容以追加的方式写入到文本文件中

            new BufferedWriter(new FileWriter(destPath))
            添加的内容以覆盖的的方式写入到文本文件中
             */
            bufferedWriter = new BufferedWriter(new FileWriter(destPath));
            bufferedWriter.write(65);
            //插入一个和系统相关的换行符
            bufferedWriter.newLine();
            bufferedWriter.write(chars);
            bufferedWriter.write("jxsdwy999", 0, 8);
            bufferedWriter.write("99999999");
            bufferedWriter.write(chars, 0, 2);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                /*
                关闭流:
                1.关闭外层流即可,传入的fileWriter字符输出流会自动关闭
                 */
                bufferedWriter.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
字符处理流文件拷贝
public class BufferedCopy {
    public static void main(String[] args) throws IOException {
        BufferedReader bufferedReader = null;
        BufferedWriter bufferedWriter = null;
        String srcPath = "D:\\HDFS_Downloads\\data\\phone_data.txt";
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\BufferedWriter\\copy.txt";

        bufferedReader = new BufferedReader(new FileReader(srcPath));
        bufferedWriter = new BufferedWriter(new FileWriter(destPath,true));

        String line;
        /*
        1.readLine()读取一行内容,但写入数据时不进行换行
        2.插入换行
         */
        while ((line = bufferedReader.readLine()) != null) {
            bufferedWriter.write(line);
            bufferedWriter.newLine();
        }

        bufferedReader.close();
        bufferedWriter.close();
    }
}
BufferedInputStream、BufferedOutputStream
1、BufferedInputStream类图

![](E:\Study\自学课程资料\Java\assets\BufferedInputStream类图.png)

2、BufferedOutputStream类图

![](E:\Study\自学课程资料\Java\assets\BufferedOutputStream类图.png)

字节处理流文件拷贝
/**
 * 使用BufferedInputStream、BufferedOutputStream实现文件拷贝
 */
public class BufferedInputStream01 {
    public static void main(String[] args) {
        BufferedInputStream bufferedInputStream = null;
        BufferedOutputStream bufferedOutputStream = null;
        //文件源路径、文件目标路径
        String srcPath = "E:\\Study\\自学课程资料\\Java\\assets\\ArrayList底层源码步骤1.png";
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Bufferedcopy\\字节处理流copy.png";

        try {
            /*
            1.BufferedInputStream继承FilterInputStream
            2.FilterInputStream继承InputStream
            3.FilterInputStream有属性InputStream in
            4.创建BufferedInputStream对象时,实参可以传入InputStream抽象类的子类
             */
            bufferedInputStream = new BufferedInputStream(new FileInputStream(srcPath));
            bufferedOutputStream = new BufferedOutputStream(new FileOutputStream(destPath));
            int read = 0;
            while ((read = bufferedInputStream.read()) != -1) {
                bufferedOutputStream.write(read);
            }
        } catch (IOException e) {

        } finally {
            try {
                bufferedInputStream.close();
                bufferedOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
字节处理流、字符处理流总结（重要！！！！！！）
(1)BufferedReader、BufferedWriter字符处理流继承Reader、Writer字符输入流、字符输出流抽象基类
(2)BufferedReader、BufferedWriter类中有属性Reader in、Writer out
(3)创建BufferedReader、BufferedWriter实例对象时,实参可以传入Reader、Writer抽象基类的子类的对象实例
(4)BufferedInputStream、BufferedOutputStream字节处理流继承FilterInputStream、FilterOutputStream字节处理流,FilterInputStream、FilterOutputStream字节处理流继承InputStream、OutputStream抽象基类
(5)FilterInputStream、FilterOutputStream中有属性InputStream in、OutputStream out
(6)创建BufferedInputStream、BufferedOutputStream实例对象时,实参可以传入InputStream、OutputStream抽象基类的子类的对象实例
(7)字节处理流可以处理二进制文件以及文本文件;字符处理流只可处理文本文件,处理二进制文件会造成数据丢失
ObjectInputStream、ObjectOutputStream对象流（重点看序列化！！！）
1、需求

(1)将int num = 100,这个int数据保存到文件中,不是数字100而是int 100,并且能够从从文件直接恢复int 100
(2)将Dog dog = new Dog("小黄",3),这个dog对象保存到文件中,并且能够从文件中恢复
(3)上面的要求,就是能够将 基本数据类型 或者 对象 进行序列化和反序列化
2、序列化和反序列化

(1)序列化:Java程序保存数据到文件中时,保存数据的值和数据类型
(2)反序列化:将保存在文件中的数据重新恢复时,恢复数据的值和数据类型
(3)支持序列化和可序列化,必须实现如下两个接口之一:Serializable(标记接口,接口中没有方法)、Externalizable(该接口有方法需要实现)
3、ObjectOutputStream对象处理流提供序列化功能

![](E:\Study\自学课程资料\Java\assets\ObjectOutputStream对象处理流.png)

4、ObjectInputStream对象处理流提供反序列化功能

![](E:\Study\自学课程资料\Java\assets\ObjectInputStream对象处理流.png)

5、ObjectOutputStream代码理解

/**
 * 将Java程序中的数据序列化到文本文件中
 * 演示ObjectOutputStream的使用,完成数据的序列化
 */
public class ObjectOutputStream01 {
    public static void main(String[] args) {
        //自定义ObjectOutputStream对象处理流对象
        ObjectOutputStream objectOutputStream = null;
        //序列化后,保存的文件格式不是存储文本,而是按照他的格式来保存
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Object\\test.txt";

        try {
            /*
            1.序列化数据到test.txt文本文件中
            2.int --> Integer(实现Serializable接口)
            3.boolean --> Boolean(实现Serializable接口)
            4.double --> Double(实现Serializable接口)
            5.String(实现Serializable接口)
             */
            objectOutputStream = new ObjectOutputStream(new FileOutputStream(destPath));

            objectOutputStream.writeInt(100);

            objectOutputStream.writeBoolean(true);

            objectOutputStream.writeDouble(100.0);

            objectOutputStream.writeUTF("jxs");

            //Dog类必须实现Serializable接口
            objectOutputStream.writeObject(new Dog("bai", 1));

        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                objectOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}

class Dog implements Serializable {
    private String name;
    private int age;

    public Dog(String name, int age) {
        this.name = name;
        this.age = age;
    }

    @Override
    public String toString() {
        return "Dog{" +
                "name='" + name + '\'' +
                ", age=" + age +
                '}';
    }

    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
}
6、ObjectInputStream代码理解

/**
 * 将文本文件中的数据反序列化到Java程序中
 */
public class ObjectInputStream01 {
    public static void main(String[] args) {
        //自定义ObjectOutputStream对象处理流对象
        ObjectInputStream objectInputStream = null;
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Object\\test.txt";

        try {
            objectInputStream = new ObjectInputStream(new FileInputStream(srcPath));
            //(读取)反序列化的顺序必须和(写入)序列化的顺序一致
            objectInputStream.readInt();

            objectInputStream.readBoolean();

            objectInputStream.readDouble();

            objectInputStream.readUTF();

            /*
            反序列化得到的o的编译类型、运行类型
            1.编译类型:Object
            2.运行类型:Dog
             */
            Object o = objectInputStream.readObject();
            System.out.println(o.getClass());
            /*
            1.System.out.println(o)默认输出o的地址
            2.重写toString()方法
            3.输出o对象的属性信息
             */
            System.out.println(o);
            /*
            若希望调用Dog类的方法,会出现访问权限问题
            1.将Dog类的定义拷贝到引用的位置
            2.需要向下转型
             */
            Dog o1 = (Dog) o;
            System.out.println(o1.getName());

        } catch (IOException | ClassNotFoundException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                objectInputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
对象处理流细节
1、反序列化、序列化顺序一致

2、实现反序列化、序列化对象要实现Serializable接口

3、序列化的类中建议添加SerialVersionUID，为提高版本兼容性

4、序列化对象时，默认将里面所有属性都进行序列化，但除了static或transient修饰的成员

5、序列化对象时，要求里面的属性的类型也需要实现序列化接口

6、序列化具备可继承性，若某类已经实现序列化，则它的所有子类也已经默认实现序列化

public class SerializableExercise {
    public static void main(String[] args) {

    }

    @Test
    public void objectOutputStreamMethod() {
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Object\\test1.txt";
        ObjectOutputStream objectOutputStream = null;
        try {
            objectOutputStream = new ObjectOutputStream(new FileOutputStream(destPath));
            objectOutputStream.writeObject(new Animal("dog", 1, "中国", "白色"));
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                objectOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }

    @Test
    public void objectInputStreamMethod() {
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Object\\test1.txt";
        ObjectInputStream objectInputStream = null;

        try {
            objectInputStream = new ObjectInputStream(new FileInputStream(srcPath));
            Object o = objectInputStream.readObject();
            System.out.println(o);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                objectInputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}

class Animal implements Serializable {
    //细节3.serialVersionUID 序列化版本号,可以提高兼容性
    private static final long serialVersionUID = 1L;

    /*
    细节4.序列化对象时,要将对象中所有的属性进行序列化,且被static、transient修饰的成员不可被序列化
    细节5.序列化对象时,对象的属性所属的数据类型要实现Serializable接口
     */
    private String name;
    private int age;
    private transient String count;
    private static String colour;

    public Animal(String name, int age, String count, String colour) {
        this.name = name;
        this.age = age;
        this.count = count;
        this.colour = colour;
    }

    @Override
    public String toString() {
        return "Animal{" +
                "name='" + name + '\'' +
                ", age=" + age +
                ", count='" + count + '\'' +
                ", colour='" + colour + '\'' +
                '}';
    }
}
System.in、System.out标准输入输出流
类型	默认设备
System.in 标准输入	InputStream	键盘
System.out 标准输出	OutputStream	显示器
public class InputAndOutput {
    public static void main(String[] args) {
        /*
        System.in
        1.System类的属性public final static InputStream in = null
        2.System.in 编译类型:InputStream
        3.System.in 运行类型:BufferedInputStream
        4.代表标准输入,即键盘
         */
        System.out.println(System.in.getClass());

        /*
        System.out
        1.System类的属性public final static PrintStream out = null
        2.System.out 编译类型:InputStream
        3.System.out 运行类型:PrintStream
        4.代表标准输出,即显示器
         */
        System.out.println(System.out.getClass());
    }
}
InputStreamReader、OutputStreamWriter转换流（重中之重！！！）
1、转换流的引出

public class CodeQuestion {
    public static void main(String[] args) {
        BufferedReader bufferedReader = null;
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\codeQuestion\\test1.txt";
        try {
            bufferedReader = new BufferedReader(new FileReader(srcPath));
            /*
            1.默认读取文件是按照UTF-8编码读取
            2.若文件不是UTF-8编码,则读取出现乱码
            */
            String s = bufferedReader.readLine();
            System.out.println(s);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                bufferedReader.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
2、InputStreamReader转换流类图

(1)InputStreamReader转换流为Reader抽象基类的子类
(2)创建InputStreamReader对象实例时,可以传入InputStream抽象基类子类的对象实例,并指定编码
![](E:\Study\自学课程资料\Java\assets\InputStreamReader转换流类图.png)

3、OutputStreamWriter转换流类图

![](E:\Study\自学课程资料\Java\assets\OutputStreamWriter转换流类图.png)

4、InputStreamReader、OutputStreamWriter总结理解

(1)InputStreamReader为Reader抽象基类的子类,创建InputStreamReader的实例对象时,实参可以传入一个InputStream抽象基类子类对象实例,可以将InputStream字节流转换为Reader字符流,并指定编码
(2)OutputStreamWriter为Writer抽象基类的子类,创建OutputStreamWriter的实例对象时,实参可以传入一个OutputStream抽象基类子类对象实例,可以将OutputStream字节流转换为Writer字符流,并指定编码
(3)处理纯文本数据时,若使用字符流效率更高,并且可以有效解决中文问题,所以建议将字节流转换成字符流
(4)可以在使用时指定编码格式(如UTF-8、GBK、GB2312、ISO8859-1等)
5、InputStreamReader案例

/**
 * 演示使用InputStreamReader转换流解决中文乱码问题
 * 将字节流FileInputStream转成处理流中的转换流InputStreamReader,指定编码为GBK
 */
public class InputStreamReader01 {
    public static void main(String[] args) {
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\codeQuestion\\test1.txt";
        InputStreamReader inputStreamReader = null;
        try {
            /*
            1.将字节输入流FileInputStream通过转换流InputStreamReader转换为字符输入流
            2.创建BufferedReader类实例对象时,实参传入InputStreamReader类实例对象
             */
            inputStreamReader = new InputStreamReader(new FileInputStream(srcPath), "GBK");
            BufferedReader bufferedReader = new BufferedReader(inputStreamReader);
            String s = bufferedReader.readLine();
            System.out.println(s);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                inputStreamReader.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
6、OutputStreamWriter案例

public class OutputStreamWriter01 {
    public static void main(String[] args) {
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\codeQuestion\\test1.txt";
        BufferedWriter bufferedWriter = null;
        try {
            /*
            1.将字节输出流FileOutputStream通过转换流OutputStreamWriter转换为字符输出流
            2.BufferedWriter为Writer抽象基类的子类,有属性Writer out,可以传入Writer抽象基类的子类对象
            3.创建一个BufferedWriter对象实例,实参中传入OutputStreamWriter对象实例
             */
            bufferedWriter = new BufferedWriter(new OutputStreamWriter(new FileOutputStream(destPath), "UTF-8"));
            bufferedWriter.write("蒋兴树丁维一");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                bufferedWriter.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            } finally {
                try {
                    //关闭外层流
                    bufferedWriter.close();
                } catch (IOException e) {
                    System.out.println(e.getMessage());
                }
            }
        }
    }
}
PrintStream、PrintWriter打印流
1、PrintStream类图

![](E:\Study\自学课程资料\Java\assets\PrintStream打印流类图.png)

2、PrintWriter类图

![](E:\Study\自学课程资料\Java\assets\PrintWriter打印流类图.png)

3、打印流代码理解

public class PrintStream01 {
    public static void main(String[] args) {

    }

    @Test
    public void printStreamExercise() {
        /*
        1.默认情况下,PrintStream输出数据位置是显示器(标准输出)
        2.public final static PrintStream out = null
         */
        PrintStream out = System.out;
        /*
        1.print底层源码:
        public void print(String s) {
            if (s == null) {
                s = "null";
            }
            write(s);
        }
        2.print底层使用write()方法,即我们可以调用write()方法进行打印输出
         */
        out.print("hello");
        try {
            out.write("jxs".getBytes());
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }

        /*
        1.可以修改打印流输出的位置
         */
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\codeQuestion\\test1.txt";
        try {
            System.setOut(new PrintStream(destPath));
            System.out.println("jxsjxsjxsxjxs");
        } catch (FileNotFoundException e) {
            System.out.println(e.getMessage());
        }
    }


    @Test
    public void printWriterExercise() {
        /*
        1.创建PrintWriter对象实例时,实参可以传入OutputStream、Writer抽象基类子类对象实例
        2.public final static PrintStream out = null,out的类型为PrintStream
        3.PrintStream类为FilterOutputStream类的子类,FilterOutputStream类为OutputStream类的子类
         */
        //PrintWriter printWriter = new PrintWriter(System.out);
        PrintWriter printWriter1 = null;
        try {
            printWriter1 = new PrintWriter(new FileWriter("E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\codeQuestion\\test1.txt"));
            printWriter1.print("jxsdwy");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            //printWriter.close();
            printWriter1.close();
        }
    }
}
##### 

Properties类
1、基本介绍

(1)专门用于读写配置文件的集合类(配置文件的格式:键=值)
(2)键值对不需要有空格,值不需要用引号引起来,默认类型为String
2、Properties读文件

public class Properties01 {
    public static void main(String[] args) {
        //创建Properties对象
        Properties properties = new Properties();
        //加载配置文件
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\IOStream\\src\\mysql.properties";
        try {
            properties.load(new FileReader(srcPath));
            //将键值对显示到控制台
            properties.list(System.out);
            //根据键获取对应的值
            String root = properties.getProperty("root");
            String pwd = properties.getProperty("pwd");
            System.out.println(root);
            System.out.println(pwd);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }
}
3、Properties修改文件

public class Properties01 {
    public static void main(String[] args) {
        /*
        1.创建Properties对象
        2.Properties的父类为HashTable
         */
        Properties properties = new Properties();
        /*
        1.若不存在key则创建键值对
        2.若存在则修改key对应的value
         */
        properties.setProperty("charset", "UTF-8");
        properties.setProperty("root", "jxs");
        properties.setProperty("pwd", "123");

        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\IOStream\\src\\mysql1.properties";
        try {
            /*
            1.将键值对存储到文件中
            2.null 添加注释
             */
            properties.store(new FileWriter(destPath), null);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }
}
IO流总练习
练习一：

(1)在判断E盘下是否有文件夹homework,若没有就创建
(2)在homework目录下,创建文件hello.txt
(3)若hello.txt已存在,提示该文件已经存在
(4)在hello.txt文件中,写入hello,world~
public class Homework01 {
    public static void main(String[] args) {

    }

    @Test
    public void createFile() {
        String directory = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Homework";
        String file = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Homework\\hello.txt";
        FileWriter fileWriter = null;
        File file1 = new File(directory);
        File file2 = new File(file);

        //若目录不存在则创建目录并提示目录创建成功,若目录存在则提示目录创建失败
        if (!file1.exists()) {
            file1.mkdirs();
            System.out.println("目录创建成功");
        } else {
            System.out.println("目录创建失败");
        }

        if (!file2.exists()) {
            try {
                file2.createNewFile();
                System.out.println("文件创建成功");
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        } else {
            System.out.println("文件已存在");
        }

        try {
            fileWriter = new FileWriter(file);
            fileWriter.write("hello,world~");
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                fileWriter.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }
    }
}
练习二：

使用BufferedReader读取一个文本文件(编码模式为GBK)，为每行加上行号，再连同内容一并输出到屏幕上。
默认读取文本文件是按照UTF-8处理,读取编码模式为GBK的文本文件就需要用到转换流
public class Homework02 {
    public static void main(String[] args) {
    }

    @Test
    public void fileRead() {
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Homework\\hello.txt";
        String line;
        int num = 1;
        InputStreamReader inputStreamReader;
        FileReader fileReader;

        try {
            inputStreamReader = new InputStreamReader(new FileInputStream(srcPath),"UTF-8");
            BufferedReader bufferedReader = new BufferedReader(inputStreamReader);
            while ((line = bufferedReader.readLine()) != null) {
                System.out.println(num++ + line);
            }
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }
    }
}
练习三：

(1)要编写一个dog.properties
name=tom
age=5
color=red
(2)编写Dog类(name,age,color)创建一个dog对象,读取dog.properties用相应的内容完成属性初始化.并输出
(3)将创建的Dog对象,序列化到文件dog.dat文件
public class Homework03 {
    public static void main(String[] args) {
        //Properties源文件路径
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\IOStream\\src\\dog.properties";
        //创建Properties对象
        Properties properties = new Properties();

        Dog dog = null;
        ObjectOutputStream objectOutputStream = null;
        ObjectInputStream objectInputStream;

        try {
            properties.load(new FileReader(srcPath));
            String name = (String) properties.get("name");
            int age = Integer.parseInt((String) properties.get("age"));
            String color = (String) properties.get("color");
            dog = new Dog(name, age, color);
            System.out.println(dog);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        }

        //序列化
        String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\Homework\\hello.txt";
        try {
            objectOutputStream = new ObjectOutputStream(new FileOutputStream(destPath));
            objectOutputStream.writeObject(dog);
        } catch (IOException e) {
            System.out.println(e.getMessage());
        } finally {
            try {
                objectOutputStream.close();
            } catch (IOException e) {
                System.out.println(e.getMessage());
            }
        }

        //反序列化
        try {
            objectInputStream = new ObjectInputStream(new FileInputStream(destPath));
            Object o = objectInputStream.readObject();
            System.out.println(o);
        } catch (IOException | ClassNotFoundException e) {
            System.out.println(e.getMessage());
        }
    }
}


class Dog implements Serializable {
    private String name;
    private int age;
    private String red;

    public Dog(String name, int age, String red) {
        this.name = name;
        this.age = age;
        this.red = red;
    }

    @Override
    public String toString() {
        return "Dog{" +
                "name='" + name + '\'' +
                ", age=" + age +
                ", red='" + red + '\'' +
                '}';
    }
}
1.3、代码实现能力
1.3.1、网络编程
网络基础
lnetAddress
Socket
TCP编程
UDP编程
1.3.2、反射
反射机制引出（总结最精辟！！！）
通过外部文件配置,在不修改源码的情况下来控制程序,也符合设计模式的ocp原则(开闭原则:不修改源码,扩展功能)
/**
 * 反射问题引入
 * 根据配置文件re.properties指定信息,创建Cat类对象实例并调用hi()方法
 * re.properties文件信息:
 * classpath=reflection.Cat
 * method=hi
 */
public class ReflectionQuestion {
    public static void main(String[] args) throws Exception {
        /*
        1.传统方法:
        使用new关键字创建Cat类对象实例并调用hi()用法
        Cat cat = new Cat();
        cat.hi();

        2.反射机制方法:
         */
        String str = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\反射\\src\\re.properties";
        //1.使用Properties类,创建对象实例,读写配置文件
        Properties properties = new Properties();
        //2.加载配置文件
        properties.load(new FileInputStream(str));
        //3.get()方法,由key得到对应的value值
        String classpath = properties.get("classpath").toString();
        String method = properties.get("method").toString();
        /*
        4.Class类的对象实例即正在运行的java应用程序中的类和接口
        5.使用Class类中的forName()静态方法获取类对应的字节码的对象
        6.解剖一个类,先获得该类的字节码对象
        6.字节码对象aClass包含了类的完整结构信息,通过这个对象得到类的结构
         */
        Class aClass = Class.forName(classpath);
        //7.通过aClass得到classpath(reflection.Cat)的对象实例
        Object o = aClass.newInstance();
        System.out.println("o的运行类型:" + o);
        /*
        8.通过aClass得到classpath(reflection.Cat)的方法对象
          在反射中,将方法视为对象
        9.传统方法:对象.方法()
          反射机制:方法.invoke(对象)
         */
        Method method1 = aClass.getMethod(method);
        method1.invoke(o);
    }
}
总结:Java应用程序中正在运行的一个类和接口都对应一个Class类型的字节码对象,该字节码对象包含该类的完整结构信息
反射机制理解（重要重要！！！！）
1、反射机制理解

(1)
反射机制允许程序在执行期间借助于Reflection API取得任何类的内部信息
并能操作对象的属性及方法。反射在设计模式以及底层框架都会用到

(2)
类加载完毕后,在堆中产生一个Class类型的字节码对象(Java应用程序中正在运行的一个类和接口对应一个字节码对象),字节码对象包含该类的完整结构信息！

(3)字节码对象就好比一面镜子,透过这个字节码对象可以看到类的结构,所以形象的称为反射！！
2、Java反射机制原理图



3、反射机制好处

(1)在运行时判断一个对象所属的类
(2)在运行时创建一个类的对象实例
(3)在运行时得到一个类的成员变量、成员方法
(4)在运行时调用一个类的成员变量、成员方法
(5)生成动态代理
4、反射相关的类

(1)java.lang.Class<T>:Java应用程序中正在运行的一个类和接口都对应一个在堆中Class类的字节码对象
(2)java.lang.reflect.Method:提供关于类或接口上单独某个方法（以及如何访问该方法）的信息。
(3)java.lang.reflect.Field:提供有关类或接口的单个字段的信息，以及对它的动态访问权限。
(4)java.lang.reflect.Constructor<T>:提供关于类的单个构造方法的信息以及对它的访问权限。 
5、反射代码理解

/**
 * 反射问题引入
 * 根据配置文件re.properties指定信息,创建Cat类对象实例并调用hi()方法
 * re.properties文件信息:
 * classpath=reflection.Cat
 * method=hi
 */
public class ReflectionQuestion {
    public static void main(String[] args) throws Exception {
        /*
        1.传统方法:
        使用new关键字创建Cat类对象实例并调用hi()用法
        Cat cat = new Cat();
        cat.hi();

        2.反射机制方法:
         */
        String str = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\反射\\src\\re.properties";
        //1.使用Properties类,创建对象实例,读写配置文件
        Properties properties = new Properties();
        //2.加载配置文件
        properties.load(new FileInputStream(str));
        //3.get()方法,由key得到对应的value值
        String classpath = properties.get("classpath").toString();
        String method = properties.get("method").toString();
        /*
        4.Class类的对象实例即正在运行的java应用程序中的类和接口
        5.使用Class类中的forName()静态方法获取类对应的字节码的对象
         */
        Class aClass = Class.forName(classpath);
        //6.通过aClass得到classpath(reflection.Cat)的对象实例
        Object o = aClass.newInstance();
        System.out.println("o的运行类型:" + o);
        /*
        7.通过aClass得到classpath(reflection.Cat)的方法对象
          在反射中,将方法视为对象
        8.传统方法:对象.方法()
          反射机制:方法.invoke(对象)
         */
        Method method1 = aClass.getMethod(method);
        method1.invoke(o);
        /*
        9.aClass字节码对象包含Cat类的完整结构信息
          java.lang.reflect.Field:提供有关类或接口的单个字段的信息
          字节码对象.getField(字段名),默认不可得到私有属性
         */
        Field name = aClass.getField("name");
        /*
        10.传统写法:对象.成员变量名
           反射机制:成员变脸名.get.(对象)
         */
        System.out.println(name.get(o));
        /*
        11.()中指定构造器参数类型
           String.class传入的是String类的Class类的对象
         */
        Constructor constructor1 = aClass.getConstructor();
        System.out.println(constructor1);
        Constructor constructor2 = aClass.getConstructor(String.class);
        System.out.println(constructor2);
    }
}

/*
输出结果：
o的运行类型:reflection.Cat@1b6d3586
hidwy
dwy
public reflection.Cat()
public reflection.Cat(java.lang.String)
*/
反射调用优化
1、优缺点

(1)优点:动态的创建和使用对象(框架底层核心),使用灵活,没有反射机制,框架技术就失去底层支撑
(2)缺点:使用反射基本是解释执行,对执行速度有影响
2、优缺点代码理解

/**
 * 测试反射调用的性能以及优化方案
 */
public class Reflection01 {
    public static void main(String[] args) throws Exception {
        method1();
        method2();
    }

    /*
    1.传统方法来调用Cat类的hi()方法
     */
    public static void method1() {
        Cat cat1 = new Cat();
        long start = System.currentTimeMillis();
        for (int i = 0; i < 90000000; i++) {
            cat1.hi();
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
    }

    /*
    2.反射机制来调用Cat类的hi()方法
     */
    public static void method2() throws Exception {
        Class aClass = Class.forName("reflection.Cat");
        Object o = aClass.newInstance();
        Method hi = aClass.getMethod("hi");
        long start = System.currentTimeMillis();
        for (int i = 0; i < 90000000; i++) {
            hi.invoke(o);
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
    }
}

/*
输出结果：
4
148
*/
3、反射调用优化

(1)Method、Filed、Constructor对象都有setAccessible()方法
(2)setAccessible()方法的作用是启动和禁用访问安全检查的开关
(3)若参数值为true则反射的对象在使用时取消访问安全检查,提高反射的效率;若参数值为false则反射的对象在使用时执行访问安全检查。
/**
 * 测试反射调用的性能以及优化方案
 */
public class Reflection01 {
    public static void main(String[] args) throws Exception {
        method1();
        method2();
        method3();
    }

    /*
    1.传统方法来调用Cat类的hi()方法
     */
    public static void method1() {
        Cat cat1 = new Cat();
        long start = System.currentTimeMillis();
        for (int i = 0; i < 90000000; i++) {
            cat1.hi();
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
    }

    /*
    2.反射机制来调用Cat类的hi()方法
     */
    public static void method2() throws Exception {
        Class aClass = Class.forName("reflection.Cat");
        Object o = aClass.newInstance();
        Method hi = aClass.getMethod("hi");
        long start = System.currentTimeMillis();
        for (int i = 0; i < 90000000; i++) {
            hi.invoke(o);
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
    }

    /*
    3.反射调用优化,关闭访问安全检查
     */
    public static void method3() throws Exception {
        Class aClass = Class.forName("reflection.Cat");
        Object o = aClass.newInstance();
        Method hi = aClass.getMethod("hi");
        hi.setAccessible(true);
        long start = System.currentTimeMillis();
        for (int i = 0; i < 90000000; i++) {
            hi.invoke(o);
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
    }
}
Class类（重要重要！！！！！！！）
1、Class类类图

![](E:\Study\自学课程资料\Java\assets\Class类类图.png)

2、基本介绍

(1)Class类也是类,也继承Object类
(2)类加载时通过类加载器(ClassLoader)的loadClass()方法得到某个类的Class类的字节码对象
(3)同一个类只加载一次,即Java应用程序中正在运行的一个类对应Class类的一个字节码对象
(4)每个类的对象实例都知道属于Class类的哪个字节码对象
(5)通过Class类的字节码对象可以完整的得到一个类的完整结构
(6)Class类的字节码对象存放在堆中
(7)
代码经javac编译后,生成.class字节码文件
.class字节码文件通过类加载器(ClassLoader)的loadClass()方法在堆中的到这个类的Class类的字节码对象以及在方法区中生成这个类的字节码二进制数据(元数据)
3、代码演示

public class Class01 {
    public static void main(String[] args) throws Exception {
        /*
        创建对象实例
        1.传统方法:new关键字
        public Class<?> loadClass(String name) throws ClassNotFoundException {
            return loadClass(name, false);
        }
         */
        Cat cat = new Cat();

        /*
        2.反射机制
        同一个类只加载一次,即Java应用程序中正在运行的一个类对应Class类的一个字节码对象
        aClass1、aClass2为同一个字节码对象
        public Class<?> loadClass(String name) throws ClassNotFoundException {
            return loadClass(name, false);
        }
         */
        Class<?> aClass1 = Class.forName("reflection.Cat");
        Class<?> aClass2 = Class.forName("reflection.Cat");
        System.out.println(aClass1.hashCode());
        System.out.println(aClass2.hashCode());

        //每个类的对象实例都知道属于Class类的哪个字节码对象
        System.out.println(cat.getClass());
    }
}
4、Class类常用方法

public class Class02 {
    public static void main(String[] args) throws Exception {
        //1.获取Car类对应的Class类的字节码对象
        Class aClass = Class.forName("class_.Car");
        //2.输出 aClass字节码对象 是 哪个类 的 Class类的字节码对象
        System.out.println(aClass);
        //3.输出aClass的运行类型
        System.out.println(aClass.getClass());
        //4.通过字节码对象得到对应的类的包名
        System.out.println(aClass.getPackage().getName());
        //5.通过字节码对象得到对应的类的全类名
        System.out.println(aClass.getName());
        //6.通过字节码对象得到对应的类的对象实例
        Object o = aClass.newInstance();
        System.out.println(o.toString());
        //7.通过字节码对象得到对应的类的成员变量
        Field brand1 = aClass.getField("brand");
        Field brand2 = aClass.getField("price");
        Field brand3 = aClass.getField("color");
        System.out.println(brand1.get(o));
        System.out.println(brand2.get(o));
        System.out.println(brand3.get(o));
        //8.通过反射为成员变量赋值
        brand1.set(o,"奔驰");
        System.out.println(brand1.get(o));
        //9.遍历Car类的所有成员变量
        Field[] fields = aClass.getFields();
        for (Field field : fields) {
            System.out.println(field.getName());
        }
    }
}

class Car {
    public String brand = "宝马";
    public int price = 1000000;
    public String color = "黑色";

    @Override
    public String toString() {
        return "Car{" +
                "brand='" + brand + '\'' +
                ", price=" + price +
                ", color='" + color + '\'' +
                '}';
    }
}
5、获取Class类字节码对象方式

(1)已知一个类的全类名,且该类在类路径下,可以通过Class类的静态方法forName()获取,可能抛出ClassNotFoundException
应用场景:多用于配置文件,读取类全路径,加载类

(2)已知具体的类,通过类的class获取,该方式最安全可靠、程序性能最高
应用场景:多用于参数传递,比如通过反射得到对应类的构造器对象

(3)已知某个类的对象实例,调用该对象实例的getClass()方法
应用场景:通过创建好的对象,获取该对象所属的类的字节码对象

(4)通过类加载器获取类对应的字节码对象,先得到类加载器,再调用类加载器的loadClass()方法得到字节码对象

(5)基本数据类型通过 基本数据类型.class 获得对应的Class类的字节码对象

(6)基本数据类型对应的包装类通过 包装类.TYPE 获得对应的Class类的字节码对象
/**
 * 演示得到Class类字节码对象的方式
 */
public class GetClass01 {
    public static void main(String[] args) throws Exception {
        /*
        1.方式一:通过字节码对象得到这个字节码对象是属于哪个类的字节码对象
         */
        Class<?> aClass = Class.forName("class_.Car");
        System.out.println(aClass);

        /*
        2.方式二
         */
        System.out.println(Car.class);

        /*
        3.方式三:已知某个类的对象实例,调用该对象实例的getClass()方法
         */
        Car car = new Car();
        System.out.println(car.getClass());

        /*
        4.方式四:通过类加载器获取类对应的字节码对象
        先得到类加载器,再调用类加载器的loadClass()方法得到字节码对象
         */
        ClassLoader classLoader = car.getClass().getClassLoader();
        Class<?> aClass1 = classLoader.loadClass("class_.Car");
        System.out.println(aClass1);

        /*
        5.方式五:基本数据类型通过 基本数据类型.class 获得对应的Class类的字节码对象
         */
        Class<Integer> integerClass = int.class;
        System.out.println(integerClass);

        /*
        6.方式六:基本数据类型对应的包装类通过 包装类.TYPE 获得对应的Class类的字节码对象
         */
        Class<Integer> type1 = Integer.TYPE;
        Class<Character> type2 = Character.TYPE;
        System.out.println(type1);
        System.out.println(type2);
    }
}
6、哪些类型有Class类型的字节码对象

(1)外部类,成员内部类,静态内部类,局部内部类,匿名内部类
(2)interface
(3)数组
(4)enum:枚举类
(5)annotation:注解类
(6)基本数据类型
(7)void
public class AllTypeClass {
    public static void main(String[] args) {
        Class<String> class1 = String.class;//外部类
        Class<Serializable> class2 = Serializable.class;//接口
        Class<Integer[]> class3 = Integer[].class;//数组
        Class<int[][]> class4 = int[][].class;//二维数组
        Class<Deprecated> class5 = Deprecated.class;//注解
        Class<Thread.State> class6 = Thread.State.class;//枚举
        Class<Long> class7 = long.class;//基本数据类型
        Class<Void> class8 = void.class;//void数据类型
        Class<Class> class9 = Class.class;
        System.out.println(class1);
        System.out.println(class2);
        System.out.println(class3);
        System.out.println(class4);
        System.out.println(class5);
        System.out.println(class6);
        System.out.println(class7);
        System.out.println(class8);
        System.out.println(class9);
    }
}
类加载
1、基本说明

(1)反射机制是Java实现动态语言的关键,也就是通过反射实现类动态加载
(2)静态加载:编译时加载相关的类,若没有则报错,依赖性强
(3)动态加载:编译时若不存在相关的类也不会报错,运行时加载需要的类,若运行时不使用该类则不报错,降低依赖性
public class ClassLoad01 {
    public static void main(String[] args) throws Exception {
        Scanner scanner = new Scanner(System.in);
        System.out.println("请输入key");
        String next = scanner.next();

        switch (next) {
            case "1":
                /*
                静态加载:编译时加载相关的类,若没有则报错,依赖性强
                1.new Dog()为静态加载
                2.编译前必须编写Dog类
                 */
                Dog dog = new Dog();
                dog.cry();
                break;
            case "2":
                /*
                动态加载:运行时加载需要的类,若运行时不使用该类则不报错,降低依赖性
                1.Person类为静态加载
                2.当动态加载到Person类时,若没有才会报错
                 */
                Class<?> person = Class.forName("class_.Person");
                Object o = person.newInstance();
                Method hi = person.getMethod("hi");
                hi.invoke(o);
                break;
        }
    }
}

class Dog {
    public void cry() {
        System.out.println("小狗汪汪叫");
    }
}

class Person {
    public void hi() {
        System.out.println("小孩打招呼");
    }
}
2、类加载时机

(1)使用new关键字创建对象时(静态加载)
(2)子类被加载时,父类也会被加载(静态加载)
(3)调用类中的静态成员(静态加载)
(4)反射(动态加载)
3、类加载流程图

![](E:\Study\自学课程资料\Java\assets\类加载三阶段.png)

4、加载阶段解析

将字节码从不同的数据源(class文件、jar包)转换为
方法区的字节码二进制数据(元数据),并且生成一个Class类的字节码对象
5、连接阶段解析

验证阶段

(1)确保Class文件的字节流中包含的信息符合当前虚拟机的要求,并且不会危害虚拟机自身安全
(2)包括:文件格式验证、元数据验证、字节码验证、符号引用验证
(3)可以考虑使用-Xverify:none参数来关闭大部分的类验证措施,缩短虚拟机类加载时间
准备阶段

(1)对静态变量分配内存并默认初始化(对应数据类型的默认初始值),这些变量所使用的内存都将在方法区中进行分配

class A {
    /*
    属性-成员变量-字段
    类加载 连接阶段 子阶段 准备阶段
    1.n1 静态变量,因此在准备阶段不会分配内存
    2.n2 静态变量,因此在准备阶段进行默认初始化0
    3.n3 静态常量,一旦分配则不可改变,因为在准备阶段直接进行赋值
     */
    public int n1 = 10;
    public static int n2 = 20;
    public static final int n3 = 30;
}
解析阶段

(1)虚拟机将常量池的符号引用替换为直接引用的过程
6、初始化阶段

(1)初始化阶段,真正执行类中定义的Java程序代码,此阶段是执行clinit()方法的过程

(2)
clinit()方法是由编译器按语句在源文件中出现的顺序
依次自动收集类中所有静态变量的赋值动作和静态代码块中的语句,并进行合并

(3)
虚拟机会保证一个类的clinit()方法在多线程环境中被正确地加锁、同步
若多个线程同时去初始化一个类,那么只会有一个线程去执行这个类clinit()方法,其他线程都需阻塞等待,直到活动线程执行clinit()方法完毕
public class ClassLoadInit {
    public static void main(String[] args) throws Exception {
        /*
        1.加载B类,并生成B类对应的Class类的字节码对象
        2.连接阶段 static int num = 0
        3.初始化阶段
            3.1执行clinit()方法
            3.2按语句在源文件中出现的顺序
            3.3依次自动收集类中所有静态变量的赋值动作和静态代码块中的语句
            clinit() {
                System.out.println("B类的静态代码块被执行");
                num = 300;
                static int num = 100;
            }
            3.4进行合并 num = 100
        4.调用类的静态成员时,进行类加载
         */
        System.out.println(B.num);
    }
}

class B {
    //定义静态代码块
    static {
        System.out.println("B类的静态代码块被执行");
        num = 300;
    }

    //定义静态属性num
    static int num = 100;

    //构造器
    public B() {
        System.out.println("B类无参构造被执行");
    }
}
反射获取类的结构信息
第一组（简单）：

public class ReflectionUtils {
    public static void main(String[] args) {

    }

    @Test
    public void api() throws Exception {
        //1.Person类对应的Class类的字节码对象
        Class personClass = Class.forName("api.Person");

        System.out.println("personClass字节码对象对应的Person类的全类名");
        System.out.println(personClass.getName());

        System.out.println("personClass字节码对象对应的Person类的简单类名");
        System.out.println(personClass.getSimpleName());

        System.out.println("获取本类以及父类所有被public修饰的成员变量(属性)");
        Field[] fields = personClass.getFields();
        for (Field field : fields) {
            System.out.println(field.getName());
        }

        System.out.println("获取本类所有成员变量(属性)");
        Field[] declaredFields = personClass.getDeclaredFields();
        for (Field declaredField : declaredFields) {
            System.out.println(declaredField.getName());
        }

        System.out.println("获取本类以及父类所有被public修饰的成员方法");
        Method[] methods = personClass.getMethods();
        for (Method method : methods) {
            System.out.println(method.getName());
        }

        System.out.println("获取本类所有方法");
        Method[] declaredMethods = personClass.getDeclaredMethods();
        for (Method declaredMethod : declaredMethods) {
            System.out.println(declaredMethod.getName());
        }

        System.out.println("获取本类所有被public修饰的构造器");
        Constructor[] constructors = personClass.getConstructors();
        for (Constructor constructor : constructors) {
            System.out.println(constructor.getName());
        }

        System.out.println("获取本类所有构造器");
        Constructor[] declaredConstructors = personClass.getDeclaredConstructors();
        for (Constructor declaredConstructor : declaredConstructors) {
            System.out.println(declaredConstructor.getName());
        }

        System.out.println("返回包信息");
        System.out.println(personClass.getPackage());

        System.out.println("根据superclass字节码对象得到对应的Animal类的全类名");
        Class superclass = personClass.getSuperclass();
        System.out.println(personClass.getSuperclass());

        System.out.println("根据personClass字节码对象得到对应的类的接口信息");
        Class[] interfaces = personClass.getInterfaces();
        for (Class anInterface : interfaces) {
            System.out.println(anInterface);
        }

        System.out.println("根据personClass字节码对象得到对应的类的注解信息");
        Annotation[] annotations = personClass.getAnnotations();
        for (Annotation annotation : annotations) {
            System.out.println(annotation);
        }
    }
}

interface Ability {
    public void fly();
}

class Animal {
    public String species;
    protected int number;

    public void run() {}

    public Animal() {}

    public Animal(String species, int number) {
        this.species = species;
        this.number = number;
    }
}

@Deprecated
class Person extends Animal implements Ability{
    //属性(成员变量)
    public String name;
    protected int age;
    String job;
    private double salary;

    //4种访问修饰符修饰的方法
    public void method1() {}
    protected void method2() {}
    void method3() {}
    private void method4() {}

    //无参构造 有参构造
    public Person() { }
    private Person(String name, int age, String job, double salary) {
        this.name = name;
        this.age = age;
        this.job = job;
        this.salary = salary;
    }

    //实现接口,重写接口方法
    @Override
    public void fly() { }
}
第二组（进阶）：

public class ReflectionUtils01 {
    public static void main(String[] args) {

    }

    @Test
    public void api() throws Exception {
        //Person类对应的Class类的字节码对象
        Class personClass = Class.forName("api.Person");

        /*
        java.lang.reflect.Field类
        1.getDeclaredFields():获取本类所有成员变量(属性)
        2.getModifiers():以int形式返回访问修饰符
          默认访问修饰符 0
          public 1
          private 2
          protected 4
          static 8
          final 16
        3.getType():返回成员变量的数据类型对应的字节码对象
        4.getName():返回属性名
         */
        Field[] declaredFields = personClass.getDeclaredFields();
        for (Field declaredField : declaredFields) {
            System.out.println(declaredField.getName() + " "
                    + declaredField.getModifiers() + " "
                    + declaredField.getType());
        }

        /*
        java.lang.reflect.Method类
        1.getModifiers():以int形式返回访问修饰符
        2.getReturnType:返回方法的返回值的数据类型的字节码对象
        3.getParameterTypes():返回Class类型的数组,元素为形参的数据类型对应的字节码对象
         */
        Method[] declaredMethods = personClass.getDeclaredMethods();
        for (Method declaredMethod : declaredMethods) {
            System.out.println(declaredMethod.getName() + " "
                    + declaredMethod.getModifiers() + " "
                    + declaredMethod.getReturnType());
            Class<?>[] parameterTypes = declaredMethod.getParameterTypes();
            for (Class<?> parameterType : parameterTypes) {
                System.out.println(parameterType);
            }
        }

        /*
        java.lang.reflect.Constructor类
        1.getModifiers():以int形式返回访问修饰符
        2.getParameterTypes():返回Class类型的数组,元素为形参的数据类型对应的字节码对象
         */
        Constructor[] declaredConstructors = personClass.getDeclaredConstructors();
        for (Constructor declaredConstructor : declaredConstructors) {
            System.out.println(declaredConstructor.getName() + " "
                    + declaredConstructor.getModifiers());
            Class[] parameterTypes = declaredConstructor.getParameterTypes();
            for (Class parameterType : parameterTypes) {
                System.out.println(parameterType);
            }
        }
    }
}
反射爆破（重要重要！！！！）
1、通过反射创建对象实例

(1)Class类newInstance()方法:调用类中的无参构造器,获取类的对象实例
(2)Constructor类getConstructor(Class...clazz)方法:根据参数列表,获取对应类被public修饰的构造器对象
(3)Constructor类getDecalaredConstructor(Class...clazz):根据参数列表,获取对应类所有的构造器对象
public class ReflectCreateInstance {
    public static void main(String[] args) throws Exception {
        //获取User类对应的字节码对象,该字节码对象包含该类的完整结构信息
        Class<?> userClass = Class.forName("User");

        /*
        Class类newInstance()方法:
        调用类中的无参构造器,获取User类的对象实例
         */
        Object o1 = userClass.newInstance();
        System.out.println(o1);

        /*
        Constructor类newInstance()方法:
        1.Constructor类getConstructor()方法:根据参数列表获取User类public修饰的构造器对象
        2.Constructor类newInstance()方法:传入实参,创建对象实例
         */
        Constructor<?> constructor = userClass.getConstructor(String.class);
        Object o2 = constructor.newInstance("jxs");
        System.out.println(o2);

        /*
        Constructor类newInstance()方法:
        1.Constructor类getDeclaredConstructor()方法:根据参数列表获取User类所有构造器对象
        2.Constructor类setAccessible()方法:暴破,破坏封装性
        3.Constructor类newInstance()方法:传入实参,创建对象实例
         */
        Constructor<?> declaredConstructor = userClass.getDeclaredConstructor(int.class,String.class);
        //暴破,使用反射可以访问private构造器,破坏私有构造器的封装性
        declaredConstructor.setAccessible(true);
        Object o3 = declaredConstructor.newInstance(21, "dwy");
        System.out.println(o3);
    }
}

class User {
    private int age = 10;
    private String name;

    //public修饰的无参构造器
    public User() {
    }

    //public修饰的有参构造器
    public User(String name) {
        this.name = name;
    }

    //非public修饰的有参构造器
    private User(int age, String name) {
        this.age = age;
        this.name = name;
    }

    @Override
    public String toString() {
        return "User{" +
                "age=" + age +
                ", name='" + name + '\'' +
                '}';
    }
}

/*
输出结果：
User{age=10, name='null'}
User{age=10, name='jxs'}
User{age=21, name='dwy'}
*/
2、通过反射访问类的属性

public class ReflectAccessProperty {
    public static void main(String[] args) throws Exception {
        //获取Student类对应的Class类的字节码对象
        Class<?> studentClass = Class.forName("Student");
        //创建Student类的对象实例
        Object o = studentClass.newInstance();
        //通过反射得到age属性对象
        Field age = studentClass.getField("age");
        //通过反射修改age属性值
        age.set(o,88);
        System.out.println(o);
        /*
        通过反射操作name属性
        1.通过暴破,破坏私有属性的封装性
         */
        Field name = studentClass.getDeclaredField("name");
        name.setAccessible(true);
        //name.set(o,"jxs");
        //name为静态属性
        name.set(null,"jxs");
        System.out.println(o);

    }
}

class Student {
    public int age;
    private static String name;

    public Student() {
    }

    @Override
    public String toString() {
        return "Student{" +
                "age=" + age + " " +
                "name=" + name +
                '}';
    }
}

/*
输出结果：
Student{age=88 name=null}
Student{age=88 name=jxs}
*/
3、通过反射访问类的方法

public class ReflectAccessMethod {
    public static void main(String[] args) throws Exception {
        //获取Boss类对应的Class类的字节码对象
        Class<?> bossClass = Class.forName("Boss");

        //获取Student类的对象实例
        Object o = bossClass.newInstance();

        //获取Student类的hi方法对象
        Method hi = bossClass.getMethod("hi", String.class);
        hi.invoke(o, "jxs");

        //获取Student类的say方法对象。通过暴破,破坏私有属性的封装性
        Method say = bossClass.getDeclaredMethod("say", int.class, String.class, char.class);
        say.setAccessible(true);
        //say()为静态方法
        System.out.println(say.invoke(null, 1, "2", '3'));
        System.out.println(say.invoke(o, 1, "2", '3'));

        /*
        在反射中,若方法有返回值则统一返回Object
        invoke运行类型和方法中定义的返回值类型一致
         */
        Object invoke = say.invoke(o, 200, "jxs", '男');
        System.out.println(invoke);
        System.out.println(invoke.getClass());
    }
}

class Boss {
    public int age;
    private static String name;

    public Boss() {
    }

    private static String say(int n, String s, char c) {
        return n + " " + s + " " + c;
    }

    public void hi(String s) {
        System.out.println("hi" + s);
    }
}

/*
输出结果：
hijxs
1 2 3
1 2 3
200 jxs 男
class java.lang.String
*/
反射总练习
1、练习一

1.定义PrivateTest类,有name私有属性,并且属性值为hellokitty
2.提供getName的公有方法
3.获取PrivateTest的类对应的Class类的字节码对象,获取name私有属性并修改属性的值
4.调用getName()的方法打印name私有属性的值
public class Homework01 {
    public static void main(String[] args) throws Exception {
        Class privateTest = Class.forName("PrivateTest");
        Object o = privateTest.newInstance();
        Field name = privateTest.getDeclaredField("name");
        name.setAccessible(true);
        name.set(o,"jxs");
        Method getName = privateTest.getMethod("getName");
        System.out.println(getName.invoke(o));
    }
}

class PrivateTest {
    private String name = "helloKitty";

    public String getName() {
        return name;
    }
}
2、练习二

1.利用Class类的forName()方法获取File类对应的的class类的字节码对象
2.在控制台打印File类的所有构造器
3.通过newlnstance()的方法创建File对象实例
4.并创建reflect.txt文件
public class Homework02 {
    public static void main(String[] args) throws Exception {
        //获取java.io.File类对应的Class类的字节码对象
        Class<?> fileClass = Class.forName("java.io.File");
        //获取File类所有构造器对象
        Constructor<?>[] constructors = fileClass.getDeclaredConstructors();
        //增强for遍历所有构造器
        for (Constructor<?> constructor : constructors) {
            System.out.println(constructor);
            String destPath = "E:\\application\\IntelliJ IDEA 2021.1\\IOStream\\reflect.txt";
            //调用构造器创建File类对象实例
            Constructor<?> constructor1 = fileClass.getConstructor(String.class);
            Object o = constructor1.newInstance(destPath);
            //获取createNewFile方法对象
            Method createNewFile = fileClass.getMethod("createNewFile");
            createNewFile.invoke(o);
        }
    }
}
1.3.3、Mysql基础
数据库介绍
1、数据库概念

淘宝网、京东、微信、抖音都有各自的功能,为何当我们退出系统时,下次再访问信息仍存在?

为解决上述问题,使用更加利用管理数据的京东-数据库

图书馆是保存书籍的,数据库即保存数据的
2、数据库简单原理图



MySQL安装
1、MySQL下载地址

https://dev.mysql.com/downloads/installer/
2、若安装过程中出现错误或重新安装MySQL，删除已安装的mysql服务

sc delete mysql
3、安装mysql-installer-community-8.0.31.0.msi





























4、添加环境变量，在任意目录下操作MySQL相关指令

此电脑 -> 属性 -> 高级系统设置 -> 环境变量 -> 用户变量 -> Path

E:\application\MySQL\MySQL Server 8.0\bin
5、Win+R打开命令行，输入mysql -u root -p，确认后输入设置的密码123456

C:\Users\86188>mysql -u root -p
Enter password: ******
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 11
Server version: 8.0.31 MySQL Community Server - GPL

Copyright (c) 2000, 2022, Oracle and/or its affiliates.

Oracle is a registered trademark of Oracle Corporation and/or its
affiliates. Other names may be trademarks of their respective
owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.
6、客户端使用命令行连接（MySQL服务）MySQL数据库指令

mysql -h 主机IP -P 端口号 -u 用户名 -p密码

(1)-p密码之间无空格
(2)-p后若没有密码,回车后要求输入
(3)若没有写主机IP,默认为localhost
(4)若没有写端口号,默认为3306
(5)实际工作中,端口号一般会修改
Navicat安装和使用
1、Navicat介绍

图形化MySQL管理软件
2、Navicat连接数据库

<img src="E:\Study\自学课程资料\Java\assets\Navicat连接数据库.png" style="zoom: 50%;" />

3、Navicat新建数据库

<img src="E:\Study\自学课程资料\Java\assets\Navicat新建数据库.png" style="zoom:50%;" />

3、Navicat新建表

<img src="E:\Study\自学课程资料\Java\assets\Navicat新建表.png" style="zoom:50%;" />

4、Navicat表中添加数据

<img src="E:\Study\自学课程资料\Java\assets\Navicat表中添加数据.png" style="zoom:50%;" />

MySQL三层结构
1、所谓安装MySQL数据库，即在主机上安装一个数据库管理系统（DBMS，DataBase Manage System），数据库管理系统可以管理多个数据库

2、一个数据库中可以创建多个表，来保存数据

3、数据库管理系统、数据库、表关系图

![](E:\Study\自学课程资料\Java\assets\MySQL三层结构.png)

4、MySQL创建的数据库的位置

![](E:\Study\自学课程资料\Java\assets\创建数据库位置.png)

5、MySQL创建的表的位置

![](E:\Study\自学课程资料\Java\assets\创建表位置.png)

6、数据在数据库中的存储方式

![](E:\Study\自学课程资料\Java\assets\数据在数据库中的存储方式.png)

7、SQL语句分类

(1)DDL:数据定义语句
(2)DML:数据操作语句(增删改)
(3)DQL:数据查询语句(查)
(4)DCL:数据控制语句
8、总结

(1)安装MySQL,即在主机上安装了一个数据库管理系统,通过端口3306可以去监听数据库管理系统
(2)MySQL数据库普通表的本质仍是文件
(3)例:客户端在命令终端属于指令select * from user,发送给端口3306监听的数据库管理系统,数据库管理系统快速定位到user表,最后将结果展示在客户端
列类型（数据类型）之整型
1、基本介绍

使用规范
(1)在满足需求的情况下,选择占用空间小的数据类型
类型	字节	最小值最大值（带符号）	最小值最大值（无符号）
tinyint	1	-128~127	0~255
smallint	2	-2^15~2^15-1	0~2^16-1
mediumint	3	-2^23~2^23-1	0~2^24-1
int	4	-2^31~2^31-1	0~2^32-1
bigint	8	-2^63~2^63-1	0~2^64-1
2、案例演示

# 若没有指定unsinged,则tinyint有符号
# tinyint有符号-128~127 无符号0~255
CREATE TABLE `tinyint`(
id TINYINT);

# 插入数据
INSERT into `tinyint` VALUES (-128);
# 插入数据
INSERT into `tinyint` VALUES (127);
# 插入数据,值超出范围
INSERT into `tinyint` VALUES (-129);
# 插入数据,值超出范围
INSERT into `tinyint` VALUES (128);
列类型（数据类型）之bit
# bit(m) m范围1~64
# 添加数据范围按照给定的位数确定,m=8则表示一个字节0~255
CREATE TABLE table01(
num bit(8));

INSERT INTO table01 VALUES(1);
INSERT INTO table01 VALUES(255);

SELECT * FROM table01;
列类型（数据类型）之小数型
1、基本介绍

(1)float单精度;double双精度
(2)DECIMAL[M,D]:支持更准确地小数位,M为小数位数的总数,D为小数点后的位数。若D为0则没有小数点或分数部分。M最大为65,D最大为30。若D被省略则默认为10
2、案例演示

CREATE TABLE table02(
num1 FLOAT,
num2 DOUBLE,
num3 DECIMAL(30,20));

# 添加数据
INSERT INTO table02 VALUES(88.123456789,88.123456789,88.123456789);

# 查询数据
SELECT * FROM table02;

# DECIMAL可以存放很大的数
CREATE TABLE table03(
num1 DECIMAL(65));

# 插入数据
INSERT INTO table03 VALUES (7898998798789789797776555554444444564656);

# 查询数据
SELECT * FROM table03;
列类型（数据类型）之字符串
1、基本介绍

(1)char(size):固定长度字符串,最大为255字符,无论中文、字母,一个为一个字符
(2)varchar(size):可变长度字符串,最大为65532字节(1-3个字节用于记录大小,utf8mb4编码为最大16383字符,(65535-3)/4=16383)
2、案例演示

# Navicat中注释快捷键Ctrl+/
CREATE TABLE table03(
`name` CHAR(255));

# 若表的编码是utf8mb4,varchar(size=(65535-3)/4=16383)
CREATE TABLE table04(
`name` VARCHAR(16383));
3、不同字符集编码下：英文、中文、emoji表情所占的字节数

编码	英文所占字节	中文所占字节	emoji表情所占字节
utf8mb4	1	3	4
UTF-8	1	3	
GBK	1	2	
Unicode	1	2	
4、字节、字符

位(bit):计算机内部数据储存的最小单位
字节(byte):计算机中数据处理的基本单位,1byte=8bit
字符:计算机中使用的字母、数字、字、符号

如下为一个字符:
(1)1个中文
(2)1个英文字母
(3)1个中文标点符号
(4)1个英文标点符号
5、MySQL创建字符串细节

(1)char(4):4表示字符数(最大255),无论中文、字母,一个为一个字符
(2)varchar(4):4表示字符数,不管字母、中文都以定义好的表的编码来存放数据
(3)char(4)为定长,即插入'aa',只插入两个字符也会占用分配的4个字符
(4)varchar(4)为变长,即插入'aa',只插入两个字符,实际占用空间大小并不是4个字符,而是按照实际占用空间来分配(varchar本身需要占用1-3个字节来记录存放内容长度)
(5)若数据定长推荐使用char,若数据不定长使用varchar,即查询速度:char > varchar
(6)存放文本时,也可以使用Text数据类型,将Text列视为varchar列
(7)TINYTEXT大小0~2^8-1字节、Text大小0~2^16-1字节、MEDIUMTEXT大小0~2^24-1字节、LONGTEXT大小0~2^32-1字节
# char(4)、varchar(6)
# 4、6表示字符,中文或字母1个为1个字符
CREATE TABLE table05(
`name` CHAR(4));
INSERT INTO table05 VALUES('蒋兴树')
INSERT INTO table05 VALUES('丁维一')


CREATE TABLE table06(
`name` VARCHAR(6));
INSERT INTO table06 VALUES ('蒋兴树dwy');


# 若varchar大小不够使用,可以考虑使用text,也可以考虑使用mediumtext(中等的, 适中的)或者longtext
CREATE TABLE IF NOT EXISTS table07(
content1 TEXT,
content2 MEDIUMTEXT,
content3 LONGTEXT)
INSERT INTO table07 VALUES('jxsjxs','jxsjxsdwydwy','jxsjxsjxsdwydwy~~~');
列类型（数据类型）之日期类型
# date datetime timestamp
# 若希望logintime自动更新到当前时间,则在TIMESTAMP添加如下配置
# 若更新table08表某条记录,logintime自动更新
CREATE TABLE IF NOT EXISTS table08(
birthday DATE,
jobtime DATETIME,
logintime TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP
ON UPDATE CURRENT_TIMESTAMP);

INSERT INTO table08(birthday,jobtime) VALUES('2022-11-11','2022-11-11 10:10:10');
操作数据库
1、创建数据库

# 创建数据库
CREATE DATABASE IF NOT EXISTS jxs_database;

# 创建使用关键字为数据库名的数据库
CREATE DATABASE IF NOT EXISTS `CREATE`

# 创建字符集为utf8mb4的dwy_database
CREATE DATABASE IF NOT EXISTS dwy_database CHARACTER SET utf8mb4;

# 创建字符集为utf8mb4,且带校验规则的tyh_database
CREATE DATABASE IF NOT EXISTS tyh_database CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci;
(1)CHARACTER SET(character set):指定数据库的字符集,若不指定字符集,默认为utf8mb4
(2)COLLATE(collate):指定数据库字符集的校对规则,默认为utf8mb4_0900_ai_ci
(3)数据库中创建表时,若没有指定字符集和字符集校对规则,则默认使用数据库的字符集以及字符集校对规则
(4)创建数据库时,为避免关键字,可以使用反引号解决
2、查询数据库

# 显示所有数据库
SHOW DATABASES

# 显示数据库创建语句
SHOW CREATE DATABASE my_database

# 删除数据库
DROP DATABASE IF EXISTS dwy_database

# 删除使用关键字为数据库名的数据库
DROP DATABASE IF EXISTS `CREATE`
3、备份、恢复数据库

# 备份数据库,在Dos下执行指令,将数据库备份到E:\application\MySQL\MySQL_Dump目录下
# mysqldump指令在MySQL安装目录\bin目录下
# 指令中不输入密码,若输入密码则提示警告:Using a password on the command line interface can be insecure.(在命令行输入密码可能会不安全)
mysqldump -u root -p -B my_database > E:\\application\\MySQL\\MySQL_Dump\\bak.sql


# 方式一:进入数据库命令行,恢复数据库
# 方式二:直接将bak.sql内容复制到查询编辑器中执行
mysql -u root -p123456
mysql> source E:\\application\\MySQL\\MySQL_Dump\\bak.sql


# 备份数据库的表
mysqldump -u root -p my_database user > E:\\application\\MySQL\\MySQL_Dump\\user.sql
创建表
1、基本介绍

CREATE TABLE IF NOT EXISTS table_name(
    field1 datatype,
    field2 datatype,
    field3 datatype
)
CHARACTER SET 字符集 COLLATE 校对规则 engine 存储引擎
(1)field:指定列名
(2)datatype:指定列的数据类型
(3)character set:指定字符集,若不指定则默认使用数据库的字符集
(4)collate:校对规则,若不指定则默认使用数据库的校对规则
(5)engine:存储引擎
2、案例演示

create table if not exists student(
id INT,
`name` VARCHAR(255),
`password` VARCHAR(255),
`birthday` DATE)
CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci ENGINE INNODB;
(1)name、password、birthday为关键字,加反引号
(2)CHARACTER SET:指定字符集为utf8mb4
(3)COLLATE:指定校对规则为utf8mb4_0900_ai_ci
(4)ENGINE:指定存储引擎为INNODB
3、创建表练习

CREATE TABLE IF NOT EXISTS emp(
id INT,
`name` VARCHAR(32),
sex CHAR,
birthday DATE,
entry_date DATETIME,
job VARCHAR(32),
salary DOUBLE,
resume TEXT)
CHARACTER SET utf8mb4 COLLATE utf8mb4_0900_ai_ci;

INSERT INTO emp VALUES(1,'jxs','男','2001-2-10','2023-3-1 9:30:30','软件工程师',10000.0,'开发');

SELECT * FROM emp;
修改表
1、基本介绍

(1)添加列:ALTER TABLE tablename ADD column datatype;
(2)修改列:ALTER TABLE tablename MODIFY column datatype;
(3)删除列:ALTER TABLE tablename DROP column;
(4)查看表结构:desc 表名;
(5)修改表名:RENAME TABLE 旧表名 TO 新表名;
(6)修改表字符集:ALTER TABLE 表名 CHARACTER SET 字符集;
2、案例演示

# 为emp表增加image列
ALTER TABLE emp ADD image VARCHAR(32) ;

# 显示表结构,查看表的所有列
DESC emp;

# 修改job列,使其字符长度为60
ALTER TABLE emp MODIFY job VARCHAR(60);

# 删除sex列
ALTER TABLE emp DROP sex;

# 修改表名
RENAME TABLE emp TO employee;

# 显示表结构,查看表的所有列
DESC employee;

# 修改employee表字符集
ALTER TABLE employee CHARACTER SET utf8;

# 修改列名
ALTER TABLE employee CHANGE name user_name VARCHAR(32);
CRUD语句（create read update delete）
Insert（添加数据）
1、基本介绍

(1)INSERT INTO 表名 (column1,column2...) VALUES (value1,value2...)
2、案例演示

CREATE TABLE goods(
id INT,
good_name VARCHAR(10),
price DOUBLE);

INSERT INTO goods (id,good_name,price) VALUES(10,'华为手机',3000.0);

SELECT * FROM goods;
3、Insert细节说明

(1)插入的数据应与字段的数据类型相同
(2)数据的长度应在列的规定范围内
(3)在values中列出的数据位置必须与被加入的列的排列位置相对应
(4)字符和日期型数据应包含在单引号中
(5)若字段允许为空,列可以插入空值
(6)insert into 表名 (column...) values(),(),()形式添加多条记录
(7)若为表中所有字段添加数据,可以不写前面的字段名称
(8)当不为某个字段赋值时,若有默认值则添加,否则报错
CREATE TABLE phone(
id INT,
phone_name VARCHAR(20),
price DOUBLE);

# 细节1:插入的数据应与字段的数据类型相同,'10'会进行隐式转换
INSERT INTO phone (id,phone_name,price) VALUES(10,'iphone',10000.0);
INSERT INTO phone (id,phone_name,price) VALUES('10','iphone',10000.0);

# 细节2:数据的长度应在列的规定范围内,'iphone小米vivo华为洛基亚红米iphone小米vivo华为洛基亚红米'超过20字符
# INSERT INTO phone (id,phone_name,price) VALUES('10','iphone小米vivo华为洛基亚红米iphone小米vivo华为洛基亚红米',10000.0);

# 细节3:在values中列出的数据位置必须与被加入的列的排列位置相对应,添加的数据与id,phone_name,price排列位置不对应
# INSERT INTO phone (id,phone_name,price) VALUES('iphone',10,10000.0);

# 细节4:字符和日期型数据应包含在单引号中,iphone应使用单引号
# INSERT INTO phone (id,phone_name,price) VALUES(10,iphone,10000.0);

# 细节5:若字段允许为空,列可以插入空值,若数据类型后插入NOT NULL则不允许为空
INSERT INTO phone (id,phone_name,price) VALUES(10,'iphone',NULL);

# 细节6:insert into 表名 (column...) values(),(),()形式添加多条记录
INSERT INTO phone (id,phone_name,price) VALUES(10,'iphone',10000.0),(11,'小米',2000.0);

# 细节7:若为表中所有字段添加数据,可以不写前面的字段名称
INSERT INTO phone VALUES(12,'华为',3000.0),(13,'洛基亚',4000.0);

# 细节8:当不为某个字段赋值时,若有默认值则添加,否则报错
# 若某个列没有指定NOT NULL,当添加数据时没有指定值,则会默认给null
INSERT INTO phone (id,phone_name) VALUES(12,'华为');
Update（更新数据）
1、基本介绍

UPDATE 表名 SET 列名1 = 值1 , 列名2 = 值2 [WHERE Clause]
2、案例演示

# 将employee表所有员工薪水修改为5000
UPDATE employee SET salary = 5000

# 修改员工jxs的薪水
UPDATE employee SET salary = 10000 WHERE user_name = 'jxs';

INSERT INTO employee VALUES(2,'dwy','2001-7-13','2022-12-17 8:30:30','公务员',10000,'服务',NULL);

# 员工dwy的薪水增加1000
UPDATE employee SET salary = salary + 1000 WHERE user_name = 'dwy';
3、update细节说明

(1)UPDATE语法可以用新值更新原有表行中各列
(2)SET子句指示将要修改的列和给予的值
(3)WHERE子句指定应更新哪些行,若没有WHERE子句则更新所有行
(4)若需修改多个字段,可以通过set 字段1 = 值1 , 字段2 = 值2...
# 修改多个列
UPDATE employee SET job = '软件开发工程师' , salary = salary + 10000.0 WHERE user_name = 'jxs';
Delete（删除数据）
1、基本介绍

DELETE FROM 表名 WHERE Clause
2、案例演示

# 删除employee表中user_name = 'dwy'的记录
DELETE FROM employee WHERE user_name = 'dwy';

# 删除employee表中所有记录
DELETE FROM employee;
3、delete细节说明

(1)若不使用WHERE子句则删除表中所有记录
(2)DELETE语句只可删除一行数据,不可删除某一列的值
(3)使用DELETE语句仅能删除记录,不可删除表本身。若要删除表,使用DROP TABLE 表名
Select单表查询（查询数据）
1、基本介绍

SELECT * | {column1,column2,column3...} FROM 表名 
(1)SELECT:指定查询哪些列的数据
(2)column:指定列名
(3)*:查询所有列
(4)FROM:查询哪张表
(5)DISTINCT:显示结果时,是否去除重复数据
2、select基础

CREATE TABLE student(
id INT NOT NULL DEFAULT 1,
name VARCHAR(20) NOT NULL DEFAULT '',
chinese FLOAT NOT NULL DEFAULT 0.0,
english FLOAT NOT NULL DEFAULT 0.0,
math FLOAT NOT NULL DEFAULT 0.0);

INSERT INTO student(id,name,chinese,english,math) VALUES(1,'jxs',100,100,100);
INSERT INTO student(id,name,chinese,english,math) VALUES(2,'dwy',90,80,90);
INSERT INTO student(id,name,chinese,english,math) VALUES(3,'tyh',80,70,50);
INSERT INTO student(id,name,chinese,english,math) VALUES(4,'zls',70,60,100);

# 查询表中所有学生信息
SELECT * FROM student;

# 查询表中学生姓名以及对应英语成绩
SELECT name,english FROM student;

# 过滤表中重复数据
SELECT DISTINCT math FROM student;

# 统计每个学生的总分
SELECT name,(chinese+english+math) FROM student;

# 使用别名表示学生分数
SELECT name,(chinese+english+math) AS total_score FROM student;

# 使用别名表示学生姓名、分数
SELECT name AS student_name,(chinese+english+math) AS total_score FROM student;
3、where子句中使用的运算符

运算符	说明
>、<、<=、>=、=、!=	大于、小于、小于等于、大于等于、等于、不等于
BETWEEN...AND...	显示某一区间的值
IN(set)	显示在in列表中的值
LIKE ''	模糊查询
NOT LIKE ''	模糊查询
IS NULL	判断是否为空
AND	多条件同时成立
OR	多条件任一成立
NOT	不成立
# 查询math大于90并且id大于1的学生成绩
SELECT * FROM student WHERE id > 1 AND math > 90;

# 查询语文成绩大于英语成绩的同学
SELECT * FROM student WHERE chinese > english;

# 查询总分大于200分并且数学成绩等于语文成绩的姓j的学生
# j%表示以j开头的就可以
SELECT * FROM student WHERE (chinese+english+math) > 200 AND math = chinese AND name LIKE 'j%';

# 查询英语分数在80-90之间的同学。
SELECT * FROM student WHERE english BETWEEN 80 AND 90;

# 查询数学分数为89,90,91的同学。(BETWEEN...AND...为闭区间)
SELECT * FROM student WHERE math BETWEEN 89 AND 91;
SELECT * FROM student WHERE math IN(89,90,91);

# 查询所有姓d的学生成绩
SELECT * FROM student WHERE name LIKE 'd%';

# 查询数学分>80且语文分>80的同学
SELECT * FROM student WHERE math > 80 AND chinese > 80;
4、select进阶

(1)order by:指定排序的列,排序的列既可以是表中的列名,也可以是select语句后指定的列名
(2)asc升序,desc降序
(3)order by子句应位于select语句结尾
# 将数学成绩排序后输出
SELECT * FROM student ORDER BY math;

# 将总分降序输出
SELECT `name`,(chinese+english+math) AS total_score FROM student ORDER BY total_score DESC;

# 将姓j的学生的总分按降序输出
SELECT `name`,(chinese+english+math) AS total_score FROM student WHERE name LIKE 'j%' ORDER BY total_score DESC;
Select查询增强（看总结）
1、查询增强

# 查询入职日期>1991-12-01
SELECT * FROM emp WHERE hiredate > '1991-12-01';

# 模糊查询
# %:表示0到多个任意字符
# _:表示单个字符

# 首字母为S的员工姓名
SELECT ename FROM emp WHERE ename LIKE 'S%'

# 第三字符为O的员工姓名
SELECT ename FROM emp WHERE ename LIKE '__O%'

# 显示上级没有雇员的情况
SELECT * FROM emp WHERE mgr is NULL

# 查询表结构
DESC emp;

# 按照工资从低到高排序
SELECT ename,sal FROM emp ORDER BY sal;

# 先按部门号升序排序,再按薪资降序排序
SELECT * FROM emp ORDER BY deptno ASC,sal DESC;
2、分页查询

start从0开始计算,从start+1行开始取,取出rows行
select * from 表名 limit start,rows
# 分页查询
# 第一页
SELECT * FROM emp ORDER BY empno LIMIT 0,3;
# 第二页
SELECT * FROM emp ORDER BY empno LIMIT 3,3;
# 第三页
SELECT * FROM emp ORDER BY empno LIMIT 6,3;
# 公式
SELECT * FROM emp ORDER BY empno 
LIMIT 每页显示记录数 * (第几页 - 1),每页显示的记录数;
3、分组增强

# 每种岗位的雇员总数、平均工资
SELECT deptno,COUNT(*),AVG(sal) FROM emp GROUP BY deptno;

# 显示雇员的总数以及获得补助的雇员数
# COUNT(comm):若该列为null则不会统计
SELECT COUNT(*),COUNT(comm) FROM emp;

# 统计没有获得补助的雇员数
SELECT COUNT(IF(comm IS NULL,1,NULL)) FROM emp;
SELECT COUNT(*) - COUNT(comm) FROM emp;

# 显示管理者的总人数,DISTINCT去重
SELECT COUNT(DISTINCT mgr) FROM emp;

# 显示雇员工资最大差额
SELECT MAX(sal) - MIN(sal) FROM emp;
4、数据分组总结

(1)若select语句中包含group by、having、limit、order by,执行顺序为where、group by、having、order by、limit

select coulmn1、column2、column3... from 表名 
group by column having condition 
order by column 
limit start,rows
# 统计各部门平均工资,平均工资大于1000,将平均工资从高到低排序
SELECT deptno,AVG(sal) AS avg_sal FROM emp GROUP BY deptno HAVING avg_sal > 1000 ORDER BY avg_sal DESC LIMIT 0,2;
Select多表查询
1、基本介绍

(1)多表查询指基于两个和两个以上的表查询。
(2)在实际应用中,查询单个表不能不能满足需求
(3)多表查询的条件不可少于 表的个数-1 ,否则会出现笛卡尔积
2、案例演示

# 显示部门号为10的部门名、员工名、工资
SELECT ename,sal,dname,emp.deptno FROM emp,dept WHERE emp.deptno = dept.deptno AND dept.deptno = 10;

# 显示各员工的姓名、工资、工资级别
# 员工姓名、工资来自表emp,工资级别来自表salgrade
SELECT ename,sal,grade FROM emp,salgrade WHERE sal BETWEEN losal AND hisal; 

# 显示雇员名,雇员工资以及所在部门名,并按部门降序排序
SELECT ename,sal,dname,dept.deptno FROM emp,dept WHERE emp.deptno = dept.deptno ORDER BY dept.deptno;
3、自连接

# 显示公司员工以及上级的名字
# 员工和上级通过emp表的mgr列关联
# 1.将一张表当作两张表使用
# 2.为表取别名 表名 表别名
SELECT worker.ename AS '职员名',boss.ename AS '上级' FROM emp AS worker,emp AS boss WHERE worker.mgr = boss.empno;
4、子查询基本介绍

(1)子查询指嵌入在其他SQL语句中的SELECT,也叫嵌套查询
(2)单行子查询:返回一行数据的子查询语句
(3)多行子查询:返回多行数据的子查询,使用in关键字
5、子查询案例演示

# 显示与SMITH同一部门的所有员工
# 查询SMITH的部门号
# 单行查询
SELECT ename FROM emp WHERE deptno = (SELECT deptno FROM emp WHERE ename = 'SMITH');

# 查询和部门10的工作相同的雇员的名字、岗位、工资、部门号,但不包含10号部门自己的雇员
# 多行查询
SELECT ename,job,sal deptno FROM emp WHERE job IN (SELECT DISTINCT job FROM emp WHERE deptno = 10) AND deptno != 10;
6、子查询临时表

# 先得到各个类别中价格最高的商品,将此子查询当作临时表
SELECT goods_id,ecs_goods.cat_id,goods_name,shop_price FROM(
SELECT cat_id,MAX(shop_price) AS max_price 
FROM ecs_goods GROUP BY cat_id) temp,ecs_goods WHERE temp.max_price = ecs_goods.shop_price AND temp.cat_id = ecs_goods.cat_id;
7、all和any

# 显示工资比部门30的所有员工的工资高的员工的姓名、工资和部门号
# 显示部门30中所有员工中工资最高的
SELECT ename,sal,deptno FROM emp WHERE sal > (
SELECT MAX(ALL(sal)) FROM emp WHERE deptno = 30);

SELECT ename,sal,deptno FROM emp WHERE sal > ANY(
SELECT sal FROM emp WHERE deptno = 30) AND deptno != 30;
8、多列子查询

# 查询与SMITH的部门和岗位完全相同的所有雇员
# 得到SMITH的部门和岗位
SELECT emp.deptno,emp.job FROM (SELECT deptno,job FROM emp WHERE ename = 'SMITH') temp , emp WHERE (temp.deptno , temp.job) = (emp.deptno,emp.job) AND ename != 'SMITH';

SELECT deptno,job FROM emp WHERE (deptno,job) = (SELECT deptno,job FROM emp WHERE ename = 'SMITH') AND ename != 'SMITH';
9、子查询练习

# 查找每个部门工资高于本部门平均工资的人的资料
# 部门名dname、编号deptno、地址loc在表dept中
SELECT dname,dept.deptno,loc,temp.count FROM dept , (
SELECT COUNT(*) AS count,deptno FROM emp GROUP BY deptno) temp WHERE dept.deptno = temp.deptno;
10、表的复制

为了对某个sql语句进行效率测试,我们需要海量数据时,可以使用此法为表创建海量数据
CREATE TABLE my_table01(
id INT,
name VARCHAR(32),
sal DOUBLE,
job VARCHAR(32),
deptno INT);

# 将emp表的数据迁移到my_table01表
INSERT INTO my_table01 (id,name,sal,job,deptno) SELECT empno,ename,sal,job,deptno FROM emp;

# 自我复制
INSERT INTO my_table01 SELECT * FROM my_table01;
11、删除表的重复记录

# 删除一张表的重复记录
# 将emp表结构复制到my_table02
CREATE TABLE my_table02 LIKE emp;

# 将emp表数据复制到my_table02
INSERT INTO my_table02 SELECT * FROM emp;

# 考虑去重
/*
1.先创建临时表my_tmp,该表结构和my_table02一样
2.将my_tmp的记录通过distinct关键字处理后将记录复制到my_tmp
3.清除my_table02记录
4.将my_tmp表的记录复制到my_table02
5.drop掉临时表my_tmp
*/
CREATE TABLE my_tmp LIKE my_table02;
INSERT INTO my_tmp SELECT DISTINCT * FROM my_table02;
DELETE FROM my_table02;
INSERT INTO my_table02 SELECT * FROM my_tmp
DROP TABLE my_tmp;
12、合并查询

# 在实际应用中,为合并多个select语句的结果,可以使用集合操作符号

# union all将查询结果合并,不去重
SELECT ename,sal,job FROM emp WHERE sal > 2500 UNION ALL SELECT ename,sal,job FROM emp WHERE job = 'MANAGER';

# union 将查询结果合并,去重
SELECT ename,sal,job FROM emp WHERE sal > 2500 UNION SELECT ename,sal,job FROM emp WHERE job = 'MANAGER';
函数
合计/统计函数
1、count函数基本介绍

(1)select count(*) | count(列名) from 表名 [where...]
(2)select sum(列名)[,sum(列名)...] from 表名 [where...]
返回行的总数
2、count函数案例演示

# count(*)返回满足条件的记录的行数
# count(列)返回满足条件的列的数量,排除null

# 统计一个班共有多少学生
SELECT COUNT(*) FROM student;

# 统计一个班数学成绩大于90的学生数量
SELECT COUNT(*) FROM student WHERE math > 90;

# 统计总分大于250的学生数量
SELECT COUNT(*) FROM student WHERE (math+chinese+english) > 250;


CREATE TABLE table09(
name VARCHAR(20));

INSERT INTO table09 VALUES('jxs');
INSERT INTO table09 VALUES('dwy');
INSERT INTO table09 VALUES(null);

SELECT COUNT(`name`) FROM table09;
3、sum函数案例演示

# 统计一个班级数学总成绩
SELECT SUM(math) FROM student;

# 统计一个班级语文、英语、数学各科的总成绩
SELECT SUM(math) AS total_math,SUM(chinese) AS total_chinese,SUM(english) AS total_english FROM student;

# 统计一个班级语文、英语、数学的成绩总和
SELECT SUM(math + chinese + english) FROM student;

# 统计一个班级语文成绩平均分
SELECT SUM(chinese)/COUNT(`name`) FROM student;
注:
(1)sum仅对数值起作用
(2)对于多列求和,","不可少
4、avg函数案例演示

# 求一个班级数学平均分
SELECT AVG(math) FROM student;

# 求一个班级总分平均分
SELECT AVG(math + chinese + english) FROM student;
5、max/min函数案例演示

# 求班级总分最高分、最低分
SELECT MAX(math + chinese + english),MIN(math + chinese + english)FROM student;
6、group by函数基本介绍

(1)select column1,column2,column3... from 表名 group by column
(2)select column1,column2,column3... from 表名 group by column having...(having过滤数据)
7、group by函数案例演示

# 部门表
CREATE TABLE dept(
deptno MEDIUMINT NOT NULL DEFAULT 0,
dname VARCHAR(20) NOT NULL DEFAULT "",
loc VARCHAR(13) NOT NULL DEFAULT ""
);
INSERT INTO dept VALUES(10,'ACCOUNTING','NEW YORK'),(20,'RESEARCH','DALLAS'),(30,'SALES','CHICAGO'),(40,'OPERATIONS','BOSHTON');


# 员工表
create table emp(
empno mediumint  unsigned not null default 0,/*编号*/
ename varchar(20) not null default '',/*姓名*/
job varchar(9) not null default '',/*工作*/
mgr mediumint unsigned,/*上级编号*/
hiredate date not null, /*入职时间*/
sal decimal(7,2) not null,/*薪水*/
comm decimal(7,2),/*红利*/
deptno mediumint unsigned not null default 0/*部门编号*/
);
INSERT INTO emp VALUES(7369,'SMITH','CLERK',7902,'1990-12-17',800.00,NULL,20),(7499,'ALLEN','SALESMAN',7698,'1991-2-20',1600.00,300.00,30),(7521,'WARD','SALESMAN',7968,'1991-2-22',1250.00,500.00,30),(7566,'JONES','MANAGER',7839,'1991-4-2',2975.00,NULL,20),(7654,'MARTIN','SALESMAN',7968,'1991-9-28',1250.00,1400.00,30),(7698,'BLAKE','MANAGER',7839,'1991-5-1',2850.00,NULL,30),(7782,'CLARK','MANAGER',7839,'1991-6-9',2450.00,NULL,10),(7788,'SCOTT','ANALYST',7566,'1991-4-19',3000.00,NULL,20),(7839,'KING','PRESIDENT',NULL,'1991-11-17',5000.00,NULL,10),(7844,'TURNER','SALESMAN',7698,'1991-9-8',1500.00,NULL,30),(7900,'JAMES','CLERK',7698,'1991-12-3',950.00,NULL,30),(7902,'FORD','ANALYST',7566,'1991-12-3',3000.00,NULL,20),(7934,'MILLER','CLERK',7782,'1991-1-23',1300.00,NULL,10);


# 工资级别表
CREATE TABLE salgrade(
grade MEDIUMINT UNSIGNED NOT NULL DEFAULT 0,/*工资级别*/
losal DECIMAL(17,2) NOT NULL,/*级别最低工资*/
hisal DECIMAL(17,2) NOT NULL);/*级别最高工资*/
INSERT INTO salgrade VALUES(1,700,1200),(2,1201,1400),(3,1401,2000),(4,2001,3000),(5,3001,9999);
# 每个部门的平均工资、最高工资
SELECT AVG(sal),MAX(sal),deptno FROM emp GROUP BY deptno;

# 每个部门每种岗位的平均工资、最高工资
SELECT AVG(sal),MAX(sal),deptno,job FROM emp GROUP BY deptno,job;

# 平均工资低于2000的部门号和它的平均工资,having过滤数据
SELECT AVG(sal),deptno FROM emp GROUP BY deptno HAVING AVG(sal) < 2000;
SELECT AVG(sal) AS avg_name,deptno FROM emp GROUP BY deptno HAVING avg_name < 2000;
字符串函数
1、字符串函数基本介绍

![](E:\Study\自学课程资料\Java\assets\MySQL字符串函数.png)

2、字符串函数案例演示

# 返回字串字符集
SELECT CHARSET(ename) FROM emp;

# 连接字串,将多个列拼接为一列
SELECT CONCAT(ename,'job is',job) FROM emp;

# 返回j在jxs中出现的位置,没有则返回0
# DUAL 系统表,可作为测试表使用
SELECT INSTR('jxs','j') FROM DUAL;

# 转大写
SELECT UCASE(ename) FROM emp;

# 转小写
SELECT LCASE(ename) FROM emp;

# 从字符串ename左边起取2个字符
SELECT LEFT(ename,2) FROM emp; 

# 从字符串ename右边起取2个字符
SELECT RIGHT(ename,2) FROM emp; 

# 字符串长度,按字节
SELECT LENGTH(ename) FROM emp;

# job中将manager替换为经理
SELECT REPLACE(job,'MANAGER','经理') FROM emp;

# 逐字符比较两字串大小
SELECT STRCMP('jxs','dwy') FROM DUAL;

# 从ename的第一个位置取出2个字符
SELECT SUBSTRING(ename,1,2) FROM emp;

# LTRIM去除前端空格 RTRIM去除后端空格 TRIM去除两端空格
SELECT LTRIM(' jxs ') FROM DUAL;
SELECT RTRIM(' jxs ') FROM DUAL;
SELECT TRIM(' jxs ') FROM DUAL;

# 以首字母小写的方式显示所有员工emp表的姓名
# 取出ename第一个字符并转换为小写
# 取出ename除第一个字符外的其他字符
# 拼接
SELECT CONCAT(LCASE(SUBSTRING(ename,1,1)),SUBSTRING(ename,2)) FROM emp;

SELECT REPLACE(ename,SUBSTRING(ename,1,1),LCASE(SUBSTRING(ename,1,1))) FROM emp;
数学函数
1、数学函数基本介绍

函数	说明
ABS(x)	返回x的绝对值
AVG(expression)	返回字段平均值
CEIL(x)/CEILING(x)	向上取整
FLOOR(x)	向下取整
MOD(nExp1,nExp2)	取余
RAND()	返回 0 到 1 的随机数
2、数学函数案例演示

# 绝对值
SELECT ABS(-10) FROM DUAL;

# 十进制转二进制
SELECT BIN(10) FROM DUAL;

# 进制转换,将十进制12转为2进制输出
SELECT CONV(12,10,2) FROM DUAL;
# 将十六进制12转为十进制输出
SELECT CONV(12,16,10) FROM DUAL;

# 转十六进制
SELECT HEX(256) FROM DUAL;

# 向上取整
SELECT CEILING(4.5) FROM DUAL;

# 向下取整
SELECT FLOOR(4.5) FROM DUAL;

# 保留2001.210两位小数
SELECT FORMAT(2001.210,2) FROM DUAL;

# 最小值
SELECT LEAST(1,2,3,4,5) FROM DUAL;

# 取余
SELECT MOD(10,3) FROM DUAL;

# 返回随机数,0<=范围<=1
# 若使用rand()每次返回不同的随机数
# 若使用rand(seed),若seed不改变,则随机数不改变
SELECT RAND(3) FROM DUAL;
日期函数
1、日期函数基本介绍

函数	描述
NOW()	返回当前日期和时间
CURRENT_DATE	返回当前日期
CURRENT_TIME	返回当前时间
CURRENT_TIMESTAMP	返回当前时间戳
DATE()	提取日期或时间表达式的日期部分
DATE_ADD()	给日期添加指定的时间间隔
DATE_SUB()	从日期减去指定的时间间隔
DATEDIFF()	返回两个日期之间的天数
TIMEDIFF()	返回两个小时之间的小时数
YEAR|MONTH|DAY	提取日期或时间表达式年月日部分
UNIX_TIMESTAMP	返回1970-1-1至今的秒数
FROM_UNIXTIME	将UNIX_TIMESTAMP秒数转换为指定格式的日期
2、日期函数案例演示

# 当前日期
SELECT CURRENT_DATE FROM DUAL;

# 当前时间
SELECT CURRENT_TIME FROM DUAL;

# 当前时间戳
SELECT CURRENT_TIMESTAMP FROM DUAL;

# 创建测试表
CREATE TABLE mes(
id INT,
content VARCHAR(30),
sendtime DATETIME);
INSERT INTO mes VALUES(1,'央视新闻',CURRENT_TIMESTAMP);
INSERT INTO mes VALUES(2,'北京新闻',NOW());
# NOW()当前时间
INSERT INTO mes VALUES(3,'浙江卫视',NOW());

# 显示所有新闻信息且只显示日期,不显示时间
SELECT id,content,DATE(sendtime) FROM mes;

# 只显示年、月、日
SELECT YEAR(NOW()) FROM DUAL;
SELECT MONTH(NOW()) FROM DUAL;
SELECT DAY(NOW()) FROM DUAL;
SELECT MONTH('2011-11-11 10:10:10') FROM DUAL;

# 查询在10分钟内发布的新闻,发布时间+10分钟,若大于现在时间则不为10分钟内发布的新闻
SELECT * FROM mes WHERE DATE_ADD(sendtime,INTERVAL 10 MINUTE) >= NOW();

# 2011-11-11和1990-1-1相差多少天
SELECT DATEDIFF('2011-11-11','1990-1-1') FROM DUAL;

# 10:10:10和6:20:20相差多少时分秒
SELECT TIMEDIFF('10:10:10','6:20:20') FROM DUAL;

# 自己出生天数
SELECT DATEDIFF(NOW(),'2001-2-10') FROM DUAL;

# 若活到80岁,还剩多少天
SELECT DATEDIFF(DATE_ADD('2001-2-10',INTERVAL 80 YEAR),NOW())FROM DUAL;

# 返回1970-1-1到现在的毫秒数
SELECT UNIX_TIMESTAMP() FROM DUAL;

# 将UNIX_TIMESTAMP秒数转换为指定格式的日期
# 开发中,存放一个整数来表示时间,通过FROM_UNIXTIME转换
SELECT FROM_UNIXTIME(1618483484,'%Y-%m-%d') FROM DUAL;
SELECT FROM_UNIXTIME(1618483484,'%Y-%m-%d %H:%i:%s') FROM DUAL;
3、日期函数细节说明

(1)DATE_ADD()中的interval后面可以为year、minute、second、day
(2)DATE_SUB()中的interval后面可以为year、minute、second、day
(3)DATEDIFF(date1,date2)得到的是date1-date2的天数
(4)DATE_ADD、DATE_SUB、DATEDIFF、DATE四个函数日期类型可以为date、datetime、timestamp
加密函数
1、基本介绍

(1)USER():查询用户,查看登录到MySQL的用户以及登录的IP
(2)DATABASE():查看当前使用数据库名称
(3)MD5(str):为字符串计算出一个MD5 32的字符串,常用于(用户密码)加密,在数据库中存放加密后的密码
(4)PASSWORD(str):从原文密码str计算并返回密码字符串,通常用于对mysql用户密码加密(MySQL 5.7.9版本后废除了PASSWORD()函数)
# 查询用户,查看登录到MySQL的用户以及登录的IP
SELECT USER() FROM DUAL;

# 查看当前使用数据库名称
SELECT DATABASE() FROM DUAL;

# 为字符串计算出一个MD5 32的字符串,常用于(用户密码)加密,在数据库中存放加密后的密码
SELECT MD5('123456') FROM DUAL;
SELECT LENGTH(MD5('123456')) FROM DUAL;

# 演示教师表存放密码时使用MD5
CREATE TABLE teacher(
id INT,
name VARCHAR(32) NOT NULL DEFAULT '',
password VARCHAR(32) NOT NULL DEFAULT '');

INSERT INTO teacher VALUES(1,'jxs',MD5('123456'));
# 查询
SELECT * FROM teacher WHERE name = 'jxs' AND password = MD5('123456');
流程控制函数
1、基本介绍

函数	说明
IF(expr1,expr2,expr3)	若expr1为true则返回expr2,否则返回expr3
IFNULL(expr1,expr2)	若expr1不为空则返回expr1,否则返回expr2
SELECT CASE case_value WHEN when_value THEN statement_list1 ELSE statement_list2 END;	若when_value为true,则返回statement_list1,否则返回statement_list2
2、案例演示

# 若expr1为true则返回expr2,否则返回expr3
SELECT IF(TRUE,'jxs','dwy') FROM DUAL;

# 若expr1不为空则返回expr1,否则返回expr2
SELECT IFNULL(NULL,'jxs') FROM DUAL;
SELECT IFNULL('dwy','jxs') FROM DUAL;

# 若comm是null,则显示0.0
# 判断是否为空使用is null,不为空使用is not null
SELECT IFNULL(comm,0.0) FROM emp;
SELECT IF(comm IS NULL,0.0,comm) FROM emp;

# 若emp表的job是CLERK则显示职员,是MANAGER则显示经理
SELECT IF(job = 'CLERK','职员','CLERK'),IF(job = 'MANAGER','经理','MANAGER')FROM emp;

SELECT ename,(SELECT CASE 
	WHEN job = 'CLERK' THEN
		'职员'
	WHEN job = 'MANAGER' THEN
		'经理'
	ELSE 
		job END) AS job FROM emp;
外连接
1、基本介绍

(1)左外连接:左侧的表完全显示即左外连接
(2)右外连接:右侧的表完全显示即右外连接
2、案例演示

CREATE TABLE stu(
id INT,
name VARCHAR(32));
INSERT INTO stu VALUES(1,'jxs'),(2,'dwy'),(3,'tyh'),(4,'zls');

CREATE TABLE exam(
id INT,
grade INT);
INSERT INTO exam VALUES(1,100),(2,90),(11,80)


# 显示所有人的成绩,若没有成绩则显示该人的姓名、id号
SELECT stu.id,name,grade FROM stu,exam WHERE stu.id = exam.id; 

# 使用左外连接,左表和右表没有匹配的记录,也会将左表的记录显示出来
SELECT stu.id,name,grade FROM stu LEFT JOIN exam ON stu.id = exam.id; 

# 使用右外连接,左表和右表没有匹配的记录,也会将右表的记录显示出来
SELECT stu.id,name,grade FROM stu RIGHT JOIN exam ON stu.id = exam.id

# 显示部门名称以及部门的员工信息,同时列出没有员工的部门
SELECT dname,ename FROM emp LEFT JOIN dept ON emp.deptno = dept.deptno;

SELECT dname,ename FROM emp RIGHT JOIN dept ON emp.deptno = dept.deptno;
3、总结

(1)实际开发中绝大多数使用的是内连接
(2)左外连接、右外连接:左边的表与右边的表没有匹配的记录也会将左边的表/右边的表的记录显示出来
约束
1、约束基本介绍

(1)约束用于确保数据库的数据满足特定的商业规则
(2)MySQL中,约束包括:not null、unique、primary key、foreign key、check、自增长
2、PRIMARY KEY主键案例演示

# id为主键
CREATE TABLE `primarykey`(
id INT PRIMARY KEY,
name VARCHAR(32),
email VARCHAR(32));

INSERT INTO primarykey VALUES (1,'jxs','2899978900@qq.com');
INSERT INTO primarykey VALUES (2,'dwy','15365040704@qq.com');
# 主键不可重复
# INSERT INTO `primarykey` VALUES (1,'tyh','2899978900@qq.com')
3、主键细节说明

(1)主键定义方式:字段名 字段数据类型 PRIMARY KEY
(2)定义主键约束后,主键约束的字段不可重复且不可为NULL
(3)一张表最多一个主键,但可以是复合主键
(4)主键的指定方式有两种:(1)字段名的数据类型后(2)表定义最后
(5)使用DESC 表名,可以查看主键情况
(6)实际开发中每个表往往都会涉及一个主键
# 一张表最多一个主键,但可以是复合主键
CREATE TABLE primarykey1(
id INT,
name VARCHAR(32),
email VARCHAR(32),
PRIMARY KEY (id,name));

INSERT INTO primarykey1 VALUES (1,'jxs','2899978900@qq.com');
INSERT INTO primarykey1 VALUES (1,'dwy','15365040704@qq.com');
# 复合主键:只有当id、name同时重复时,才违反复合主键
INSERT INTO primarykey1 VALUES (1,'jxs','15365040704@qq.com');
4、unique基本介绍

(1)当定义unique(唯一)约束后,该字段值不可重复
(2)若被unique修饰的字段没有指定not null,则unique字段可以有多个null
(3)一张表可以有多个unique字段
(4)若字段为unique not null使用效果类似主键(不可重复且不可为null)
create TABLE `unique`(
id INT UNIQUE,
name VARCHAR(32),
email VARCHAR(32));

INSERT INTO `unique` VALUES (1,'jxs','2899978900@qq.com');
# 添加失败
# INSERT INTO `unique` VALUES (1,'dwy','2899978900@qq.com');
INSERT INTO `unique` VALUES (null,'dwy','2899978900@qq.com');
INSERT INTO `unique` VALUES (null,'dwy','2899978900@qq.com');
5、外键基本介绍

(1)用于定义主表和从表之间的关系:外键约束要定义在表上,主表必须具有主键约束或unique约束,当定义外键约束后,要求外键列数据必须在主表的主键列存在或是为null
(2)foreign key (本表字段名) references 主表名(主键名/unique字段名)
6、外键案例演示

CREATE TABLE class(
id INT PRIMARY KEY,
class_name VARCHAR(32) NOT NULL DEFAULT '',
address VARCHAR(32));

CREATE TABLE student(
id INT PRIMARY KEY,
name VARCHAR(32) NOT NULL DEFAULT '',
class_id INT,
# 指定外键关系
FOREIGN KEY (class_id) REFERENCES class(id));

# 测试数据
INSERT INTO class VALUES (1,'java','南京'),(2,'mysql','南京');
INSERT INTO student VALUES (1,'jxs',1),(2,'dwy',2)
# 添加失败,主表中不存在id=3的记录
INSERT INTO student VALUES (3,'tyh',3)
7、外键细节说明

(1)外键指向主表的字段,要求该字段为主键(不可重复且不可为null)或者是unique(不可重复)
(2)表的类型为innodb,这样才支持外键
(3)外键字段的数据类型和主键字段的数据类型一致
(4)外键字段的值必须在主键字段中出现过,或者为null(前提:外键字段允许为null)
(5)一旦建立主外键的关系,主表记录不可随意删除,从表中没有记录指向主表的记录则可以删除
8、check基本介绍

(1)用于强制数据必须满足条件
(2)oracle、sql server均支持check
9、check案例演示

CREATE TABLE `check`(
id INT PRIMARY KEY,
`name` VARCHAR(32),
sex VARCHAR(4) CHECK (sex IN('man','woman')),
salary DOUBLE CHECK (salary > 1000 AND salary < 2000));

# 插入失败
INSERT INTO `check` VALUES (1,'jxs','男',10000.0);
10、商店表设计案例

现有一个商店的数据库shop_db,记录客户及共购物情况,由下面三个表组成:商品goods(商品号goods_id,商品名goods_name,单价unitprice,商品类别category,供应provider)
客户customer(客户号customer_id,姓名name,住址address,邮箱email,性别sex,身份证card_ld);
购买purchase(购买订单号order_id,客户号customer_id,商品号goods_id,购买数量nums);
建表,在定义中声明[进行合理设计]:
(1)每个表的主外键;
(2)客户的姓名不能为空值;
(3)邮箱不可重复;
(4)客户的性别[男女]
(5)单价unitprice在 1.0 - 9999.99之间
CREATE TABLE goods(
goods_id INT PRIMARY KEY,
goods_name VARCHAR(32),
unitprice DOUBLE CHECK (unitprice > 1.0 AND unitprice < 9999.99),
category VARCHAR(32),
provider VARCHAR(32));

CREATE TABLE customer(
customer_id VARCHAR(32) PRIMARY KEY,
name VARCHAR(32) NOT NULL DEFAULT '',
address VARCHAR(32),
email VARCHAR(32) UNIQUE,
sex CHAR(4) CHECK ( sex IN ('男','女') ),
card_id VARCHAR(32));


CREATE TABLE purchase(
order_id INT PRIMARY KEY,
customer_id VARCHAR(32),
goods_id INT,
nums INT,
FOREIGN KEY (customer_id) REFERENCES customer(customer_id),
FOREIGN KEY (goods_id) REFERENCES goods(goods_id));
11、自增长案例演示

# 自增长
CREATE TABLE table10(
id INT PRIMARY KEY AUTO_INCREMENT,
email VARCHAR(32) NOT NULL DEFAULT '',
name VARCHAR(32) NOT NULL DEFAULT '')

# id为null,但id字段为自增长,会自动分配1
INSERT INTO table10 VALUES (null,'2899978900@qq.com','jxs');
INSERT INTO table10 VALUES (null,'15365040704@qq.com','dwy');
INSERT INTO table10 (email,name) VALUES ('11@qq.com','tyh');
12、自增长细节说明

(1)auto_increment和primary key配合使用 
(2)自增长可单独使用,但需配合unique
(3)自增长修饰的字段为整数型
(4)自增长默认从1开始,也可通过如下命令修改
alter table 表名 auto_increment = xxx;
(5)若添加数据值,为自增长字段指定值,则以指定的值为准
索引
1、索引基本介绍

(1)不需增加内存,不需改程序,不需调SQL,利用索引提高数据库性能
(2)创建索引后,索引本身占用空间
2、索引原理

(1)没有索引时会进行全表扫描
(2)有索引时,形成一个索引的数据结构,如二叉树...
(3)索引代价:磁盘占用;对增删改语句的效率影响,会对索引进行维护,对速度有影响
![](E:\Study\自学课程资料\Java\assets\MySQL索引原理.png)

3、索引类型

(1)主键索引(primary key)
(2)唯一索引(unique)
(3)普通索引(index)
(4)全文索引(fulltext)[适用于MyISAM]
一般开发中,不使用MySQL自带的全文索引,开发中考虑使用全文搜索Solr、ElasticSearch
4、添加索引

(1)如何选择普通索引、唯一索引、主键索引
若某列的值不可重复,优先考虑使用unique索引,否则使用普通索引
CREATE TABLE table10(
id INT,
name VARCHAR(32));


# 查看表索引
SHOW INDEX FROM table10;


# 添加唯一索引,Non_unique为0代表是唯一索引,Non_unique为1代表不为唯一索引
CREATE UNIQUE INDEX id_index ON table10(id);
# 添加普通索引方式一:
CREATE INDEX id_index ON table10(id)
# 添加普通索引方式二:
ALTER TABLE table10 ADD INDEX id_index(id);


# 添加主键索引方式一:
CREATE TABLE table11(
id INT PRIMARY KEY,
name VARCHAR(32));
# 添加主键索引方式二:
ALTER TABLE table11 ADD PRIMARY KEY (id);
5、删除索引

CREATE TABLE table10(
id INT,
name VARCHAR(32));

# 查看索引
SHOW INDEX FROM table10;

# 添加普通索引
CREATE INDEX id_index ON table10(id);

# 删除普通索引
DROP INDEX id_index ON table10;


# 删除主键索引
CREATE TABLE table11(
id INT PRIMARY KEY,
name VARCHAR(32));

# 删除主键索引
ALTER TABLE table11 DROP PRIMARY KEY;

# 查看索引
SHOW INDEX FROM table11;
6、查询索引

CREATE TABLE table10(
id INT,
name VARCHAR(32));

# 查看索引方式一:
SHOW INDEX FROM table10;

# 查看索引方式二:
SHOW INDEXES FROM table10;

# 查看索引方式三:
SHOW KEYS FROM table10;

# 查看索引方式四:
DESC table10;
7、索引练习题

CREATE TABLE sportman1(
id INT PRIMARY KEY,
name VARCHAR(32));

# 创建索引方式一:
CREATE INDEX name_index ON sportman1(name);

# 查看索引
SHOW INDEX FROM sportman1;


CREATE TABLE sportman2(
id INT PRIMARY KEY,
name VARCHAR(32));

# 创建索引方式二:
ALTER TABLE sportman2 ADD INDEX name_index(name); 

SHOW INDEX FROM sportman2;
8、创建索引规则

(1)较频繁的作为查询条件的字段应该创建索引
(2)唯一性太差的字段不适合单独创建索引,即使频繁作为查询条件
(3)更新非常频繁的字段不适合创建索引
(4)不会出现在WHERE子句中的字段不应该创建索引
事务（看第7点总结！！）
1、基本介绍

事务用于保证数据的一致性,它由一组相关的dml语句组成,该组的dml语句要么全部成功,要么全部失败。
如:转账需要事务来处理,用来保证数据的一致性。
![](E:\Study\自学课程资料\Java\assets\MySQL事务理解.png)

2、事务基本操作

(1)start transaction:开始一个事务
(2)savepoint 保存点名:设置保存点
(3)rollback to 保存点名:回退事务
(4)rollback:回退全部事务
(5)commit:提交事务,所有操作生效,不可回退
![](E:\Study\自学课程资料\Java\assets\MySQL事务操作示意图.png)

3、事务操作

(1)保存点是事务中的点,用于取消部分事务,当结束事务时,会自动删除该事务所定义的所有保存点,当执行回退事务时,通过指定保存点可以回退到指定的点。
(2)使用commit语句提交事务,提交事务后会确认事务的变化、结束事务、删除保存点、释放锁、数据生效。当使用commit语句结束事务后,其他会话将可以查看到事务变化后的新数据。
# 创建表格
CREATE TABLE `transaction`(
id INT,
name VARCHAR(32));
# 开启事务
START TRANSACTION;
# 设置保存点
SAVEPOINT a
# 执行dml操作
INSERT INTO `transaction` VALUES (1,'jxs');
# 设置保存点
SAVEPOINT b
# 执行dml操作
INSERT INTO `transaction` VALUES (2,'dwy');
# 回退
ROLLBACK TO b;
# 继续回退
ROLLBACK TO a;
# 回退全部事务
ROLLBACK;
# 提交事务
COMMIT;
4、事务注意事项

(1)若不开启事务,默认情况下dml操作自动提交,不可回滚
(2)若开始事务但没有创建保存点,执行rollback,默认回滚到事务开始的状态
(3)在事务提交前,可以回滚到任意保存点
(4)mysql事务机制需要innode存储引擎
(5)开启事务:start transaction、set autocommit = off
5、事务隔离级别

(1)多个连接开启各自事务操作数据库中的数据时,数据库系统负责隔离操作,保证各个连接在获取数据时的准确性
(2)若不考虑隔离性,可能会引发如下问题:脏读、不可重复读、幻读
(1)脏读:当一个事务读取另一个事务尚未提交的修改时,产生脏读
(2)不可重复读:同一查询在同一事务中多次进行,由于其他提交事务所做的修改或删除操作,每次返回不同的结果集,此时发生不可重复读。
(3)幻读:同一查询在同一事务中多次进行,由于其他提交事务所做的插入操作,每次返回不同的结果集,此时发生幻读。
MySQL隔离级别	脏读	不可重复读	幻读	加锁读
读未提交（read uncommitted）	√	√	√	不加锁
读已提交（read committed）	×	√	√	不加锁
可重复读（repeatable read）	×	×	×	不加锁
可串行化（serializable）	×	×	×	加锁
6、事务隔离级别案例演示

(1)打开两个mysql控制台

(2)使用my_database数据库
mysql> use my_database;
Database changed

(3)将其中一个控制台隔离级别设置为read uncommitted(读未提交)
mysql> set session transaction isolation level read uncommitted;

(4)两个控制台分别启动事务
mysql> start transaction;

(5)创建表
mysql> CREATE TABLE account(
    -> id INT,
    -> name VARCHAR(32),
    -> money INT);
    
(6)在未修改隔离级别的控制台修改、删除、插入数据但未提交事务,另一个事务可读取到尚未提交的修改,产生脏读，不可重复读、幻读。
mysql> insert into account values (1,'jxs',1000);
mysql> update account set money = 800 where id = 1;

(7)两个控制台分别提交事务,将其中一个控制台隔离级别修改为读已提交,再分别开启事务
mysql> set session transaction isolation level read committed;

(8)在未修改隔离级别的控制台修改、删除、插入数据后提交事务,另一个事务可读取到已提交的修改,产生不可重复读、幻读。
mysql> insert into account values (2,'dwy',3000);
mysql> update account set money = 3000 where id = 2;

(9)两个控制台分别提交事务,将其中一个控制台隔离级别修改为可重复读,再分别开启事务
mysql> set session transaction isolation level repeatable read;

(10)在未修改隔离级别的控制台修改、删除、插入数据后提交事务,另一个事务不可读取到已提交的修改
mysql> update account set money = 4000 where id = 2;
mysql> insert into account values (3,'lzz',7000);
7、总结

(1)读未提交(read uncommitted):最低隔离级别,事务A可读取到事务B尚未提交对数据的修改、删除、插入的记录,产生脏读、不可重复读、幻读。
(2)读已提交(read committed):事务A可读取到事务B已提交对数据的修改、删除、插入的记录,产生不可重复读(事务A在事务B提交前和事务B提交后查询的数据不一致)、幻读。
(3)可重复读(repeatable read):事务A不可读取到事务B已提交对数据的修改、删除、插入的记录。
(4)可串行化(serializable):最高隔离级别,事务B未提交对数据的修改、删除、插入的记录,事务A不可对数据进行修改、删除、插入、查找。强制事务排序,使之不可相互冲突,期间会导致大量的超时现象和锁竞争。
(5)修改数据库隔离级别:set session transaction isolation level 事务隔离级别
8、设置隔离

(1)查看当前会话隔离级别:select @@transaction_isolation
(2)查看系统当前隔离级别:select @@global.transaction_isolation;
(3)设置当前会话隔离级别:set session transaction isolation level 隔离级别
(4)设置系统当前隔离级别:set global transaction isolation level 隔离级别
(5)mysq默认事务隔离级别:repeatable read
9、事务ACID

(1)原子性:原子性是事务不可分割的工作单位,事务中的操作要么全部发生、要么全部失败
(2)一致性:事务必须使数据库从一个一致性状态变换到另一个一致性状态
(3)隔离性:多个用户并发访问数据库时,数据库为每一个用户开启的事务不可被其他事务的操作数据所干扰
(4)持久性:一个事务一旦提交,对数据库中数据的改变即永久性的,即使数据库发生故障也不对其有任何影响
存储引擎
1、基本介绍

(1)MySQL表类型由存储引擎(Storage Engines)决定,常用存储引擎包括MyISAM、InnoDB、Memory
(2)MySQL数据表主要支持6种类型,分别是CSV、Memory、ARCHIVE、MRG MYISAM、MYISAM、InnoDB
(3)6种类型又分两类,一类"事务安全型"(transaction-safe),比如:InnoDB;其余为第二类"非事务安全型"
2、存储引擎支持类型

(1)InnoDB(默认):支持事务、行级锁定和外键
(2)MRG MYSIAM:相同的 MyISAM 表的集合
(3)MEMORY:基于哈希，存储在内存中，对临时表很有用
(4)BLACKHOLE:/dev/null 存储引擎（你写入它的任何内容都会消失）
(5)MyISAM:MyISAM存储引擎
(6)ARCHIVE:ARCHIVE存储引擎
存储引擎	MyISAM	InnoDB	Memory	Archive
批量插入速度	高	低	高	很高
事务安全		支持		
全文索引	支持			
锁机制	表锁	行锁	表锁	行锁
存储限制	无	64TB	有	无
B树索引	支持	支持	支持	
哈希索引		支持	支持	
集群索引		支持		
数据缓存		支持	支持	
索引缓存	支持	支持	支持	
数据可压缩	支持			支持
空间使用	低	高	N/A	很低
内存使用	低	高	中	低
支持外键		支持		
3、MyISAM、InnoDB、Memory细节说明

(1)MyISAM:不支持事务、不支持外键,但访问速度快、对事务完整性无要求
(2)InnoDB:处理效率低、占用更多的磁盘空间保留数据和索引,具有提交、回滚、崩溃恢复能力的事务安全
(3)Memory:使用内存中的内容创建表。每个Memory表实际对应一个磁盘文件。因为数据存放在内存中所以Memory类型的表访问很快,并默认为hash索引。一旦MySQL服务关闭,表中数据就会丢失,但表的结构存在
4、如何选择表的存储引擎

(1)若应用不需事务,只处理基本的CRUD操作,使用MyISAM存储引擎
(2)若需支持事务,使用InnoDB存储引擎
(3)Memory存储引擎将数据存储在内存中,由于没有磁盘IO等待,速度极快。但重启MySQL服务后数据消失,结构仍存在(经典用法:用户的在线状态)。
视图
1、视图引出

emp表字段很多,有些信息为个人重要信息,希望某些用户只能查询emp表的某些字段信息,则使用视图
2、视图基本概念

视图是一个虚拟表,其内容由查询定义。同真实的表一样,视图包含列,其数据来自对应的真实表(基表)
![](E:\Study\自学课程资料\Java\assets\视图和基表关系.png)

3、视图概念总结

(1)视图(虚拟的表)根据基表创建
(2)视图也有列,数据来自基表
(3)通过视图可修改基表的数据,通过基表可修改视图的数据
(4)视图:限制对基表的查询
4、视图操作

(1)创建视图:create view 视图名 as select语句
(2)修改视图:alter view 视图名 as select语句
(3)显示视图:show create view 视图名
(4)删除视图:drop view 视图名1,视图名2
# 创建视图emp_view1,只可查询emp表的(empon,ename,job,deptno)
CREATE VIEW emp_view1 AS SELECT empno,ename,job,deptno FROM emp;
# 查看视图
DESC emp_view1;
# 查看创建视图指令
SHOW CREATE VIEW emp_view1;
# 删除视图
DROP VIEW emp_view1;
5、视图细节说明

(1)创建视图后,在数据库中对应的视图只有一个视图结构文件
(2)视图的数据变化影响基表,基表的数据变化影响视图
(3)视图中可再使用视图
6、视图应用案例

(1)安全。一些数据表有重要信息,有些字段保密,不可让用户直接看到。即可创建一个视图,在这张视图中只保留一部分字段。这样,用户可以查询到自己需要的字段,不可查看保密的字段
(2)性能。关系数据库的数据常常会分表存储,使用外键建立这些表的之间关系。这时,数据库查询通常会用到连接(JOIN)。这样做不但麻烦,效率相对也比较低。如果建立一个视图,将相关的表和字段组合在一起,就可以避免使用JOIN查询数据。
(3)灵活。如果系统中有一张旧的表,这张表由于设计的问题,即将被废弃。然而,很多应用都是基于这张表,不易修改。这时就可以建立一张视图,视图中的数据直接映射到新建的表。这样,就可以少做很多改动,也达到了升级数据表的目的。
7、视图练习

# 针对emp、dept、salgrade三张表,创建一个视图emp_view2,可显示雇员编号、雇员名、雇员部门名和薪水级别
CREATE VIEW emp_view2 AS SELECT empno,ename,dname,grade FROM emp,dept,salgrade WHERE emp.deptno = dept.deptno AND sal BETWEEN losal AND hisal;
MySQL管理
1、MySQL用户

(1)MySQL用户都存储在系统数据库mysql中user表中
(2)host:允许登录的"位置",localhost表示该用户只允许本机登录,也可指定ip地址
(3)user:用户名
(4)authentication_string:密码,通过mysql的password()函数加密后的密码
2、创建、删除用户

create user '用户名'@'登录地址' identified by '123456';

drop user '用户名'@'登录地址';
3、修改密码

alter user 'jxs'@'localhost' identified by '密码';
4、为用户授权

grant 权限列表 on 库.对象名 to '用户名'@'登录地址' [identified by '密码']
(1)权限列表,多个权限用逗号隔开
grant select,delete,create on ...
(2)特别说明
*.*:代表本系统所有数据库的所有对象(表、视图、存储过程)
库.*:表示某个数据库中所有数据对象(表、视图、存储过程)
(3)identified by可省略
若用户存在即修改用户密码;若用户不存在即创建用户
5、回收用户权限

revoke 权限列表 on 库.对象名 from '用户名'@'登录位置';
6、权限生效指令

flush privileges;
7、MySQL管理练习

# 创建数据库用户
CREATE USER 'jxs'@'localhost' IDENTIFIED BY '123456';

# root用户下创建news表
CREATE DATABASE testdb;
CREATE TABLE news(
id INT,
name VARCHAR(32));
# 插入数据
INSERT INTO news VALUES (1,'jxs');

# 为创建的jxs用户分配权限
GRANT SELECT,INSERT ON my_database.news TO 'jxs'@'localhost';

# 修改jxs用户密码
ALTER USER 'jxs'@'localhost' IDENTIFIED BY 'abcdef';

# 删除用户
DROP USER 'jxs'@'localhost';
8、MySQL细节说明

(1)创建用户时,若不指定host,则为%,%表示所有ip都有连接权限
(2)创建用户也可create user 'xxx'@'192.168.184.%'表示xxx用户在192.168.184.%的ip可以登录mysql
(3)删除用户时,若host不为%,则需明确指定'用户'@'host值'
9、练习题

(1)语句错误？C,别名间有空格,使用双引号
A.SELECT empno,ename name,sal salary FROM emp;
B.SELECT empno,ename name,sal AS salary FROM emp;
C.SELECT ename,sal*12 AS "Annual Salary" FROM emp;
D.SELECT ename,sal*12 Annual Salary FROM emp;

(2)
# 显示所有部门名称
SELECT dname FROM dept;
# 显示所有雇员名及其全年收入13月(工资+补助),并指定列别名"年收入"
SELECT ename,(sal + IFNULL(comm,0))*13 year_sal FROM emp; 
# 显示工资超过2850的雇员姓名和工资。
SELECT ename,sal FROM emp WHERE sal > 2850;
# 显示工资不在1500到2850之间的所有雇员名及工资。
SELECT ename,sal FROM emp WHERE sal < 1500 OR sal > 2850;
# 显示编号为7566的雇员姓名及所在部门编号。
SELECT ename,deptno FROM emp WHERE empno = 7566;
# 显示部门10和30中工资超过1500的雇员名及工资。
SELECT ename,sal FROM emp WHERE deptno IN (10,30);
# 显示无管理者的雇员名及岗位。
SELECT ename,job FROM emp WHERE mgr IS NULL;
# 显示在1991年2月1日到1991年5月1日之间雇用的雇员名,岗位及雇佣日期，并以雇佣日期进行排序。
SELECT ename,job,hiredate FROM emp WHERE hiredate BETWEEN '1991-2-1' AND '1991-5-1' ORDER BY hiredate;
# 显示获得补助的所有雇员名,工资及补助,并以工资降序排序
SELECT ename,sal,comm FROM emp WHERE comm IS NOT NULL ORDER BY sal DESC;

(3)
# 找出部门10中所有经理(MANAGER)和部门20中所有办事员(CLERK)的详细资料
SELECT * FROM emp WHERE (job = 'MANAGER' AND deptno = 10) OR (job = 'CLERK' AND deptno = 20);
# 找出各月倒数第3天受雇的所有员工
# LAST_DAY(date)返回该日期所在月份的最后一天
SELECT * FROM emp WHERE DATEDIFF(LAST_DAY(hiredate),hiredate) = 2;
# 找出早于12年前受雇的员工,即入职时间超过12年
SELECT * FROM emp WHERE DATEDIFF(NOW(),hiredate) > 12;
# 以首字母小写的方式显示所有员工的姓名
SELECT CONCAT(LCASE(SUBSTRING(ename FROM 1 FOR 1)),SUBSTRING(ename FROM 2)) FROM emp;
# 显示正好为5个字符的员工的姓名
SELECT * FROM emp WHERE LENGTH(ename) = 5;
1.3.4、JDBC和连接池
JDBC概述
1、基本介绍

(1)JDBC为访问不同的数据库提供了统一的接口,为使用者屏蔽了细节问题
(2)Java程序员使用JDBC,可以连接任何提供了JDBC驱动程序的数据库系统,从而完成对数据库的各种操作
2、JDBC基本原理

![](E:\Study\自学课程资料\Java\assets\JDBC理解图.png)

3、JDBC基本原理代码理解

/**
 * 规定JDBC接口
 */
public interface JdbcInterface {
    //连接
    public Object getConnection();

    //关闭连接
    public Object closeConnection();

    //增删改查
    public void crud();
}

class MySQLJdbc implements JdbcInterface {

    @Override
    public Object getConnection() {
        return "连接数据库";
    }

    @Override
    public Object closeConnection() {
        return "关闭数据库";
    }

    @Override
    public void crud() {
        System.out.println("数据库增删改查");
    }
}
4、总结

(1)JDBC API是Java提供用于数据库操作的接口API,统一和规范应用程序与数据库的连接,执行SQL语句并返回结果等操作,相关类和接口在java.sql和javax.sql
(2)Java程序员只需面向这套接口编程即可
(3)不同的数据库厂商需要针对JDBC接口提供不同实现
Java通过驱动包（jar包）连接MySQL数据库
1、my_database数据库中建立表

CREATE TABLE actor(
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(32) NOT NULL DEFAULT '',
sex CHAR(1) NOT NULL DEFAULT '女',
borndate DATETIME,
phone VARCHAR(12));
2、下载驱动包并解压

驱动包下载地址:https://dev.mysql.com/downloads/connector/j/

选择操作系统:Select Operating System:Platform Independent(独立于平台)

选择压缩包:Platform Independent (Architecture Independent), ZIP Archive
3、在与src同级目录下创建libs目录，并在libs目录下导入jar包

jar包:JDBC是Java提供用于操作数据库的接口,各数据库厂商实现JDBC接口并打包为jar包,java用JDBC连接MySQL数据库时必须使用该jar包。
4、右击jar包，选择Add as Library

5、编写JDBC程序编写步骤

(1)注册驱动-加载Driver类
(2)获取连接-得到Connection
(3)执行增删改查-给MySQL发送相关SQL指令
(4)释放资源-关闭相关连接
6、代码演示

package jxs.jdbc;

import com.mysql.cj.jdbc.Driver;
import java.sql.Connection;
import java.sql.SQLException;
import java.sql.Statement;
import java.util.Properties;

/*
1.注册驱动
2.获取连接
3.执行SQL
4.释放资源
 */
public class Jdbc01 {
    public static void main(String[] args) throws SQLException {
        Driver driver = new com.mysql.cj.jdbc.Driver();

        /*
        注册驱动解读:
        1.jdbc:mysql:// 协议,表示通过jdbc的方式连接到mysql
        2.localhost ip地址
        3.my_database 数据库名
        4.指定连接数据库的用户名、密码
         */
        String url = "jdbc:mysql://localhost:3306/my_database";
        Properties properties = new Properties();
        properties.setProperty("user", "root");
        properties.setProperty("password", "123456");

        //获取连接
        Connection connect = driver.connect(url, properties);

        /*
        执行SQL
        1.定义SQL语句
        2.statement:用于执行静态SQL语句并返回其生成的结果的对象
         */
        String sql = "insert into actor values (1,'刘德华','男','1961-9-27','18851071324')";
        Statement statement = connect.createStatement();
        //若为dml语句,返回的是影响行数,若rows>0则表示成功,反之失败
        int rows = statement.executeUpdate(sql);
        System.out.println(rows > 0 ? "成功" : "失败");

        statement.close();
        connect.close();
    }
}
数据库5种连接方式（看总结！！！）
1、方式一：new关键字获取Driver驱动类对象实例（静态加载）

Driver driver = new com.mysql.cj.jdbc.Driver();
/*
注册驱动解读:
1.jdbc:mysql:// 协议,表示通过jdbc的方式连接到mysql
2.localhost ip地址
3.my_database 数据库名
4.指定连接数据库的用户名、密码
*/
String url = "jdbc:mysql://localhost:3306/my_database";
Properties properties = new Properties();
properties.setProperty("user", "root");
properties.setProperty("password", "123456");
//获取连接
Connection connect = driver.connect(url, properties);
2、方式二：反射获取Driver驱动类对象实例（动态加载）

public class Jdbc02 {
    public static void main(String[] args) throws Exception {
        //通过反射获取Driver类的字节码对象
        Class<?> driverClass = Class.forName("com.mysql.cj.jdbc.Driver");
        //调用Driver类的无参构造创建对象实例
        Object o = driverClass.newInstance();
        //向下转型
        Driver driver = (Driver) o;
        //指定数据库
        String url = "jdbc:mysql://localhost:3306/my_database";
        //指定连接数据库的用户名和密码
        Properties properties = new Properties();
        properties.setProperty("user","root");
        properties.setProperty("password","123456");
        
        //连接
        Connection connect = driver.connect(url, properties);

        //statement:执行静态SQL语句并返回生成结果的对象
        String sql = "insert into actor values (2,'蒋兴树','男','2001-2-10','15715269957')";
        Statement statement = connect.createStatement();
        //i:静态SQL语句执行成功影响的行数
        int i = statement.executeUpdate(sql);
        //释放资源
        statement.close();
        connect.close();
    }
}
3、方式三：DriverManager替换Driver

public class Jdbc03 {
    public static void main(String[] args) throws Exception {
        Class<?> driverClass = Class.forName("com.mysql.cj.jdbc.Driver");
        Driver driver = (Driver) driverClass.newInstance();
        String url = "jdbc:mysql://localhost:3306/my_database";
        String user = "root";
        String password = "123456";
        //注册Driver驱动
        DriverManager.registerDriver(driver);
        Connection connection = DriverManager.getConnection(url, user, password);

        String sql = "insert into actor values (3,'丁维一','女','2001-7-13','15365040704')";
        Statement statement = connection.createStatement();
        /*
        1.Statement:执行静态SQL语句并且返回生成结果的对象
        2.创建Statement对象实例,执行修改
        3.i:SQL语句执行成功影响的行数
         */
        int i = statement.executeUpdate(sql);
        System.out.println(i);

        statement.close();
        connection.close();
    }
}
4、方式四：Class.forName自动完成注册

public class Jdbc04 {
    public static void main(String[] args) throws Exception {
        /*
        1.通过反射获取Class类的字节码对象
        2.何时类加载:(1)new关键字创建对象实例(2)子类加载,父类也加载
                   (3)调用类的静态成员(4)反射
        3.Driver类类加载时,静态代码块执行,注册Driver驱动
        public class Driver extends NonRegisteringDriver implements java.sql.Driver {
            public Driver() throws SQLException {
            }

            static {
                try {
                    DriverManager.registerDriver(new Driver());
                } catch (SQLException var1) {
                    throw new RuntimeException("Can't register driver!");
                }
            }
        }
         */
        Class.forName("com.mysql.cj.jdbc.Driver");


        String url = "jdbc:mysql://localhost:3306/my_database";
        String user = "root";
        String password = "123456";

        Connection connection = DriverManager.getConnection(url, user, password);

        String sql = "insert into actor values (4,'田宇浩','男','2001-1-1','110')";

        /*
        statement对象实例:执行静态SQL语句并返回生成结果
         */
        Statement statement = connection.createStatement();
        int i = statement.executeUpdate(sql);

        statement.close();
        connection.close();
    }
}
5、方式五：使用配置文件连接数据库

(1)mysql驱动5.1.6后无需class.forName("com.mysql.cj.jdbc.Driver")
(2)jdk1.5后使用了jdbc4,不需显式调用class.forName("com.mysql.cj.jdbc.Driver")注册驱动,而是自动调用驱动jar包下META-INF\services\java.sql.Driver文本中的类名称去注册
src目录下创建配置文件:
user=root
password=123456
url=jdbc:mysql://localhost:3306/my_database
driver=com.mysql.cj.jdbc.Driver
public class Jdbc05 {
    public static void main(String[] args) throws Exception {
        //创建Properties类对象实例
        Properties properties = new Properties();
        //加载properties配置文件
        properties.load(new FileInputStream("E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties"));
        //获取相关值
        String url = properties.getProperty("url");
        String user = (String)properties.get("user");
        String password = properties.getProperty("password");
        String driver = properties.getProperty("driver");

        /*
        可写可不写
        1.若不写则自动调用驱动jar包下META-INF\services\java.sql.Driver文本中的类名称去注册
         */
        Class<?> driverClass = Class.forName(driver);

        //连接
        Connection connection = DriverManager.getConnection(url, user, password);

        String sql = "insert into actor values (5,'刘中珍','女','1973-4-29','13812483280')";
        Statement statement = connection.createStatement();
        int i = statement.executeUpdate(sql);

        statement.close();
        connection.close();
    }
}
6、总结

连接数据库步骤:
(1)创建配置文件对象实例
(2)加载配置文件
(3)获取配置文件信息
(4)通过反射加载Driver类(底层执行静态代码块中DriverManager.registerDriver()方法,注册Driver驱动,创建Driver类对象实例)
(5)获取连接(DriverManager.getConnection(url, user, password))
(6)创建实现Statement接口的类对象实例,执行静态SQL语句并生成结果(connection.createStatement()方法)
(7)dml操作使用statement.executeUpdate()方法;select操作使用statement.executeQuery()方法
(8)释放资源
ResultSet底层（重要！！！）
1、题目要求

1.创建news表
2.使用jdbc添加5条数据
3.修改id=1的记录,将name改为自己的名字
4.删除id=3的记录
5.查看news表
2、创建表

CREATE TABLE news(
id INT,
name VARCHAR(32));
3、代码演示

public class JdbcExercise {
    public static void main(String[] args) throws Exception {
        //创建配置文件对象
        Properties properties = new Properties();
        //加载配置文件
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties";
        properties.load(new FileInputStream(srcPath));
        //获取配置文件信息
        String driver = properties.getProperty("driver");
        String url = properties.getProperty("url");
        String user = properties.getProperty("user");
        String password = (String) properties.get("password");

        //加载Driver类,底层自动注册Driver驱动,创建Driver类对象实例
        Class.forName(driver);

        //获取连接
        Connection connection = DriverManager.getConnection(url, user, password);

        //statement对象:执行静态SQL语句并生成结果
        Statement statement = connection.createStatement();
        String sql1 = "delete from news ";
        String sql2 = "insert into news values (1,'jxs'),(2,'lzz'),(3,'dwy'),(4,'tyh'),(5,'zls')";
        String sql3 = "update news set name = '蒋兴树' where id = 1";
        String sql4 = "select * from news";
        //dml语句
        statement.executeUpdate(sql1);
        statement.executeUpdate(sql2);
        statement.executeUpdate(sql3);
        /*
        select语句
        1.执行给定的SQL语句,返回单个resultSet对象
         */
        ResultSet resultSet = statement.executeQuery(sql4);
        /*
        resultSet.next(),光标移动到表的下一行,循环取出表的每一列数据
        1.
         */
        while (resultSet.next()) {
            //获取该行第一列数据
            int id = resultSet.getInt(1);
            //获取改行第二列数据
            String name = resultSet.getString(2);
            System.out.println(id + name);
        }

        //释放资源
        resultSet.close();
        statement.close();
        connection.close();
    }
}
4、ResultSet对象结构图：

![](E:\Study\自学课程资料\Java\assets\ResultSet对象结构图.png)

Statement
1、基本介绍

(1)Statement对象用于执行静态SQL语句并返回生成结果
(2)建立与数据库的连接后,需对数据库进行访问,执行、命名、SQL语句可以通过Statement[存在SQL注入]、PreparedStatement[预处理]、CallableStatement[存储过程]
(3)Statement对象执行SQL语句存在SQL注入风险
(4)SQL注入是利用某些系统没有对用户输入的数据进行充分的检查,而在用户输入数据时注入非法的SQL语句段或命令,恶意攻击数据库
(5)防范SQL注入只需用PreparedStatement(Statement扩展)取代Statement即可
2、SQL注入案例演示

# 创建表
CREATE TABLE admin(
name VARCHAR(32),
pwd VARCHAR(32));
# 插入数据
INSERT INTO admin VALUES ('jxs','123456');
# 查找数据
SELECT * FROM admin WHERE name = 'jxs' AND pwd = '123456';
# SQL注入
SELECT * FROM admin WHERE name = ' 1' OR ' AND pwd =' OR '1' = '1 '
3、SQL注入代码演示

public class JdbcStatement {
    public static void main(String[] args) throws Exception {
        Scanner scanner = new Scanner(System.in);

        /*
        1.使用scanner.next()当接收到空格或单引号时表示结束
        2.使用scanner.nextLine()当回车时表示结束
         */
        System.out.print("输入用户名");
        String admin_name = scanner.nextLine();
        System.out.print("输入密码");
        String admin_pwd = scanner.nextLine();

        //创建配置文件对象
        Properties properties = new Properties();
        //加载配置文件
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties";
        properties.load(new FileInputStream(srcPath));
        //获取配置文件信息
        String driver = properties.getProperty("driver");
        String url = properties.getProperty("url");
        String user = properties.getProperty("user");
        String password = (String) properties.get("password");

        //加载Driver类,底层自动注册Driver驱动,创建Driver类对象实例
        Class.forName(driver);

        //获取连接
        Connection connection = DriverManager.getConnection(url, user, password);

        //statement对象:执行静态SQL语句并生成结果
        Statement statement = connection.createStatement();
        String sql = " select name,pwd from admin where name = '"+admin_name+"' and pwd = '"+admin_pwd+"' ";
        //执行给定的SQL语句,返回单个resultSet对象
        ResultSet resultSet = statement.executeQuery(sql);
        //光标指向下一行,循环取出每一列数据,若查询到数据说明该用户存在
        if (resultSet.next()) {
            System.out.println("用户存在");
        } else {
            System.out.println("用户不存在");
        }

        resultSet.close();
        statement.close();
        connection.close();
    }
}

/*
输入用户名1' OR
输入密码OR '1' = '1
用户存在
*/
PreparedStatement预处理（重中之重！！！看总结！！！）
1、PreparedStatement图解



2、基本介绍

(1)PreparedStatement执行的SQL语句中的参数用问号?来表示,调用PreparedStatement对象的setXxx()方法来设置这些参数,setXxx()方法有两个参数,第一个参数是设置SQL语句中的参数的索引(从1开始),第二个参数是设置SQL语句中参数的值
(2)调用executeQuery()方法返回ResultSet对象
(3)调用executeUpdate()方法执行增删改操作,返回SQL语句执行成功影响的行数
3、PreparedStatement好处

(1)不再使用+拼接SQL语句,减少语法错误
(2)有效解决SQL注入问题
(3)减少编译次数,提高效率
4、代码演示

public class JdbcPreparedStatement {
    public static void main(String[] args) throws Exception {
        Scanner scanner = new Scanner(System.in);

        //创建配置文件对象
        Properties properties = new Properties();
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties";
        //加载配置文件
        properties.load(new FileInputStream(srcPath));
        //获取配置文件信息
        String url = properties.getProperty("url");
        String user = properties.getProperty("user");
        String password = properties.getProperty("password");
        String driver = properties.getProperty("driver");
        //通过反射进行类加载,底层自动注册Driver驱动,创建Driver类对象实例
        Class.forName(driver);
        //获取连接
        Connection connection = DriverManager.getConnection(url, user, password);


        /*
        1.SQL语句?相当于占位符
        2.connection.prepareStatement(sql)返回的是实现了PreparedStatement接口的类的对象实例
         */
        String sql1 = "select name,pwd from admin where name = ? and pwd = ?";
        PreparedStatement preparedStatement1 = connection.prepareStatement(sql1);
        System.out.print("输入查询的用户名");
        String admin_name1 = scanner.nextLine();
        System.out.print("输入查询的密码");
        String admin_pwd1 = scanner.nextLine();
        //为第一个?赋值admin_name1,为第二个?赋值admin_pwd1
        preparedStatement1.setString(1,admin_name1);
        preparedStatement1.setString(2,admin_pwd1);
        /*
        1.执行SQL增删改指令使用executeUpdate()方法
        2.执行SQL查找指令使用executeQuery()方法
         */
        ResultSet resultSet = preparedStatement1.executeQuery();
        if (resultSet.next()) {
            System.out.println("用户存在");
        } else {
            System.out.println("用户不存在");
        }


        String sql2 = "insert into admin values (?,?)";
        PreparedStatement preparedStatement2 = connection.prepareStatement(sql2);
        System.out.print("输入添加的用户名");
        String admin_name2 = scanner.nextLine();
        System.out.print("输入添加的密码");
        String admin_pwd2 = scanner.nextLine();
        //为第一个?赋值admin_name2,为第二个?赋值admin_name2
        preparedStatement2.setString(1,admin_name2);
        preparedStatement2.setString(2,admin_pwd2);
        int i1 = preparedStatement2.executeUpdate();
        if (i1 != 0) {
            System.out.println("用户添加成功");
        } else {
            System.out.println("用户添加失败");
        }


        String sql3 = "update admin set pwd = ? where name = ?";
        PreparedStatement preparedStatement3 = connection.prepareStatement(sql3);
        System.out.print("输入修改的用户名");
        String admin_name3 = scanner.nextLine();
        System.out.print("输入修改的密码");
        String admin_pwd3 = scanner.nextLine();
        preparedStatement3.setString(2,admin_name3);
        preparedStatement3.setString(1,admin_pwd3);
        int i2 = preparedStatement3.executeUpdate();
        if (i2 != 0) {
            System.out.println("用户修改成功");
        } else {
            System.out.println("用户修改失败");
        }

        resultSet.close();
        preparedStatement1.close();
        preparedStatement2.close();
        preparedStatement3.close();
        connection.close();
    }
}
5、总结

(1)创建配置文件对象实例
(2)加载配置文件
(3)获取配置文件信息
(4)通过反射加载Driver类,底层源码自动注册Driver驱动,创建Driver类对象实例。若不加载Driver类,则自动调用jar包下META-INF\services\java.sql.Driver文本中的类名称去注册
(5)获取连接(DriverManager.getConnection()),传入获取的配置文件信息
(6)编写静态SQL指令
(7)创建实现PreparedStatement接口的类的对象实例(connection.prepareStatement(sql)),并传入SQL语句,执行静态SQL语句并生成结果,防止SQL注入
(8)执行preparedStatement.setString(1,'jxs')方法,为第一个?赋值'jxs'
(9)preparedStatement.executeQuery()用于查找指令;preparedStatement.executeUpdate()用于增删改指令
JDBC API小结
![](E:\Study\自学课程资料\Java\assets\JDBC API.png)

JDBCUtils工具类
public class JDBCUtils {
    private static String driver;
    private static String user;
    private static String password;
    private static String url;

    /**
     * 创建配置文件对象实例
     * 加载配置文件
     * 获取配置文件信息
     */
    static {
        Properties properties = new Properties();
        try {
            properties.load(new FileInputStream("E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties"));
            driver = properties.getProperty("driver");
            user = properties.getProperty("user");
            password = properties.getProperty("password");
            url = properties.getProperty("url");
        } catch (IOException e) {
            /*
            1.实际开发中,可以将编译异常转为运行时异常
            2.调用者可以选择抛出异常或解决异常
             */
            throw new RuntimeException(e);
        }
    }

    /**
     * 获取连接
     *
     * @return 连接对象实例
     */
    public static Connection getConnection() {
        try {
            return DriverManager.getConnection(url, user, password);
        } catch (SQLException throwable) {
            throw new RuntimeException(throwable);
        }
    }

    /**
     * 释放资源
     *
     * @param resultSet  结果集
     * @param statement  Statement或preparedStatement
     * @param connection 连接对象实例
     */
    public static void Close(ResultSet resultSet, Statement statement, Connection connection) {
        try {
            if (resultSet != null) {
                resultSet.close();
            }
            if (statement != null) {
                statement.close();
            }
            if (connection != null) {
                connection.close();
            }
        } catch (SQLException throwable) {
            throw new RuntimeException(throwable);
        }
    }
}

class JdbcUtils_Use {
    public static void main(String[] args) {

    }

    @Test
    public void testDML() {
        Connection connection = null;
        PreparedStatement preparedStatement = null;
        try {
            connection = JDBCUtils.getConnection();
            String sql = "update admin set name = ? where pwd = ?";
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(2, "123");
            preparedStatement.setString(1, "蒋兴树");
            preparedStatement.executeUpdate();
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        } finally {
            JDBCUtils.Close(null, preparedStatement, connection);
        }
    }

    @Test
    public void testSelect() {
        ResultSet resultSet = null;
        Connection connection = null;
        PreparedStatement preparedStatement = null;
        try {
            connection = JDBCUtils.getConnection();
            String sql = "select name,pwd from admin where pwd = ?";
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, "123");
            resultSet = preparedStatement.executeQuery();
            while (resultSet.next()) {
                String name = resultSet.getString(1);
                String pwd = resultSet.getString(2);
                System.out.println(name + pwd);
            }
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        } finally {
            JDBCUtils.Close(resultSet, preparedStatement, connection);
        }
    }
}
事务
1、基本介绍

(1)JDBC程序中当一个Connection对象创建时,默认情况下自动提交事务:每次执行一个SQL语句时,若执行成功则向数据库自动提交,不可回滚
(2)JDBC程序中为了让多个SQL语句作为一个整体执行,需使用事务
(3)调用Connection的setAutoCommit(false)可取消自动提交事务
(4)所有SQL语句都执行成功后,调用Connection的commit()方法提交事务
(5)其中某个操作失败或出现异常时,调用Connection的rollback()方法回滚事务
2、应用实例

create table account(
id INT PRIMARY KEY AUTO_INCREMENT,
name VARCHAR(32) NOT NULL DEFAULT '',
balance DOUBLE NOT NULL DEFAULT 0);

INSERT INTO account VALUES (NULL,'马云',2900);
INSERT INTO account VALUES (NULL,'马化腾',3100);

SELECT * FROM account;
public class Transaction {
    public static void main(String[] args) {
    }

    /**
     * 不开启事务
     */
    @Test
    public void noTransaction() {
        //获取连接
        Connection connection = JDBCUtils.getConnection();

        String sql1 = "update account set balance = balance - 100 where id = ?";
        String sql2 = "update account set balance = balance + 100 where id = ?";
        PreparedStatement preparedStatement1 = null;
        PreparedStatement preparedStatement2 = null;
        
        try {
            /*
            1.创建connection对象实例后,默认情况下,每执行成功一个SQL语句则自动向数据库提交
            2.若中途抛出异常,下面的代码不再执行
             */
            preparedStatement1 = connection.prepareStatement(sql1);
            preparedStatement1.setInt(1, 2);
            preparedStatement1.executeUpdate();

            //捕获异常
            int i = 1 / 0;

            preparedStatement2 = connection.prepareStatement(sql2);
            preparedStatement2.setInt(1, 1);
            preparedStatement2.executeUpdate();

        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        } finally {
            JDBCUtils.Close(null,preparedStatement1,connection);
            JDBCUtils.Close(null,preparedStatement2,connection);
        }
    }

    /**
     * 开启事务
     * @throws Exception
     */
    @Test
    public void useTransaction() throws Exception {
        Connection connection = JDBCUtils.getConnection();
        //开启事务,将connection设置为不自动提交
        connection.setAutoCommit(false);
        //设置回滚点savepoint1
        Savepoint savepoint1 = connection.setSavepoint();

        String sql1 = "update account set balance = balance - 100 where id = ?";
        String sql2 = "update account set balance = balance + 100 where id = ?";
        PreparedStatement preparedStatement1 = null;
        PreparedStatement preparedStatement2 = null;
        try {
            /*
            1.创建connection对象实例后,默认情况下,每执行成功一个SQL语句则自动向数据库提交
            2.若中途抛出异常,下面的代码不再执行
             */
            preparedStatement1 = connection.prepareStatement(sql1);
            preparedStatement1.setInt(1, 2);
            preparedStatement1.executeUpdate();

            //捕获异常
            int i = 1 / 0;

            preparedStatement2 = connection.prepareStatement(sql2);
            preparedStatement2.setInt(1, 1);
            preparedStatement2.executeUpdate();

            //提交事务
            connection.commit();

        } catch (SQLException throwable) {

            //回滚到savepoint1,撤销执行的SQL指令
            System.out.println("回滚到savepoint1");
            connection.rollback(savepoint1);
            
            System.out.println(throwable.getMessage());

        } finally {
            JDBCUtils.Close(null,preparedStatement1,connection);
            JDBCUtils.Close(null,preparedStatement2,connection);
        }
    }
}
批处理
1、基本介绍

(1)当需要成批插入或更新记录时,可以采用Java批量更新机制,允许多条SQL语句一次性提交给数据库批量处理。通常情况下比单独提交处理更有效率
(2)JDBC批量处理SQL语句包括以下方法
addBatch():添加需要批处理的SQL语句或参数
executeBatch():执行批处理语句
clearBatch():清空批处理语句
(3)JDBC连接数据库若想使用批处理功能则需在url中加入参数?rewriteBatchedStatements=true
(4)批处理往往和PreparedStatement搭配使用,减少编译次数和运行次数,提高效率
2、应用实例

CREATE TABLE admin(
id INT PRIMARY KEY AUTO_INCREMENT,
username VARCHAR(32) NOT NULL,
password VARCHAR(32) NOT NULL);
public class Batch {
    public static void main(String[] args) {

    }

    /**
     * 不使用批处理
     *
     * @throws Exception
     */
    @Test
    public void noBatch() throws Exception {
        Connection connection = JDBCUtils.getConnection();
        String sql = "insert into admin values (null,?,?)";
        PreparedStatement preparedStatement = connection.prepareStatement(sql);

        long start = System.currentTimeMillis();
        for (int i = 0; i < 5000; i++) {
            preparedStatement.setString(1, "jack" + i);
            preparedStatement.setString(2, "123");
            preparedStatement.executeUpdate();
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);//5507

        JDBCUtils.Close(null, preparedStatement, connection);
    }

    /**
     * 使用批处理
     */
    @Test
    public void useBatch() throws Exception {
        Connection connection = JDBCUtils.getConnection();
        String sql = "insert into admin values (null,?,?)";
        PreparedStatement preparedStatement = connection.prepareStatement(sql);

        long start = System.currentTimeMillis();
        for (int i = 0; i < 5000; i++) {
            preparedStatement.setString(1, "jack" + i);
            preparedStatement.setString(2, "123");
            //将SQL语句添加到批处理包中
            preparedStatement.addBatch();
            //满1000条SQL语句分批处理一次
            if ((i + 1) % 1000 == 0) {
                //批量执行SQL语句
                preparedStatement.executeBatch();
                //清空
                preparedStatement.clearBatch();
            }
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);
        //释放资源
        JDBCUtils.Close(null, preparedStatement, connection);
    }
}
3、批处理源码分析

/*
1.ArrayList中维护了一个Object类型的数组elementData
2.elementData数组存放预处理的SQL语句
3.当elementData对象数组满后,扩容1.5倍
4.当到达指定值后则执行executeBatch()方法
*/
public void addBatch(Object batch) {
    if (this.batchedArgs == null) {
        this.batchedArgs = new ArrayList();
    }
    this.batchedArgs.add(batch);
}

public boolean add(E e) {
    ensureCapacityInternal(size + 1);  // Increments modCount!!
    elementData[size++] = e;
    return true;
}
连接池（DBCP-Database Connection Pool）（重点看德鲁伊连接池！！！）
1、传统方式连接数据库弊端

(1)传统的JDBC数据库连接使用DriverManager获取,每次向数据库建立连接时都要将Connection加载到内存中,再验证IP地址、用户名、密码。频繁的进行数据库连接操作将占用很多系统资源,易造成服务器崩溃
(2)每连接数据库,使用完后断开连接,若程序中出现异常而未能关闭,将导致数据库内存泄漏,最终导致重启数据库
(3)传统获取连接的方式,不可控制连接数据库的数量
(4)为解决传统开发中数据库连接问题,可采用数据库连接池技术
2、数据库连接池基本介绍

(1)预先在缓冲池中放入一定数量的连接,当需要建立数据库连接时,只需从"缓冲池"中取出一个,使用完毕后再放回"缓冲池"
(2)数据库连接池负责分配、管理、释放数据库连接,允许应用程序重复使用一个现有的数据库连接,而不是重新建立一个
(3)当应用程序向连接池请求的连接数超过最大连接数量时,这些请求将被加入到等待队列中
3、数据库连接池示意图

![](E:\Study\自学课程资料\Java\assets\数据库连接池示意图.png)

4、数据库连接池种类

(1)JDBC的数据库连接池使用javax.sql.DataSource表示,DataSource只是一个接口,该接口由第三方提供实现
(2)C3P0数据库连接池,速度相对较慢,稳定性不错
(3)DBCP数据库连接池,速度比C3P0快,不稳定
(4)Proxool数据库连接池,可监控连接池状态,稳定性比C3P0差
(5)BoneCP数据库连接池,速度快
(6)Druid阿里提供的数据库连接池,集DBCP、C3P0、Proxool优点于一身的数据库连接池
5、C3P0连接池应用实例

(1)C3P0连接池jar包下载地址
https://sourceforge.net/projects/c3p0/

(2)解压后将c3p0-0.9.5.5.jar包、mchange-commons-java-0.2.19.jar包导入到项目的libs目录下

(3)项目src目录下添加配置文件c3p0-config.xml
<?xml version="1.0" encoding="UTF-8"?>
<c3p0-config>
    <!-- 数据源名称 代表连接池 -->
    <named-config name = "jxs_database_connection_pool">
        <property name="driverClass">com.mysql.cj.jdbc.Driver</property>
        <property name="jdbcUrl">jdbc:mysql://localhost:3306/my_database</property>
        <property name="user">root</property>
        <property name="password">123456</property>

        <!-- 初始连接数 -->
        <property name="initialPoolSize">10</property>
        <!-- 最大连接数 -->
        <property name="maxPoolSize">100</property>
        <!-- 最小连接数 -->
        <property name="minPoolSize">10</property>
    </named-config>
</c3p0-config>
    
(4)编写代码
public class ConnectionPool {
    public static void main(String[] args) {
    }

    /**
     * 传统方式连接数据库
     */
    @Test
    public void noConnectionPool() {
        //Too many connections
        long start = System.currentTimeMillis();
        for (int i = 0; i < 5000; i++) {
            Connection connection = JDBCUtils.getConnection();
            JDBCUtils.Close(null,null,connection);
        }
        long stop = System.currentTimeMillis();
        System.out.println("传统方式耗时" + (stop - start));//62322
    }

    
    /**
     * C3P0连接池使用方式一:在程序中指定相关参数url、user、password
     */
    @Test
    public void useConnectionPool01() throws Exception {
        //1.创建数据源对象
        ComboPooledDataSource comboPooledDataSource = new ComboPooledDataSource();
        //2.通过配置文件对象获取配置文件信息
        Properties properties = new Properties();
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\mysql.properties";
        properties.load(new FileInputStream(srcPath));
        String driver = properties.getProperty("driver");
        String user = properties.getProperty("user");
        String password = properties.getProperty("password");
        String url = properties.getProperty("url");
        /*
        3.为数据源设置相关参数
          将数据源连接到数据库
          java程序通过数据源连接数据库
         */
        comboPooledDataSource.setDriverClass(driver);
        comboPooledDataSource.setUser(user);
        comboPooledDataSource.setPassword(password);
        comboPooledDataSource.setJdbcUrl(url);
        //4.初始化连接池连接数
        comboPooledDataSource.setInitialPoolSize(10);
        //5.设置连接池最大连接数
        comboPooledDataSource.setMaxPoolSize(50);

        long start = System.currentTimeMillis();
        for (int i = 0; i < 5000; i++) {
            //6.获取连接
            Connection connection = comboPooledDataSource.getConnection();
            //7.释放资源
            connection.close();
        }
        long stop = System.currentTimeMillis();
        System.out.println("使用连接池耗时" + (stop - start));//1351
    }


    /**
     * C3P0连接池使用方式二:使用配置文件模板完成
     */
    @Test
    public void useConnectionPool02() throws Exception {
        ComboPooledDataSource comboPooledDataSource = new ComboPooledDataSource("jxs_database_connection_pool");
        Connection connection = comboPooledDataSource.getConnection();
        System.out.println("连接成功");
    }
}
6、Druid（德鲁伊）应用实例

(1)Druid连接池jar包下载地址
https://repo1.maven.org/maven2/com/alibaba/druid/

(2)将druid-1.2.9.jar包拷贝到项目的libs目录下

(3)项目src目录下添加配置文件druid.properties
driverClassName=com.mysql.cj.jdbc.Driver
url=jdbc:mysql://localhost:3306/my_database?rewriteBatchedStatements=true
username=root
password=123456
#初始化连接数
initialSize=10
# 最小空闲数
minIdle=5
#最大连接数
maxActive=10
#获取连接时最大等待时间
maxWait=3000
    
(4)编写代码
public class ConnectionPool {
    public static void main(String[] args) {
    }
    
    /**
     * Druid(德鲁伊)连接池
     */
    @Test
    public void useConnectionPool03() throws Exception {
        //创建配置文件对象实例
        Properties properties = new Properties();
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\druid.properties";
        properties.load(new FileInputStream(srcPath));
        //创建指定参数的Druid数据库连接池
        DataSource dataSource = DruidDataSourceFactory.createDataSource(properties);

        long start = System.currentTimeMillis();
        for (int i = 0; i < 500000; i++) {
            //6.获取连接
            Connection connection = dataSource.getConnection();
            //7.释放资源
            connection.close();
        }
        long stop = System.currentTimeMillis();
        System.out.println(stop - start);//1722
    }
}
7、Druid（德鲁伊）工具类

public class JdbcUtilsByDruid {

    private static DataSource ds;

    /*
    类加载时执行static静态代码块
    1.通过反射加载Driver类,底层源码自动注册Driver驱动,创建Driver类对象实例
    2.若不加载Driver类
      则自动调用jar包下META-INF\services\java.sql.Driver文本中的类名称去注册
     */
    static {
        //创建配置文件对象实例
        Properties properties = new Properties();
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\druid.properties";
        try {
            //加载配置文件
            properties.load(new FileInputStream(srcPath));
            /*
            1.使用配置文件信息创建Druid(德鲁伊)连接池
            driverClassName=com.mysql.cj.jdbc.Driver
            url=jdbc:mysql://localhost:3306/my_database?rewriteBatchedStatements=true
            username=root
            password=123456
            #初始化连接数
            initialSize=10
            # 最小空闲数
            minIdle=5
            #最大连接数
            maxActive=10
            #获取连接时最大等待时间
            maxWait=3000
             */

            ds = DruidDataSourceFactory.createDataSource(properties);
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }

    /**
     * 获取连接
     * @return
     */
    public static Connection getConnection() {
        Connection connection = null;
        try {
            //java程序从连接池取出连接,连接到MySQL数据库
            connection = ds.getConnection();
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
        return connection;
    }

    /**
     * 将connection对象放回连接池
     */
    public static void close(ResultSet resultSet, Statement statement, Connection connection) {
        try {
            if (resultSet != null) {
                resultSet.close();
            }
            if (statement != null) {
                statement.close();
            }
            if (connection != null) {
                connection.close();
            }
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
    }
}
public class JdbcUtilsByDruidExercise {
    public static void main(String[] args) {
        Connection connection = null;
        PreparedStatement preparedStatement = null;
        String sql = "insert into admin values (null,'jxs','123')";

        try {
            //调用Druid德鲁伊连接池工具类的getConnection()获取连接
            connection = JdbcUtilsByDruid.getConnection();
            //运行类型:class com.alibaba.druid.pool.DruidPooledConnection
            System.out.println(connection.getClass());
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.executeUpdate();
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        } finally {
            //调用Druid德鲁伊连接池工具类的close()释放资源
            JdbcUtilsByDruid.close(null,preparedStatement,connection);
        }
    }
}
Apache-DBUtils
1、问题分析

(1)关闭connection后,resultSet结果集无法使用
(2)resultSet不利用数据的管理
2、resultSet结果集问题分析示意图

![](E:\Study\自学课程资料\Java\assets\resultSet结果集问题分析示意图.png)

3、传统方法将resultSet结果集封装到ArrayList集合中

CREATE TABLE admin(
id INT PRIMARY KEY AUTO_INCREMENT,
username VARCHAR(32) NOT NULL,
password VARCHAR(32) NOT NULL);

INSERT INTO admin VALUES (1,'jxs','123'),(2,'dwy','123'),(3,'lzz','123');
public class Admin {

    private int id;
    private String username;
    private String password;

    public Admin() {
    }

    public Admin(int id, String username, String password) {
        this.id = id;
        this.username = username;
        this.password = password;
    }

    public int getId() { return id; }
    public void setId(int id) { this.id = id; }
    public String getUsername() { return username; }
    public void setUsername(String username) { this.username = username; }
    public String getPassword() { return password; }
    public void setPassword(String password) { this.password = password; }

    @Override
    public String toString() {
        return "jxs.DBUtils.Admin{" +
                "id=" + id +
                ", username='" + username + '\'' +
                ", password='" + password + '\'' +
                '}';
    }
}


class DBUtils_Exercise {
    /**
     * 传统方法将resultSet结果集封装到ArrayList集合中
     */
    @Test
    public void test1() {
        //创建泛型为Admin类型的ArrayList集合
        ArrayList<Admin> admins = new ArrayList<>();
        //定义连接
        Connection connection = null;
        //定义ResultSet结果集
        ResultSet resultSet = null;
        //定义预处理
        PreparedStatement preparedStatement = null;

        try {
            //获取连接
            connection = JdbcUtilsByDruid.getConnection();
            String sql = "select * from admin where id >= ?";
            //创建PreparedStatement预处理对象,执行静态SQL语句
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句第1个?赋值1
            preparedStatement.setInt(1, 1);
            resultSet = preparedStatement.executeQuery();
            //while循环遍历resultSet结果集每一行,取出每一行每一列的数据
            while (resultSet.next()) {
                int id = resultSet.getInt("id");
                String username = resultSet.getString("username");
                String password = resultSet.getString("password");
                /*
                1.将每一列数据封装为admin对象,添加到集合中
                2.关闭连接后,可以继续使用resultSet结果集中数据
                 */
                Admin admin = new Admin(id, username, password);
                admins.add(admin);
            }
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        } finally {
            JdbcUtilsByDruid.close(resultSet, preparedStatement, connection);
        }

        Iterator<Admin> iterator = admins.iterator();
        while (iterator.hasNext()) {
            System.out.println(iterator.next());
        }
    }
}
4、Apache-DBUtils基本介绍

(1)commons-dbutils是Apache组织提供的一个开源JDBC工具类库,它是对JDBC的封装,使用dbutils能极大简化jdbc编码的工作量
(2)QueryRunner类:封装了SQL的执行,是线程安全的。可以实现增删改查、批处理
(3)ResultSetHandler接口:此接口用于处理java.sql.ResultSet,将数据按要求转换为另一种形式
ScalarHandler:获取单行单列的值,单值查询

ArrayHandler:将结果集中的第一行数据封装成Object[]
ArrayListHandler:将结果集中的每一行数据封装成Object[]并存放到List中,即List<Object[]>

BeanHandler:将结果集中的第一行数据封装到一个对应的JavaBean对象实例中。
BeanListHandler:将结果集中的每一行数据都封装到一个对应的JavaBean实例中并存放到List中,即List<JavaBean>

ColumnListHandler:将结果集中某一列的数据存放到List中,即List<某一列的类型>

KeyedHandler(name):将结果集中的每行数据都封装到Map中并再存放到Map中,即Map<某一列Java类型,Map<列名类型,列值类型>>

MapHandler:将结果集中的第一行数据封装到一个Map中,key是列名,value是列值
MapListHandler:将结果集中的每一行数据都封装到一个Map中并存放到List中,即List<Map<列名类型,列值类型>>
5、Apache-DBUtils应用实例

(1)将commons-dbutils-1.7.jar包拷贝到项目的libs目录下

(2)编写代码
public class Admin {

    private int id;
    private String username;
    private String password;

    public Admin() { }

    public Admin(int id, String username, String password) {
        this.id = id;
        this.username = username;
        this.password = password;
    }

    public int getId() {
        return id;
    }
    public void setId(int id) {
        this.id = id;
    }
    public String getUsername() {
        return username;
    }
    public void setUsername(String username) {
        this.username = username;
    }
    public String getPassword() {
        return password;
    }
    public void setPassword(String password) {
        this.password = password;
    }

    @Override
    public String toString() {
        return "jxs.DBUtils.Admin{" +
                "id=" + id +
                ", username='" + username + '\'' +
                ", password='" + password + '\'' +
                '}';
    }
}


class DBUtils_Exercise {

    /**
     * 使用Druid连接池和Apache-DBUtils工具类返回多行记录(多个对象)
     */
    @Test
    public void test2() throws Exception {
        //获取连接
        Connection connection = JdbcUtilsByDruid.getConnection();
        String sql = "select id,username,password from admin where id >= ?";
        //创建QueryRunner类对象实例
        QueryRunner queryRunner = new QueryRunner();
        /*
        解读
        1.query()方法:执行SQL语句,获取resultSet结果集,封装到ArrayList集合中,返回集合
        2.new BeanListHandler<>(jxs.DBUtils.Admin.class):
          底层通过反射获取Admin类属性
          将resultSet结果集封装为Admin对象实例
          将Admin对象实例放入ArrayList集合
          获取的resultSet结果集、preparedStatement会自动关闭
        3.1是为SQL语句中的第一个?赋值为1,最后一个实参为可变参数,可以为多个?赋值
         */
        List<Admin> query = queryRunner.query(connection, sql, new BeanListHandler<>(Admin.class), 1);
        //增强for循环遍历集合
        for (Admin admin : query) {
            System.out.println(admin);
        }
        JdbcUtilsByDruid.close(null, null, connection);
    }


    /**
     * 使用Druid连接池和Apache-DBUtils工具类返回单行记录(单个对象)
     */
    @Test
    public void test3() {
        //获取连接池中的连接
        Connection connection = JDBCUtils.getConnection();
        //创建QueryRunner类对象实例
        QueryRunner queryRunner = new QueryRunner();
        //定义SQL语句
        String sql = "select * from admin where id = ?";
        /*
        BeanHandler:返回单行记录(单个对象)
         */
        try {
            Admin admin = queryRunner.query(connection, sql, new BeanHandler<>(Admin.class), 1);
            System.out.println(admin);
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
        JdbcUtilsByDruid.close(null, null, connection);
    }


    /**
     * 使用Druid连接池和Apache-DBUtils工具类返回单行单列
     */
    @Test
    public void test4() {
        //获取连接池中的连接
        Connection connection = JDBCUtils.getConnection();
        //创建QueryRunner类对象实例
        QueryRunner queryRunner = new QueryRunner();
        //定义SQL语句
        String sql = "select username from admin where id = ?";
        /*
        BeanHandler:返回单行记录(单个对象)
         */
        try {
            Object o = queryRunner.query(connection, sql, new ScalarHandler<>(), 1);
            System.out.println(o);
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
        JdbcUtilsByDruid.close(null, null, connection);
    }


    /**
     * 使用Druid连接池和Apache-DBUtils工具类完成DML操作
     */
    @Test
    public void test5() {
        //获取连接池中的连接
        Connection connection = JDBCUtils.getConnection();
        //创建QueryRunner类对象实例
        QueryRunner queryRunner = new QueryRunner();
        //定义SQL语句
        String sql1 = "update admin set username = ? where id = ?";
        String sql2 = "select * from admin where id = ?";
        String sql3 = "insert into admin values (null,?,?)";
        String sql4 = "delete from admin where id = ?";
        /*
        BeanHandler:返回单行记录(单个对象)
         */
        try {
            /*
            1.为SQL语句sql1第1个?赋值蒋兴树,第2个?赋值1
            2.i:SQL语句执行成功受影响的行数
             */
            int i1 = queryRunner.update(connection, sql1, "蒋兴树", 1);
            System.out.println(i1);
            /*
            1.new BeanHandler<>(Admin.class)返回单行记录
             */
            Admin admin = queryRunner.query(connection, sql2, new BeanHandler<>(Admin.class), 1);
            System.out.println(admin);
            /*
            1.为SQL语句sql3第1个?赋值zls,第2个?赋值123
            2.i:SQL语句执行成功受影响的行数
             */
            int i2 = queryRunner.update(connection, sql3, "zls", "123");
            System.out.println(i2);
            /*
            1.为SQL语句sql4第1个?赋值4
            2.i:SQL语句执行成功受影响的行数
             */
            int i3 = queryRunner.update(connection, sql4, 4);
            System.out.println(i3);

        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
        JdbcUtilsByDruid.close(null, null, connection);
    }
}
6、Apache-DBUtuils源码分析

private <T> T query(Connection conn, boolean closeConn, String sql, ResultSetHandler<T> rsh, Object... params) throws SQLException {
    if (conn == null) {
        throw new SQLException("Null connection");
    } else if (sql == null) {
        if (closeConn) {
            this.close(conn);
        }

        throw new SQLException("Null SQL statement");
    } else if (rsh == null) {
        if (closeConn) {
            this.close(conn);
        }

        throw new SQLException("Null ResultSetHandler");
    } else {
        //定义PreparedStatement
        PreparedStatement stmt = null;
        //接收返回的结果集
        ResultSet rs = null;
        //接收返回的ArrayList
        Object result = null;

        try {
            //创建PreparedStatement
            stmt = this.prepareStatement(conn, sql);
            //对SQL语句的?进行赋值
            this.fillStatement(stmt, params);
            //执行SQL语句返回resultSet
            rs = this.wrap(stmt.executeQuery());
            //将返回的resultSet结果集放入ArrayList
            result = rsh.handle(rs);
        } catch (SQLException var33) {
            this.rethrow(var33, sql, params);
        } finally {
            try {
                //关闭ResultSet,释放资源
                this.close(rs);
            } finally {
                //关闭PreparedStatement,释放资源
                this.close(stmt);
                if (closeConn) {
                    //关闭连接
                    this.close(conn);
                }

            }
        }
        return result;
    }
}
DAO增删改查-BasicDao
1、问题分析

Apache-DBUtils+Druid简化JDBC开发,但仍有不足
(1)SQL语句固定,不可通过参数传入,通用性不好,需进行改进,更方便执行增删改查
(2)对于select操作,若有返回值,返回值类型不可固定,需使用泛型
(3)将来表很多,业务需求复杂,不可只依靠一个java类完成
2、BasicDao示意图

![](E:\Study\自学课程资料\Java\assets\BasicDao示意图.png)

3、BasicDao基本说明

(1)Dao(data access object):数据访问对象
(2)BasicDao为通用类,专门用于和数据库的交互,即完成对数据库的crud操作
(3)在BasicDao基础上,实现一张表对应一个Dao和pojo,更好的完成功能。例:Customer表-Customer.java类(pojo)、CustomerDao.java
4、BasicDao分析

(1)utils包:工具类
(2)pojo包:pojo
(3)dao包:存放XxxDao、BasicDao
(4)test包:测试类
5、BasicDao实现

Utils工具类

public class JdbcUtilsByDruid {

    private static DataSource ds;

    /*
    类加载时执行static静态代码块
    1.通过反射加载Driver类,底层源码自动注册Driver驱动,创建Driver类对象实例
    2.若不加载Driver类
      则自动调用jar包下META-INF\services\java.sql.Driver文本中的类名称去注册
     */
    static {
        //创建配置文件对象实例
        Properties properties = new Properties();
        String srcPath = "E:\\application\\IntelliJ IDEA 2021.1\\workspace\\Java\\JDBC\\src\\druid.properties";
        try {
            //加载配置文件
            properties.load(new FileInputStream(srcPath));
            /*
            1.使用配置文件信息创建Druid(德鲁伊)连接池
            driverClassName=com.mysql.cj.jdbc.Driver
            url=jdbc:mysql://localhost:3306/my_database?rewriteBatchedStatements=true
            username=root
            password=123456
            #初始化连接数
            initialSize=10
            # 最小空闲数
            minIdle=5
            #最大连接数
            maxActive=10
            #获取连接时最大等待时间
            maxWait=3000
             */

            ds = DruidDataSourceFactory.createDataSource(properties);
        } catch (Exception e) {
            System.out.println(e.getMessage());
        }
    }

    /**
     * 获取连接
     * @return
     */
    public static Connection getConnection() {
        Connection connection = null;
        try {
            //java程序从连接池取出连接,连接到MySQL数据库
            connection = ds.getConnection();
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
        return connection;
    }

    /**
     * 将connection对象放回连接池
     */
    public static void close(ResultSet resultSet, Statement statement, Connection connection) {
        try {
            if (resultSet != null) {
                resultSet.close();
            }
            if (statement != null) {
                statement.close();
            }
            if (connection != null) {
                connection.close();
            }
        } catch (SQLException throwable) {
            System.out.println(throwable.getMessage());
        }
    }
}
Dao

/**
 * 开发BasicDao,为其他Dao的父类
 */
public class BasicDao<T> {
    QueryRunner queryRunner = new QueryRunner();

    /**
     * 开发通用的dml方法,针对任意的表
     *
     * @param sql        SQL操作
     * @param parameters 可变参数
     * @return SQL操作执行成功受影响的行
     */
    public int update(String sql, Object... parameters) {
        Connection connection = null;
        try {
            connection = JdbcUtilsByDruid.getConnection();
            int update = queryRunner.update(connection, sql, parameters);
            return update;
        } catch (Exception exception) {
            throw new RuntimeException(exception);
        } finally {
            JdbcUtilsByDruid.close(null, null, connection);
        }
    }


    /**
     * 返回多个对象(多行记录),针对任意表
     *
     * @param sql        SQL语句
     * @param tClass     Class类的字节码对象
     * @param parameters 可变形参
     * @return ArrayList集合
     */
    public List<T> queryMulti(String sql, Class<T> tClass, Object... parameters) {
        Connection connection = null;
        try {
            connection = JdbcUtilsByDruid.getConnection();
            return queryRunner.query(connection, sql, new BeanListHandler<>(tClass), parameters);
        } catch (Exception exception) {
            throw new RuntimeException(exception);
        } finally {
            JdbcUtilsByDruid.close(null, null, connection);
        }
    }


    /**
     * 返回单个对象(单行记录),针对任意表
     *
     * @param sql        SQL操作
     * @param tClass     Class类的字节码对象
     * @param parameters 可变形参
     * @return T类对象实例
     */
    public T querySingle(String sql, Class<T> tClass, Object... parameters) {
        Connection connection = null;
        try {
            connection = JdbcUtilsByDruid.getConnection();
            return queryRunner.query(connection, sql, new BeanHandler<>(tClass), parameters);
        } catch (Exception exception) {
            throw new RuntimeException(exception);
        } finally {
            JdbcUtilsByDruid.close(null, null, connection);
        }
    }


    /**
     * 返回单行单列的值
     * @param sql SQL操作
     * @param parameters 可变形参
     * @return
     */
    public Object queryScalar(String sql, Object... parameters) {
        Connection connection = null;
        try {
            connection = JdbcUtilsByDruid.getConnection();
            return queryRunner.query(connection, sql, new ScalarHandler<>(), parameters);
        } catch (Exception exception) {
            throw new RuntimeException(exception);
        } finally {
            JdbcUtilsByDruid.close(null, null, connection);
        }
    }
}
public class AdminDao extends BasicDao<Admin>{
}
pojo

public class Admin {

    private int id;
    private String username;
    private String password;

    public Admin() { }

    public Admin(int id, String username, String password) {
        this.id = id;
        this.username = username;
        this.password = password;
    }

    public int getId() {
        return id;
    }
    public void setId(int id) {
        this.id = id;
    }
    public String getUsername() {
        return username;
    }
    public void setUsername(String username) {
        this.username = username;
    }
    public String getPassword() {
        return password;
    }
    public void setPassword(String password) {
        this.password = password;
    }

    @Override
    public String toString() {
        return "jxs.DBUtils.Admin{" +
                "id=" + id +
                ", username='" + username + '\'' +
                ", password='" + password + '\'' +
                '}';
    }
}
TestDao

public class TestDao {
    @Test
    public void testAdminDao() {
        AdminDao adminDao = new AdminDao();

        //查询多行记录
        String sql1 = "select * from admin where id >= ?";
        List<Admin> admins = adminDao.queryMulti(sql1, Admin.class, 1);
        for (Admin admin : admins) {
            System.out.println(admin);
        }

        //查询单行记录
        String sql2 = "select * from admin where id >= ?";
        Admin admin1 = adminDao.querySingle(sql2, Admin.class, 1);
        System.out.println(admin1);

        //查询单行单列
        String sql3 = "select * from admin where id >= ?";
        Object o = adminDao.queryScalar(sql3, 1);
        System.out.println(o);

        //dml操作
        String sql4 = "insert into admin values (6,'刘中珍','123')";
        int update = adminDao.update(sql4);
        System.out.println(update);
    }
}
1.3.5、正则表达式
快速入门
正则表达式基本语法
三个常用类
分组、捕获、反向引用
元字符
应用实例
1.3.6、Java8 Java11新特性
Java8新特性
Java11新特性
数据结构与算法
数据结构和算法概述
为何学习数据结构
数据结构与算法介绍
数据结构与算法概述
线性结构与非线性结构
栈
栈的介绍
栈的应用场景
栈的入门
计算器案例实现
链表
链表介绍
单链表介绍
单链表应用
双向链表应用
单项环形链表场景
单项环形链表介绍
稀疏数组和队列
稀疏数组介绍
案例需求
稀疏数组需求分析
稀疏数组需求实现
队列介绍
数组模拟队列应用
递归
递归介绍
递归可解决的问题
递归规则
递归需求案例
排序算法
基数排序
冒泡排序
快速排序
插入排序
选择排序
希尔排序
归并排序
查询算法
线性查找算法
二分查找算法
插值查找算法
斐波那契算法
哈希表
哈希表介绍
哈希表原理
哈希表应用
树
二叉树介绍
二叉树应用案例
二叉树查询结点
二叉树删除结点
顺序存储二叉树介绍
顺序存储二叉树遍历
线索化二叉树
线索化二叉树案例
树结构应用
赫夫曼编码原理
赫夫曼编码数据压缩
赫夫曼编码数据解压
赫夫曼编码文件压缩
赫夫曼编码文件解压
平衡二叉树分析
单旋转即左旋转
单旋转即右旋转
双旋转
多路查询树
二叉树与B树
多叉树
B树介绍
树的应用场景
B树、B+树、B*树
图
图介绍
图常用概念
邻接矩阵
邻接表
图案例实现
图的深度优先
深度优先遍历基本思想
深度优先遍历算法步骤
深度优先算法需求实现
图广度优先基本思想
图广度优先算法分析
图广度优先遍历实现
图深度优先对比广度优先
常用10种算法
二分查找算法
分治算法
动态规划算法
KMP算法
贪心算法
普里姆算法
克鲁斯卡尔算法
迪杰斯特拉算法
JavaWeb
HTML
系统结构
1、B/S、C/S架构

(1)B/S架构:Browser/Server(浏览器/服务器交互形式)
	1.1、Browser端支持HTML、CSS、JavaScript,写HTML、CSS、JavaScript代码的为Web前端开发工程师,Server端支持C、C++、Java、Python...
	1.2、B/S架构系统优缺点:优点:升级更新方便,只需升级服务端,维护成本低;缺点:速度慢、体验差、界面不炫酷
	1.3、企业内部采用B/S架构的系统,只需做数据的增删改查,维护成本低。
	1.4、B/S架构代表:京东、百度、天猫...

(2)C/S架构:Client/Server(客户端/服务器交互形式)
	2.1、C/S架构系统优缺点:优点:速度快、体验好、界面炫酷;缺点:升级更新繁琐,每一客户端都需升级维护
	2.2、C/S架构代表:QQ、微信...
	2.3、娱乐型的系统多数采用C/S架构
HTML概述
1、何为HTML？

(1)HTML:Hyper Text Markup Language(超文本标记语言),由大量标签组成,每一个标签都有开始标签、结束标签
<标签>
    <标签>
        <标签 属性名="属性值" 属性名="属性值"></标签>
    </标签>
</标签>
(2)超文本:图片、声音、视频...
2、如何开发HTML？

(1)使用文本编辑器开发,创建文件的扩展名为.html或.htm
(2)html集成开发工具:HBuilderX、Dreamweaver...
3、如何运行HTML？

(1)使用浏览器打开即运行
4、谁制定HTML？

(1)W3C:世界万维网联盟(World Wide Web Consortium)
(2)W3C制定了HTML规范,每一浏览器厂家都遵守规范,HTML程序员按照规范编写代码
(3)HTML规范目前最高版本为HTML5.0,简称H5
5、w3school、w3cschool

(1)为方便中国JavaWeb前端程序员的开发,提供了大量的帮助文档,为开发提供方便。
(2)w3school官方网址:https://www.w3school.com.cn/
第一个HTML（重要！！）
<!-- HTML不区分大小写,语法松散不严格 -->
<!-- 加入<!DOCTYPE HTML>则表示为HTML5语法,省略则表示为HTML4.0 -->
<!DOCTYPE HTML>
<!-- 根节点 -->
<html>
	<!-- 网页头部 -->
	<head>
		<!-- 网页标题 -->
		<title>第一个HTML页面</title>
	</head>
	<!-- 网页主体 -->
	<body>
		欢迎学习HTML
	</body>
</html>
基本标签
1、基本介绍

(1)段落标记:<p></p>
(2)标题字:<h1></h1>...<h6></h6>
(3)换行:<br>
(4)横线:<hr>
(5)预留格式:<pre></pre>
(6)删除字:<del></del>
(7)插入字:<ins></ins>
(8)粗体字:<b></b>
(9)斜体字:<i></i>
(10)右上角加字:<sup></sup>
(11)右下角加字:<sub></sub>
(12)字体标签:<font></font>
2、案例演示

<!DOCTYPE HTML>
<html>
	<!-- 网页头部 -->
	<head>
		<title>HTML基本标签</title>
	</head>
	
	<!-- 网页主体 -->
	<body>
		<!-- 段落标记 -->
		<p>W3C 指万维网联盟（World Wide Web Consortium）</p>
		<p>W3C 创建于1994年10月</p>
		<p>W3C 由 Tim Berners-Lee 创建</p>
		
		<!-- 标题字,为HTML中预留格式-->
		<h1>标题字</h1>
		<h2>标题字</h2>
		<h3>标题字</h3>
		<h4>标题字</h4>
		<h5>标题字</h5>
		<h6>标题字</h6>
		
		<!-- 换行,独目标记 -->
		hello<br>hello
		
		<!-- 横线,独目标记 -->
		<!-- color、width为hr标签属性 -->
		<hr color="red" width="50%">
		
		<!-- 预留格式 -->
		<pre>
			for(int i = 0;i < 10;i++) {
				System.out.println("i = " + i);
			}
		</pre>
		
		<del>删除字</del>
		<ins>插入字</ins>
		<b>粗体字</b>
		<i>斜体字</i>
		<!-- 右上角加字 -->
		10<sup>2</sup>
		<!-- 右下角加字 -->
		10<sub>m</sub>
		<!-- 字体标签 -->
		<font color="red" size="10">字体标签</font>
	</body>
</html>
实体符号
1、基本介绍

(1)<:&lt;
(2)>:&gt;
(3)=:&nbsp;
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>实体符号</title>
	</head>
	<body>
		<!-- 
		实体符号以&开头,以;结尾
		&lt;为<
		&gt;为>
		 -->
		10 &lt; 20
		100 &gt; 90
		
		<!-- 空格&nbsp; -->
		a&nbsp;b&nbsp;c&nbsp;d
	</body>
</html>
表格（重要！！）
1、基本介绍

(1)表格:<table></table>
(2)行:<tr></tr>
(3)单元格:<td></td>
(4)表头:<th></th>
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>表格</title>
	</head>
	<body>
		<center><h2>南京理工大学紫金学院学生信息</h2></center>
		<hr color="black" align="center">
		<!-- 
		border="1px":设置表格边框为1像素
		width="300px":设置表格宽度为300像素
		height="150px":设置表格高度为150像素
		align="center":设置表格对齐方式为居中
		 -->
		<table border="1px" width="300px" height="150px" align="center">
			<!-- 
			tr:table row
			td:table data cell
			 -->
			<tr>
				<td>姓名</td>
				<td>班级</td>
				<td>年级</td>
			</tr>
			<tr>
				<td>蒋兴树</td>
				<td>软件工程嵌入式(2)班</td>
				<td>19级</td>
			</tr>
		</table>
	</body>
</html>
3、单元格合并

(1)行合并:假设将第1行第3个单元格、第2行第3个单元格进行合并,删除第2行第3个单元格,在第1行第3个单元格加上属性rowspan="2"
(2)列合并:假设将第2行第1列、第2行第2列进行合并,删除第2行第1列、第2行第2列单元格其中之一,在单元格加上属性colspan="2"
4、单元格合并、th标签案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>单元格合并、th标签</title>
	</head>
	<body>
		<table border="1px" align="center" width="300px" height="150px">
			<tr>
				<!-- 
				th标签为单元格标签
				th标签相比td标签多居中、加粗特性
				 -->
				<th>姓名</th>
				<td>班级</td>
				<td>年级</td>
			</tr>
			<tr>
				<td colspan="2">蒋兴树软件工程2班</td>
				<td rowspan="2">19级</td>
			</tr>
			<tr>
				<td>丁维一</td>
				<td>软件工程2班</td>
			</tr>
		</table>
	</body>
</html>
5、thead、tbody、tfoot标签案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>thead、tbody、tfoot不是必须的,但便于后期编写JS代码</title>
	</head>
	<body>
		<table align="center" border="1px" width="300px" heigth="150px">
			<!-- 头 -->
			<thead>
				<th>姓名</th>
				<th>班级</th>
				<th>年级</th>
			</thead>
			<!-- 体 -->
			<tbody>
				<tr>
					<td>蒋兴树</td>
					<td>软嵌2班</td>
					<td>19级</td>
				</tr>
			</tbody>
			<!-- 脚 -->
			<tfoot>
				<tr>
					<td>丁维一</td>
					<td>软嵌2班</td>
					<td>19级</td>
				</tr>
			</tfoot>
		</table>
	</body>
</html>
背景颜色、背景图片
1、基本介绍

(1)bgcolor标签:设置背景色
(2)background标签:设置背景图
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<!-- 
		浏览器采用"utf-8"字符集打开当前html文件
		并不是设置当前html文件字符集为"utf-8"
		 -->
		<meta charset="utf-8">
		<title>背景颜色、背景图片</title>
	</head>
	<!-- 
	bgcolor属性:设置页面主体背景色为red
	background属性:设置页面主体背景图片为image/枫原万叶.jpg
	 -->
	<body bgcolor="red" background="image/枫原万叶.jpg">
		
	</body>
</html>
图片（重要！！）
1、基本介绍

(1)img标签:图片标签
(2)src属性:图片路径
(3)title属性:鼠标悬停此图片时提示信息
(4)alt属性:图片加载失败时提示信息
(5)设置图片宽度、高度其一即可,设置宽度时高度会进行等比例缩放
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>图片</title>
	</head>
	<body>
		<!-- 
		img标签:图片标签
		src属性:图片路径
		设置图片宽度、高度时,设置其一即可
		设置宽度,高度会进行等比例缩放
		title属性:设置鼠标悬停时信息
		alt属性:设置图片加载失败提示信息
		 -->
		<img src="image/枫原万叶.jpg" width="500px" title="枫原万叶" alt="图片加载失败"/>
	</body>
</html>
超链接（重要！！）
1、基本介绍

(1)a标签:超链接、热链接。超链接、热链接特性:存在下划线;鼠标悬停在超链接上显示小手图标;点击超链接后跳转页面。
(2)href属性:hot references,热引用。href属性后为资源地址,可以为网络资源地址或本地资源地址
(3)target属性:存在4个值。
	_blank:点击超链接后打开新的窗口
	_self:点击超链接后覆盖当前窗口
	_top:点击超链接后返回顶级窗口
	_parent:点击超链接后返回父窗口
(4)超链接、热链接可以为文本超链接或图片超链接
(5)通过超链接,浏览器向服务器发送请求。浏览器向服务器发送请求(请求:request);服务器向浏览器发送数据(响应:response)
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>超链接 热链接</title>
	</head>
	<body>
		<!-- 
		a标签:超链接、热链接
		超链接特点:有下划线、鼠标悬停在超链接上显示小手形状、点击超链接后可跳转页面
		href属性:hot references,热引用
		href属性后为资源地址
		href属性后的资源地址可以为网络资源路径、本地资源路径
		 -->
		<a href="http://baidu.com">百度</a>
		<a href="007-背景颜色和背景图片.html">007</a>
		
		<!-- 
		图片超链接
		target属性:_blank:新窗口
				   _self:当前窗口
				   _top:顶级窗口
				   _parent:父窗口
		 -->
		<a href="http://www.jd.com" target="_blank">
			<img src="image/京东年货节主会场.jpg" height="120px"/>
		</a>
	</body>
</html>
列表
1、基本介绍

(1)无序列表<ul></ul>
(2)有序列表<ol></ol>
(3)无序列表中插入无序列表
<ul>
    <li>水果
        <ul>
            <li>苹果</li>
            <li>梨</li>
            <li>香蕉</li>
        </ul>
    </li>
</ul>
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>列表</title>
	</head>
	<body>
		<!-- 有序列表 -->
		<ul type="circle">
			<li>中国
			<ul type="square">
				<li>北京
				<ul type="disc">
					<li>海淀区</li>
					<li>朝阳区</li>
				</ul>
				</li>
				<li>天津</li>
				<li>深圳</li>
			</ul>
			</li>
			<li>美国</li>
			<li>日本</li>
		</ul>
		
		<!-- 有序列表 -->
		<ol type="1">
			<li>水果
			<ol type="A">
				<li>车厘子
				<ol type="a">
					<li>布鲁克斯</li>
					<li>桑提娜</li>
					<li>拉宾斯</li>
				</ol>
				</li>
				<li>榴莲</li>
				<li>晴王</li>
			</ol>
			</li>
			<li>蔬菜</li>
			<li>零食</li>
		</ol>
	</body>
</html>
表单（重中之重！！）
1、何为表单

<img src="E:\Study\自学课程资料\Java\assets\表单.png" style="zoom: 80%;" />

2、基本介绍

(1)form标签:表单
(2)表单作用:提交表单中的数据至服务器
(3)action属性:提交表单中的数据至哪台服务器,action属性与超链接中href属性一样,可以发送请求至服务器(例:<form action="192.168.111.3:8080/test/save"></form>,192.168.111.3:8080/test/save为请求路径,表单中的数据提交至192.168.111.3主机8080端口对应的软件)
(4)method属性:默认采用get方式提交表单中的数据
	get:提交表单中的数据会显示在浏览器地址栏
	post:提交表单中的数据不会显示在浏览器地址栏
	get和post提交数据的格式一致,只不过post方式提交表单中的数据不会显示在浏览器地址栏
(5)input标签:输入域,存在属性type、value
(6)type属性:
	text:文本框
	password:密码框
	checkbox:复选框,增加checked属性为默认选中
	radio:单选按钮,增加checked属性为默认选中
	button:普通按钮
	submit:提交按钮
(7)value属性:设置按钮上显示的文本
(8)submit提交按钮和普通超链接无太大区别,超链接、表单都可以向服务器发送请求,表单发送请求时可携带数据。
(9)submit、reset按钮应放置<form></form>标签内部才可提交、清空表单中的数据
(10)HTTP协议规定表单提交数据至服务器格式:action?name=value&name=value...
(11)若提交<input/>标签中的数据至服务器,则必须在<input/>标签中加入name属性,若不提交<input/>标签中的数据至服务器,不加入name属性即可。
(12)text、password,文本框以及密码框中的value属性不需程序员指定,用户在文本框、密码框输入的即为value。当value为空时,value默认值为空字符串"",会将空字符串提交至服务器。
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>表单form</title>
	</head>
	<body>
		<!-- 
		1、表单:form标签
		2、表单作用:提交表单中的数据至服务器
		3、action属性:提交表单中的数据至哪台服务器
		-->
		<form action="192.168.111.3:8080/test/save">
			<!-- 按钮,type="submit"时表示该按钮为提交按钮,可提交表单中的数据 -->
			<input type="submit" value="注册"/>
			<!-- 普通按钮,不可提交表单中数据 -->
			<input type="button" value="设置按钮上显示的文本"/>
			<!-- 文本框 -->
			<input type="text"/>
			<!-- 密码框 -->
			<input type="password"/>
			<!-- 复选框 -->
			<input type="checkbox"/>
			<!-- 单选按钮 -->
			<input type="radio"/>
		</form>
		
		<form action="http://www.baidu.com">
			<!-- 
			此按钮和普通超链接无太大区别
			超链接、表单都可以向服务器发送请求
			表单发送请求时可携带数据
			 -->
			<input type="submit" value="百度"/>
		</form>
		
		<form action="http://localhost:8080/test/login">
			用户名<input type="text"/><br>
			密码<input type="password"/><br>
			<input type="submit" value="注册"/>
		</form>
		
		<!-- 表单以action?name=value&name=value...格式提交数据至服务器 -->
		<form action="http://localhost:8080/test/login">
			<table>
				<tr>
					<td>用户名</td>
					<!-- 若提交<input/>标签中的数据至服务器,则必须在<input/>标签中加入name属性 -->
					<td><input type="text" name="username"/></td>
				</tr>
				<tr>
					<td>密码</td>
					<td><input type="password" name="userpassword"/></td>
				</tr>
				<tr>
					<td colspan="2" align="center">
						<!-- submit、reset按钮应放置<form></form>标签内部 -->
						<input type="submit" value="登录"/>
						&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
						<input type="reset" value="清空"/>
					</td>
				</tr>
			</table>
		</form>
		
	</body>
</html>
4、用户注册表单的实现

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>用户注册表单</title>
	</head>
	<body>
		<!-- 
		用户注册:
		用户名
		密码
		确认密码
		性别
		兴趣爱好
		学历
		个人简介
		 -->
		 
		<!-- 
		form表单method属性,默认采用get方式提交表单中的数据
		get:采用get方式提交时,用户提交的表单中的数据会显示在浏览器地址栏
		post:采用post方式提交时,用户提交的表单中的数据不会显示在浏览器地址栏
		post提交的数据格式与get一致,只不过不将表单中的数据显示在浏览器地址栏
		 -->
		<form action="http://localhost:8080/test/regist" method="post">
			<table>
				<tr>
					<td>用户名</td>
					<td><input type="text" name="username" /></td>
				</tr>
				<tr>
					<td>密码</td>
					<td><input type="password" name="userpassword" /></td>
				</tr>
				<tr>
					<td>确认密码</td>
					<td><input type="password" /></td>
				</tr>
				<tr>
					<td>性别</td>
					<td>
						<!-- 单选按钮value必须手动指定,checked为默认选中 -->
						<input type="radio" name="gender" value="1" checked>男
						&nbsp;
						<input type="radio" name="gender" value="0" />女
					</td>
				</tr>
				<tr>
					<td>兴趣爱好</td>
					<td>
						<input type="checkbox" name="hobby" value="smoke" />抽烟
						&nbsp;
						<input type="checkbox" name="hobby" value="drink" />喝酒
						&nbsp;
						<input type="checkbox" name="hobby" value="perm" />烫头
					</td>
				</tr>
				<tr>
					<td>学历</td>
					<td>
						<select name="学历">
							<!-- selected为默认选中 -->
							<option value="xx">小学</option>
							<option value="cz">初中</option>
							<option value="gz">高中</option>
							<option value="zk">专科</option>
							<option value="bk" selected>本科</option>
							<option value="ss">硕士</option>
							<option value="bs">博士</option>
						</select>
					</td>
				</tr>
				<tr>
					<td>个人简介</td>
					<td>
						<!-- 
						<textarea></textarea>标签:文本域
						文本域不存在value属性,用户填写的内容即value
						-->
						<textarea rows="10" clos="60" name="introduce"></textarea>
					</td>
				</tr>
				<tr>
					<td align="center"><input type="submit" value="注册"/></td>
					<td align="center"><input type="reset" value="清空"/></td>
				</tr>
			</table>
		</form>
		
		<!-- 
		输出格式
		http://localhost:8080/test/regist?username=jxs&userpassword=123&gender=1&hobby=smoke&hobby=drink&hobby=perm&%E5%AD%A6%E5%8E%86=bk&introduce=jxs%E5%A4%A7%E5%B8%85%E5%93%A5 
		-->
	</body>
</html>
5、下拉列表支持多选

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>下拉列表</title>
	</head>
	<body>
		<!-- 
		multiple="multiple":支持多选,按住Ctrl键支持多选
		size属性:设置显示条目数量
		-->
		<select multiple="multiple" size="2">
			<option>篮球</option>
			<option>蔡徐坤</option>
			<option>鸡</option>
			<option>两年半</option>
		</select>
	</body>
</html>
6、file控件

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>file控件</title>
	</head>
	<body>
		<!-- file控件,上传文件 -->
		<input type="file"/>
	</body>
</html>
7、hidden控件

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>hidden控件</title>
	</head>
	<body>
		<form action="http://localhost:8080/test/save">
			<!-- hidden:隐藏域,隐藏在网页中的显示,提交表单中的数据时会自动提交至服务器 -->
			<input type="hidden" name="userid" value="1"/>
			用户代码<input type="text" name="usercode"/>
			<input type="submit" name="提交"/>
		</form>
	</body>
</html>
8、readonly与disabled

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<form action="http:localhost:8080/test/save">
			<!-- 
			readonly、disabled相同点:只读不可修改
			readonly可提交数据至服务器,disabled不可提交数据至服务器
			-->
			用户代码<input type="text" name="usercode" value="1" readonly/>
			用户姓名<input type="text" name="username" value="jxs" disabled/>
			<input type="submit" value="提交"/>
		</form>
	</body>
</html>
9、input控件maxlength

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		maxlength属性:设置文本框中可输入的字符数量
		<input type="text" maxlength="3"/>
	</body>
</html>
HTML中元素id属性（重要！！）
1、基本介绍

(1)HTML文档中每一元素都存在id属性,id属性为每一元素的唯一标识(id属性相当于元素的身份证号),同一HTML文档中id属性不可重复
(2)id属性作用:通过id属性更易获取元素
(3)javascript可以对HTML文档中任意元素进行增删改操作,进行增删改操作之前需通过id属性获取元素
(4)HTML文档相当于一棵树,树上存在众多元素,每一元素都存在唯一id
(5)javascript主要对DOM树上的元素进行增删改操作
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 
		1.HTML文档中,任何元素(节点)都存在id属性
		2.id属性为每一元素的唯一标识(id属性相当于元素的身份证号)
		3.同一HTML文档中id属性不可重复
		4.id属性作用:通过id属性更易的获取元素(节点)。
		5.javascript可以对HTML文档中的任意元素进行增删改操作,对元素进行增删改之前需通过id属性获取元素
		6.HTML文档相当于一棵树,树上存在众多节点(元素),每一节点都存在唯一id
		7.javascript主要对DOM树上的元素进行增删改操作
		-->
		<form id="myform">
			<input type="text" id="username" name="username"/>
			<input type="password" id="userpassword" name="userpassword"/>
		</form>
	</body>
</html>
3、DOM树图解

![](E:\Study\自学课程资料\Java\assets\DOM树图解.png)

div和span（重要！！）
1、基本介绍

(1)何为div、span:div、sapn为图层
(2)图层作用:保证页面布局灵活,图层即1个盒子。div嵌套div,即盒子套盒子
(3)div、span可以通过定下左上角x轴、y轴坐标实现定位
(4)最初布局时采用table进行布局,但table不灵活。现代的网页开发div布局使用广泛
(5)div、span区别:div默认情况下独自占用1行;span不独自占用一行
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 
		1.何为div、span?有何用？
		div、span:图层
		图层作用:保证页面可灵活布局
		图层即一个盒子,div嵌套div即盒子套盒子
		div和span可以定位,只需定下div左上角的x轴、y轴坐标即可
		2.最初布局时采用table进行布局,但table不灵活。现代的网页开发div布局使用广泛
		3.div、span区别
		div默认情况下独自占用1行;span不独自占用一行
		-->
		<div id="div1">
			DIV
		</div>
		<div id="div2">
			DIV
		</div>
		<span id="span1">
			SPAN
		</span>
		<span id="span2">
			SPAN
		</span>
		<div id="div3">
			<div id="div4">DIV</div>
		</div>
	</body>
</html>
CSS
CSS作用
1、基本介绍

(1)CSS(Cascading Style Sheet):层叠样式表语言
(2)CSS作用:修饰HTML页面,设置HTML页面中某些元素的样式,让HTML页面更好看。
(3)CSS好比HTML的化妆品。HTML为主体,CSS的存在就是修饰HTML。新建的文件还为html文件。
2、CSS掌握程度

(1)可书写常见的CSS样式
(2)可看懂别人的CSS样式
HTML中嵌入CSS样式的三种方式（重中之重！！）
内联定义（Inline Styles）
1、基本介绍

(1)内联定义:使用元素style属性定义适用其的样式表属性
2、语法

<标签 style="样式名:样式值;样式名:样式值;..."></标签>
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>内联定义</title>
	</head>
	<body>
		<!-- 
		width 宽度样式
		heigth 高度样式
		background-color 背景颜色样式
		display 布局样式(none表示隐藏,block表示显示)
		border-color 边框颜色样式
		border-weight 边框宽度样式
		border-style 边框风格样式
		-->
		<div style="width: 300px;height: 300px;background-color: lightgreen;display: block;
		border-color: black;border-width: 1px;border-style: solid;"></div>
		
		<!-- 边框样式还可如此定义border: 1px solid black -->
		<div style="width: 300px;height: 300px;background-color: lightgreen;display: block;
		border: 1px solid black;"></div>
	</body>
</html>
定义内部样式块对象（Embedding a Style Block）
1、基本介绍

(1)HTML文档的<head></head>标签中插入<style></style>标签
2、语法

<html>
    <head>
        <title>文档标题</title>
        <!-- style元素type属性设置为"text/css",允许不支持这类型的浏览器忽略样式表单 -->
        <style type="text/css">
            选择器 {
                样式名:样式值;
                样式名:样式值;
                ...
            }
            选择器 {
                样式名:样式值;
                样式名:样式值;
                ...
            }
        </style>
    </head>
    <body>  
    </body>
</html>
3、选择器

(1)id选择器:#id{样式名:样式值...}
(2)标签选择器:标签名{样式名:样式值...}
(3)类选择器:.类名{样式名:样式值...}
4、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>样式块</title>
		<style type="text/css">
			/* 
			id选择器
			语法格式:#id名{样式名:样式值;样式名:样式值...}
			*/
			#p1 {
				color: red;
				font-size: 1px;
			}
			
			/* 
			标签选择器
			语法格式:标签名{样式名:样式值;样式名:样式值...}
			标签选择器作用范围大于id选择器作用范围
			*/
			div {
				background-color: black;
				border: 1px solid red;
				width: 100px;
				height: 100px;
			}
			
			/* 
			类选择器 
			语法格式:.类名{样式名:样式值;样式名:样式值...}
			*/
		   .myclass {
			   border: 1px solid red;
			   width: 200px;
			   height: 20px;
		   }
		</style>
	</head>
	<body>
		设置字体颜色为红色,设置字体大小为1px
		<p id="p1">蒋兴树</p>
		<p id="p2">丁维一</p>
		
		<div></div>
		<div></div>
		
		设置文本框、下拉框
		<input type="text" class="myclass"/>
		<select class="myclass">
			<option>专科</option>
			<option>本科</option>
		</select>
	</body>
</html>
链入外部样式表文件（Linking to a Style Sheet）
1、基本介绍

(1)建立外部样式表文件(.css),再使用HTML的link标签
2、语法

<html>
    <head>
        <title></title>
        <link type="text/css" rel="stylesheet" href="css文件路径"/>
    </head>
    <body>
        
    </body>
</html>
3、优点

(1)这种方式最常用
(2)易维护,维护成本低
(3)假设html1文件、html2文件、html3文件使用<link/>标签引入css文件,维护时只需编辑css文件即可。
4、案例演示

css文件

/* 标签选择器 */
a {
	/* 
	text-decoration属性用于设置和删除文本装饰
	text-decoration: none常用于超链接中删除下划线 
	cursor属性用于设置鼠标样式
	*/
	text-decoration: none;
	cursor: pointer;
}
html文件

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<!-- 引入css -->
		<link type="text/css" rel="stylesheet" href="css_code/01.css"/>
	</head>
	<body>
		<a href="http://www.baidu.com">百度</a>
	</body>
</html>
列表样式
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>列表样式</title>
		<style type="text/css">
			ul {
				list-style-type: none;
			}
		</style>
	</head>
	<body>
		<ul>
			<li>中国
				<ul>
					<li>南京</li>
					<li>北京</li>
					<li>上海</li>
					<li>广州</li>
				</ul>
			</li>
			<li>美国</li>
			<li>俄国</li>
		</ul>
	</body>
</html>
绝对定位
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>绝对定位</title>
		<style type="text/css">
			#div1 {
				background-color: black;
				border: 1px solid red;
				width: 300px;
				height: 300px;
				/* 绝对定位 */
				position: absolute;
				left: 100px;
				top: 100px;
			}
		</style>
	</head>
	<body>
		<div id="div1"></div>
	</body>
</html>
JavaScript
JavaScript概述（重中之重！！）
1、何为JavaScript？

(1)JavaScript,简称JS,是网景公司(NetScape)的布兰登艾奇开发的,最初叫做LiveScript。因SUN公司与网景公司曾经存在合作关系,SUN公司将LiveScript修改为JavaScript。
(2)网景公司最著名的就是Navigator浏览器。LiveScript是为Navigator浏览器量身定制的一门语言,不支持其他浏览器。当Navigator浏览器使用广泛时,微软研发出只支持IE浏览器的脚本语言:JScript。JavaScript和JScript并存的时代,程序员极其痛苦,因为程序员需编写两套程序。在此情况下,有一非营利性组织ECMA根据JavaScript制定了ECMA-262号标准,叫做ECMA-Script,JavaScript与JScript都实现了ECMA-Script规范,即JavaScript和JScript统一。
(3)JavaScript为事件驱动型编程语言,依靠事件驱动,执行相应程序。每一事件对应一个事件句柄(例:若事件为click,事件句柄为onclick),事件句柄作为html标签中的属性而存在。
(4)事件句柄JavaScript代码执行原理:页面打开时,事件句柄JavaScript代码并不会执行。只是将事件句柄JavaScript代码注册到按钮事件句柄对应的事件上,若按钮发生事件后,事件句柄JavaScript代码会被浏览器自动调用。
2、JavaScript作用

(1)JavaScript是运行在浏览器上的脚本语言
(2)JavaScript的出现是浏览器更加生动形象,不再为单纯的静态页面,而让页面更具交互性。
(3)JavaScript可以改变HTML内容、可以改变HTML属性、可以改变HTML样式、可以隐藏HTML元素、可以显示HTML元素
3、Java与JavaScript区别

(1)JavaScript名字中虽然存在"Java",但和Java没有关系,只是语法上有类似之处。
(2)JavaScript与Java运行位置不同,Java运行于JVM虚拟机中,JavaScript运行于浏览器内存中。
(3)Java的"目标程序"以class形式保存,class文件不可使用文本编辑器打开,不是"脚本语言";JavaScript的"目标程序"以普通文本形式保存,称为"脚本语言"
(4)JavaScript程序不需程序员手动编译,编写完代码后可用浏览器直接打开解释执行。
4、JS与JSP区别

(1)JS:JavaScript,运行在浏览器上
(2)JSP:JavaServer Pages,隶属于Java语言,运行在JVM虚拟机上。
5、JS鼠标事件

鼠标事件	说明
click	单击鼠标
dblclick	双击鼠标
mouseover	鼠标移入
mouseout	鼠标移出
mousemove	鼠标移动
mousedown	鼠标按下
mouseup	鼠标松开
嵌入JS三种方式（重中之重！！）
方式一：事件句柄
1、如何使用JS代码弹出消息框

(1)JS中有一内置对象window
(2)window为浏览器对象
(3)浏览器对象有一函数alert
(4)事件句柄="window.alert('消息')"或者事件句柄='window.alert("消息")'
2、事件句柄案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 
		实现功能:用户点击按钮弹出消息框
		1.JS是事件驱动型编程语言,依靠事件去驱动,执行相应程序。
		  每一事件都对应一个事件句柄,事件句柄即事件前添加on
		  事件句柄作为html标签中的属性而存在
		2.onclick="JS代码"执行原理:页面打开时,JS代码并不会执行,只是将JS代码注册到按钮的click事件上
		  若此按钮发生click事件后,注册在onclick后的JS代码会被浏览器自动调用
		3.如何使用JS代码弹出消息框:
		  JS中有一内置的对象叫做window,window代表浏览器对象,window对象有一函数叫做:alert
		  用法:window.alert("消息"),这样就可以实现弹窗。window可以省略。
		4.JavaScript中的字符串可以使用双引号,也可以使用单引号。
		5.JavaScript的一条语句结束之后可以使用分号";",也可以不使用
		-->
		<input type="button" value="普通按钮" onclick="window.alert('Hello,JavaScript')"/>
	</body>
</html>
方式二：脚本块
1、脚本块基本概念

(1)脚本块语法:<script type="text/javascript"></script>
(2)脚本块在html中出现次数、出现位置无要求
(3)JavaScript单行注释//,JavaScript多行注释/**/
2、脚本块案例演示

<!-- script脚本块在html文档中出现次数、出现位置无要求 -->
<script type="text/javascript">
	window.alert("first");
</script>

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		
		<script type="text/javascript">
			window.alert("head");
		</script>
		
	</head>
	<body>
		
		<input type="button" value="按钮1"/>
		
		<!-- 脚本块 -->
		<script type="text/javascript">
			// 脚本块中的程序在页面打开时按照自上而下的顺序逐行执行
			window.alert("body");
		</script>
		
		<input type="button" value="按钮2"/>
		
	</body>
</html>

<script type="text/javascript">
	window.alert("last");
</script>
方式三：引入外部js文件
1、基本介绍

(1)建立外部JavaScript文件(.js),再使用script标签中的src属性引入js文件
2、引入外部js文件案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 
		需要位置引入js脚本文件
		引入外部js文件时,js文件中的代码会遵循自上而下的顺序依次逐行执行
		-->
		<script type="text/javascript" src="javascript_code/001-js.js">
			// window.alert("Hello JXS");代码不会执行
		</script>
		
		<!-- 脚本块 -->
		<script type="text/javascript">
			window.alert("Hello JXS");
		</script>
		
		<!-- 
		这种方式不可以,必须存在结束的script标签
		<script type="text/javascript" src="javascript_code/001-js.js"/> 
		-->
	</body>
</html>
3、细节整理

(1)通过script标签中的src属性引入外部js文件时,script标签中的代码不会执行。
(2)通过script标签中的src属性引入外部js文件时,必须存在结束的script标签,即</script>
(3)html文件中引入js文件的同时,可以再加入脚本块。
HTML中嵌入CSS与JavaScript对比（重中之重！！）
(1)
HTML中嵌入CSS方式一:标签中添加style属性,style="样式名:样式值;样式名:样式值..."
HTML中嵌入JavaScript方式一:标签中添加事件句柄,事件句柄="JavaScript代码"

(2)
HTML中嵌入CSS方式二:样式块中定义id选择器或标签选择器或类选择器,<style type="text/css">#id/标签名/.类名{样式名:样式值;样式名:样式值...}</style>
HTML中嵌入JavaScript方式二:脚本块,<script type="text/javascript"></script>

(3)
HTML中嵌入CSS方式三:通过HTML的link标签引入css文件(常用！)
HTML中嵌入JavaScript方式三:通过script标签中的src属性引入js文件(常用！)
标识符和关键字
1、何为标识符？

Java语言中,标识符常用来给类、对象、变量、方法、接口、自定义数据类型等命名
2、Java中标识符命名规则和命名规范

(1)命名规则:由大小写字母(a-z、A-Z)、数字(0-9)、下划线(_)、美元符号($)组成,不可以数字(0-9)开头。标识符区别大小写。标识符无长度限制。不可将Java关键字作为标识符。

(2)命名规范:
包名:字母全部小写
类名、接口名:每一单词首字母大写,其余小写
常量名:字母全部大写,单词间以下划线(_)连接
变量名、方法名:第一个单词首字母小写,从第二个单词起首字母大写,其余小写。驼峰命名法。
变量（重中之重！！）
变量的声明与赋值
1、Java中变量与JavaScript中变量对比

Java中变量
(1)如何定义变量:数据类型 变量名;
(2)变量如何赋值:变量名 = 值,"="运算符右边先执行,将右边执行的结果赋值给左边的变量
(3)Java为强类型语言,假设有代码int i,Java在编译阶段已确定变量i的数据类型为int类型,则此变量从定义到最终内存释放都为int类型,不可变为其他数据类型。

JavaScript中变量
(1)如何定义变量:var 变量名;(var-variable)
(2)变量如何赋值:变量名 = 值;
(3)JavaScript为弱类型语言,一个变量可随意赋值,值的数据类型随意。
2、变量案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			// JavaScript中若一个变量没有手动赋值,则系统默认为undefined
			var i;
			// undefined在JavaScript为一具体存在的值
			window.alert(i);
			// 若没有定义变量直接访问则出现age is not defined(未定义age)
			// window.alert(age);

			// a,b默认赋值undefined;将200赋值给c
			var a, b, c = 200;
			window.alert(a);
			window.alert(b);
			window.alert(c);
			// JavaScript为弱类型语言,可将任意数据类型的值赋值给变量
			a = false;
			window.alert(a);
			a = "abc";
			window.alert(a);
			a = 1.2;
			window.alert(a);
			
		</script>
	</body>
</html>
3、变量注意事项

(1)若定义1个变量,没有进行手动赋值,则系统默认为undefined
(2)若没有定义1个变量,直接进行访问,则出现XXX is not defined
(3)JavaScript为弱类型语言,可将任意数据类型的值赋值给变量
函数的定义与调用
1、基本介绍

(1)JavaScript中的函数相当于Java中的方法
(2)JavaScript中的函数为一段可重复利用的代码片段
(3)JavaScript中的函数可完成某个特定功能
(4)函数语法格式:function 函数名(参数列表) {函数体}或函数名 = function(参数列表) {函数体}
(5)函数中不需指定返回值类型,因为JavaScript中可以将任意数据类型的值赋给变量
(6)Java中重载(两同三不同,同一个类同一方法名,参数列表中参数顺序、参数数据类型、参数个数不同),JavaScript中不存在重载,若重载则函数名相同,JavaScript中函数名不可重复,若函数名相同,后声明的函数会覆盖先声明的函数。
2、函数的定义与调用案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			JS中的函数:
			(1)JavaScript中的函数相当于Java中的方法
			(2)函数为一段可重复利用的代码片段
			(3)函数一般可完成某个特定功能
			
			JS中定义函数
			(1)语法格式:
			第一种方式:function 函数名(参数列表){函数体;}
			第二种方式:函数名 = function(参数列表){函数体};
			(2)JS中的函数不需指定返回值类型
			   因为JavaScript中可以将任意数据类型的值赋给变量,返回任何数据类型都可以。
			*/
			function sum(a, b) {
				return a + b;
			}
			var resultValue1 = sum(10, 20);
			// 30
			window.alert(resultValue1);

			var resultValue2 = sum(10);
			// NaN
			window.alert(resultValue2);

			var resultValue3 = sum("JXS");
			// 将JXS赋值给a,b系统默认为undefined
			window.alert(resultValue3);

			var resultValue4 = sum();
			// NaN:Not a Number
			window.alert(resultValue4);

			var resultValue5 = sum(1, 2, 3);
			// 3
			window.alert(resultValue5)

			sayHello = function(username) {
				alert("Hello," + username);
			}
			// 调用函数
			sayHello("JXS");
			
			function test(username) {
				window.alert("第一个test函数");
			}
			
			function test() {
				window.alert("第二个test函数");
			}
			
			/*
			调用函数,输出"第二个test函数"
			JavaScript中,函数名不可重复,当函数重名时,后声明的函数会覆盖先声明的函数
			*/
			test("JXS");
		</script>

		<input type="button" value="Hello" ondblclick="sayHello('DWY')" />
		<input type="button" value="求和" onclick="sum(10,20)" />
	</body>
</html>
局部变量与全局变量
1、基本介绍

(1)全局变量:函数体外声明的变量属于全局变量
(2)局部变量:函数体内声明的变量以及函数的形参属于局部变量
(3)全局变量生命周期:浏览器打开时声明,浏览器关闭时销毁
(4)局部变量生命周期:函数执行时声明,函数执行结束销毁
(5)若声明变量时没有使用var关键字,则此变量为全局变量
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			全局变量:函数体之外声明的变量属于全局变量
			全局变量生命周期:浏览器打开时声明,浏览器关闭时销毁
			全局变量尽量少用,因为全局变量会一直占据浏览器的内存空间
			局部变量:函数体中声明的变量以及函数的形参属于局部变量
			局部变量的生命周期:函数开始执行时开辟局部变量内存空间,函数执行结束时释放局部变量的内存空间
			*/
		   // 全局变量
			var i = 100;
			function accessI() {
				// 访问全局变量
				window.alert("i = " + i);
			}
			// 调用函数
			accessI();

			// 全局变量
			var username = "jxs"
			function accessUsername() {
				// 局部变量
				var username = "dwy";
				// 就近原则:访问局部变量
				window.alert(username);
			}
			accessUsername();
			// accessUsername函数执行结束后,var username = "dwy"变量释放
			window.alert(username);

			function accessAge() {
				var age = 21;
				window.alert(age);
			}
			accessAge();
			// age is not defined
			// window.alert(age);
			
			function getEmail() {
				若声明变量时没有使用var关键字,则此变量为全局变量
				myEmail = "2899978900@qq.com";
			}
			// 调用函数
			getEmail();
			// 2899978900@qq.com
			window.alert(myEmail);
		</script>
	</body>
</html>
JS数据类型
1、基本介绍

(1)JavaScript中声明变量时无需指定数据类型,但将值赋给变量时,值具有数据类型。
(2)ES6版本之前存在6种数据类型:Undefined、Number、String、Boolean、Null、Object
(3)ES6版本之后存在7种数据类型:Undefined、Number、String、Boolean、Null、Object、Symbol
(4)数据类型分为:原始类型(Undefined、Number、String、Boolean、Null)、引用类型(Object)
2、typeof运算符基本介绍

(1)typeof运算符可以在程序运行阶段动态地获取变量的数据类型
(2)typeof运算符语法格式:typeof 变量名
(3)typeof运算符运算结果为以下6个字符串之1:"undefined"、"number"、"string"、"boolean"、"object"、"function"
(4)JavaScript中比较字符串是否相等使用"=="完成
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.JavaScript中声明变量时无需指定数据类型,将值赋给变量时,值具有数据类型
			2.JavaScript中数据类型分为原始类型、引用类型
			3.ES6版本前的6种数据类型:Undefined、Number、String、Boolean、Null、Object
			4.ES6版本后的7种数据类型:Undefined、Number、String、Boolean、Null、Object、Symbol
			5.原始类型:Undefined、Number、String、Boolean、Null
			6.引用类型:Object以及Object的子类
			7.ES规范(ECMAScript规范),ES6之后,基于以上6种数据类型又添加了一种新的数据类型:Symbol
			8.JavaScript中有运算符typeof,此运算符可以在程序运行阶段动态地获取变量的数据类型
			9.typeof运算符语法格式:typeof 变量名
			  typeof运算符的运算结果为以下6个字符串之一:"undefined" "number" "string" "boolean" "object" "function"
			10.JavaScript中比较字符串是否相等使用"=="完成
			*/

			// 求和,要求变量a和变量b的数据类型必须为数字,不可为其他数据类型
			function sum(a, b) {
				if (typeof a == "number" && typeof b == "number") {
					return a + b;
				}
				alert(a + "、" + b + "必须全为数字");
			}
			var resultValue1 = sum("jxs", "dwy");
			window.alert(resultValue1);

			var resultValue2 = sum(1, 2);
			window.alert(resultValue2);

			var a;
			window.alert(typeof a); //"undefined"
			var b = 10;
			window.alert(typeof b); //"number"
			var c = "abc";
			window.alert(typeof c); //"string"
			var d = null;
			window.alert(typeof d); //null属于Null类型,typeof运算符结果为"object"
			var e = false;
			window.alert(typeof e); //"boolean"
			var object = new Object();
			window.alert(typeof object);//"object"
			var function01 = function() {} 
			window.alert(typeof function01);//"function"
		</script>
	</body>
</html>
Undefined数据类型
1、基本介绍

(1)当1个值为undefined时,此值属于Undefined数据类型
(2)Undefined数据类型只有1个值,此值为undefined
(3)当1个变量没有手动赋值时系统默认为undefined
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			Undefined类型只存在1个值:undefined
			当一个变量没有手动赋值,系统默认赋值undefined
			*/
			var a;
			var b = undefined;
			var c = "undefined";
			window.alert(a);// 系统默认赋值undefined
			window.alert(b);// undefined
			window.alert(c);// "undefined"
		</script>
	</body>
</html>
Number数据类型
1、基本介绍

(1)Number数据类型包括:正数、负数、浮点数、NaN(Not a Number)、Infinity(无穷)
(2)NaN(Not a Number):属于Number数据类型。当运算结果应当为数字,最后运算结果却不为数字时,运算结果的数据类型为NaN(例:var result = 10/"jxs",除号运算结果应当为数字,运算过程中第2个数字为字符串导致运算结果不为数字,所以变量result的数据类型为NaN)。
(3)Infinity(无穷):当除数为0时结果为Infinity
2、函数基本介绍

(1)isNaN(数据):返回结果为true则不为数字,返回结果为false则为数字
(2)parseInt(数据):将字符串转换为数字并取整数位
(3)parseFloat(数据):将字符串转换为数字
(4)Math.ceil(数据):Math为数学类,向上取整
3、Number数据类型案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			Number数据类型包括负数、正数、浮点数、NaN(Not a Number)、Infinity(无穷)
			*/
		   var a = 1;
		   var b = -1;
		   var c = 3.14;
		   var d = NaN;
		   var e = Infinity;
		   window.alert(typeof a);// "number"
		   window.alert(typeof b);// "number"
		   window.alert(typeof c);// "number"
		   window.alert(typeof d);// "number"
		   window.alert(typeof e);// "number"
		   
		   /*
		   NaN(Not a Number):不是1个数字,属于Number类型
		   什么情况下结果为NaN:当运算结果本应为数字,最后运算结果却不为数字时
		   例:a/b运算结果本应为数字,运算过程中第2个数字为字符串导致运算结果不为数字
		   */
		  var a = 100;
		  var b = "jxs";
		  window.alert(a / b);
		  
		  var a = "jxs";
		  var b = 99;
		  var c = "dwy";
		  window.alert(a + b + c);// jxs99dwy字符串拼接
		  
		  /*
		  Infinity(当除数为0时结果为Infinity)
		  */
		   window.alert(10 / 0);// Infinity
		   
		   // 思考:JavaScript中10/3=?
		   window.alert(10 / 3);// 3.3333333333333335
		   
		   /*
		   函数isNaN(数据):返回结果为true则不为1个数字,返回结果为false则为1个数字
		   函数parseInt:将字符串转换为数字,并且取整数位
		   函数parseFloat:将字符串转换为数字
		   函数Math.ceil():Math为数学类,函数ceil:向上取整
		   */
		  var a = 10 / "jxs";
		  window.alert(isNaN(a));
		  window.alert(parseInt("3.99"));
		  window.alert(parseInt(3.99));
		  window.alert(parseFloat("3.99"));
		  window.alert(parseFloat(3.99));
		  window.alert(Math.ceil(2.1));
		</script>
	</body>
</html>
Boolean数据类型
1、基本介绍

(1)Boolean数据类型包括true、false
2、Boolean()函数基本介绍

(1)将非布尔类型数据转换为布尔类型数据
(2)非布尔类型数据转换为布尔类型数据时可省略函数Boolean()
(3)Boolean()函数转换规则:"有"则true,"无"则false
3、Boolean数据类型案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			JavaScript中Boolean数据类型包括true、false
			Boolean数据类型中有函数Boolean(数据),将非布尔类型的数据转换为布尔类型
			*/
			var username = "";
			/*
			if条件表达式应为布尔类型
		    函数Boolean(数据)可以省略,系统自动调用Boolean(数据)函数将username转换为布尔类型
			*/
			if (username) {
				alert("用户名不可为空");
			} else {
				window.alert(username + ",欢迎你");
			}
			// Boolean(数据)函数转换规则:"有"为true,"无"为false
			window.alert(Boolean(undefined)); // false
			window.alert(Boolean(1)); // true
			window.alert(Boolean(-1)); // true
			window.alert(Boolean(0)); // false
			window.alert(Boolean(3.14)); // true
			window.alert(Boolean(NaN)); // false
			window.alert(Boolean(Infinity)); // true
			window.alert(Boolean("")); // false
			window.alert(Boolean("abc")); // true
		</script>
	</body>
</html>
String数据类型
1、基本介绍

(1)JavaScript中字符串可以使用单引号或双引号
(2)JavaScript中创建字符串的两种方式:
	var s1 = "abc"(小string) typeof s1为"string"
	var s2 = new String("abc")(大String) typeof s2为"object"
(3)小string和大String属性和函数通用
2、String数据类型常用属性和常用函数

(1)常用属性:length、constructor、prototype
(2)常用方法:charAt、concat、indexOf、lastIndexOf、replace、split、substr、substring、toLowerCase、toUpperCase
(3)substr、substring区别:
	substr(startIndex,length)
	substring(startIndex,endIndex)
3、String数据类型案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.JavaScript中字符串可以使用单引号或双引号
			2.JavaScript创建字符串的两种方式:var s1 = "abc";
											var s2 = new String("abc")
			3.String为内置类,String的父类为Object
			4.小string和大String,属性和函数通用
			5.关于String数据类型的常用属性和函数
				常用函数:charAt、concat、indexOf、lastIndexOf
				         replace、split、substr、substring
						 toLowerCase、toUpperCase
				常用属性:length、constructor、prototype
			*/

			// 小string(属于String类型)
			var s1 = "abc";
			window.alert(typeof s1); // "string"

			// 大String(属于Object类型)
			var s2 = new String("abc");
			window.alert(typeof s2); // "object"

			// 获取字符串长度
			window.alert(s1.length); // 3
			window.alert(s2.length); // 3

			var s3 = "http://www.baidu.";
			window.alert(s3.charAt(1)); // t
			window.alert(s3.concat("com")); // http://www.baidu.com
			window.alert(s3.indexOf("http")); // 0
			window.alert(s3.lastIndexOf("com")); // -1
			window.alert(s3.replace("baidu", "jd")); // http://www.jd.
			window.alert(s3.split(".")); // http://www,baidu,
			/*
			substr、substring区别:
			substr(startIndex,length)
			substring(startIndex,endIndex),不包含endIndex
			*/
			window.alert(s3.substr(0, 3)); // htt
			window.alert(s3.substring(0, 3)); // htt
			window.alert(s3.toLowerCase()); // http://www.baidu.
			window.alert(s3.toUpperCase()); // HTTP://WWW.BAIDU.
		</script>
	</body>
</html>
Object数据类型（重要！！）
1、基本介绍

(1)Object常用属性和常用函数
	常用属性:prototype
	常用函数:toLocaleString、toString、valueOf
(2)JavaScript中定义的类继承Object类,即继承Object类中所有的属性和函数,即自定义的类中存在prototype属性
2、JavaScript中自定义类、创建对象、访问对象属性方式

(1)自定义类的两种方式:
	第一种方式:function 类名(形参) {}
	第二种方式:类名 = function(形参) {}
(2)创建对象语法:new 构造函数(实参)
(3)访问对象属性的两种方式:
	第一种方式:对象名.属性名
	第二种方式:对象名["属性名"]
3、创建函数和创建类区别

function test() {}
//将test当作函数调用
test();
//将test当作类创建对象
var obj = new test();
4、JavaScript中定义类的同时完成构造函数的定义

5、prototype属性基本介绍

(1)Object类中常用属性prototype
(2)自定义的类默认继承Object类
(3)prototype属性作用:为类动态扩展属性和函数
6、Java与JavaScript中定义类与创建对象对比

Java中定义类
public class User {
    private String username;
    private String userpassword;
    public User() {}
    public User(String username,String userpassword) {
        this.username = username;
        this.userpassword = userpassword;
    }
}

Java中创建对象
User user1 = new User();
User user2 = new User("jxs","123")
    
JavaScript中定义类
User = function(username,userpassword) {
    this.username = username;
    this.userpassword = userpassword;
}

JavaScript中创建对象
var user1 = new User();
var user2 = new User("jxs");
var user3 = new User("jxs","123");
7、Object数据类型案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			Object数据类型:
			1.Object常用属性和常用函数
				常用属性:prototype(作用:动态的为类扩展属性和函数)
				常用函数:toLocaleString、toString、valueOf
			2.JavaScript中定义的类默认继承Object,继承Object类中所有属性和函数
			  即自定义的类中存在prototype属性
			3.JavaScript中定义类的两种方式
				第一种方式:function 类名(形参) {}
				第二种方式:类名 = function(形参) {}
			4.JavaScript中创建对象的语法
				new 构造函数(实参);
			*/

			function test() {}
			//将test当作函数调用
			test();
			//将test当作类创建对象
			var obj = new test(); // obj为一个引用,保存内存地址指向堆中的对象

			/*
			JavaScript中定义类的同时完成构造函数的定义
			*/
			function User(username, userage) {
				this.username = username;
				this.userage = userage;
			}
			// 创建对象
			var user = new User("jxs", 21);
			// 访问对象属性方式一
			window.alert(user.username);
			window.alert(user.userage);
			// 访问对象属性方式二
			window.alert(user["username"]);
			window.alert(user["userage"]);

			Product = function(pname, price) {
				// 属性pname、price,将传入的pname、price赋给属性
				this.pname = pname;
				this.price = price;
				//定义函数
				this.getPrice = function() {
					return this.price;
				}
			}
			var product = new Product("卫龙", 3.5);
			window.alert(product.pname);// 卫龙
			window.alert(product["price"]);// 3.5
			window.alert(product.getPrice());
			
			// 通过prototype属性为类动态扩展属性和函数
			Product.prototype.getPname = function() {
				return this.pname;
			}
			// 调用后期扩展的getPname()函数
			window.alert(product.getPname());
			
			//为String扩展函数
			String.prototype.add = function() {
				window.alert("为String类型扩展函数");
			}
			var test = "JXS";
			// 通过字符串test调用add函数
			test.add();
		</script>
	</body>
</html>
null、NaN、undefinded区别（重中之重！！）
1、基本介绍

(1)null、NaN、undefined数据类型不同
(2)null等同于undefined,即null==undefined
2、==运算符和===运算符

(1)==运算符:判断值是否相等
(2)===运算符:判断值和数据类型是否相等
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			null、NaN、undefined区别
			1.数据类型不同
			2.null等同于undefined
			*/
			alert(typeof null); // "object"
			alert(typeof NaN); // "number"
			alert(typeof undefined); // "undefined"

			alert(null == NaN); // false
			alert(null == undefined); // true
			alert(NaN == undefined); // false
			
			/*
			JavaScript中两个特殊的运算符
			1.==(等同运算符):判断值是否相等
			2.===(全等运算符):判断值和数据类型是否相等
			*/
		   alert(null === NaN); // false
		   alert(null === undefined); // false
		   alert(NaN === undefined); // false
		</script>
	</body>
</html>
JS中事件
1、JavaScript中常用事件

(1)click:单击鼠标
(2)dblclick(double click):双击鼠标
(3)mousedown:鼠标按下
(4)mouseup:鼠标弹起
(5)mouseover:鼠标经过
(6)mousemove:鼠标移动
(7)mouseout:鼠标离开
(8)blur:失去焦点
(9)focus:获得焦点
(10)keydown:键盘按下
(11)keyup:键盘弹起
(12)reset:重置表单
(13)submit:提交表单
(14)load:html页面所有元素加载完毕
(15)change:下拉列表选项改变或文本框内容改变
(16)select:文本被选定
2、事件基本介绍

(1)JavaScript中每一事件都对应事件句柄
(2)事件前添加on即事件句柄
(3)事件句柄作为标签中的属性而存在
3、彻底理解回调函数

(1)假设公司开发一款主打解决国民早餐问题的APP,为加快开发进度,这款应用由A小组、B小组协同开发。
(2)其中有一核心模块由A小组开发B小组调用,此模块被封装为makeApp函数
(3)若makeApp函数执行快速并可以立即返回,则B小组只需调用makeApp函数、等待makeApp函数执行完毕后继续后续流程
(4)若世界总这么简单就好了！！
(5)若makeApp函数处理庞大的数据量,makeApp函数执行缓慢,不会立即返回
(6)此时,需B小组调用makeApp函数,A小组不再等待makeApp函数执行完毕而直接返回继续后续流程,此时A小组的程序可以和makeApp函数同时进行(异步)
(7)假设编写App第一版的代码为:B小组调用makeApp函数,制作10000条油条,制作完毕后返回。A小组继续后续的售卖流程
makeApp(10000);
sell();
(8)A小组要苦苦等待B小组制作完油条才可进行后续的售卖
(9)更好的方法是makeApp函数知道制作完油条后该干什么,即makeApp(10000,sell)
(10)makeApp函数多了一个参数,除了指定制作油条的数量外还可以指定制作好油条后的后续操作
(11)A小组定义了sell函数,sell函数被B小组调用执行,sell函数就叫回调函数(callback)
(12)makeApp函数如何实现回调
void makeApp(int num,function sell) {
	//制作油条
	//执行回调
	sell();
}
(13)A小组编写makeApp函数,B小组调用执行,A小组不必苦苦等待B小组执行makeApp函数完毕后再进行售卖油条,makeApp函数制作完油条后自动调用sell函数进行售卖操作
(14)
同步调用:request()函数返回获取结果后,才可调用handle函数处理结果,request函数返回结果前我们必须等待
res = request();
handle(res);
异步调用:将handle函数作为参数传递给request
request(handle);
(15)回调函数正式定义:一段以参数形式传递给其他代码的可执行代码
(16)对于一般函数来说,自己编写的函数会在自己的程序内部调用,即函数编写方为自己,函数调用方为自己
(17)对于回调函数来说,调用第三方库中的函数,将回调函数传递给第三方库,第三方库中的函数调用我们编写的回调函数
4、注册事件的两种方式

(1)标签中使用事件句柄
(2)JavaScript代码完成事件的注册
	第一步:获取按钮对象
	第二步:为按钮对象的onclick属性赋值
5、事件案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!--
		注册事件方式一:标签中使用事件句柄
		将sayHello函数注册到按钮上,等待click事件发生后,sayHello函数被浏览器调用,我们称sayHello为回调函数 
		-->
		<input type="button" value="普通按钮" onclick=sayHello("Jxs") />
		<input type="button" value="普通按钮" id="button"/>
		<input type="button" value="普通按钮" id="button1"/>
		<input type="button" value="普通按钮" id="button2"/>
		
		<script type="text/javascript">
			/*
			JavaScript中常用事件
			1.click:单击鼠标
			2.dblclick(double click):双击鼠标
			
			3.mousedown:鼠标按下
			4.mouseup:鼠标弹起
			5.mouseover:鼠标经过
			6.mousemove:鼠标移动
			7.mouseout:鼠标离开
			
			8.blur:失去焦点
			9.focus:获得焦点
			
			10.keydown:键盘按下
			11.keyup:键盘弹起
			
			12.reset:重置表单
			13.submit:提交表单
			
			14.load:页面加载完毕(html页面中所有元素加载完毕)
			15.change:下拉列表选项改变或文本框内容改变
			16.select:文本被选定
			
			JavaScript中每一事件对应一个事件句柄
			事件句柄即在事件前添加on
			事件句柄作为标签的属性而存在
			*/

			/*
			对于当前程序,sayHello()属于回调函数
			回调函数:编写出函数代码却不负责调用,由其他程序负责调用该函数
			*/
			function sayHello(name) {
				window.alert("Hello," + name);
			}
			
			function test() {
				window.alert("test");
			}
			
			/*
			注册事件方式二:纯JavaScript代码完成事件的注册 
				第一步:获取按钮对象(document为内置对象,代表整个html页面)
				第二步:为按钮对象的onclick属性赋值
			*/
			var button = document.getElementById("button");
			/*
			错误写法:button.onclick = sayHello();
			将test函数注册到click事件
			*/
			button.onclick = test;
			
			var button1 = document.getElementById("button1");
			/*
			匿名回调函数
			页面打开时将此函数注册在click事件上,当click事件发生后浏览器调用此函数
			*/
			button1.onclick = function() {
				window.alert("test...")
			}
			
			document.getElementById("button2").onclick = function() {window.alert("test......")}
		</script>
	</body>
</html>
JS代码执行顺序
1、案例一

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<!-- 页面全部元素加载完毕后执行ready函数 -->
	<body onload="ready()">
		<script type="text/javascript">
			/*
			匿名回调函数
			1.返回null,代码执行到此处时id="button"的元素还未加载到内存
			*/
		   function ready() {
			   document.getElementById("button").onclick = function() {
			   	window.alert("Hello Jxs");
			   }
		   }
		</script>
		
		<input type="button" value="按钮" id="button"/>
	</body>
</html>
2、案例二

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.页面加载过程中将回调函数a注册给load事件
			2.页面所有元素加载完毕后执行load事件,执行回调函数a
			3.回调函数a执行过程中将回调函数b注册给click事件
			4.当id="button"的元素发生click事件后,b回调函数被调用执行
			*/
			window.onload = function() { // 匿名回调函数a
				document.getElementById("button").onclick = function() { // 匿名回调函数b
					window.alert("Hello JXS");
				}
			}
		</script>

		<input type="button" value="按钮" id="button" />
	</body>
</html>
3、案例三

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button").onclick = function() {
					document.getElementById("text").type = "checkbox";
				}
			}
		</script>
		
		<input type="text" id="text"/>
		<input type="button" id="button" value="将文本框转换为复选框"/>
	</body>
</html>
捕捉回车键
1、基本介绍

(1)事件发生时,浏览器自动创建事件对象
(2)事件发生时执行相应函数,若函数参数列表中存在参数则将事件对象返回给此参数
(3)键盘对象存在属性keyCode用于获取键盘每一个键对应的键值
(4)回车键对应13,Esc对应27
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				/*
				1.event参数用于获取键盘事件对象
				2.当发生键盘事件时,浏览器自动创建键盘事件对象,并将键盘事件对象返回给event
				3.对于每一键盘事件对象都有keyCode属性用于获取键值
				*/
				document.getElementById("username").onkeydown = function(event) {
					/*
					键盘中每一个键都对应键值
					回车键对应13
					Esc对应27
					*/
					if(event.keyCode === 13) {
						window.alert("正在验证")
					}
				}
			}
		</script>

		<form>
			<table>
				<tr>
					<td>用户名</td>
					<td><input type="text" id="username"/></td>
				</tr>
				<tr>
					<td>密码</td>
					<td><input type="password" id="userpassword"/></td>
				</tr>
			</table>
		</form>

	</body>
</html>
JS运算符之void（重要！！）
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!--
		void运算符语法:void(表达式)
		运算原理:执行表达式,不返回任何结果
		
		javascript:void
		1.javascript:告知浏览器后面为js代码,不可省略
		-->
		<a href="javascript:void()" onclick="window,alert('test')">
			既保留超链接样式,同时点击超链接时执行JavaScript代码,并且页面可不跳转
		</a>
	</body>
</html>
JS之控制语句
1、基本介绍

控制语句:
(1)if
(2)switch
(3)while
(4)do...while
(5)for
(6)break
(7)continue
(8)for...in...(了解)
(9)with(了解)

for...in...可以遍历数组,也可以遍历对象属性
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.if
			2.switch
			
			3.while
			4.do..while...
			5.for
			
			6.break
			7.continue
			
			8.for..in...(了解)
			9.with(了解)
			*/

			// 定义数组
			var array = [1, 3.14, "abc", true, false, undefined];
			// 遍历数组
			for (var i = 0; i < array.length; i++) {
				alert(array[i]);
			}
			// for...in...
			for (var i in array) {
				alert(array[i]);
			}
			// for...in...遍历对象属性
			function User(username, userpassword) {
				this.username = username;
				this.userpassword = userpassword;
			}
			var user = new User("蒋兴树", "123");
			alert(user.username + user.userpassword);
			alert(user["username"] + user["userpassword"]);
			for (var attributeName in user) {
				alert(typeof attributeName); // "string"
				alert(user[attributeName]);
			}
			
			alert(user.username);
			alert(user.userpassword);
			with(user) {
				alert(username + userpassword)
			}
		</script>
	</body>
</html>
JavaScript包括ECMAScript、DOM、BOM（重要！！）
1、基本介绍

(1)JavaScript = ECMAScript + DOM + BOM
(2)ECMAScript是由ECMA国际(European Computer Manufacturers Association)通过ECMA-262标准化的脚本程序设计语言
(3)DOM(Document Object Model 文档对象模型)是HTML和XML文档的编程接口,提供了对文档的结构化的表述,并定义了一种方式可以使从程序中对该结构进行访问,从而改变文档的结构、样式和内容。DOM将文档解析为一个由元素和对象(包含属性和函数的对象)组成的结构集合
(4)BOM(Browser Object Model 浏览器对象模型)赋予JavaScript程序与浏览器交互的能力。window 对象是BOM的核心,用来表示当前浏览器窗口,其中提供了一系列用来操作或访问浏览器的方法和属性。另外,JavaScript中的所有全局对象、函数以及变量也都属于window对象
2、DOM与BOM关系

(1)DOM顶级对象:document
(2)BOM顶级对象:window
(3)DOM与BOM关系:BOM包含DOM
3、DOM与BOM关系图

![](E:\Study\自学课程资料\Java\assets\DOM与BOM区别.png)

DOM编程案例
基础案例：按钮获取文本框的值
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button").onclick = function() {
					document.getElementById("text2").value = document.getElementById("text").value;
				}
			}
		</script>

		<input type="text" id="text" />
		<input type="button" id="button" value="获取文本框的值"/>
		<input type="text" id="text2"/>
		<!--
		blur:失去焦点事件
		this:表示当前节点对象
		this.value:表示当前节点对象的value属性
		-->
		<input type="text" onblur="window.alert(this.value)"/>
	</body>
</html>
innerHTML、innerText操作div、span
1、基本介绍

(1)innerHTML、innerText:设置元素内部内容
(2)innerHTML:将字符串作为HTML代码解释执行
(3)innerText:即使字符串中为HTML代码,也将其视为普通字符串处理
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			#div1 {
				background-color: white;
				border: 1px black solid;
				width: 300px;
				height: 300px;
			}
		</style>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button1").onclick = function() {
					// 获取div对象
					var div = document.getElementById("div1");
					/*
					innerHTML、innerText:设置元素内部内容
					innerHTML:将字符串作为HTML代码解释执行
					innerText:即使字符串中为HTML代码,也将其视为普通字符串处理
					*/
					// 使用innerHTML属性设置元素内部内容
					// div.innerHTML = "<font color = 'red'>div内容</font>";
					div.innerText = "<font color = 'red'>div内容</font>";
				}
			}
		</script>

		<input type="button" value="设置div中内容" id="button1" />
		<div id="div1"></div>
	</body>
</html>
正则表达式
1、基本介绍

(1)正则表达式:regular expression
(2)正则表达式用于字符串匹配
(3)正则表达式为一门独立学科,大部分编程语言都支持正则表达式
(4)正则表达式最初用于医学方面表示神经符号,目前使用最多的是计算机领域用于字符串匹配
2、掌握正则表达式哪些内容

(1)掌握常见正则表达式
(2)编写简单正则表达式
(3)看懂他人编写的正则表达式
(4)JavaScript中如何创建正则表达式对象
(5)JavaScript中正则表达式对象的方法
3、常见正则表达式

(1).:匹配换行符以外的任意字符
(2)\w:word,匹配数字、字母、汉字、下划线
(3)\s:space,匹配任意空白符
(4)\d:digit,匹配任意数字
(5)\b:begin,匹配单词的开始或结束
(6)^:匹配字符串的开始
(7)$:匹配字符串的结束
(8)\W:匹配数字、字母、汉字、下划线以外的字符
(9)\S:匹配空白符以外的字符
(10)\D:匹配数字以外的字符
(11)\B:匹配单词的开始或结束以外的位置
(12)[^x]:匹配除x以外的字符
(13)[^abc]:匹配abc字母以外的字符

(14)*:重复零次或更多次
(15)+:重复一次或更多次
(16)?:重复零次或一次
(17){n}:重复n次
(18){n,}:重复n次或更多次
(19){n,m}:重复n到m次

(20)[0-9]:表示0-9中任意一个数字
(21)[0-9a-zA-Z]:表示0-9或a-z或A-Z中任意一个字符
4、简单的正则表达式

QQ号的正则表达式:^[1-9]{1}[0-9]{4-9}$
QQ邮箱正则表达式:^[1-9]{1}[0-9]{4,9}@qq.com$
5、创建正则表达式对象方式

方式一:var regularExpression = /正则表达式/flags
方式二:var regularExpression = new RegExp("正则表达式","flags")

关于flags:
g:全局匹配
i:区别大小写
m:匹配和多行匹配

当前面为正则表达式时,m属性不可使用;反之,m属性可使用
6、调用正则表达式对象方法

调用正则表达式对象test方法:var true/false = 正则表达式对象.test(字符串);
若返回true表示字符串匹配正则表达式;若返回false表示字符串不匹配正则表达式
7、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>

		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button").onclick = function() {
					var email = document.getElementById("email").value;
					var regularExpression = /^[1-9]{1}[0-9]{4,9}@qq.com$/;
					var result = regularExpression.test(email);
					if (result) {
						document.getElementById("sapn1").innerText = "邮箱格式正确";
					} else {
						document.getElementById("span1").innerText = "邮箱格式错误";
					}
				}

				document.getElementById("email").onfocus = function() {
					document.getElementById("span1").innerText = "";
				}
			}
		</script>

		<input type="text" id="email" />
		<span id="span1" style="color: red;font-size: 12px;"></span><br>
		<input type="button" value="验证邮箱" id="button" />

	</body>
</html>
去除字符串前后空白
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			// 低版本的IE浏览器不支持字符串的trim函数,可以为String类扩展trim函数
			String.prototype.trim = function() {
				return this.replace(/^\s+/,"").replace(/\s+$/,"");
			}
			
			window.onload = function() {
				document.getElementById("button").onclick = function() {
					var value = document.getElementById("username").value;
					// 去除前后空白
					value = value.trim()
					alert("-->" + value + "<--");
				}
			}
		</script>
		<input type="text" id="username" />
		<input type="button" value="获取用户名" id="button" />
	</body>
</html>
表单验证（重中之重！！）
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!--
		表单验证
		1.用户名不可为空
		2.用户名长度在6-14位之间
		3.用户名由数字和字母组成
		
		4.密码和确认密码一致
		
		5.邮箱地址合法
		
		6.统一失去焦点验证
		
		7.错误提示信息在span中提示,字体12号,红色
		
		8.文本框获得焦点后清空错误提示信息
		9.文本框中数据不合法要求清空文本框的value
		
		10.表单中数据均合法方可提交数据
		-->
		<script>
			window.onload = function() {
				// 用户名文本框失去焦点时验证用户名是否合法
				document.getElementById("text01").onblur = function() {
					// 获取用户名
					var username = document.getElementById("text01").value;
					// 去除空白
					username = username.trim();
					// 判断字符串是否为空
					if (username === "") {
						document.getElementById("span1").innerText = "用户名不可为空";
					} else {
						// 判断长度是否在6 - 14 位之间
						if (username.length < 6 || username.length > 14) {
							document.getElementById("span1").innerText = "用户名长度必须在[6-14]之间";
						} else {
							var regularExpression = /^[0-9a-zA-Z]{6,14}$/;
							var result = regularExpression.test(username);
							if (!result) {
								document.getElementById("span1").innerText = "用户名由数字字母组成";
							}
						}
					}
				}

				// 用户名文本框获得焦点事件
				document.getElementById("text01").onfocus = function() {
					if (document.getElementById("span1").innerText != "") {
						document.getElementById("text01").value = "";
						document.getElementById("span1").innerText = "";
					}
				}
				
				// 确认密码框失去焦点时验证确认密码是否合法
				document.getElementById("password02").onblur = function() {
					// 获取密码和确认密码
					var password01 = document.getElementById("password01").value;
					var password02 = document.getElementById("password02").value;
					// 判断确认密码与密码是否相等
					if (password01 != password02) {
						document.getElementById("span3").innerText = "两次密码不一致";
					}
				}
				
				// 确认密码框获取焦点事件
				document.getElementById("password02").onfocus = function() {
					if (document.getElementById("span3").innerText != "") {
						document.getElementById("password02").value = "";
						document.getElementById("span3").innerText = "";
					}
				}
				
				// 邮箱文本框失去焦点时验证邮箱是否合法
				document.getElementById("text02").onblur = function() {
					var email = document.getElementById("text02").value;
					// 正则表达式
					var regularExpression = /^[1-9]{1}[0-9]{4,9}@qq.com$/;
					// 判断邮箱是否合法
					var result = regularExpression.test(email);
					if(!result) {
						document.getElementById("span4").innerText = "邮箱格式不合法"
					}
				}
				
				// 邮箱文本框获取焦点事件
				document.getElementById("text02").onfocus = function() {
					if (document.getElementById("span4").innerText != "") {
						document.getElementById("text02").value = "";
						document.getElementById("span4").innerText = "";
					}
				}
				
				// 提交按钮绑定鼠标单击事件
				document.getElementById("button01").onclick = function() {
					// 触发blur事件并且span内部内容为空
					var username = document.getElementById("text01");
					// 按钮触发鼠标单击后,用户名文本框触发获得焦点、失去焦点事件
					username.focus();
					username.blur();
					
					var password01 = document.getElementById("password01");
					password01.focus();
					password01.blur();
					
					var password02 = document.getElementById("password02");
					password02.focus();
					password02.blur();
					
					var email = document.getElementById("text02");
					email.focus();
					email.blur();
					
					var span1 = document.getElementById("span1").innerText;
					var span2 = document.getElementById("span2").innerText;
					var span3 = document.getElementById("span3").innerText;
					var span4 = document.getElementById("span4").innerText;
					if(span1 == "" && span2 == "" && span3 == "" && span4 == "") {
						// 提交表单
						document.getElementById("form01").submit();
					}
				}
			}
		</script>

		<form action="http://localhost:8080/test/save" method="post" id="form01">
			<table>
				<tr>
					<td>用户名</td>
					<td><input type="text" name="username" id="text01" /></td>
					<td><span id="span1" style="color: red;font-size: 12px;"></span></td>
				</tr>
				<tr>
					<td>密码</td>
					<td><input type="password" name="userpassword" id="password01" /></td>
					<td><span id="span2" style="color: red;font-size: 12px;"></span></td>
				</tr>
				<tr>
					<td>确认密码</td>
					<td><input type="password" id="password02" /></td>
					<td><span id="span3" style="color: red;font-size: 12px;"></span></td>
				</tr>
				<tr>
					<td>邮箱</td>
					<td><input type="text" name="email" id="text02" /></td>
					<td><span id="span4" style="color: red;font-size: 12px;"></span></td>
				</tr>
				<tr>
					<td><input type="reset" value="重置" id="reset01" /></td>
					<td><input type="button" value="注册" id="button01" /></td>
				</tr>
			</table>
		</form>
	</body>
</html>
复选框全选、取消全选（难点）
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				var checkbox01 = document.getElementById("checkbox01");
				var hobbys = document.getElementsByName("hobby");

				checkbox01.onclick = function() {
					for (var i = 0; i < hobbys.length; i++) {
						// checked:获取复选框的选中状态。返回true即选中, 返回false即未选中
						hobbys[i].checked = checkbox01.checked;
					}
				}

				// 总数量
				var allCount = hobbys.length;
				// 遍历数组
				for (var i = 0; i < hobbys.length; i++) {
					hobbys[i].onclick = function() {
						// 选中的复选框的数量
						var checkedCount = 0;
						// 当复选框总数量与选中的复选框数量相等时
						for (var i = 0; i < hobbys.length; i++) {
							if (hobbys[i].checked == true) {
								checkedCount++;
							}
						}
						checkbox01.checked = (checkedCount == allCount);
					}
				}

			}
		</script>
		<input type="checkbox" id="checkbox01" /><br>
		<input type="checkbox" name="hobby" value="smoke" id="checkbox02" />抽烟
		<input type="checkbox" name="hobby" value="drink" id="checkbox03" />喝酒
		<input type="checkbox" name="hobby" value="perm" id="checkbox04" />烫头
	</body>
</html>
获取下拉列表选项中的value
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				// change:下拉列表出现选项改变事件
				document.getElementById("select01").onchange = function() {
					window.alert(this.value);
				}
			}
		</script>

	</body>
	<select id="select01">
		<option>请选择省份</option>
		<option value="001">小学</option>
		<option value="002">中学</option>
		<option value="003">高中</option>
		<option value="004">专科</option>
		<option value="005">本科</option>
		<option value="006">硕士</option>
		<option value="007">博士</option>
	</select>
</html>
熟练使用F12
设置table的tbody
1、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			var datas = {
				"total": 4,
				"emps": [{
						"emp_id": 001,
						"emp_name": "jxs",
						"emp_salary": 10000
					},
					{
						"emp_id": 002,
						"emp_name": "dwy",
						"emp_salary": 8000
					}
				]
			}

			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					// 获取所有员工信息
					var emps = datas.emps;
					// 定义空字符串
					var html = "";
					// 遍历获取每一员工信息
					for (var i = 0; i < emps.length; i++) {
						var emp = emps[i];
						html += "<tr>";
						html += "<td>" + emp.emp_id + "</td>";
						html += "<td>" + emp.emp_name + "</td>";
						html += "<td>" + emp.emp_salary + "</td>";
						html += "</tr>";
					}
					document.getElementById("emp_tbody").innerHTML = html;
				}
			}
		</script>

		<h2>员工信息表</h2>
		<table border="1px">
			<tbody>
				<tr>
					<td>员工编号</td>
					<td>员工姓名</td>
					<td>员工薪水</td>
				</tr>
			</tbody>

			<tbody id="emp_tbody"></tbody>
		</table>

		<input type="button" value="显示员工信息" id="button01" />
	</body>
</html>
JavaScript内置对象
JavaScript中内置对象之Date（显示网页时钟）
1、基本介绍

(1)Date:获取当前系统时间
(2)new Date().toLocaleString():获取当前系统时间并转化为本地语言环境的日期格式
(3)new Date().getFullYear():获取当前系统时间的年信息
(4)new Date().getMonth():获取当前系统时间的月信息-1
(5)new Date().getDate():获取当前系统时间的日信息
(6)new Date().getDay():获取当前系统时间为一周中第几天(0-6天)
(7)new Date().getTime():获取1970年1月1日00:00:00至当前系统时间的总毫秒数
2、window.setInterval()、window.clearInterval()基本介绍

(1)window.setInterval("函数名",毫秒数):每隔?毫秒数执行?函数,返回一个可以传递给window.clearInterval()从而取消周期性执行的值
(2)window.clearInterval(window.setInterval("函数名",毫秒数)):取消?函数的周期性执行
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>

		<style>
			#div01 {
				color: red;
				font-size: 12px;
			}
		</style>

	</head>
	<body>
		<script type="text/javascript">
			// 获取当前系统时间
			var nowTime = new Date();
			//document.write(nowTime);

			//转换为本地语言环境的日期格式
			var nowTime = nowTime.toLocaleString();
			//document.write(nowTime);

			// 自定义日期格式
			var nowTime = new Date();
			var year = nowTime.getFullYear(); // 返回年信息
			var month = nowTime.getMonth(); // 0-11月
			//var day = nowTime.getDay();// 获取一周的第几天,0-6天
			var day = nowTime.getDate();
			//document.write(year + "年" + (month + 1) + "月" + day + "日");

			// 获取毫秒数,从1970年1月1日00:00:00 000到当前系统时间的总毫秒数
			var time = nowTime.getTime();
			//document.write(time); // 一般使用毫秒数作为时间戳(timestamp)


			window.onload = function() {
				document.getElementById("button01").onclick = start();
				
				document.getElementById("button02").onclick = function() {
					window.clearInterval(value);
				}
			}

			var value;
			
			function start() {
				// 每隔1秒执行showTime函数,返回一个可以传递给window.clearInterval()从而取消周期性执行的值
				value = window.setInterval("showTime()", 1000);
			}

			function showTime() {
				var nowTime = new Date();
				var strTime = nowTime.toLocaleString();
				var div01 = document.getElementById("div01");
				div01.innerText = strTime;
			}
		</script>

		<input type="button" value="显示系统时间" id="button01" />
		<input type="button" value="系统时间停止" id="button02" />
		<div id="div01"></div>
	</body>
</html>
JavaScript中内置对象之Array
1、基本介绍

(1)创建数组方式
	方式一:var array1 = [1,3.14,true,"abc",undefined]
	方式二:var array2 = new Array();
(2)数组中插入数据,数组下标越界时会进行自动扩容
(3)以方式二创建数组时,参数列表中无参数时数组长度为0;参数列表中存在1个参数时,参数的值即数组的长度;参数列表中存在2个及2个以上参数时,参数即数组元素
2、数组常用方法介绍

(1)join(""):以""中的元素连接数组中所有元素
(2)push(元素):增加元素至数组末尾
(3)pop():剔除数组末尾元素
(4)reverse(数组名):数组反转
3、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			// 创建长度为5的数组,数组中数据类型随意
			var array1 = [1, 3.14, false, "abc", undefined];
			document.writeln(array1.length);

			// 数组中插入数据,数组下标越界时会进行自动扩容
			array1[5] = "jxs";
			for (var i = 0; i < array1.length; i++) {
				document.writeln(array1[i]);
			}
			
			// 创建数组方式二,创建长度为3的数组
			var array2 = new Array(3);
			document.writeln(array2.length);
			
			// 数组长度为0
			var array3 = new Array();
			document.writeln(array3.length);
			
			/*
			创建数组时,参数列表中无参数数组长度默认为0
			参数列表中存在1个参数,参数的值即数组的长度
			参数列表中存在2个及2个以上,参数即代表数组中具体存储的值
			*/
			var array4 = new Array(1,2,3);
			document.writeln(array4.length);
			
			var array5 = new Array(1,2,3);
			// 以-连接数组中所有元素
			var value1 = array5.join("-");
			document.writeln(value1);
			
			var array6 = new Array(1,2,3,4,5,6,7);
			// 将元素8添加到数组末尾,数组长度+1
			array6.push(8);
			var value2 = array6.join("-");
			document.writeln(value2);
			
			// 将数组末尾的元素剔除,数组长度-1
			var value3 = array6.pop();
			document.writeln(value3);
			
			array6.reverse();
			document.writeln(array6);
		</script>
	</body>
</html>
BOM编程案例
window.open()和window.close()
1、基本介绍

(1)window.open():打开窗口
(2)window.close():关闭窗口
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.BOM编程中window对象为顶级对象,代表浏览器窗口
			2.window对象存在open、close方法,即开启窗口、关闭窗口
			*/
			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					window.open("http://www.baidu.com");
				}
				
				document.getElementById("button02").onclick = function() {
					window.open("http://www.baidu.com","_self");
				}
				
				document.getElementById("button03").onclick = function() {
					window.open("http://www.baidu.com","_blank");
				}
				
				document.getElementById("button04").onclick = function() {
					window.open("http://www.baidu.com","_parent");
				}
				
				document.getElementById("button05").onclick = function() {
					window.open("http://www.baidu.com","top");
				}
				
				document.getElementById("button06").onclick = function() {
					window.close("001-open、close.html");
				}
			}
		</script>

		<input type="button" value="百度(新窗口)" id="button01" />
		<input type="button" value="百度(当前窗口)" id="button02" />
		<input type="button" value="百度(新窗口)" id="button03" />
		<input type="button" value="百度(父窗口)" id="button04" />
		<input type="button" value="百度(顶级窗口)" id="button05" />
		<input type="button" value="关闭窗口" id="button06"/>
	</body>
</html>
window.alert()和window.confirm()
1、基本介绍

(1)window.alert():消息框
(2)window.confirm():确认框
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					window.alert("消息框");
				}
				
				document.getElementById("button02").onclick = function() {
					var result = window.confirm("确认删除");
					document.write(result);
				}
			}
		</script>
		
		<input type="button" id="button01" value="消息"/>
		<input type="button" id="button02" value="删除"/>
	</body>
</html>
历史记录
1、基本介绍

(1)window.history.back():回退到上一页面
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					window.history.back();
				}
			}
		</script>
		<input type="button" value="后退" id="button01"/>
	</body>
</html>
浏览器地址栏
1、基本介绍

(1)window.location.href:获取窗口地址栏对象,输入URL
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					// 获取窗口中的地址栏对象
					var location = window.location;
					location.href = "http://www.baidu.com";
				}
			}
		</script>
		<input type="button" value="百度" id="button01" />
	</body>
</html>
浏览器向服务器发送请求的常见方式（重要！！）
1、常见方式

(1)超链接
(2)提交表单
(3)window.location或document.location
(4)window.open("url")
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!-- 方式一 -->
		<a href="http://localhost:8080/test/save?username=jxs&userpassword=123">方式一:超链接</a>

		<script type="text/javascript">
			window.onload = function() {
				// 方式二
				document.getElementById("button01").onclick = function() {
					window.location.href = "http://www.baidu.com";
				}

				// 方式三
				document.getElementById("button02").onclick = function() {
					window.open("http://www.baidu.com");
				}
			}
		</script>

		<input type="button" value="方式二:window.location.href" id="button01" />
		<input type="button" value="方式三:window.open()" id="button02" />
		
		<!-- 方式四 -->
		<form action="http://localhost:8080/test/save">
			用户名<input type="text" name="username"/>
			密码<input type="password" name="userpassword"/>
			<input type="submit" value="方式四:提交表单"/>
		</form>
	</body>
</html>
顶级窗口
1、基本介绍

(1)window.top:当前浏览器窗口的顶级窗口
(2)window.self:当前浏览器窗口
(3)if(window.top != window.self){window.top.location = window.self.location};若当前浏览器的顶级窗口不为当前浏览器窗口,则将当前浏览器窗口地址栏中的URL覆盖当前浏览器窗口的顶级窗口地址栏中的URL
2、父窗口

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<iframe src="008-设置顶级窗口.html" width="200px" height="200px"></iframe>
	</body>
</html>
3、子窗口

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.onload = function() {
				document.getElementById("button01").onclick = function() {
					/*
					window为当前浏览器窗口
					window.top为当前浏览器窗口的顶级窗口
					window.self为当前浏览器窗口
					若当前浏览器窗口的顶级窗口不为本身则将本身设置为顶级窗口
					*/
					if(window.top != window.self) {
						// 使用当前浏览器窗口地址栏中的URL覆盖当前浏览器窗口的顶级窗口地址栏中的URL
						window.top.location = window.self.location;
					}
				}
			}
		</script>
		
		<input type="button" value="设置顶级窗口" id="button01"/>
	</body>
</html>
JSON对象（重中之重！！）
json概述
1、何为JSON

(1)JavaScript Object Notation(JavaScript对象标记,数据交换格式)
(2)JSON为一种标准的轻量级的数据交换格式
2、JSON作用

(1)JSON作为一种标准的轻量级的数据交换格式,目前非常流行
(2)系统A与系统B之间交换数据可以采用JSON
3、XML和JSON

(1)XML与JSON为实际开发中使用最多的两种数据交换格式
(2)JSON优点、缺点
	优点:轻量级、易解析
	缺点:语法松散
(3)XML优点、缺点
	优点:语法严谨
	缺点:体积大、不易解析
4、XML与HTML

(1)XML与HTML有一父类SGML(一种标准的标记语言)
(2)HTML主要处理页面展示,语法松散
(3)XML主要处理数据交换,语法严谨
5、创建JSON对象以及访问JSON对象属性

var studentObj = {
    "属性名" : "属性值",
    "属性名" : "属性值",
    "属性名" : "属性值",
    ...
};

document.write(studentObj.属性名 + studentObj.属性名 + studentObj.属性名 + ...);
6、创建JSON数组

var students = [
    {"属性名" : "属性值","属性名" : "属性值","属性名" : "属性值"},
    {"属性名" : "属性值","属性名" : "属性值","属性名" : "属性值"},
    {"属性名" : "属性值","属性名" : "属性值","属性名" : "属性值"},
    ...
];
7、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			/*
			1.何为JSON？
			JavaScript Object Notation(JavaScript对象标记,数据交换格式)
			JSON为一种标准的轻量级的数据交换格式
			优点:体积小、易解析
			在实际开发中使用最多的两种数据交换格式:JSON、XML
			XML优点:语法严谨  XML缺点:体积大、解析繁琐
			
			2.JSON作用
			JSON为一种标准的数据交换格式,目前非常流行。
			系统A与系统B进行数据交换可以采用JSON
			
			3.XML和HTML
			XML和HTML有一父类SGML(一种标准的标记语言)
			HTML主要处理页面展示,语法松散
			XML主要处理数据交换,语法严谨
			*/
		   
		   // 创建JSON对象,JSON对象中的属性无数据类型
		   var studentObj = {
			   "student_id" : "123",
			   "student_name" : "jxs",
			   "student_gender" : "男"
		   };
		   // 访问JSON对象属性
		   document.write(studentObj.student_id + " " + studentObj.student_name + " " + studentObj.student_gender);
		   // JSON数组
		   var students = [
			   {"student_id" : "123","student_name" : "jxs","student_gender" : "男"},
			   {"student_id" : "123","student_name" : "dwy","student_gender" : "女"},
			   {"student_id" : "123","student_name" : "lzz","student_gender" : "女"},
		   ];
		</script>
	</body>
</html>
json进阶案例
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			var user = {
				"userid" : "1",
				"username" : "jxs",
				"gender" : "男",
				"adress" : {
					"city" : "北京",
					"street" : "大兴"
				},
				"hobby" : ["smoke","drink"],
			};
			// 访问JSON对象居住的城市
			document.write(user.adress.city);
			
		</script>
	</body>
</html>
eval函数
1、基本介绍

(1)eval函数:将字符串当作一段js代码解释执行
(2)java连接数据库,查询数据库中的数据后,在java程序中将数据拼接为JSON格式的字符串,将JSON格式的字符串响应到浏览器,使用eval函数将JSON格式的字符串转换为JSON对象
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<script type="text/javascript">
			window.eval("var i = 1");
			document.write(i);
			
			/*
			java连接数据库,查询数据库中的数据后,在java程序中将数据拼接为JSON格式的字符串
			将JSON格式的字符串响应到浏览器,使用eval函数将JSON格式的字符串转换为JSON对象
			*/
		   var fromJava = "{\"name\":\"jxs\",\"password\":\"123\"}";
		   window.eval("var jsonObj = " + fromJava);
		   document.write(jsonObj.name);
		</script>
	</body>
</html>
JavaScript中[]和{}区别
1、基本介绍

(1)[]:数组
(2){}:JSON对象
2、案例演示

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
	</head>
	<body>
		<!--
		JavaScript中
		[]代表数组
		{}代表JSON
		-->
		<script type="text/javascript">
			var array = [1,2,3,4,5];
			
			var jsonObj = {
				"username" : "jxs",
				"userpassword" : "123"
			};
			访问json对象属性
			document.write(jsonObj.username);
			document.write(jsonObj["username"]);
		</script>
	</body>
</html>
Servlet
系统架构
1、系统架构形式

(1)C/S架构
(2)B/S架构
2、C/S架构

(1)Client/Server(客户端/服务器)
(2)C/S架构软件或系统有?(QQ,先去腾讯官网下载QQ软件,安装客户端软件后,输入账号密码登录后即可使用软件)
(3)C/S架构特点:需安装特定的客户端软件
(4)C/S架构的系统的优点、缺点
	优点:速度快(软件中的数据大多数都集成到客户端软件中,少量数据从服务端传送而来,所以C/S结构的系统速度快)、体验好(速度快、界面炫、体验好)、界面炫(专门的语言去实现界面,更加灵活)、服务器压力小(大量数据集成在客户端软件中,服务器只传送少量数据,服务器压力小)、安全(大量数据集成在客户端软件中,客户端中存有缓存)
	缺点:升级维护(每一个客户端软件都需升级维护)
3、B/S架构

(1)Browser/Server(浏览器/服务器)
(2)B/S架构系统有?(www.baidu.com)
(3)B/S架构的系统是一个特殊的C/S架构的系统,Client为一个固定不变的浏览器软件
(4)B/S架构的系统的优点、缺点
	优点:升级维护方便(只需升级服务器即可)、不需安装客户端软件(打开浏览器,输入网址即可)
	缺点:速度慢(全部数据在服务器上,用户发送的每一请求都需服务器响应,B/S架构的系统在网络中传输的数据量大)、体验差(浏览器只支持三种语言(HTML、CSS、JavaScript))、不安全(全部数据在服务器上,易导致数据丢失)
4、C/S、B/S架构适用场景

(1)娱乐性软件建议使用C/S架构
(2)公司内部使用的业务软件建议使用B/S架构(公司内部使用的系统需维护成本低、公司内部使用的系统不需界面炫、公司内部使用的系统主要能够进行数据的维护即可)
5、开发B/S架构的系统即开发网站，开发一个Web系统

(1)开发Web系统所需技术
	Web前端-运行在浏览器上的程序(HTML、CSS、JavaScript)
	Web后端-运行在Web服务器端的程序(Java、C语言、C++、Python、PHP)
(2)选择Java做Web开发我们称为JavaWeb开发
(3)JavaWeb开发最核心规范:Servlet(Server Applet服务器端的java程序)
6、Java三大模块

(1)JavaSE:Java标准版(别人写好的一套标准类库,JavaEE、JavaME基础)
(2)JavaEE:Java企业版(别人写好的一套类库,帮助完成企业级项目的开发,为企业内部提供解决方案的一套(多套)类库)
(3)JavaME:Java微型版(一套类库,帮助进行电子微型设备内核程序开发)
7、JavaEE规范

(1)JavaEE十三种规范:JDBC、JNDI、EJB、RMI、JSP、Servlets、XML、JMS、Java IDL、JTS、JTA、JavaMail、JAF
(2)Servlet为JavaEE规范之一
B/S结构原理剖析（重要！！）
1、Web系统访问过程

(1)打开浏览器
(2)地址栏输入合法网址
(3)浏览器上展示响应结果
2、域名

(1)https://www.baidu.com 网址
(2)www.baidu.com 域名
(3)浏览器地址栏输入域名,域名解析器解析域名,解析出具体的IP地址、端口号等(打开Windows命令行,输入ping www.baidu.com,得到具体IP地址,在浏览器地址栏输入112.80.248.76:80/index.html,浏览器上也展示响应结果)
(5)IP地址:计算机在网络中的身份证号,同一网络中,IP地址唯一。若A计算机与B计算机通信,A计算机需知道B计算机的IP地址才可建立连接
(6)端口号:一个端口号代表一个软件(一个端口号代表一个应用,一个端口号代表一个服务),一个计算机中有若干软件,每一个软件启动后都对应一个端口号,同一计算机中端口号唯一。
3、Web系统通信原理

(1)浏览器地址栏输入网址(URL(统一资源定位符 https://www.baidu.com))
(2)域名解析器解析域名得到http://112.80.248.76:80/index.html
(3)浏览器在网络中搜索IP地址为112.80.248.76的主机
(4)定位IP地址为112.80.248.76的主机上的80端口对应的服务器软件
(5)80端口对应的服务器软件得知浏览器所需资源名index.html
(6)80端口对应的服务器软件找到index.html文件,并将index.html文件中的内容直接输出响应到浏览器上。
(7)浏览器接收到服务器的代码(HTML CSS JavaScript)
(8)浏览器渲染,执行HTML CSS JavaScript代码,展示效果
4、B/S结构原理剖析图



5、请求、响应

(1)请求和响应指数据的流向不同
(2)请求:Browser端发送数据到Server端,英语单词Request
(3)响应:Server端发送数据到Browser端,英语单词Response
(4)B/S架构,B->S称为请求,S->B称为响应
Web服务器软件
1、服务器软件

(1)Tomcat(Web服务器)
(2)jetty(Web服务器)
(3)JBOSS(应用服务器)
(4)WebLogic(应用服务器)
(5)WebSphere(应用服务器)
2、Web服务器与应用服务器关系

(1)应用服务器实现了JavaEE的所有规范
(2)Web服务器实现了JavaEE中Servlet、JSP两个核心规范
(3)应用服务器包含Web服务器
3、Tomcat

(1)Apache官网地址:https://apache.org
(2)Tomcat官网地址:https://tomcat.apache.org
(3)Tomcat:开源、轻量级Web服务器
(4)Tomcat,又称Catalinna,Catalina是美国一个风景秀丽的岛屿,据说作者在这个岛屿上开发了一个轻量级(体积小、速度快)的Web服务器。
(5)Tomcat的logo是一只公猫,寓意Tomcat服务器是体积小、速度快,只实现Servlet+JSP规范
(6)Tomcat是Java语言编写的,Tomcat服务器运行必须依赖JRE(Java Runtime Environment)
配置Tomcat服务器
1、配置环境

(1)Tomcat是Java语言编写的,Tomcat服务器运行必须依赖JRE
(2)配置JDK环境变量
JAVA_HOME=E:\Software Development Kit\JDK\Windows\JDK8\JDK_8
Path=%JAVA_HOME%\bin
(3)安装Tomcat,官网下载zip包解压,解压即安装
(4)配置Tomcat环境变量
CATALINA_HOME=E:\Software Development Kit\Tomcat\apache-tomcat-10.0.27
Path=%CATALINA_HOME%\bin
(5)启动Tomcat,dos命令窗口执行bin目录下startup.bat文件
(6)启动Tomcat服务器只配置Path对应的bin目录是不行的,有两个环境变量必须配置:JAVA_HOME、CATALINA_HOME
2、Tomcat服务器目录

(1)bin:Tomcat服务器命令文件存放目录
(2)conf:Tomcat服务器配置文件存放目录(server.xml中可配置端口号,Tomcat默认端口号为8080)
(3)lib:Tomcat服务器核心程序目录,Tomcat服务器是Java语言编写的,目录下jar包都为class文件
(4)logs:Tomcat服务器日志目录,Tomcat服务器启动等信息都会在此目录下生成日志文件
(5)temp:Tomcat服务器临时目录,存储临时文件
(6)webapps:Tomcat服务器存放webapp(web application:web 应用)目录
(7)work:Tomcat服务器存放JSP文件翻译后的java文件以及编译后的class文件
3、Tomcat服务器bin目录知识扩展

(1)startup.bat:bat文件为Windows系统专用,bat文件为批处理文件,bat文件可以编写大量Windows系统的dos命令,执行bat文件相当于批量执行dos命令
(2)startup.sh:sh文件无法在Windows系统中执行,sh文件在Linux环境中可使用,sh文件中可以大量编写shell命令,执行sh文件相当于批量执行shell命令
(3)Tomcat服务器bin目录下提供了sh文件、bat文件,说明Tomcat的通用性。
(4)分析startup.bat文件,执行bat文件,实际执行catalina.bat文件
(5)catalina.bat文件中有配置set MAINCLASS=org.apache.catalina.startup.Bootstrap(Bootstrap类即main方法所在类)
(6)Tomcat服务器是Java语言编写的,启动Tomcat服务器即执行main方法
4、启动、关闭Tomcat服务器

(1)startup.bat
(2)shutdown.bat(shutdown命令与Windows系统中关机命令冲突,必须写shutdown.bat)
5、测试Tomcat服务器是否启动成功

(1)浏览器地址栏输入:localhost:8080
编写webapp（web应用）
1、找到CATALINA_HOME\webapps目录（Tomcat服务器要求：所有webapp存放在webapps目录下，若不存放至webapps目录下，Tomcat服务器无法找到应用）

2、CATALINA_HOME\webapps目录下新建子目录test，此目录为webapp的名字

3、test目录下新建资源文件，例如index.html

<!doctype html>
<html>
<head>
    <title>index page</title>
</head>
<body>
<h1>my index page</h1>
</body>
</html>
4、启动Tomcat服务器

5、打开浏览器，地址栏输入

localhost:8080/test/index.html
6、test目录下新建资源文件login.html

<!doctype html>
<html>
<head>
    <title>login page</title>
</head>
<body>
<form>
    <h2>user login</h2>
    username:<input type="text" name="userName"/><br>
    password:<input type="password" name="userPassword"/><br>
    <input type="submit" value="login"/>
</form>
</body>
</html>
7、打开浏览器，地址栏输入

http://localhost:8080/test/login.html
8、思考问题：浏览器地址栏输入URL回车和超链接操作一样吗

一样！
9、修改index.html资源文件，加入超链接

<!doctype html>
<html>
<head>
    <title>index page</title>
</head>
<body>
<h1>my index page</h1>
<!--超链接:相当于在浏览器地址栏输入URL-->
<a href="http://localhost:8080/test/login.html">user login</a><br>
<!--超链接中的IP地址、端口号可以省略-->
<!--以下路径为绝对路径,以"/"开头,/项目名/资源名-->
<a href="/test/login.html">user login</a>
</body>
</html>
B/S结构系统的角色和协议（重要！！）
1、test目录下新建资源文件userlist.html

<!doctype html>
<html>
<head>
    <title>user list</title>
</head>
<body>
<table border="1px" align="center" width="50%">
    <tr>
        <th>number</th>
        <th>username</th>
    </tr>
    <tr>
        <td>1</td>
        <td>jxs</td>
    </tr>
    <tr>
        <td>2</td>
        <td>dwy</td>
    </tr>
    <tr>
        <td>3</td>
        <td>lzz</td>
    </tr>
    <tr>
        <td>4</td>
        <td>jxj</td>
    </tr>
    <tr>
        <td>5</td>
        <td>jxq</td>
    </tr>
</table>
</body>
</html>
2、浏览器地址栏输入，可展示用户列表页面，但此用户列表页面为静态资源。如何成为动态资源（连接数据库）

http://localhost:8080/test/userlist.html
3、连接数据库需JDBC，即编写Java程序连接数据库。数据库中有多少条记录页面上就显示多少记录，这种技术称为动态网页技术

动态网页技术:页面中的数据根据数据库中的数据的变化而变化
4、B/S结构原理剖析图2



5、B/S结构原理剖析图2细节

(1)一个路径代表一个资源,该资源可以为静态资源、动态资源(Java小程序)
(2)根据前端浏览器发送的请求路径执行Java小程序,一个路径对应一个Servlet程序
6、对于动态Web应用，请求与响应过程有多少角色参与，角色与角色之间有多少协议

角色:
(1)浏览器软件开发团队(浏览器:谷歌浏览器、IE浏览器...)
(2)Web Server开发团队(Web Server:Tomcat、Jetty、WebLogic、JBOSS、WebSphere...)
(3)DB Server开发团队(DB Server:Oracle、MySQL...)
(4)Webapp开发团队(JavaWeb程序员)

协议:
(1)Browser开发团队、Web Server开发团队遵循HTTP协议(超文本传输协议)
(2)Webapp开发团队、Web Server开发团队遵循JavaEE规范之一:Servlet(实现Web Server、Webapp解耦)
(3)Webapp开发团队、DB Server开发团队遵循JDBC规范
7、B/S结构的系统的角色、协议图

![](E:\Study\自学课程资料\Java\assets\BS结构的系统的角色、协议图.png)

模拟Servlet本质
1、充当SUN公司，制定Servlet规范

/**
 * 充当SUN公司
 * 制定Servlet接口,制定规范
 */
public interface Servlet {
    //提供服务方法
    void service();
}
2、充当webapp开发者

/**
 * 充当webapp开发者
 * webapp开发者编写的XXXServlet都需实现Servlet接口
 */
public class UserListServlet implements Servlet {
    @Override
    public void service() {
        System.out.println("UserListServlet service");
    }
}
3、充当Tomcat服务器开发者

/**
 * 充当Tomcat开发者
 */
public class Tomcat {
    public static void main(String[] args) throws Exception {
        System.out.println("Tomcat服务器启动成功,开始接收用户访问");
        Scanner scanner = new Scanner(System.in);
        /*
        简单使用Scanner模拟用户请求
        (1)用户通过请求路径访问服务器资源
        (2)用户请求路径不同,后台执行的Servlet不同
         */
        System.out.print("请输入请求路径:");
        String key = scanner.next();
        /*
        (1)Tomcat服务器通过用户请求路径获取相应XXXServlet
        (2)web.properties配置文件中指定请求路径、XXXServlet对应关系
         */
        //解析配置文件
        FileReader fileReader = new FileReader("web.properties");
        Properties properties = new Properties();
        properties.load(fileReader);
        //由请求路径获取XXXServlet
        String value = properties.getProperty(key);
        Class<?> aClass = Class.forName(value);
        Object o = aClass.newInstance();
        //Tomcat服务器不知道o对象实例的数据类型,但Tomcat服务器知道XXXServlet一定实现Servlet接口
        Servlet servlet = (Servlet) o;
        servlet.service();
    }
}
4、请求路径、Java小程序对应关系图解



5、对于JavaWeb程序员，只需做两件事

(1)编写一个类,实现Servlet接口
(2)将编写的类配置到配置文件中,在配置文件中指定请求路径与类名的关系
6、注意事项

(1)配置文件名以及配置文件存放路径为SUN公司制定的Servlet规范中的明细
(2)遵循Servlet规范的webapp可以在不同的Web服务器中运行
(3)Servlet规范包括:规范哪些接口、规范哪些类、规范了一个webapp中该有哪些配置文件、规范了配置文件名、规范了配置文件存放路径、规范配置文件内容、规范了一个合法有效的webapp的目录结构
开发带Servlet的webapp（重中之重！！）
1、开发步骤

(1)webapps目录下新建目录test
(2)test目录下新建目录WEB-INF(注:目录名为Servlet规范中规定的,必须保持一致、必须全部大写)
(3)WEB-INF目录下新建目录classes(注:目录名为Servlet规范中规定的,必须保持一致、必须全部小写,此目录下存放Java程序编译后的class文件)
(4)WEB-INF目录下新建目录lib(注:目录名为Servlet规范中规定的,必须保持一致、必须全部小写。此目录不是必须的,若webapp需第三方jar包,则jar包须存放到该目录下。例:Java程序连接到数据库的jar包须存放到该目录下)
(5)WEB-INF目录下新建文件web.xml(注:文件名为Servlet规范中规定的,必须保持一致、必须全部小写,此文件必须存放到该目录下。web.xml为配置文件,描述请求路径与Servlet类的对应关系)
(6)编写实现Servlet接口的Java程序(注:Servlet接口不存在于JDK中,Servlet属于JavaEE规范之一,存在于另一套类库中。Oracle提供Srevlet接口(最初SUN提供Servlet接口)。Tomcat服务器也需使用Servlet接口,Tomcat服务器实现了Servlet规范)
(7)编译编写的Java程序(Java程序中导入jakarta.servlet.Servlet等包,Windows系统中需配置系统环境变量CLASSPATH=.;E:\Software Development Kit\Tomcat\apache-tomcat-10.0.27\lib\servlet-api.jar。配置的环境变量与Tomcat服务器无关,配置的环境变量只是让Java程序可正常编译为Class字节码文件)
(8)将编译后的字节码文件拷贝到WEB-INF/classes目录下
(9)web.xml文件中编写配置信息,将请求路径与Servlet类对应(在web.xml文件中注册Servlet类)
(10)启动Tomcat服务器,startup
(11)打开浏览器,地址栏输入http://localhost:8080/test/请求路径
(12)浏览器地址栏输入的URL太复杂,可以使用超链接(注:html页面只可存放到WEB-INF目录外)
//Java程序
package webapp;

import jakarta.servlet.Servlet;
import jakarta.servlet.ServletConfig;
import jakarta.servlet.ServletRequest;
import jakarta.servlet.ServletResponse;
import jakarta.servlet.ServletException;
import java.io.IOException;
import java.io.PrintWriter;

public class UserListServlet implements Servlet {

    @Override
    public void init(ServletConfig servletConfig) throws ServletException { }

    @Override
    public ServletConfig getServletConfig() { return null; }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse) throws ServletException, IOException {
        //控制台输出打印
        System.out.println("My First Servlet");
        /*
        设置响应的内容类型为普通文本或html代码
        设置响应的内容类型在获取流之前设置
         */
        servletResponse.setContentType("text/html");
        //使用ServletResponse接口将信息输出到浏览器上
        PrintWriter out = servletResponse.getWriter();
        //浏览器可识别html、css、javascript
        out.print("<h1>hello servlet</h1>");
        /*
        out属于字符输出流,负责输出字符串到浏览器
        此字符输出流无需程序员刷新、关闭,刷新、关闭由Tomcat维护
        */
    }

    @Override
    public String getServletInfo() { return null; }

    @Override
    public void destroy() { }
}
<!--web.xml内容-->
<?xml version="1.0" encoding="UTF-8"?>

<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee
                      https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0"
         metadata-complete="true">

  <!--servlet描述信息-->
  <!--servlet描述信息、servlet映射信息的servlet-name一致-->
  <servlet>
    <servlet-name>userList</servlet-name>
    <!--带包名的全限定类名-->
    <servlet-class>webapp.UserListServlet</servlet-class>
  </servlet>

  <!--servlet映射信息-->
  <servlet-mapping>
    <servlet-name>userList</servlet-name>
    <!--当前路径唯一要求必须以/开头-->
    <url-pattern>/aaa</url-pattern>
  </servlet-mapping>

</web-app>
2、注意事项

(1)web.xml文件可从其他webapp中拷贝,不易出错
(2)Servlet接口不存在于JDK中,Servlet规范不属于JavaSE,Servlet属于JavaEE规范之一,存在于另一套类库中
(3)Oracle公司提供Servlet接口,最初为SUN公司提供Servlet接口
(4)Tomcat服务器CATALINA_HOME\lib目录下存在servlet-api.jar,解压servlet-api.jar后,解压目录jakarta/servlet目录下存在Servlet.class文件
(5)jakartaEE9.0后,Servlet接口全类名从javax.servlet.Servlet变为jakarta.servlet.Servlet
(6)Java源代码位置随意,只需将Java源代码编译后的class字节码文件存放到WEB-INF/classes目录下
(7)html页面只可存放到WEB-INF目录外
(8)编写Java程序不需编写main方法,Tomcat服务器负责调用main方法,Tomcat服务器启动时执行main方法,JavaWeb程序员只需编写Servlet实现类,将实现类注册到web.xml文件中
3、web.xml模板

<?xml version="1.0" encoding="UTF-8"?>

<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee
                      https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
  version="5.0"
  metadata-complete="true">

</web-app>
4、关于JavaEE版本

(1)JavaEE目前最高版本为JavaEE8.0
(2)Oracle将JavaEE捐献给Apache
(3)Apache将JavaEE改名为jakartaEE
(4)JavaEE8.0版本升级后不再是JavaEE9.0,而是jakartaEE9.0
(5)JavaEE8.0对应的Servlet类名为javax.servlet.Servlet
(6)jakartaEE9.0对应的Servlet类名为jakarta.servlet.Servlet
(7)若项目使用javax.servlet.Servlet,则项目无法直接部署到Tomcat10+版本上,只可部署到Tomcat9-版本上。
5、DOS命令行启动Tomcat服务器乱码问题

将CATALINA_HOME/config/logging.properties文件中
java.util.logging.ConsoleHandler.encoding = UTF-8
修改为
java.util.logging.ConsoleHandler.encoding = GBK
6、总结：合法的webapp目录结构

webapps
	webapp
		WEB-INF
			classes(存放Java程序编译后的class字节码文件)
			lib(存放第三方jar包)
			web.xml(将请求路径与Servlet类对应,注册Servlet类)
		html
		css
		javascript
		image
7、浏览器地址栏输入请求路径，最终服务器调用Servlet中的方法的过程

粗糙描述:
(1)用户输入URL或点击超链接
(2)Tomcat服务器接收请求
(3)Tomcat服务器找到的对应项目
(4)Tomcat服务器在web.xml文件中查找请求路径对应的Servlet类
(5)Tomcat服务器通过反射机制创建Servlet类的对象实例
(6)Tomcat调用对应Servlet类对象实例的方法
8、webapp中编写JDBC程序连接数据库

package webapp;

import jakarta.servlet.Servlet;
import jakarta.servlet.ServletConfig;
import jakarta.servlet.ServletRequest;
import jakarta.servlet.ServletResponse;
import jakarta.servlet.ServletException;

import java.io.IOException;
import java.io.PrintWriter;
import java.sql.*;

public class UserListServlet implements Servlet {

    @Override
    public void init(ServletConfig servletConfig) throws ServletException { }

    @Override
    public ServletConfig getServletConfig() { return null; }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse) throws ServletException, IOException {
        
        servletResponse.setContentType("text/html");
        PrintWriter out = servletResponse.getWriter();

        //编写JDBC代码,连接数据库,查询所有学生信息
        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            //加载驱动类
            Class<?> driverClass = Class.forName("com.mysql.cj.jdbc.Driver");
            //获取连接
            String url = "jdbc:mysql://localhost:3306/javaweb";
            String user = "root";
            String password = "123456";
            connection = DriverManager.getConnection(url, user, password);
            //获取预编译的数据库操作对象,执行SQL语句
            String sql = "select * from student";
            preparedStatement = connection.prepareStatement(sql);
            //获取结果集
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while(resultSet.next()) {
                String id = resultSet.getString("id");
                String name = resultSet.getString("name");
                out.print(id + " " + name + "<br>");
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            if (resultSet != null) {
                try {
                    resultSet.close();
                } catch (Exception exception) {
                    System.out.println(exception.getMessage());
                }
            }

            if (preparedStatement != null) {
                try {
                    preparedStatement.close();
                } catch (Exception exception) {
                    System.out.println(exception.getMessage());
                }
            }

            if (connection != null) {
                try {
                    connection.close();
                } catch (Exception exception) {
                    System.out.println(exception.getMessage());
                }
            }
        }
    }

    @Override
    public String getServletInfo() { return null; }

    @Override
    public void destroy() { }
}
9、webapp中编写JDBC程序连接数据库总结

(1)Servlet为Java程序,在Servlet类中编写JDBC程序连接数据库
(2)webapp中连接数据库,需将数据库驱动jar包放置WEB-INF/lib目录下
(3)Servlet类编写JDBC程序连接数据库步骤:注册驱动、获取连接、获取预编译的数据库操作对象、执行SQL语句
集成开发环境中开发Servlet程序（重中之重！！）
1、集成开发工具

(1)IntelliJ IDEA(IDEA在提示功能方面强于Eclipse,IDEA的使用比Eclipse更加智能,IDEA为JetBrain公司开发)
(2)Eclipse(使用Eclipse作为集成开发工具的团队日趋减少,Eclipse是IBM团队开发的,Eclipse寓意"日食",表示将太阳(SUN)吞并,Oracle公司2009年收购SUN公司,IBM并没有成功收购SUN公司)
2、使用IntelliJ IDEA集成开发工具开发Servlet

(1)new Project(习惯:新建Empty Project(空工程),在Empty Project中新建Module(模块)),将Empty Project(空工程名起名为JavaWeb,新建的Empty Project名字和目录名一致)
(2)new Module(File -> New -> Module),新建普通的JavaSE模块,此Module自动存放至JavaWeb工程下
(3)Module添加框架支持(让Module符合Servlet规范),右击Module -> Add Frameworks Support -> Web Application,选择Web Application支持后,IDEA自动生成符合Servlet规范的webapp目录结构,IDEA集成开发工具中根据Web Application模板生成的目录中存在web目录,此目录代表webapp的根
(4)编写Servlet类,此Servlet类需实现Servlet接口,此时需要Servlet.class文件。将CATALINA_HOME/lib/servlet-api.jar、jsp-api.jar添加到classpath中。(File -> Project Structrue -> Modules ->  + -> JARs or Directories)。实现jakarta.servlet.Servlet接口中5个方法
(5)在Servlet类中的service方法中编写业务代码,使用JDBC连接数据库。WEB-INF目录下新建lib目录,将连接数据库的驱动jar包放置lib目录下
(6)在web.xml文件中完成Servlet类注册(将请求路径与Servlet类对应)
(7)设置html页面,html页面中设置超链接,用户点击超链接发送请求,Tomcat服务器执行后台的StudentServlet类(编写student.html文件,此文件放置WEB-INF同级目录下)
(8)IntelliJ IDEA集成开发工具关联Tomcat服务器,关联过程中将webapp部署到Tomcat服务器中(IntelliJ IDEA集成开发工具右上角绿色小锤旁Add Configuration -> + -> Tomcat Server -> local -> 弹出的界面中设置Tomcat服务器参数 -> Deployment部署webapp -> 修改Application context为/aaa)
(9)启动Tomcat服务器(IntelliJ IDEA集成开发工具右上角绿色箭头或绿色小虫,可以采用debug模式启动Tomcat服务器,开发中建议使用debug模式启动Tomcat服务器)
(10)打开浏览器,地址栏输入http://localhost:8080/aaa/student.html
3、StudentServlet类

package javaweb.servlet;

import jakarta.servlet.*;

import java.io.IOException;
import java.io.PrintWriter;
import java.sql.*;

public class StudentServlet implements Servlet {
    @Override
    public void init(ServletConfig servletConfig) throws ServletException { }

    @Override
    public ServletConfig getServletConfig() { return null; }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        //设置响应的内容类型
        servletResponse.setContentType("text/html");
        PrintWriter out = servletResponse.getWriter();
        //连接数据库
        ResultSet resultSet = null;
        PreparedStatement preparedStatement = null;
        Connection connection = null;
        try {
            //注册驱动类
            Class<?> driverClass = Class.forName("com.mysql.cj.jdbc.Driver");
            //获取连接
            String url = "jdbc:mysql://localhost:3306/javaweb";
            String user = "root";
            String password = "123456";
            connection = DriverManager.getConnection(url, user, password);
            //获取预编译的数据库操作对象
            String sql = "select * from student";
            preparedStatement = connection.prepareStatement(sql);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {
                String id = resultSet.getString("id");
                String name = resultSet.getString("name");
                out.print(id + "," + name + "<br>");
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            if (resultSet != null) {
                try {
                    resultSet.close();
                } catch (SQLException throwable) {
                    System.out.println(throwable.getMessage());
                }
            }
            if (preparedStatement != null) {
                try {
                    preparedStatement.close();
                } catch (SQLException throwable) {
                    System.out.println(throwable.getMessage());
                }
            }
            if (connection != null) {
                try {
                    connection.close();
                } catch (SQLException throwable) {
                    System.out.println(throwable.getMessage());
                }
            }
        }
    }

    @Override
    public String getServletInfo() { return null; }

    @Override
    public void destroy() { }
}
4、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="http://xmlns.jcp.org/xml/ns/javaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://xmlns.jcp.org/xml/ns/javaee http://xmlns.jcp.org/xml/ns/javaee/web-app_4_0.xsd"
         version="4.0">
    <servlet>
        <servlet-name>studentServlet</servlet-name>
        <servlet-class>javaweb.servlet.StudentServlet</servlet-class>
    </servlet>

    <servlet-mapping>
        <servlet-name>studentServlet</servlet-name>
        <url-pattern>/bbb</url-pattern>
    </servlet-mapping>
</web-app>
5、student.html文件

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>student page</title>
</head>
<body>
<!--
aaa为项目名
bbb为资源名
-->
<a href="/aaa/bbb">student list</a>
</body>
</html>
Servlet对象生命周期（重中之重！！）
1、何为Servlet对象生命周期?

(1)Servlet对象生命周期:一个Servlet对象从创建到销毁的过程
(2)Servlet对象何时被创建?
(3)Servlet对象何时被销毁?
(4)创建几个Servlet对象?
2、Servlet对象由谁维护

(1)Servlet对象的创建、Servlet对象方法的调用、Servlet对象的销毁,JavaWeb程序员无权干涉。
(2)Servlet对象的生命周期由Tomcat服务器(Web Server)全权负责
(3)Tomcat服务器通常我们又称Tomcat容器(Web Container)
(4)Web容器来管理Servlet对象
3、思考：Web容器是否管理JavaWeb程序员创建的Servlet对象?

(1)Web容器不管理JavaWeb程序员创建的Servlet对象
(2)Web容器创建的Servlet对象会放置到HashMap集合中,只有放置到HashMap集合中的Servlet对象才会被Web容器管理,JavaWeb程序员创建的Servlet对象不在Web容器中,不会被Web容器管理
(3)Web容器底层存在HashMap集合,集合中存储Servlet对象和请求路径对应关系
4、默认情况下Tomcat服务器启动时Servlet对象是否被创建

(1)Servlet类中提供无参构造方法,启动Tomcat服务器时无参构造方法是否运行
(2)默认情况下,Tomcat服务器在启动时不会创建Servlet对象实例
(3)此设计合理,用户发送请求前创建出Servlet对象是损耗内存的
5、如何使Tomcat服务器启动时创建Servlet对象

(1)web.xml文件<servlet></servlet>标签中添加<load-on-startup></load-on-startup>子标签,在该标签中填写整数,整数越小优先级越高
<servlet>
    <servlet-name>AServlet</servlet-name>
    <servlet-class>javaweb.servlet.AServlet</servlet-class>
    <load-on-startup>0</load-on-startup>
</servlet>

<servlet-mapping>
    <servlet-name>AServlet</servlet-name>
    <url-pattern>/a</url-pattern>
</servlet-mapping>
6、Servlet对象生命周期

//Servlet类
package javaweb.servlet;

import jakarta.servlet.*;
import java.io.IOException;

public class AServlet implements Servlet {

    //无参构造方法
    public AServlet() {
        System.out.println("AServlet无参构造方法执行");
    }

    @Override
    public void init(ServletConfig servletConfig) throws ServletException {
        System.out.println("AServlet init method execute");
    }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        System.out.println("AServlet service method execute");
    }

    @Override
    public void destroy() {
        System.out.println("AServlet destroy method execute");
    }

    @Override
    public ServletConfig getServletConfig() { return null; }

    @Override
    public String getServletInfo() { return null; }
}
(1)默认情况下启动Tomcat服务器时AServlet对象没有被实例化
(2)用户发送第一次请求时控制台输出以下内容:
AServlet无参构造方法执行
AServlet init method execute
AServlet service method execute
(3)根据以上输出内容得出结论:
3.1用户在发送第一次请求时AServlet对象被实例化(AServlet的无参构造方法被执行)
3.2AServlet对象创建后,Tomcat服务器调用AServlet对象的init方法(init方法执行前AServlet对象已经被实例化)
3.2用户发送第一次请求,AServlet对象被实例化,init方法执行后,Tomcat服务器调用AServlet对象的service方法
(4)用户发送第二次请求时控制台输出以下内容:
AServlet service method execute
(5)根据以上输出内容得出结论:
5.1用户在发送第二次请求时,AServlet对象并没有新建,直接调用AServlet对象的service方法(Servlet对象为单例的,但Servlet类不符合单例模式,我们称之为假单例。因为JavaWeb程序员无法创建Servlet对象,Servlet对象由Tomcat服务器创建,Tomcat只创建一个Servlet对象,所以导致单例。真单例模式构造方法为私有方法)
5.2无参构造方法、init方法只在用户发送第一次请求时执行,即Tomcat服务器只调用一次无参构造方法、init方法
5.3用户发送一次请求,Tomcat服务器执行一次service方法
(6)关闭Tomcat服务器时控制台输出以下内容:
AServlet service method execute
(7)根据以上输出内容得出结论:
7.1在Tomcat服务器关闭时执行Servlet对象的destroy方法,destroy方法只被Tomcat服务器调用一次。
7.2Tomcat服务器在销毁AServlet对象内存之前,Tomcat服务器会自动调用AServlet对象的destroy方法
(8)destroy方法执行时AServlet对象仍存在,destroy方法执行结束后AServlet对象的内存被Tomcat服务器释放。
7、Servlet类方法调用次数

(1)执行1次构造方法
(2)执行1次init方法
(3)执行1次destroy方法
(4)用户发送1次请求执行1次service方法
8、JavaWeb程序员在Servlet类中手动编写有参构造方法，有参构造方法会覆盖原有的无参构造方法，若JavaWeb程序员不手动编写无参构造方法出现什么问题？

(1)HTTP状态 500 - 内部服务器错误(注:500是HTTP协议的错误状态码,一般因为Tomcat服务器端Java程序出现异常,即服务器内部错误)
(2)若Servlet类中无无参构造方法,会导致500错误,无法实例化Servlet对象。即在Servlet开发中不建议JavaWeb程序员自定义构造方法
9、Servlet无参构造方法在创建Servlet对象时执行1次，init方法在创建完Servlet对象后执行1次。可以将无参构造方法代替init方法吗？(即将init方法代码块中的内容转移到无参构造方法代码块中)

(1)Servlet规范中不建议JavaWeb程序员编写无参构造方法
(2)JavaWeb程序员编写构造方法很容易让无参构造方法消失,导致Servlet对象无法实例化。
(3)为避免此操作,由此引出init方法
10、init、service、destroy方法使用次数比较

(1)使用次数最多的为service方法,service方法为处理用户请求的核心方法
(2)使用次数较少的为init方法,init方法执行初始化操作,比如:初始化数据库连接池、初始化线程池...
(3)使用次数较少的为destroy方法,destroy方法执行资源操作
11、Servlet对象生命周期总结

(1)Tomcat服务器启动时,web.xml文件中<servlet></servlet>标签中存在<load-on-startup></load-on-startup>标签则创建Servlet对象;若无此标签则不创建Servlet对象。用户发送第一次请求时,通过请求路径找到对应Servlet类,通过反射机制调用Servlet类的无参构造方法创建Servlet对象,创建Servlet对象后调用Servlet对象init方法,调用init方法后再调用Servlet对象service方法。用户发送第二次请求时,通过请求路径在Web容器中找对应的Servlet类对象是否被创建,若找到,则直接调用该Servlet对象的service方法。关闭Tomcat服务器时,Tomcat服务器自动调用Servlet对象destroy方法,destroy方法执行时Servlet对象仍存在,destroy方法执行后Servlet对象的内存被Tomcat服务器释放。destroy方法中可以编写释放Servlet对象前的准备,比如:AServlet对象开启了流、数据库连接,即关闭流、数据库连接的代码可以写入destroy方法中
(2)Servlet对象生命周期就好比一个人的一生:Servlet无参构造方法执行标志着人的出生、Servlet对象init方法执行标志着人接受教育、Servlet对象service方法执行标志着为人类提供服务、Servlet对象destroy方法执行标志着临终前的遗言。
适配器设计模式（看总结！！）
1、编写Servlet类直接实现Servlet接口缺点

(1)大部分情况下只需service方法,其他方法不需使用
2、适配器设计模式adapter

(1)若手机直接插入到220V的电压则直接报废,可以选择充电器,此充电器就相当于适配器。手机连接充电器,充电器连接220V电压
3、编写ServletAdapter类，该类为抽象类，ServletAdapter类存在抽象方法service

(1)ServletAdapter类实现Servlet接口
(2)ServletAdapter类为适配器
(3)此后编写的Servlet类继承ServletAdapter类,重写service方法
4、思考：ServletAdapter类是否需要改进？如何改进更利用子类程序的编写？

(1)第一个问题:提供ServletAdapter适配器类后,init方法会执行吗?(会,会执行ServletAdapter类中的init方法)
(2)第二个问题:谁调用init方法?(Tomcat服务器)
(3)第三个问题:谁创建init方法参数列表中ServletConfig对象?谁传输?(Tomcat服务器。Tomcat服务器先创建ServletConfig对象,再调用init方法,最后将ServletConfig对象传输给init方法)
5、JavaWeb程序员编写的ServletAdapter适配器类

package javaweb.servlet;

import jakarta.servlet.*;
import java.io.IOException;

/**
 * 编写标准通用的Servlet类,起名ServletAdapter
 * Servlet类无需直接实现Servlet接口
 * Servlet类直接继承ServletAdapter类
 * ServletAdapter类为一个适配器
 */
public abstract class ServletAdapter implements Servlet {
    //成员变量
    private ServletConfig servletConfig;

    /**
     * Tomcat服务器创建ServletConfig对象
     * 将ServletConfig对象传入init方法
     * ServletConfig对象为局部变量
     * 若ServletConfig对象需在service方法中使用,则将ServletConfig对象从局部变量提升为成员变量
     * @param servletConfig
     * @throws ServletException
     */
    @Override
    public final void init(ServletConfig servletConfig) throws ServletException {
        this.servletConfig = servletConfig;
        this.init();
    }

    /**
     * 此init方法供子类重写
     */
    public void init() { }

    @Override
    public ServletConfig getServletConfig() {
        return servletConfig;
    }

    /**
     * 抽象方法,此方法最常用,子类必须实现service方法
     * @param servletRequest
     * @param servletResponse
     * @throws ServletException
     * @throws IOException
     */
    @Override
    public abstract void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException;

    @Override
    public String getServletInfo() { return null; }

    @Override
    public void destroy() { }
}
6、JavaWeb程序员编写的ServletAdapter适配器类继承子类

public class AServlet extends ServletAdapter{
    /*
    若需在AServlet类中重写init方法,步骤?
    (1)父类将init方法用final关键字修饰,子类无法重写init方法
    (2)父类定义不被final修饰的init方法,子类重写该init方法
    (3)父类被final修饰的init方法中调用不被final修饰的init方法
     */
    @Override
    public void init(){
        System.out.println("AServlet init method execute");
    }

    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        ServletConfig servletConfig = this.getServletConfig();
    }
}
7、手撕官方GenericServlet源码第一阶段

public abstract class GenericServlet implements Servlet, ServletConfig, Serializable {
    //序列化版本号
    private static final long serialVersionUID = 1L;
    //被transient修饰的属性不可被序列化
    private transient ServletConfig config;
    //无参构造方法
    public GenericServlet() { }
    //init方法,将参数列表中传入的ServletConfig config对象赋给GenericServlet类的成员变量config,并执行无参init方法
    public void init(ServletConfig config) throws ServletException {
        this.config = config;
        this.init();
    }
    //getServletConfig方法,返回ServletConfig对象
    public ServletConfig getServletConfig() { return this.config; }
    //提供给子类重写的init方法,无参init方法
    public void init() throws ServletException { }
    //service方法,用户发送1次请求执行1次service方法
    public abstract void service(ServletRequest var1, ServletResponse var2) throws ServletException, IOException;
    //destroy方法
    public void destroy() { }

    public String getInitParameter(String name) {
        return this.getServletConfig().getInitParameter(name);
    }

    public Enumeration<String> getInitParameterNames() {
        return this.getServletConfig().getInitParameterNames();
    }

    public ServletContext getServletContext() {
        return this.getServletConfig().getServletContext();
    }

    public String getServletInfo() { return ""; }

    public void log(String message) {
        this.getServletContext().log(this.getServletName() + ": " + message);
    }

    public void log(String message, Throwable t) {
        this.getServletContext().log(this.getServletName() + ": " + message, t);
    }

    public String getServletName() { return this.config.getServletName(); }
}
8、总结

(1)编写Servlet类,Servlet类实现Servlet接口必须实现Servlet接口中所有方法。大多数情况下只需service方法。
(2)Servlet类继承适配器抽象类GenericServlet,实现GenericServlet类中唯一抽象方法service
(3)用户发送请求,通过请求路径找到对应Servlet类,再通过反射机制调用Servlet类的无参构造方法创建Servlet对象。
(4)调用Servlet对象的有参init方法,若Servlet类中没有重写init方法则默认调用GenericServlet类的有参init方法。
(5)调用有参init方法前,Tomcat服务器创建ServletConfig对象,将ServletConfig对象传入有参init方法
(6)init方法中将传入的ServletConfig对象赋给GenericServlet类中的成员变量ServletConfig config,再执行无参init方法
(7)若Servlet类需重写init方法,可以重写无参init方法,若重写有参init方法可能会导致GenericServlet类中成员变量ServletConfig config为空,导致GenericServlet类中getServletConfig方法返回值为空。
ServletConfig接口详解（重中之重！！）
1、何为ServletConfig？

(1)jakarta.servlet.ServletConfig
(2)ServletConfig为Servlet规范中的一员
(3)ServletConfig为1个接口,jakarta.servlet.Servlet也为1个接口
2、谁去实现ServletConfig接口

(1)编写ServletConfigTest类继承GenericServlet类
(2)用户第一次发送请求,Tomcat服务器通过反射机制调用ServletConfigTest类无参构造方法创建ServletConfigTest对象实例,再调用ServletConfigTest对象的有参init方法,若ServletConfigTest类没有重写父类GenericServlet类的有参init方法,则默认调用父类的有参init方法
(3)执行有参init方法前,Tomcat服务器会创建ServletConfig config对象传入有参init方法,将传入的ServletConfig config对象赋给GenericServlet类中的成员变量ServletConfig config
(4)GenericServlet类中提供getServletConfig方法,返回GenericServlet类中的成员变量ServletConfig config
(5)ServletConfigTest类中的service方法中调用getServletConfig方法并在浏览器输出,得到org.apache.catalina.core.StandardWrapperFacade@1037dc6b,即StandardWrapperFacade类实现ServletConfig接口
(6)结论:Tomcat服务器实现ServletConfig接口。若将Tomcat服务器换成Jetty服务器,输出ServletConfig对象时包名可能不相同,但接口名一定为ServletConfig
3、1个Servlet对象对应1个ServletConfig对象

(1)创建ServletConfigTest01类、ServletConfigTest02类,分别继承GenericServlet类
(2)ServletConfigTest01、ServletConfigTest02类中service方法调用getServletConfig方法,并在浏览器输出ServletConfig对象,输出内容如下:
org.apache.catalina.core.StandardWrapperFacade@3c419fae
org.apache.catalina.core.StandardWrapperFacade@275eeea6
4、谁创建ServletConfig对象？何时创建ServletConfig对象？

(1)Tomcat服务器创建ServletConfig对象
(2)创建Servlet对象时创建ServletConfig对象
5、ServletConfig接口作用

(1)Config为Configuration缩写
(2)ServletConfig对象可理解为Servlet对象的配置信息对象
(3)1个Servlet对象对应1个ServletConfig对象,即1个Servlet对象对应1个Servlet对象的配置信息对象
6、ServletConfig对象中包装的信息

<servlet>
    <servlet-name>servletConfig01</servlet-name>
    <servlet-class>javaweb.ServletConfigTest01</servlet-class>
    <!--Servlet对象初始化信息-->
    <init-param>
        <param-name>driver</param-name>
        <param-value>com.mysql.cj.jdbc.Driver</param-value>
    </init-param>
    <init-param>
        <param-name>url</param-name>
        <param-value>jdbc:mysql://localhost:3306/javaweb</param-value>
    </init-param>
    <init-param>
        <param-name>user</param-name>
        <param-value>root</param-value>
    </init-param>
    <init-param>
        <param-name>password</param-name>
        <param-value>123456</param-value>
    </init-param>
</servlet>

(1)ServletConfig对象中包装的信息:对应的Servlet对象在web.xml文件中<servlet></servlet>标签的配置信息
(2)Tomcat服务器解析web.xml文件,将web.xml文件中<servlet></servlet>标签中的配置信息自动包装到对应的servletConfig对象中
7、ServletConfig对象方法解析

(1)getServletName():获取ServletConfig对象对应的Servlet对象在web.xml文件<servlet-name></servlet-name>标签中的信息
(2)getInitParamterNames():获取ServletConfig对象对应的Servlet对象在web.xml文件<init-param></init-param>标签中<param-name></param-name>标签中的信息
(3)getInitParameter():获取<param-name></param-name>标签对应的<param-value></param-value>标签中的信息
(4)getServletContext():
package javaweb;

import jakarta.servlet.*;
import java.io.IOException;
import java.io.PrintWriter;
import java.util.Enumeration;

public class ServletConfigTest01 extends GenericServlet {
    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        servletResponse.setContentType("text/html");
        PrintWriter out = servletResponse.getWriter();
        //获取ServletConfig对象实例,ServletConfig对象中包装的信息为对应的Servlet对象在web.xml文件中<servlet></servlet>标签中的信息
        ServletConfig servletConfig = this.getServletConfig();
        //输出ServletConfig对象
        out.print(servletConfig);
        //换行
        out.print("<br>");
        //获取ServletConfig对象对应的Servlet对象在web.xml文件中<servlet-name></servlet-name>标签中的信息
        out.print(servletConfig.getServletName());
        //换行
        out.print("<br>");
        //获取ServletConfig对象对应的Servlet对象在web.xml文件中<init-param></init-param>标签中<param-name></param-name>标签中的信息
        Enumeration<String> initParameterNames = servletConfig.getInitParameterNames();
        //遍历集合,判断是否有更多元素
        while (initParameterNames.hasMoreElements()) {
            //取出每一元素
            String parameterName = initParameterNames.nextElement();
            //获取<param-name></param-name>标签对应的<param-value></param-value>标签中的信息
            String parameterValue = servletConfig.getInitParameter(parameterName);
            out.print(parameterName + "=" + parameterValue + "<br>");
        }
    }
}
8、修改Java代码需重启Tomcat服务器才可生效，进行配置不需重启Tomcat服务器即可生效代码，当修改Servlet类代码以及光标脱离IntelliJ IDEA集成开发工具时不需重启Tomcat服务器即可生效代码

IntelliJ IDEA集成开发工具右上角绿色小锤旁Edit Configurations... -> On 'Update' action & On frame deactivation -> Update classes and resources
9、手撕官方GenericServlet源码第二阶段

public abstract class GenericServlet implements Servlet, ServletConfig, Serializable {
    //序列化版本号
    private static final long serialVersionUID = 1L;
    //被transient修饰的属性不可被序列化
    private transient ServletConfig config;
    //无参构造方法
    public GenericServlet() { }
    //init方法,将参数列表中传入的ServletConfig config对象赋给GenericServlet类的成员变量config,并执行无参init方法
    public void init(ServletConfig config) throws ServletException {
        this.config = config;
        this.init();
    }
    //getServletConfig方法,返回ServletConfig对象
    public ServletConfig getServletConfig() { return this.config; }
    //提供给子类重写的init方法,无参init方法
    public void init() throws ServletException { }
    //service方法,用户发送1次请求执行1次service方法
    public abstract void service(ServletRequest var1, ServletResponse var2) throws ServletException, IOException;
    //destroy方法
    public void destroy() { }
    //获取ServletConfig配置信息对象对应的Servlet对象在web.xml文件中<init-param></init-param>标签中<param-name></param-name>标签中的信息
    public Enumeration<String> getInitParameterNames() {
        return this.getServletConfig().getInitParameterNames();
    }
    //获取<param-name></param-name>标签对应的<param-value></param-value>标签中的信息
    public String getInitParameter(String name) {
        return this.getServletConfig().getInitParameter(name);
    }
    //获取ServletConfig对象对应的Servlet对象在web.xml文件中<servlet-name></servlet-name>标签中的信息
    public String getServletName() { return this.config.getServletName(); }

    public ServletContext getServletContext() {
        return this.getServletConfig().getServletContext();
    }

    public void log(String message) {
        this.getServletContext().log(this.getServletName() + ": " + message);
    }

    public void log(String message, Throwable t) {
        this.getServletContext().log(this.getServletName() + ": " + message, t);
    }
}
ServletContext接口详解（重中之重！！）
1、ServletConfig接口4个方法

(1)public String getServletName();
(2)public ServletContext getServletContext();
(3)public Enumeration<String> getInitParameterNames();
(4)public String getInitParameter(String name);
(5)以上4个方法在JavaWeb程序员编写的Servlet类中可以使用this调用(此Servlet类继承GenericServlet)
2、获取ServletContext方式

(1)通过ServletConfig对象getServletContext()方法获取ServletContext对象
(2)通过this关键字调用getServletContext()方法获取ServletContext对象
3、何为ServletContext？

(1)jakarta.servlet.ServletContext
(2)ServletContext为接口
(3)ServletContext为Servlet规范中的一员
4、谁实现ServletContext接口？

Tomcat服务器实现ServletContext接口
public class org.apache.catalina.core.ApplicationContextFacade implements ServletContext {}
5、谁创建ServletContext对象？何时创建？创建个数？何时销毁？

(1)ServletContext对象是Tomcat服务器创建的
(2)ServletContext对象在Tomcat服务器启动时创建
(3)对于一个webapp,ServletContext对象只有1个
(4)ServletContext对象在Tomcat服务器关闭时销毁
6、ServletContext如何理解

(1)context:上下文、环境
(2)ServletContext对象为Servlet对象的环境对象、上下文对象
(3)ServletContext对象对应的为web.xml文件。
(4)50个学生,每个学生为1个Servlet对象,50个学生在1个班级中,此班级就相当于ServletContext对象。存放在ServletContext对象中的数据被所有Servlet对象共享,班级中的空调、风扇、黑板被所有学生共享
(5)Tomcat服务器为Web容器,Web容器中可存放多个webapp,1个webapp对应1个ServletContext对象
7、ServletContext理解扩展

(1)ServletContext对象又称应用域
(2)若一份数据被所有Servlet对象共享、数据量小、很少修改此数据,则可以将此数据存放到ServletContext应用域中
(3)为何需数据量小?Tomcat服务器启动时创建ServletContext对象,Tomcat服务器关闭时销毁ServletContext对象,生命周期较长。若数据量大则会导致服务器性能下降、大量占用堆内存
(4)为何需很少修改此数据?此数据被所有Servlet对象共享,涉及修改操作时存在线程并发所带来的安全问题
(5)数据量小、很少修改、所有用户共享的数据可存放到ServletContext应用域中,从而大大提高效率
(6)ServletContext应用域相当于一个缓存,存放至缓存中的数据,下次使用时无需再从数据库中获取,大大提高效率
(7)ServletContext应用域如何存取删数据?
	存:void setAttribute(String name, Object value);
	取:Object getAttribute(String name);
	删:void removeAttribute(String name);
8、ServletContext接口重要方法

(1)Enumeration<String> getInitParameterNames();//获取<context-param></context-param>标签中<param-name></param-name>标签中的信息
(2)String getInitParameter(String name);//获取<param-name></param-name>标签对应的<param-value></param-value>标签中的信息
(3)String getContextPath();//动态获取webapp(应用)的根路径
(4)String getRealPath(String path);//动态获取webapp(应用)目录下任意文件的绝对路径
(5)void log(String message);//记录日志到CATALINA_HOME/logs目录下
(6)void log(String message, Throwable throwable);
(7)Object getAttribute(String name);//获取ServletContext应用域中的数据
(8)void setAttribute(String name, Object value);//存放数据至ServletContext应用域
(9)void removeAttribute(String name);//删除ServletContext应用域中的数据
9、ServletContext接口方法解析

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">

    <!--配置ServletContext对象的初始化参数-->
    <context-param>
        <param-name>pageSize</param-name>
        <param-value>10</param-value>
    </context-param>


    <servlet>
        <servlet-name>aServlet</servlet-name>
        <servlet-class>javaweb.servlet.AServlet</servlet-class>
        <!--配置ServletConfig对象的初始化参数-->
        <init-param>
            <param-name>driver</param-name>
            <param-value>com.mysql.cj.jdbc.Driver</param-value>
        </init-param>
        <init-param>
            <param-name>url</param-name>
            <param-value>jdbc:mysql://localhost:3306/javaweb</param-value>
        </init-param>
        <init-param>
            <param-name>user</param-name>
            <param-value>root</param-value>
        </init-param>
        <init-param>
            <param-name>password</param-name>
            <param-value>123456</param-value>
        </init-param>
    </servlet>
    <servlet-mapping>
        <servlet-name>aServlet</servlet-name>
        <url-pattern>/a</url-pattern>
    </servlet-mapping>

    <servlet>
        <servlet-name>bServlet</servlet-name>
        <servlet-class>javaweb.servlet.BServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>bServlet</servlet-name>
        <url-pattern>/b</url-pattern>
    </servlet-mapping>
</web-app>
package javaweb.servlet;

import jakarta.servlet.*;
import java.io.IOException;
import java.io.PrintWriter;
import java.util.Enumeration;

public class AServlet extends GenericServlet {
    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse) throws ServletException, IOException {
        servletResponse.setContentType("text/html");
        PrintWriter out = servletResponse.getWriter();
        //获取ServletContext对象
        ServletContext servletContext = this.getServletContext();
        //输出ServletContext对象
        out.print(servletContext + "<br>");
        //获取ServletContext对象的初始化参数
        Enumeration<String> initParameterNames = servletContext.getInitParameterNames();
        //while循环遍历ServletContext对象的所有初始化参数名、初始化参数值
        while (initParameterNames.hasMoreElements()) {
            String initParameterName = initParameterNames.nextElement();
            String initParameterValue = servletContext.getInitParameter(initParameterName);
            out.print(initParameterName + ":" + initParameterValue + "<br>");
        }
        //获取webapp(应用)的根路径
        String contextPath = servletContext.getContextPath();
        out.print(contextPath + "<br>");
        //获取webapp(应用)下任意文件的绝对路径
        String realPath1 = servletContext.getRealPath("/JavaScript/test.html");
        String realPath2 = servletContext.getRealPath("JavaScript/test.html");
        out.print(realPath1 + "<br>");
        out.print(realPath2 + "<br>");
        //记录日志
        servletContext.log("南理工紫金蒋兴树");
        //日志中记录异常信息
        int age = 17;
        if (age < 18) {
            servletContext.log("您未成年", new RuntimeException("未成年人请勿进入"));
        }
        //创建User对象实例
        User user = new User("jxs", "123");
        //存放数据至ServletContext应用域
        servletContext.setAttribute("userObj", user);
        //获取ServletContext应用域中的数据
        Object userObj = servletContext.getAttribute("userObj");
        out.print(userObj);
        //删除ServletContext应用域中的数据
        servletContext.removeAttribute("userObj");
    }
}
10、ServletConfig对象初始化参数与ServletContext初始化参数区别

(1)1个ServletContext对象,对应1个web.xml文件,对应1个webapp,ServletContext对象初始化参数属于应用级别的配置信息,该配置信息被1个web.xml文件中的所有Servlet对象共享
(2)ServletConfig对象为Servlet对象的配置信息对象,1个ServletConfig对象对应1个Servlet对象,ServletConfig对象初始化参数被对应的Servlet对象独享
11、IntelliJ IDEA集成开发工具中Tomcat服务器log（日志）存放位置

![](E:\Study\自学课程资料\Java\assets\IntelliJ IDEA集成开发工具中Tomcat服务器log（日志）存放位置.png)

12、Tomcat服务器日志类别

catalina.2023-01-20.log:存放Tomcat服务器端java程序运行的控制台信息
localhost.2023-01-20.log:存放ServletContext对象log方法记录的日志信息
localhost_access_log.2023-01-20.txt:存放访问日志信息
手撕官方GenericServlet源码（重中之重！！）
1、GenericServlet源码

public abstract class GenericServlet implements Servlet, ServletConfig, Serializable {
    //序列化版本号
    private static final long serialVersionUID = 1L;
    //被transient修饰的属性不可被序列化
    private transient ServletConfig config;
    //无参构造方法
    public GenericServlet() { }
    //init方法,将参数列表中传入的ServletConfig config对象赋给GenericServlet类的成员变量config,并执行无参init方法
    public void init(ServletConfig config) throws ServletException {
        this.config = config;
        this.init();
    }
    //getServletConfig方法,返回ServletConfig对象
    public ServletConfig getServletConfig() { return this.config; }
    //提供给子类重写的init方法,无参init方法
    public void init() throws ServletException { }
    //service方法,用户发送1次请求执行1次service方法
    public abstract void service(ServletRequest var1, ServletResponse var2) throws ServletException, IOException;
    //destroy方法
    public void destroy() { }
    //获取ServletConfig配置信息对象对应的Servlet对象在web.xml文件中<init-param></init-param>标签中<param-name></param-name>标签中的信息
    public Enumeration<String> getInitParameterNames() {
        return this.getServletConfig().getInitParameterNames();
    }
    //获取<param-name></param-name>标签对应的<param-value></param-value>标签中的信息
    public String getInitParameter(String name) {
        return this.getServletConfig().getInitParameter(name);
    }
    //获取ServletConfig对象对应的Servlet对象在web.xml文件中<servlet-name></servlet-name>标签中的信息
    public String getServletName() { return this.config.getServletName(); }
    //getServletContext方法,返回ServletContext对象
    public ServletContext getServletContext() {
        return this.getServletConfig().getServletContext();
    }
    //记录日志至CATALINA_HOME/logs目录下
    public void log(String message) {
        this.getServletContext().log(this.getServletName() + ": " + message);
    }
    //记录日志中的异常信息
    public void log(String message, Throwable t) {
        this.getServletContext().log(this.getServletName() + ": " + message, t);
    }
}
2、注意事项

(1)此后编写Servlet类时无需继承GenericServlet类,因为B/S结构的系统是基于HTTP超文本传输协议的,Servlet规范中提供了HttpServlet类(专门为HTTP超文本传输协议准备的Servlet类),使用HttpServlet处理HTTP超文本传输协议更便捷
3、HttpServlet继承结构

![](E:\Study\自学课程资料\Java\assets\HttpServlet继承结构.png)

4、JVM常量池

Java6以及6之前,常量池存放在方法区中
Java7,常量池存放在堆中
Java8,取消方法区,取而代之的是元空间,运行时常量池和静态常量池存放在元空间中,而字符串常量池依然存放在堆中。
5、缓存机制

(1)堆内存中的字符串常量池
	String s = new String("jxs");
	堆中创建String对象,String对象的value属性指向字符串常量池中对应字符串的地址
	若字符串常量池中存在"jxs",则value属性指向字符串常量池中"jxs"的地址
	若字符串常量池中不存在"jxs",则新建"jxs"将其放入字符串常量池
(2)堆内存中的整数型常量池
	存放[-128~127]共256个Integer引用
	通过new Integer()方式创建Integer对象,不管传入的值是否相等,Integer对象的地址都不相等
	通过Integer.valueOf()方式创建Integer对象,在-128 ~ +127范围内为同一个对象,超出此范围则通过new Integer()的方式创建Integer对象
(3)连接池
	将创建好的java.sql.Connection连接对象存放在连接池中,当用户请求连接数据库时直接使用创建好的Connection连接对象对数据库进行访问,无需新建连接以及销毁连接,提高性能
(4)线程池
	所有Web服务器都支持多线程,都存在线程池。Tomcat服务器启动时,创建N个Thread线程对象,将Thread线程对象存放在线程池中。当用户发送请求时直接使用创建好的Thread线程对象,提高性能
(5)redis
	NoSQL数据库,非关系型数据库,缓存数据库
(6)ServletContext应用域中存储数据相当于将数据存入缓存cache中
HTTP协议剖析
1、何为协议？

(1)某些人或某些组织制定的一套规范、一套标准。按照此规范、此标准可以沟通无障碍
(2)就好比中国人遵守汉语协议即可以做到沟通无障碍
2、何为HTTP协议？

(1)W3C(World Wide Web Consortium-世界万维网联盟),制定了HTTP、HTML4.0、HTML5、DOM等规范,世界万维网联盟之父:蒂姆·伯纳斯·李
(2)HTTP协议是W3C制定的一种超文本传输协议(通信协议)
(3)HTTP协议游走在B(Browser)与S(Server)之间,Browser向Server发送数据须遵循HTTP协议,Server向Browser发送数据也须遵循HTTP协议,如此Browser与Server之间才可解耦
(4)解耦:Web服务器不依赖具体的浏览器(火狐、Chrome、IE都可);浏览器也不依赖具体的Web服务器(Tomcat、Jetty都可)。Browser不依赖Server,Server不依赖Browser
(5)超文本:不是普通文本,比如:图片、视频、声音
(6)B/S表示B/S架构的系统
Browser向Server发送数据叫做Request
Server向Browser发送数据叫做Response
(7)HTTP协议包括请求协议、响应协议。
请求协议:浏览器向服务器发送数据时遵循一套规范、一套标准,这套标准中规定了发送数据的具体格式。
响应协议:服务器向浏览器发送数据时遵循一套规范、一套标准,这套标准中规定了发送数据的具体格式。
(8)HTTP协议即消息模板,浏览器端向服务器端请求数据必须按照此消息模板,服务器端向浏览器端发送数据也必须按照此消息模板
HTTP请求协议（Browser向Server请求数据）
1、HTTP请求协议包括4个部分

(1)请求行
(2)请求头
(3)空白行
(4)请求体
2、HTTP请求协议具体报文（Get请求）

GET /http/getServlet?username=jxs&password=123 HTTP/1.1                      请求行
Accept:                                                                      请求头  text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate, br
Accept-Language: zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6
Connection: keep-alive
Cookie: Idea-e674796a=4657f190-c62a-4692-a94d-4d4b242fb357
Host: localhost:8080
Referer: http://localhost:8080/http/index.html
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 Edg/109.0.1518.61
sec-ch-ua: "Not_A Brand";v="99", "Microsoft Edge";v="109", "Chromium";v="109"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"
                                                                             空白行
                                                                             请求体
3、HTTP请求协议具体报文（POST请求）

POST /http/postServlet HTTP/1.1                                              请求行
Accept:                                                                      请求头 text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate, br
Accept-Language: zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6
Cache-Control: max-age=0
Connection: keep-alive
Content-Length: 25
Content-Type: application/x-www-form-urlencoded
Cookie: Idea-e674796a=4657f190-c62a-4692-a94d-4d4b242fb357
Host: localhost:8080
Origin: http://localhost:8080
Referer: http://localhost:8080/http/index.html
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: same-origin
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36 Edg/109.0.1518.61
sec-ch-ua: "Not_A Brand";v="99", "Microsoft Edge";v="109", "Chromium";v="109"
sec-ch-ua-mobile: ?0
sec-ch-ua-platform: "Windows"
                                                                             空白行
username=jxs&password=123                                                    请求体
4、请求行、请求头、空白行、请求体具体解释

(1)请求行由3部分组成:
	请求方式:(GET、POST、DELETE、PUT、HEAD、OPTIONS、TRACE)
	URI:统一资源标识符
		URI:Uniform Resource Identifier,统一资源标识符,代表网络中某个资源的资源名,通过URI不可以定位到该资源
		URL:Uniform Resource Locator,统一资源定位符,代表网络中某个资源,通过URL可以定位到该资源
		URL包括URI
		URL:http://localhost:8080/http/getServlet
		URI:/http/getServlet
	协议版本号
	
(2)请求头

(3)空白行用于分隔请求头、请求体

(4)请求体:向服务器发送的具体数据
HTTP响应协议（Server向Browser响应数据）
1、HTTP响应协议包括4个部分

(1)状态行
(2)响应头
(3)空白行
(4)响应体
2、HTTP响应协议具体报文

HTTP/1.1 200 ok                                  状态行
Content-Type: text/html;charset=UTF-8            响应头
Content-Length: 84
Date: Tue, 24 Jan 2023 07:22:46 GMT
Keep-Alive: timeout=20
Connection: keep-alive
                                                 空白行
<!DOCTYPE html>                                  响应体
<html>
    <head>
        <title>get</title>
    </head>
    <body>
        <h1>get</h1>
    </body>
</html>
3、状态行、响应头、空白行、响应体具体解释

(1)状态行由3部分组成:
	协议版本号:HTTP/1.1
	状态码:200
		HTTP协议中规定的响应状态号,不同的响应状态号对应不同的响应结果
		200表示响应成功
		404表示访问的资源不存在
		405表示前端发送的请求方式与后端发送的请求方式不一致
		500表示服务器端程序出现异常
		以4开头的状态码一般是Browser端错误;以5开头的状态码一般是Server端错误
	状态描述信息:ok
		ok表示正常
		not found表示资源不存在
		
(2)响应头由响应类型、响应长度、响应时间等

(3)空白行用于分隔响应头、响应体

(4)响应体即响应的正文,响应体为长字符串,该长字符串被浏览器渲染,解释并执行
HTTP请求协议、响应协议案例演示
1、案例步骤

(1)创建Java普通模块servlet05
(2)servlet05模块添加web框架支持
(3)servlet05模块web目录(webapp根目录)编写index.html文件
(4)启动Tomcat服务器,浏览器访问index.html文件(http://localhost:8080/http/index.html)
(5)编写GetServlet、PostServlet类
(6)编写web.xml文件,将请求路径与对应的Servlet类绑定
(7)使用谷歌浏览器F12,通过network面板查看协议具体内容
2、index.html文件

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>HTTP协议</title>
</head>
<body>
<h1>get请求</h1>
<!-- form表单中action请求路径需加上webapp的根路径 -->
<form action="/http/getServlet" method="get">
    <table>
        <tr>
            <td>username</td>
            <td><input type="text" name="username"></td>
        </tr>
        <tr>
            <td>password</td>
            <td><input type="password" name="password"></td>
        </tr>
        <tr>
            <td><input type="submit" value="提交"></td>
        </tr>
    </table>
</form>

<h1>post请求</h1>
<form action="/http/postServlet" method="post">
    <table>
        <tr>
            <td>username</td>
            <td><input type="text" name="username"></td>
        </tr>
        <tr>
            <td>password</td>
            <td><input type="password" name="password"></td>
        </tr>
        <tr>
            <td><input type="submit" value="提交"></td>
        </tr>
    </table>
</form>
</body>
</html>
3、GetServlet、PostServlet类

public class GetServlet extends GenericServlet {
    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        servletResponse.setContentType("text/html");
        PrintWriter out = servletResponse.getWriter();
        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("<head>");
        out.print("<title>get</title>");
        out.print("</head>");
        out.print("<body>");
        out.print("<h1>get</h1>");
        out.print("</body>");
        out.print("</html>");
    }
}

public class PostServlet extends GenericServlet {
    @Override
    public void service(ServletRequest servletRequest, ServletResponse servletResponse)
            throws ServletException, IOException {
        //设置响应类型
        servletResponse.setContentType("text/html");
        //servletResponse.getWriter()返回打印输出流PrintWriter,在浏览器打印输出
        PrintWriter out = servletResponse.getWriter();
        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("<head>");
        out.print("<title>post</title>");
        out.print("</head>");
        out.print("<body>");
        out.print("<h1>post</h1>");
        out.print("</body>");
        out.print("</html>");
    }
}
4、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    <servlet>
        <servlet-name>getServlet</servlet-name>
        <servlet-class>http.GetServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>getServlet</servlet-name>
        <url-pattern>/getServlet</url-pattern>
    </servlet-mapping>

    <servlet>
        <servlet-name>postServlet</servlet-name>
        <servlet-class>http.PostServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>postServlet</servlet-name>
        <url-pattern>/postServlet</url-pattern>
    </servlet-mapping>
</web-app>
GET和POST本质区别及选择（重要！！）
1、如何向服务器发送GET请求？如何向服务器发送POST请求？

(1)发送POST请求:使用form表单,并且form表单中method属性值为post
(2)发送GET请求:除以上POST请求情况外均为GET请求
(3)GET请求例:
	浏览器地址栏输入URL
	点击浏览器上的超链接
	form表单提交数据时,method属性默认为GET请求
2、GET请求与POST请求相同点、不同点

(1)
GET请求发送数据时,数据在URI+?后(例:/http/getServlet?username=jxs&password=123),数据会回显在浏览器地址栏上
POST请求发送数据时,数据在请求体中,数据不会回显在浏览器地址栏上

(2)
GET请求不可发送大数据量,GET请求只可发送普通字符串,并且字符串长度有限
POST请求可以发送大数据量,POST请求可以发送任意类型的数据,包括普通字符串、视频、声音、图片

(3)W3C中GET请求、POST请求说明:GET请求适合从服务器端获取数据;POST请求适合向服务器端传送数据

(4)
GET请求是安全的,因为GET请求从服务器获取数据
POST请求是危险的,因为POST请求向服务器传送数据,并且一般情况下拦截数据请求时大部分会选择拦截POST请求

(5)GET请求支持缓存;POST请求不支持缓存
任何1个GET请求得到的响应结果都会被浏览器缓存,在浏览器缓存中,1个GET请求路径对应1个资源
用户发送GET请求,先从浏览器本地缓存中寻找,若没有则从服务器中获取,这种缓存机制是为提高用户体验。
若用户发送GET请求,希望直接从服务器中获取数据,而不希望从本地缓存中获取数据,则可以在GET请求路径后添加变化的时间戳。如此,每次GET请求路径都不相同则可避免从本地缓存获取数据

(6)GET请求、POST请求发送数据格式相同:name=value&name=value...
3、如何选择GET请求、POST请求

(1)获取服务器中的数据使用GET请求;向服务器传送数据使用POST请求
(2)若表单中含有敏感信息使用POST请求
(3)向服务器中上传文件使用POST请求
设计模式之模板方法设计模式
1、何为设计模式？

(1)问题的固定解决方案
2、设计模式

(1)GoF设计模式(Gang of Four - 四人组)提出23种设计模式:单例模式、工厂模式、代理模式、门面模式、责任链设计模式、观察者模式、模板方法设计模式...
(2)JavaEE设计模式:DAO、DTO、VO、PO、pojo...
3、模板方法设计模式

(1)模板类中定义核心算法骨架,即定义具体实现步骤
(2)模板类通常为抽象类,模板方法设计模式中模板方法通常被final修饰
(3)模板类中的抽象方法即不确定实现的方法,该方法交由子类重写
模板方法设计模式
1、模板类

/**
 * Person类为模板类
 * Student、Teacher类为子类
 * day()方法为模板方法设计模式中的模板方法
 */
public abstract class Person {
    /*
    1.模板方法定义核心的算法骨架,即定义具体的实现步骤
    2.添加final关键字后,一方面模板方法得到保护,子类不可重写该模板方法
      另一方面算法可重复使用,具体实现步骤不会因为子类的变化而变化
     */
    public void day() {
        getUp();
        wash();
        eatBreakfast();
        daSomething();
        eatDinner();
        sleep();
    }
    public void getUp() { System.out.println("起床"); }
    public void wash() { System.out.println("洗漱"); }
    public void eatBreakfast() { System.out.println("吃早饭"); }
    //doSomething()方法交由子类实现
    public abstract void daSomething();
    public void eatDinner() { System.out.println("吃晚饭"); }
    public void sleep() { System.out.println("睡觉"); }
}
2、Student子类

public class Student extends Person {
    @Override
    public void daSomething() {
        System.out.println("学习");
    }
}
3、Teacher子类

public class Teacher extends Person{
    @Override
    public void daSomething() {
        System.out.println("教学");
    }
}
4、测试类

public class Test {
    public static void main(String[] args) {
        Person person01 = new Student();
        person01.day();

        Person person02 = new Teacher();
        person02.day();
    }
}
IntelliJ IDEA集成开发工具中查找当前类的方法、属性、内容的常用快捷键
1、展示类下的所有方法和属性快捷键

Ctrl+F12
2、快速查找类或方法或属性在整个项目中的位置

Ctrl+类或方法或属性
3、按照文本的内容查找

Ctrl+F/Ctrl+Shift+F
HttpServlet源码分析
HttpServlet基本介绍
1、基本介绍

(1)HttpServlet类是为HTTP协议准备的,HttpServlet比GenericServlet更适合HTTP协议下的开发
(2)HttpServlet类在jakarta.servlet.http.HttpServlet
(3)servlet规范中的类和接口:
jakarta.servlet.Servlet 核心接口(接口)
jakarta.servlet.ServletConfig Servlet配置信息接口(接口)
jakarta.servlet.ServletContext Servlet上下文接口(接口)
jakarta.servlet.ServletRequest Servlet请求接口(接口)
jakarta.servlet.ServletResponse Servlet响应接口(接口)
jakarta.servlet.ServletException Servlet异常(类)
jakarta.servlet.GenericServlet 标准通用的Servlet类(抽象类)
(4)http包下的类和接口:
jakarta.servlet.http.HttpServlet HTTP协议专用的Servlet抽象类
jakarta.servlet.http.HttpServletRequest HTTP协议专用的请求对象
jakarta.servlet.http.HttpServletResponse HTTP协议专用的响应对象
(5)HttpServletRequest对象
HttpServletRequest对象简称request对象,Web服务器(Tomcat服务器)将请求协议中的数据全部解析出来,再将这些数据全部封装到request对象,即面向HttpServletRequest就可以获取请求协议中的数据
(6)HttpServletResponse对象响应HTTP协议到浏览器
2、回忆Servlet生命周期

(1)用户第一次请求
	通过web.xml文件中请求路径获取对应Servlet类
	Tomcat服务器通过反射机制,调用无参构造方法创建Servlet对象
	Tomcat服务器调用Servlet对象的init方法完成初始化
	Tomcat服务器调用Servlet对象的service方法处理请求
(2)用户第二次请求
	Tomcat服务器调用Servlet对象的service方法处理请求
(3)用户第三次请求
	Tomcat服务器调用Servlet对象的service方法处理请求
(4)服务器关闭
	Tomcat服务器调用Servlet对象的destroy方法处理销毁Servlet对象前的准备工作
	Tomcat服务器销毁Servlet对象
HttpServlet源码分析
/*
(1)通过反射机制调用无参构造方法创建HelloServlet对象
*/
public class HelloServlet extends HttpServlet {
    public HelloServlet() { }
}

/*
(2)
用户发送第一次请求,HelloServlet对象第一次创建后,会执行如下init方法
带参init方法执行之后会执行无参init方法
*/
public abstract class GenericServlet implements Servlet, ServletConfig, Serializable {
    public void init(ServletConfig config) throws ServletException {
        this.config = config;
        this.init();
    }
    public void init() throws ServletException {
    }
}

/*
(3)
用户发送第一次请求,init方法执行之后执行service方法
将ServletRequest、ServletResponse强转为HttpServletRequest、HttpServletResponse
执行service(ServletRequest, ServletResponse)方法后执行service(HttpServletRequest, HttpServletResponse)方法
*/
public void service(ServletRequest req, ServletResponse res) throws ServletException, IOException {
    HttpServletRequest request;
    HttpServletResponse response;
    try {
        request = (HttpServletRequest)req;
        response = (HttpServletResponse)res;
    } catch (ClassCastException var6) {
        throw new ServletException(lStrings.getString("http.non_http"));
    }
    this.service(request, response);
}

/*
(4)
HttpServlet为模板类,service(HttpServletRequest, HttpServletResponse)方法为模板方法
在service(HttpServletRequest, HttpServletResponse)方法中定义核心算法骨架
调用HttpServletRequest对象getMethod()方法获取请求方式,获取结果为GET、POST、PUT、DELETE、HEAD、OPTIONS、TRACE其中之一
若请求方式为GET则执行doGet方法,若请求方式为POST则执行doPost()方法...
*/
protected void service(HttpServletRequest req, HttpServletResponse resp) throws ServletException, IOException {
    String method = req.getMethod();
    long lastModified;
    if (method.equals("GET")) {
        lastModified = this.getLastModified(req);
        if (lastModified == -1L) {
            this.doGet(req, resp);
        } else {
            long ifModifiedSince;
            try {
                ifModifiedSince = req.getDateHeader("If-Modified-Since");
            } catch (IllegalArgumentException var9) {
                ifModifiedSince = -1L;
            }

            if (ifModifiedSince < lastModified / 1000L * 1000L) {
                this.maybeSetLastModified(resp, lastModified);
                this.doGet(req, resp);
            } else {
                resp.setStatus(304);
            }
        }
    } else if (method.equals("HEAD")) {
        lastModified = this.getLastModified(req);
        this.maybeSetLastModified(resp, lastModified);
        this.doHead(req, resp);
    } else if (method.equals("POST")) {
        this.doPost(req, resp);
    } else if (method.equals("PUT")) {
        this.doPut(req, resp);
    } else if (method.equals("DELETE")) {
        this.doDelete(req, resp);
    } else if (method.equals("OPTIONS")) {
        this.doOptions(req, resp);
    } else if (method.equals("TRACE")) {
        this.doTrace(req, resp);
    } else {
        String errMsg = lStrings.getString("http.method_not_implemented");
        Object[] errArgs = new Object[]{method};
        errMsg = MessageFormat.format(errMsg, errArgs);
        resp.sendError(501, errMsg);
    }
}
405错误
1、index.html

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>index page</title>
    </head>
    
    <body>
    <h1>get请求</h1>
    <a href="/HttpServlet/httpServlet">hello</a>
        
    <h1>post请求</h1>
    <form action="/HttpServlet/httpServlet" method="post">
        <input type="submit" value="提交">
    </form>
    </body>
    
</html>
2、HelloServlet类

public class HelloServlet extends HttpServlet {
    /*
    1.通过反射机制调用无参构造方法创建HelloServlet对象
    2.若HelloServlet类没有提供init方法,则默认调用父类HttpServlet类的init方法
    3.HttpServlet类中没有提供init方法,则继续调用父类GenericServlet类的init方法
    4.若HelloServlet类中没有提供service方法,则默认调用父类HttpServlet类的service方法
     */

    /*若发送get请求则重写doGet方法
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        PrintWriter out = response.getWriter();
        out.print("<h1>doGet</h1>");
    }
    */

    //若发送post请求则重写doPost方法
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        PrintWriter out = response.getWriter();
        out.print("<h1>doPost</h1>");
    }
}
3、总结概括

(1)若Web前端发送get请求,Web后端程序员重写doPost方法且没有重写doGet方法 或 Web前端发送post请求,Web后端程序员重写doGet方法且没有重写doPost方法,会发生405错误
(2)405错误:前端发送的请求方式和后端服务器的请求方式不一致
(3)HttpServlet类中的doGet方法或doPost方法执行必然出现405错误
(4)Web后端重写doGet方法,前端只可发送get请求;Web后端重写doPost方法,前端只可发送post请求,如此可避免405错误
(5)Web后端程序员为避免405错误而重写doGet方法以及doPost方法,虽然确实可以避免405错误但不建议
Servlet类开发步骤（重要！！）
(1)编写Servlet类,继承HttpServlet类
(2)重写doGet方法或doPost方法
(3)web.xml文件中配置Servlet类
(4)准备前端页面,form表单action属性中指定/项目名/请求路径
WEB欢迎页
1、何为Web站点欢迎页面

(1)对于webapp,可以设置它的欢迎页面
(2)设置欢迎页面后,访问此webapp时,没有指定任何请求路径,则默认访问欢迎页面
(3)一般访问方式:http://localhost:8080/项目名/请求路径
(4)若访问http://localhost:8080/项目名,则默认访问欢迎页面
设置静态欢迎页面
1、webapp根目录下创建静态欢迎页面

(1)IntelliJ IDEA集成开发工具中webapp目录下新建login.html文件
(2)web.xml文件中新增配置如下(注:设置欢迎页时,欢迎页面路径不需以"/"开始,并且欢迎页面路径默认从webapp的根下寻找)
(3)启动Tomcat服务器时,地址栏输入:http://localhost:8080/servlet07/
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    
    <welcome-file-list>
        <welcome-file>login.html</welcome-file>
    </welcome-file-list>
    
</web-app>
2、若webapp根下新建目录，此目录下创建静态欢迎页面文件，欢迎页面路径如何设置

(1)webapp根下新建page01目录
(2)page01目录下新建page02目录
(3)page02目录下新建login.html文件
(4)web.xml文件中新增配置如下
<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    
    <welcome-file-list>
        <welcome-file>page01/page02/login.html</welcome-file>
    </welcome-file-list>
    
</web-app>
3、webapp可设置多个欢迎页面，从上而下优先级越来越低，高优先级寻找不到则继续向下寻找

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    
    <welcome-file-list>
        <welcome-file>page01/page02/login.html</welcome-file>
        <welcome-file>login.html</welcome-file>
    </welcome-file-list>
    
</web-app>
4、为何当文件名为index.html时无需在web.xml文件中配置欢迎页

(1)Tomcat服务器已提前配置完毕
(2)配置欢迎页面位置
	web.xml文件内部(此位置配置的欢迎页面属于局部配置)
	CATALINA_HOME/conf/web.xml(此位置配置的欢迎页面属于全局配置)
	局部配置优先于全局配置
(3)若web站点没有设置局部欢迎页面,Tomcat服务器会以index.html、index.htm、index.jsp作为web站点的欢迎页面
5、CATALINA_HOME/conf/web.xml文件

<welcome-file-list>
    <welcome-file>index.html</welcome-file>
    <welcome-file>index.htm</welcome-file>
    <welcome-file>index.jsp</welcome-file>
</welcome-file-list>
设置动态欢迎页面
1、欢迎页可以为静态资源或动态资源

(1)静态资源:html
(2)动态资源:Servlet类
2、WelcomeServlet类

public class WelcomeServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        out.print("<h1>Welcome to XSEmpire</h1>");
    }
}
3、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">

    <servlet>
        <servlet-name>welcome</servlet-name>
        <servlet-class>WelcomeServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>welcome</servlet-name>
        <url-pattern>/servlet07/welcome</url-pattern>
    </servlet-mapping>
    
    <welcome-file-list>
        <welcome-file>servlet07/welcome</welcome-file>
    </welcome-file-list>
</web-app>
4、设置动态欢迎页面步骤

(1)编写Servlet类
(2)web.xml文件中配置Servlet类
(3)web.xml文件中配置欢迎页
WEB-INF目录结构
1、WEB-INF目录下新建文件welcome.html文件，打开浏览器访问http://localhost:8080/servlet07/WEB-INF/welcome.html出现404错误

(1)WEB-INF目录下的资源是受保护的,浏览器地址栏不可通过路径直接访问
(2)HTML、CSS、JavaScript、image等静态资源需放置WEB-INF目录外
HttpServletRequest源码分析（重点！！！！）
1、基本概念

(1)HttpServletRequest是一个接口,全限定类名为jakarta.servlet.http.HttpServletRequest
(2)HttpServletRequest接口为Servlet规范中的一员
(3)HttpServletRequest接口父接口为ServletRequest
(4)org.apache.catalina.connector.RequestFacade实现了HttpServletRequest接口
(5)Tomcat服务器实现HttpServletRequest接口,即Tomcat服务器实现了Servlet规范。但对于javaweb程序员来说只需面向接口编程即可,javaweb程序员关心的是HttpServletRequest接口中的方法以及方法实现的功能
(6)HttpServletRequest对象由Tomcat服务器负责创建,HttpServletRequest对象中封装了Http请求协议
(7)用户发送请求时,遵循HTTP协议,发送HTTP请求协议,Tomcat服务器将HTTP请求协议中的数据解析出来封装到HttpServletRequest对象中,调用HttpServletRequest对象的方法可以获取对应数据
(8)javaweb程序员面向HttpServletRequest编程,调用相应方法可以获取请求信息
(9)HttpServletRequest对象、HttpServletResponse对象的生命周期只在当前请求和当前响应中有效
HttpServletRequest接口常用方法
1、获取前端浏览器用户提交的数据

(1)Map<String,String[]> getParameterMap();获取存储数据的Map集合
(2)Enumeration<String> getParameterNames();获取Map集合中所有key
(3)String[] getParameterValues(String name);获取Map集合中key对应的value
(4)String getParameter(String name);大部分情况下,一维数组中只存在一个元素,为简化开发,可根据key获取一维数组中唯一value
2、前端form表单提交数据后，如何存储数据，采用何种数据结构存储数据

(1)前端提交的数据格式:name=value&name=value&name=value...
(2)采用Map集合存储数据
	Map<String,String>
	key存储String,value存储String
	若采用以上数据结构存储数据,key重复时会覆盖value
	
	Map<String,String[]>
	key存储String,value存储String[]
3、注意事项

(1)若前端提交userpassword=123456,123456是以字符串的方式提交至服务器,并采用Map集合的方式存储数据
HttpServletRequest接口常用方法案例演示
1、index.html文件

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>index page</title>
    </head>
    <body>
        <form action="/servlet09/request" method="post">
            <table>
                <tr>
                    <td>用户名</td>
                    <td><input type="text" name="username"></td>
                </tr>
                <tr>
                    <td>密码</td>
                    <td><input type="password" name="userpassword"></td>
                </tr>
                <tr>
                    <td>兴趣爱好</td>
                    <td>
                        抽烟<input type="checkbox" name="hobby" value="smoke">
                        喝酒<input type="checkbox" name="hobby" value="drink">
                    </td>
                </tr>
                <tr>
                    <td><input type="submit" value="提交"></td>
                </tr>
            </table>
        </form>
    </body>
</html>
2、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    <servlet>
        <servlet-name>request</servlet-name>
        <servlet-class>RequestTestServlet</servlet-class>
    </servlet>

    <servlet-mapping>
        <servlet-name>request</servlet-name>
        <url-pattern>/request</url-pattern>
    </servlet-mapping>
</web-app>
3、Servlet类

public class RequestTestServlet extends HttpServlet {
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        /*
        1.Tomcat服务器将Http请求协议中的数据封装到HttpServletRequest对象中
        2.Web前端提交的数据保存在Http请求协议中
        3.面向HttpServletRequest接口编程可获取前端提交的数据
         */
        Map<String, String[]> map = request.getParameterMap();
        //遍历map集合,获取所有key
        Set<String> keys = map.keySet();
        /*
        key            value
        username       {"jxs"}
        userpassword   {"123456"}
        hobby          {"smoke","drink"}
         */
        for (String key : keys) {
            //通过key获取value数组
            String[] values = map.get(key);
            /*
            username=[Ljava.lang.String;@6d0f12ee
            userpassword=[Ljava.lang.String;@4a655414
            hobby=[Ljava.lang.String;@585ddafa
             */
            out.print(key + "=" + values);
            //遍历value数组
            for (String value : values) {
                out.print("," + value + "<br>");
            }
        }

        //获取Map集合所有key
        Enumeration<String> names = request.getParameterNames();
        //遍历取出每个key
        while (names.hasMoreElements()) {
            String key = names.nextElement();
            out.print(key + " ");
        }

        //通过key获取value数组
        String[] usernames = request.getParameterValues("username");
        String[] userpasswords = request.getParameterValues("userpassword");
        String[] hobbies = request.getParameterValues("hobby");
        //遍历value数组
        for (String username : usernames) {
            out.print(username);
        }
        for (String userpassword : userpasswords) {
            out.print(userpassword);
        }
        for (String hobby : hobbies) {
            out.print(hobby);
        }

        /*
        通过key获取value数组第一个元素
        此方法使用最多,因为value数组中一般只有一个元素
         */
        String username = request.getParameter("username");
        String userpassword = request.getParameter("userpassword");
        String hobby = request.getParameter("hobby");
        out.print(username);
        out.print(userpassword);
        out.print(hobby);
    }
}
4、浏览器地址栏输入http://localhost:8080/servlet09/index.html

5、用户在Web前端表单中填写数据，以post方式提交表单中的数据至服务器，将表单中的数据封装在HttpServletRequest对象中，采用Map集合的方式存储数据，面向HttpServletRequest接口编程，调用HttpServletRequest对象方法获取数据

请求域对象（重要！！）
1、请求域对象、应用域对象

(1)应用域对象:ServletContext(Servlet上下文对象)
	所有用户共享的的数据,共享的数据量小,共享的数据少次的修改
	三个条件满足的情况下,使用ServletContext应用域对象,可以提高程序执行效率
	ServletContext应用域中绑定数据,就相当于将数据放入缓存(Cache)中,用户访问时直接从缓存中取出,减少IO操作,提升系统性能,缓存技术是提高系统性能的重要手段
(2)请求域对象:ServletRequest(请求域对象只在一次请求中有效)
	对象范围:请求域对象小,应用域对象大
	生命周期:请求域对象短,应用域对象长
	请求域与应用域选用原则:尽量使用请求域对象,请求域占用的资源小。Tomcat服务器启动时创建应用域对象,Tomcat服务器关闭时销毁应用域对象;用户发送一次请求对应一个请求域对象,一次请求结束后请求域对象销毁
2、缓存技术

(1)字符串常量池
	String s = new String("jxs");
	堆中创建String对象,String对象的value属性指向字符串常量池对应的字符串地址
	若字符串常量池中存在"jxs"则value属性指向"jxs"的地址
	若字符串常量池中不存在"jxs"则在字符串常量池中新建"jxs"
(2)整数型常量池
	存放[-128~127]共256个Integer引用
	通过new Integer()方式创建Integer对象,不管传入的值是否相等,Integer对象的地址都不相等
	通过Integer.valueOf()方式创建Integer对象,在-128 ~ +127范围内为同一个对象,超出此范围则通过new Integer()的方式创建Integer对象
(3)数据库连接池
	提前创建好数据库连接对象,将连接对象放置集合中,当使用连接对象时直接从缓存中取出,省去创建数据库连接对象的过程,提高效率
(4)线程池
	Tomcat服务器支持多线程
	提交创建好线程对象,将线程对象放置集合中,用户发送请求后直接从线程池获取线程对象
3、ServletContext中操作应用域数据方法

void setAttribute(String name,Object obj);//应用域中绑定数据
Object getAttribute(String name);//应用域中获取数据
void removeAttribute(String name);//应用域中移除数据

操作应用域中的数据的方法类似于Map集合中的操作
Map map = new HashMap<String,Object>();
map.put("name","jxs");
Object obj = map.get("name");
4、请求域对象方法

(1)void setAttribute(String name,Object obj);//请求域中绑定数据
(2)Object getAttribute(String name);//请求域中获取数据
(3)void removeAttribute(String name);//请求域中删除数据
请求域对象方法解析
1、index.html文件

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>index page</title>
    </head>
    <body>
        <form action="/servlet10/request" method="post">
            <table>
                <tr>
                    <td>用户名</td>
                    <td><input type="text" name="username"></td>
                </tr>
                <tr>
                    <td>密码</td>
                    <td><input type="password" name="userpassword"></td>
                </tr>
                <tr>
                    <td><input type="submit" value="提交"></td>
                </tr>
            </table>
        </form>
    </body>
</html>
2、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    <servlet>
        <servlet-name>request</servlet-name>
        <servlet-class>RequestTest</servlet-class>
    </servlet>
    
    <servlet-mapping>
        <servlet-name>request</servlet-name>
        <url-pattern>/request</url-pattern>
    </servlet-mapping>
</web-app>
3、RequestTest类

public class RequestTest extends HttpServlet {
    /*
    (1)Web前端是以post方式提交表单中的数据
    (2)用户发送第一次请求时执行init方法,HttpServlet类中不存在init方法,默认执行父类GenericServlet类中的init方法
    (3)执行HttpServlet类中的service(ServletRequest req, ServletResponse res)方法
       先定义局部变量HttpServletRequest request、HttpServletResponse response
       将HttpServletRequest request、HttpServletResponse response强转为ServletRequest、ServletResponse
       执行service(HttpServletRequest req, HttpServletResponse resp)方法
    (4)若RequestTest类中没有重写doPost方法,则默认执行HttpServlet中的doPost方法,提示405错误
     */
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //用户提交form表单中的数据,数据存在于请求协议中,将请求协议中的数据封装在request对象中
        String username = request.getParameter("username");
        String userpassword = request.getParameter("userpassword");
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        out.print(username + " " + userpassword);
        //获取系统时间
        Date date = new Date();
        //request请求域中绑定数据
        request.setAttribute("time", date);
        //request请求域中获取数据
        Object time = request.getAttribute("time");
        out.print(time);
        //request请求域中删除数据
        request.removeAttribute("time");
    }
}
转发机制
1、转发步骤

//(1)获取请求转发器对象
RequestDispatcher dispatcher = new getRequestDispatcher(下一跳转的资源路径);
//(2)调用请求转发器对象的forward方法
dispatcher.forward(request,response);
2、两个Servlet如何共享数据

(1)将数据存放到ServletContext应用域中
(2)将数据存放到ServletRequest请求域中,AServlet使用转发机制转发数据到BServlet中
3、转发的资源必须为Servlet吗？

(1)Tomcat服务器中的合法资源都可以转发
(2)转发资源时,路径的写法以"/"开始,不加项目名
4、关于request对象中两个容易混淆的方法

String name = request.getParameter(String name);
Object name = request.getAttribute(String name);

/*
区别:
(1)第一个方法:获取用户在浏览器上提交的数据
(2)第二个方法:获取请求域中绑定的数据
*/
转发机制案例演示
1、AServlet、BServlet类

public class AServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取当前系统时间
        Date date = new Date();

        //ServletRequest请求域中绑定数据
        request.setAttribute("time", date);

        //ServletRequest请求域中获取数据
        //Object time = request.getAttribute("time");

        //ServletRequest请求域中删除数据
        //request.removeAttribute("time");

        /*
        Servlet转发机制(资源跳转)
        (1)获取请求转发器对象(将"/b"路径包装到请求转发器对象中,即将下一个跳转的资源的路径告知Tomcat服务器)
        (2)调用请求转发器对象的forward方法
        (3)将request、response传递给下一个资源
        RequestDispatcher dispatcher = request.getRequestDispatcher("/b");
        dispatcher.forward(request, response);
         */
        request.getRequestDispatcher("/b").forward(request, response);
    }
}
public class BServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        Object time = request.getAttribute("time");

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.print(time);
    }
}
2、web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    <servlet>
        <servlet-name>a</servlet-name>
        <servlet-class>AServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>a</servlet-name>
        <url-pattern>/a</url-pattern>
    </servlet-mapping>

    <servlet>
        <servlet-name>b</servlet-name>
        <servlet-class>BServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>b</servlet-name>
        <url-pattern>/b</url-pattern>
    </servlet-mapping>
</web-app>
HttpServletRequest接口其他常用方法
1、方法解析

(1)String remoteAddr = request.getRemoteAddr();//获取客户端IP地址
(2)String contextPath = request.getContextPath();//动态获取应用根路径
(3)String method = request.getMethod();//获取请求方式
(4)String requestURI = request.getRequestURI();//获取请求的URI
(5)String servletPath = request.getServletPath();//获取Servlet类对应的请求路径
2、post请求乱码问题

/*
设置请求体的字符集
(1)get请求在请求行中提交数据;post请求在请求体中提交数据
(2)此方法处理post请求乱码问题,但这种方式不能解决get请求乱码问题
(3)Tomcat10之后,request请求体中的字符集默认为UTF-8,无需设置字符集,不会出现乱码问题
(4)Tomcat9之前包括Tomcat9,若前端提交的数据是中文,则需设置request请求体中的字符集为UTF-8
*/
(1)request.setCharacterEncoding("UTF-8");

/*
(1)Tomcat9之前包括Tomcat9,若响应中文则需设置响应的字符集为UTF-8
(2)Tomcat10之后,响应的字符集默认为UTF-8,无需设置字符集,不会出现乱码问题
*/
(2)response.setContentType("text/html;charset=UTF-8")
3、get请求乱码问题

/*
(1)get请求,用户提交的数据在请求行中,不在请求体中
(2)get请求乱码解决
	修改CATALINA_HOME/conf/server.xml配置文件
	<Connector port="8080" 
			   protocol="HTTP/1.1" 
			   connectionTimeout="20000" 
			   redirectPort="8443" 
			   URIEncoding="UTF-8"/>
(3)Tomcat8之后,URIEncoding默认为UTF-8,所以get请求不存在乱码问题
*/
乱码问题总结（精华！！）
1、post请求乱码问题

用户以post方式提交数据至服务器,数据在Http请求协议中的请求体中,Tomcat服务器将数据封装在HttpServletRequest对象中,采用Map集合的方式存储数据,设置请求体的字符集可以避免乱码问题(request.setCharacterEncoding("UTF-8"))。
2、get请求乱码问题

用户以get方式提交数据至服务器,数据在Http请求协议中的请求行中,Tomcat服务器将数据封装在HttpServletRequest对象中,采用Map集合的方式存储数据,设置请求行的字符集可以避免乱码问题,修改CATALINA_HOME/conf/server.xml配置文件
<Connector port="8080" 
           protocol="HTTP/1.1" 
           connectionTimeout="20000" 
           redirectPort="8443" 
           URIEncoding="UTF-8"/>
3、响应乱码问题

response.setContentType("text/html;charset=UTF-8");
HttpServletRequest接口方法总结（精华！！）
(1)Map<String, String[]> map = request.getParameterMap();//获取Map集合
(2)Enumeration<String> keys = request.getParameterNames();//获取Map集合中所有key
(3)String[] values = request.getParameterValues(String key);//获取Map集合中key对应的value数组
(4)String value = request.getParameter(String key);//获取Map集合中key对应的value数组中的第一个元素

(5)request.setAttribute(String name, Object obj);//请求域中绑定数据
(6)Object name = request.getAttribute(String name);//请求域中获取数据
(7)request.removeAttribute(String name);//请求域中删除数据

(8)request.getRequestDispatcher(路径).forward(request, response);//转发数据

(9)String remoteAddr = request.getRemoteAddr();//获取客户端IP地址
(10)String contextPath = request.getContextPath();//动态获取应用根路径
(11)String method = request.getMethod();//获取请求方式
(12)String requestURI = request.getRequestURI();//获取请求的URI
(13)String servletPath = request.getServletPath();//获取Servlet类对应的请求路径
使用Servlet完成单表CRUD操作
实现步骤
数据库中准备部门表（Navicat）
DROP TABLE IF EXISTS dept;

CREATE TABLE dept(
deptno INT PRIMARY KEY,
deptname VARCHAR(255),
location VARCHAR(255));

INSERT INTO dept(deptno,deptname,location) VALUES(1,'销售部','南京'),(2,'研发部','北京'),(3,'技术部','上海'),(4,'媒体部','广州');
准备HTML页面-项目原型（HBuilder X）
1、准备HTML页面

欢迎页面:index.html
部门列表页面:list.html
新增页面:add.html
修改页面:edit.html
详情页面:detail.html
2、欢迎页面

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>欢迎页</title>
	</head>
	<body>
		<a href="list.html">部门列表</a>
	</body>
</html>
3、部门列表页面

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>部门列表页面</title>
	</head>
	<body>
		<form>
			<table>
				<tr>
					<td>部门编号</td>
					<td>部门名称</td>
					<td>部门地址</td>
					<td>部门操作</td>
				</tr>
				<tr>
					<td>1</td>
					<td>销售部</td>
					<td>南京</td>
					<td>
						<a href="">删除</a>
						<a href="edit.html">修改</a>
						<a href="detail.html">详情</a>
					</td>
				</tr>
				<tr>
					<td>2</td>
					<td>研发部</td>
					<td>北京</td>
					<td>
						<a href="">删除</a>
						<a href="edit.html">修改</a>
						<a href="detail.html">详情</a>
					</td>
				</tr>
				<tr>
					<td>3</td>
					<td>技术部</td>
					<td>上海</td>
					<td>
						<a href="">删除</a>
						<a href="edit.html">修改</a>
						<a href="detail.html">详情</a>
					</td>
				</tr>
				<tr>
					<td>4</td>
					<td>媒体部</td>
					<td>广州</td>
					<td>
						<a href="">删除</a>
						<a href="edit.html">修改</a>
						<a href="detail.html">详情</a>
					</td>
				</tr>
			</table>
			<a href="add.html">新增部门</a>
		</form>
	</body>
</html>
4、新增页面

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>新增部门</title>
	</head>
	<body>
		<form action="list.html" method="get">
			<table>
				<tr>
					<td>部门编号</td>
					<td><input type="text" name="deptno"/></td>
				</tr>
				<tr>
					<td>部门名称</td>
					<td><input type="text" name="deptname"/></td>
				</tr>
				<tr>
					<td>部门地址</td>
					<td><input type="text" name="location"/></td>
				</tr>
				<tr>
					<td><input type="submit" value="新增部门"/></td>
				</tr>
			</table>
		</form>
	</body>
</html>
5、修改页面

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>修改部门</title>
	</head>
	<body>
		<form action="list.html" method="get">
			<table>
				<tr>
					<td>部门编号</td>
					<td><input type="text" name="deptno" value="" readonly/></td>
				</tr>
				<tr>
					<td>部门名称</td>
					<td><input type="text" name="deptname" value=""/></td>
				</tr>
				<tr>
					<td>部门地址</td>
					<td><input type="text" name="location" value=""/></td>
				</tr>
				<tr>
					<td><input type="submit" value="修改部门"/></td>
				</tr>
			</table>
		</form>
	</body>
</html>
6、详情页面

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>部门详情</title>
	</head>
	<body>
		<h1>部门详情</h1>
		<h4>部门编号:</h4>
		<h4>部门名称:</h4>
		<h4>部门地址:</h4>
		<a href="list.html">返回上一级</a>
	</body>
</html>
系统功能
1、数据库中查询部门列表

2、数据库中新增部门

3、数据库中删除部门

4、数据库中修改部门

5、数据库中部门详情

IntelliJ IDEA集成开发工具中搭建开发环境
1、创建webapp（添加servlet-api.jar和jsp-api.jar）

2、webapp的lib目录下添加连接数据库的jar包（mysql驱动）

3、JDBC工具类

driver=com.mysql.cj.jdbc.Driver
url=jdbc:mysql://localhost:3306/javaweb
user=root
password=123456
/**
 * JDBC工具类
 * 1.注册数据库驱动
 * 2.获取数据库连接对象
 * 3.获取数据库操作对象
 * 4.执行SQL语句
 * 5.处理结果集
 * 6.释放资源
 */
public class DBUtils {
    //绑定资源文件
    private static ResourceBundle bundle = ResourceBundle.getBundle("resources.jdbc");
    //静态变量,类加载时由自上而下的顺序执行,根据资源文件的key获取value并赋值给静态变量
    private static String driver = bundle.getString("driver");
    private static String url = bundle.getString("url");
    private static String user = bundle.getString("user");
    private static String password = bundle.getString("password");

    static {
        try {
            /*
            (1)注册驱动(DBUtils类加载时执行静态代码块,相当于类的初始化)
            (2)com.mysql.jdbc.cj.Driver为连接数据库驱动
            (3)若此后连接Oracle数据库,则需修改数据库驱动,需修改Java代码,违背OCP开闭原则
            (4)OCP开闭原则:开放扩展,关闭修改。即进行功能扩展时无需修改java源代码
            */
            Class.forName(driver);
        } catch (ClassNotFoundException exception) {
            System.out.println(exception.getMessage());
        }
    }

    /**
     * 获取数据库连接对象
     *
     * @return 返回数据库连接对象connection
     * @throws Exception
     */
    public static Connection getConnection() throws Exception {
        //注册驱动,获取连接
        Connection connection = DriverManager.getConnection(url, user, password);
        return connection;
    }

    /**
     * 释放资源
     * @param connection 数据库连接对象
     * @param statement 数据库操作对象
     * @param resultSet 结果集
     */
    public static void close(Connection connection, Statement statement, ResultSet resultSet) {
        if (connection != null) {
            try {
                connection.close();
            } catch (SQLException throwable) {
                System.out.println(throwable.getMessage());
            }
        }
        if (statement != null) {
            try {
                statement.close();
            } catch (SQLException throwable) {
                System.out.println(throwable.getMessage());
            }
        }
        if (resultSet != null) {
            try {
                resultSet.close();
            } catch (SQLException throwable) {
                System.out.println(throwable.getMessage());
            }
        }
    }
}
功能一：查看部门列表
1、用户点击欢迎页部门列表超链接，从数据库中获取各个部门信息

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>欢迎页</title>
    </head>
    <body>
        <!-- crud为项目名,list为请求路径 -->
        <a href="/crud/list">部门列表</a>
    </body>
</html>
2、编辑web.xml文件

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">
    <servlet>
        <servlet-name>list</servlet-name>
        <servlet-class>ListServlet</servlet-class>
    </servlet>
    <servlet-mapping>
        <servlet-name>list</servlet-name>
        <url-pattern>/list</url-pattern>
    </servlet-mapping>
</web-app>
3、编写ListServlet类，继承HttpServlet类，重写doGet方法

4、ListServlet类中注册数据库驱动、获取数据库连接对象、获取数据库操作对象、执行SQL语句、处理结果集、释放资源，查询数据库中所有部门信息，动态展示所有部门信息。

(1)分析list.html文件中固态以及动态部分
(2)list.html文件中的双引号替换为单引号,因为out.print("")中存在双引号,引发冲突
5、ListServlet类代码繁琐，纯Servlet开发代码太繁琐！！

public class ListServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应的内容类型以及字符集
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("<head>");
        out.print("<meta charset='utf-8'>");
        out.print("<title>部门列表页面</title>");
        out.print("</head>");
        out.print("<body>");
        out.print("	<form>");
        out.print("		<table>");
        out.print("			<tr>");
        out.print("				<td>部门编号</td>");
        out.print("				<td>部门名称</td>");
        out.print("				<td>部门地址</td>");
        out.print("				<td>部门操作</td>");
        out.print("			</tr>");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select deptno,deptname,location from dept";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {

                String deptno = resultSet.getString("deptno");
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                //以下为动态的
                out.print("			<tr>");
                out.print("				<td>" +  deptno + "</td>");
                out.print("				<td>" +  deptname + "</td>");
                out.print("				<td>" + location + "</td>");
                out.print("				<td>");
                out.print("					<a href=''>删除</a>");
                out.print("					<a href=''>修改</a>");
                out.print("					<a href=''>详情</a>");
                out.print("				</td>");
                out.print("			</tr>");
                //以上为动态的
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        //以下为固定的
        out.print("		</table>");
        out.print("		<a href='add.html'>新增部门</a>");
        out.print("	</form>");
        out.print("</body>");
        out.print("</html>");
    }
}
功能二：部门详情
1、功能实现建议

(1)从前端往后端一步一步实现,首先考虑用户点击什么?
(2)用户点击java程序中的"详情"超链接
(3)部门详情需连接数据库,点击超链接后需执行java代码,所以修改超链接的路径
2、超链接

out.print("<a href='" + contextPath + "/detail?deptno= " + deptno + "'>详情</a>");

//重点:用户向服务器提交数据的格式:url?name=value&name=value...
3、web.xml文件中配置DetailServlet类，解决404问题

<servlet>
    <servlet-name>detail</servlet-name>
    <servlet-class>DetailServlet</servlet-class>
</servlet>

<servlet-mapping>
    <servlet-name>detail</servlet-name>
    <url-pattern>/detail</url-pattern>
</servlet-mapping>
4、编写DetailServlet类

(1)获取部门编号
(2)根据部门编号查询数据库,获取部门编号对应的部门信息
(3)将部门信息响应到浏览器
public class DetailServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应内容类型
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        //获取部门编号
        String deptno = request.getParameter("deptno");
        //获取webapp的根路径
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print(" <head>");
        out.print("     <meta charset='utf-8'>");
        out.print("     <title>部门详情</title>");
        out.print("</head>");
        out.print("<body>");
        out.print(" <h1>部门详情</h1>");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select * from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集(deptno为主键,不可重复,所以此结果集只有一条记录)
            while (resultSet.next()) {
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                out.print(" <h4>部门编号:" + deptno + "</h4>");
                out.print(" <h4>部门名称:" + deptname + "</h4>");
                out.print(" <h4>部门地址:" + location + "</h4>");

            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        out.print(" <a href='" + contextPath + "/list" + "'>返回上一级</a>");
        out.print("</body>");
        out.print("</html>");
    }
}
功能三：删除部门
1、从前端页面开始，用户点击删除时提示用户是否删除，因为删除操作较危险，需进行二次确认。任何系统在进行删除操作前必须提示用户。因为删除操作可能为误操作。

<a href='javascript:void(0)' onclick='del(" + deptno + ")'>删除</a>

<script type='text/javascript'>
    function del(deptno) {
        //弹出确认框,用户点击确定返回true,用户点击取消返回false
        if(window.confirm('确认删除?')) {
            /*
            发送请求进行数据删除操作
			document.location.href = "请求路径"
			window.location.href = "请求路径"
			document.location = "请求路径"
			window.location = "请求路径"
            */
            document.location.href = '" + contextPath + "/delete?deptno=' + deptno;
        }
    }
</script>
2、web.xml文件中配置DeleteServlet类

<servlet>
    <servlet-name>delete</servlet-name>
    <servlet-class>DeleteServlet</servlet-class>
</servlet>
<servlet-mapping>
    <servlet-name>delete</servlet-name>
    <url-pattern>/delete</url-pattern>
</servlet-mapping>
3、将变量加入字符串中（"+变量名+"）

4、将以上的前端程序写入到后端ListServlet中

public class ListServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应的内容类型以及字符集
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        //获取webapp的根路径
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("<head>");
        out.print("<meta charset='utf-8'>");
        out.print("<title>部门列表页面</title>");

        out.print("<script type='text/javascript'>");
        out.print("    function del(deptno) {");
        out.print("        if(window.confirm('确认删除?')) {");
        out.print("            document.location.href = '" + contextPath + "/delete?deptno=' + deptno;");
        out.print("        }");
        out.print("    }");
	    out.print("</script>");

        out.print("</head>");
        out.print("<body>");
        out.print("	<form>");
        out.print("		<table>");
        out.print("			<tr>");
        out.print("				<td>部门编号</td>");
        out.print("				<td>部门名称</td>");
        out.print("				<td>部门地址</td>");
        out.print("				<td>部门操作</td>");
        out.print("			</tr>");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select deptno,deptname,location from dept";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {

                String deptno = resultSet.getString("deptno");
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                //以下为动态的
                out.print("			<tr>");
                out.print("				<td>" +  deptno + "</td>");
                out.print("				<td>" +  deptname + "</td>");
                out.print("				<td>" + location + "</td>");
                out.print("				<td>");
                //href后设置javascript:void(0)表示点击此超链接后执行一段JS代码而不进行页面的跳转
                out.print("					<a href='javascript:void(0)' onclick='del(" + deptno + ")'>删除</a>");
                out.print("					<a href=''>修改</a>");
                out.print("					<a href='" + contextPath + "/detail?deptno= " + deptno + "'>详情</a>");
                out.print("				</td>");
                out.print("			</tr>");
                //以上为动态的
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        //以下为固定的
        out.print("		</table>");
        out.print("		<a href='add.html'>新增部门</a>");
        out.print("	</form>");
        out.print("</body>");
        out.print("</html>");
    }
}
5、编写DeleteServlet类

public class DeleteServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "delete from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            //返回数据库中表的受影响的行数
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        if (i == 1) {
            //删除成功跳转到部门列表页面,使用转发机制跳转到部门列表页面
            request.getRequestDispatcher("/list").forward(request, response);
        }
    }
}
功能四：新增部门
1、用户点击部门列表中新增部门超链接，用户输入部门编号、部门名称、部门地址，以post方式提交数据至服务器。add.html文件

<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>新增部门</title>
	</head>
	<body>
		<form action="/crud/add" method="post">
			<table>
				<tr>
					<td>部门编号</td>
					<td><input type="text" name="deptno"/></td>
				</tr>
				<tr>
					<td>部门名称</td>
					<td><input type="text" name="deptname"/></td>
				</tr>
				<tr>
					<td>部门地址</td>
					<td><input type="text" name="location"/></td>
				</tr>
				<tr>
					<td><input type="submit" value="新增部门"/></td>
				</tr>
			</table>
		</form>
	</body>
</html>
2、AddServlet类中连接数据库，将数据保存到数据库中

public class AddServlet extends HttpServlet {
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        /*
        (1)前端用户以post方式提交的数据封装在Http请求协议的请求体中
        (2)Tomcat服务器将Http请求协议中的数据封装在HttpServletRequest对象中
        (3)用户的一次请求对应一个HttpServletRequest对象
        (4)面向HttpServletRequest接口编程可以获取用户提交的数据
         */
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        int i = 0;
        String contextPath = request.getContextPath();

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "insert into dept values (?,?,?)";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            preparedStatement.setString(2, deptname);
            preparedStatement.setString(3, location);
            //执行SQL语句,返回受影响的行数
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, null);
        }

        //新增页面成功跳转到部门列表
        if (i == 1) {
            request.getRequestDispatcher("/list").forward(request, response);
        }
    }
}
3、数据保存成功后转发到/list时出现405错误

(1)用户以post方式提交数据至服务器
(2)AddServlet类中若没有重写doPost方法,则默认执行HttpServlet类中的doPost方法,出现405错误
(3)AddServlet类中重写doPost方法,转发到/list时为一次请求
(4)ListServlet类中没有重写doPost方法,则默认执行HttpServlet类中的doPost方法,出现405错误
(5)两种解决方案
	(1)ListServlet类中重写doPost方法,在doPost方法中调用doGet
	(2)重定向
功能五：修改部门
1、用户点击修改超链接，以get方式提交部门编号

<a href='" + contextPath + "/edit?deptno=" + deptno + "'>修改</a>
2、连接数据库，通过部门编号获取部门信息，以get方式提交部门信息

public class EditServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应内容的类型
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("	<head>");
        out.print("		<meta charset='utf-8'>");
        out.print("		<title>修改部门</title>");
        out.print("	</head>");
        out.print("	<body>");
        out.print("		<form action='" + contextPath + "/modify' method='post'>");
        out.print("			<table>");


        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            connection = DBUtils.getConnection();
            String sql = "select * from dept where deptno = ?";
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            resultSet = preparedStatement.executeQuery();
            if (resultSet.next()) {
                //deptname、location为SQL语句查询结果列的列名
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                out.print("				<tr>");
                out.print("					<td>部门编号</td>");
                out.print("					<td><input type='text' name='deptno' value='" + deptno + "' readonly/></td>");
                out.print("				</tr>");
                out.print("				<tr>");
                out.print("					<td>部门名称</td>");
                out.print("					<td><input type='text' name='deptname' value='" + deptname + "'/></td>");
                out.print("				</tr>");
                out.print("				<tr>");
                out.print("					<td>部门地址</td>");
                out.print("					<td><input type='text' name='location' value='" + location + "'/></td>");
                out.print("				</tr>");
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        out.print("				<tr>");
        out.print("					<td><input type='submit' value='修改部门'/></td>");
        out.print("				</tr>");
        out.print("			</table>");
        out.print("		</form>");
        out.print("	</body>");
        out.print("</html>");
    }
}
3、web.xml文件中配置EditServlet、ModifyServlet类

<servlet>
    <servlet-name>edit</servlet-name>
    <servlet-class>EditServlet</servlet-class>
</servlet>
<servlet-mapping>
    <servlet-name>edit</servlet-name>
    <url-pattern>/edit</url-pattern>
</servlet-mapping>

<servlet>
    <servlet-name>modify</servlet-name>
    <servlet-class>ModifyServlet</servlet-class>
</servlet>
<servlet-mapping>
    <servlet-name>modify</servlet-name>
    <url-pattern>/modify</url-pattern>
</servlet-mapping>
4、编写ModifyServlet类，修改部门信息

public class ModifyServlet extends HttpServlet {
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            String sql = "update dept set deptname = ? , location = ? where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptname);
            preparedStatement.setString(2, location);
            preparedStatement.setString(3,deptno);
            //执行SQL语句
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        }

        if (i == 1) {
            request.getRequestDispatcher("/list").forward(request, response);
        }
    }
}
转发和重定向深度剖析
1、web应用中，转发和重定向可以完成资源的跳转。转发和重定向的区别？

转发:request.getRequestDispatcher("请求路径").foward(request,response)
转发为一次请求,AServlet转发到BServlet,BServlet转发到CServlet,不管转发的次数,都在同一request请求域中,调用forward方法时将当前的request、response传递给下一个Servlet

重定向:response.sendRedirect("项目名+请求路径");
重定向为两次请求,重定向由浏览器完成,浏览器发送请求,请求路径需加上项目名
2、转发和重定向形式上的区别？

转发(一次请求):
浏览器地址栏发送请求:http://localhost:8080/servlet11/a,转发之后以及最终请求结束之后,浏览器地址栏地址始终不变

重定向(两次请求):
浏览器地址栏发送请求:http://localhost:8080/servlet11/a,重定向后,浏览器地址栏地址为http://localhost:8080/servlet11/b
3、总结

(1)转发为一次请求,重定向为两次请求
(2)转发中的路径为请求路径,重定向中的路径为项目名+请求路径
(3)转发由Tomcat服务器控制,在Tomcat服务器内部完成;重定向由浏览器完成
(4)转发、重定向例子:
	转发:张三向李四借钱,李四没钱但够义气,李四向王五借钱,将钱给了张三(李四帮助张三向王五借钱)
	重定向:张三向李四借钱,李四没钱不够义气,李四推荐张三向王五借钱,张三又向王五借钱(张三向李四借钱未果又向王五借钱)
4、转发图解



5、重定向图解



5、何时使用转发？何时使用重定向？

(1)AServlet中向request请求域中绑定数据,若BServlet中向request请求域中获取数据使用转发
(2)其余均使用重定向,重定向使用较多
6、跳转资源要求

(1)转发、重定向跳转的资源只要是Tomcat服务器内部合法的资源即可
7、转发存在浏览器的刷新问题。

Servlet注解式开发
1、crud项目问题分析

(1)crud项目只实现了单表的增删改查,web.xml文件中却有大量配置信息。
(2)对于一个大项目,web.xml文件会非常庞大。
(3)web.xml文件中进行Servlet信息的配置,每一Servlet类都需在web.xml文件中进行配置,效率低
(4)web.xml文件中Servlet的配置信息很少修改
(5)Servlet3.0之后,推出Servlet类基于注解式开发
2、注解式开发优点

(1)开发效率高,web.xml文件中无需编写大量配置信息,直接在java类上使用注解进行标注
(2)java类上使用注解进行标注后,web.xml文件体积缩小
(3)注解式开发推出后,web.xml文件仍有存在的需求,一般是注解+web.xml文件配合开发
(4)一些需变化的信息配置到web.xml文件中;一些无需经常变化的信息使用注解式开发
3、@WebServlet注解

package jakarta.servlet.annotation;

/**
 * @Target说明了Annotation所修饰的对象范围
 * 取值(ElementType)有:
 		1.constructor:用于修饰构造器
 		2.field:用于修饰全局变量(成员变量)
 		3.local_variable:用于修饰局部变量
 		4.method:用于修饰方法
 		5.package:用于修饰包
 		6.parameter:用于修饰参数
 		7.type:用于修饰类、接口(包括注解类型)、enum声明
 */
@Target({ElementType.TYPE})
@Retention(RetentionPolicy.RUNTIME)
@Documented
public @interface WebServlet {
    //指定Servlet类的name,相当于<servlet-name>
    String name() default "";
    //指定Servlet类的请求路径,相当于<url-pattern>
    String[] urlPatterns() default {};
    //Tomcat服务器启动时是否创建Servlet类对象实例,相当于<load-on-startup>
    int loadOnStartup() default -1;
    //@WebInitParam类型的数组,使用@WebInitParam注解可配置多个初始化参数
    WebInitParam[] initParams() default {};
    //指定Servlet类的请求路径,相当于<url-pattern>
    String[] value() default {};
    
    boolean asyncSupported() default false;
    String smallIcon() default "";
    String largeIcon() default "";
    String description() default "";
    String displayName() default "";
}
4、@WebServlet注解案例演示

/**
 * 当注解的属性为一个数组且数组中只存在一个元素,大括号可以省略
 * value属性与urlPatterns属性一致,用于指定Servlet类对应的请求路径
 * 若属性名为value,则value属性名可以省略,@WebServlet("请求路径")
 */
@WebServlet(name = "hello",
        urlPatterns = {"/hello01", "/hello02"}, loadOnStartup = 1,
        initParams = {@WebInitParam(name = "username", value = "jxs"), @WebInitParam(name = "userid", value = "1")}
)
public class HelloServlet extends HttpServlet {
    //无参构造方法
    public HelloServlet() {
        System.out.println("HelloServlet无参构造方法执行");
    }

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        //获取Servlet的name
        String servletName = getServletName();
        out.print(servletName + "<br>");
        //获取Servlet类对应的请求路径
        String servletPath = request.getServletPath();
        out.print(servletPath + "<br>");
        //获取初始化参数
        Enumeration<String> names = getInitParameterNames();
        while (names.hasMoreElements()) {
            String name = names.nextElement();
            String value = getInitParameter(name);
            out.print(name + "=" + value + "<br>");
        }
    }
}
5、使用反射机制解析注解

/**
 * 使用反射机制将HelloServlet类上的注解进行解析
 */
public class ReflectAnnotation {
    public static void main(String[] args) {
        try {
            //获取HelloServlet类对应的字节码对象
            Class<?> helloServletClass = Class.forName("HelloServlet");
            //判断HelloServlet类上是否存在@WebServlet注解对象
            if (helloServletClass.isAnnotationPresent(WebServlet.class)) {
                //获取HelloServlet类上的注解对象
                WebServlet webServletAnnotation = helloServletClass.getAnnotation(WebServlet.class);
                //获取注解对象的value属性的值
                String[] paths = webServletAnnotation.urlPatterns();
                for (int i = 0; i < paths.length; i++) {
                    String path = paths[i];
                    System.out.println(path);
                }
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        }
    }
}
模板方法设计模式优化crud项目
1、注解解决web.xml文件问题，crud项目仍存在臃肿问题

2、单表的crud，编写了6个Servlet类，若一个复杂的业务系统遵循该开发方式会导致类爆炸

3、解决类爆炸问题

(1)以前的设计是一个请求对应一个Servlet类
(2)修改设计:一个请求对应一个方法,一个业务对应一个Servlet类
4、编写DeptServlet类

/**
 * 模板类
 */
@WebServlet({"/list", "/add", "/delete", "/edit", "/modify", "/detail"})
public class DeptServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取Servlet对应的请求路径
        String servletPath = request.getServletPath();
        //
        if ("/list".equals(servletPath)) {
            doList(request, response);
        } else if ("/add".equals(servletPath)) {
            doAdd(request, response);
        } else if ("/delete".equals(servletPath)) {
            doDel(request, response);
        } else if ("/edit".equals(servletPath)) {
            doEdit(request, response);
        } else if ("/modify".equals(servletPath)) {
            doModify(request, response);
        } else if ("/detail".equals(servletPath)) {
            doDetail(request, response);
        }
    }

    private void doList(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应的内容类型以及字符集
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        //获取webapp的根路径
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("<head>");
        out.print("<meta charset='utf-8'>");
        out.print("<title>部门列表页面</title>");

        out.print("<script type='text/javascript'>");
        out.print("    function del(deptno) {");
        out.print("        if(window.confirm('确认删除?')) {");
        out.print("            document.location.href = '" + contextPath + "/delete?deptno=' + deptno;");
        out.print("        }");
        out.print("    }");
        out.print("</script>");

        out.print("</head>");
        out.print("<body>");
        out.print("	<form>");
        out.print("		<table>");
        out.print("			<tr>");
        out.print("				<td>部门编号</td>");
        out.print("				<td>部门名称</td>");
        out.print("				<td>部门地址</td>");
        out.print("				<td>部门操作</td>");
        out.print("			</tr>");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select deptno,deptname,location from dept";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {

                String deptno = resultSet.getString("deptno");
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                //以下为动态的
                out.print("			<tr>");
                out.print("				<td>" + deptno + "</td>");
                out.print("				<td>" + deptname + "</td>");
                out.print("				<td>" + location + "</td>");
                out.print("				<td>");
                //href后设置javascript:void(0)表示点击此超链接后执行一段JS代码而不进行页面的跳转
                out.print("					<a href='javascript:void(0)' onclick='del(" + deptno + ")'>删除</a>");
                out.print("					<a href='" + contextPath + "/edit?deptno=" + deptno + "'>修改</a>");
                out.print("					<a href='" + contextPath + "/detail?deptno= " + deptno + "'>详情</a>");
                out.print("				</td>");
                out.print("			</tr>");
                //以上为动态的
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        //以下为固定的
        out.print("		</table>");
        out.print("		<a href='" + contextPath + "/add.html'>新增部门</a>");
        out.print("	</form>");
        out.print("</body>");
        out.print("</html>");
    }

    private void doAdd(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        /*
        (1)前端用户以post方式提交的数据封装在Http请求协议的请求体中
        (2)Tomcat服务器将Http请求协议中的数据封装在HttpServletRequest对象中
        (3)用户的一次请求对应一个HttpServletRequest对象
        (4)面向HttpServletRequest接口编程可以获取用户提交的数据
         */
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        int i = 0;
        String contextPath = request.getContextPath();

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "insert into dept values (?,?,?)";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            preparedStatement.setString(2, deptname);
            preparedStatement.setString(3, location);
            //执行SQL语句,返回受影响的行数
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, null);
        }

        //新增页面成功跳转到部门列表
        if (i == 1) {
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doDel(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "delete from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            //返回数据库中表的受影响的行数
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        if (i == 1) {
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doEdit(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应内容的类型
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print("	<head>");
        out.print("		<meta charset='utf-8'>");
        out.print("		<title>修改部门</title>");
        out.print("	</head>");
        out.print("	<body>");
        out.print("		<form action='" + contextPath + "/modify' method='post'>");
        out.print("			<table>");


        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        try {
            connection = DBUtils.getConnection();
            String sql = "select * from dept where deptno = ?";
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            resultSet = preparedStatement.executeQuery();
            if (resultSet.next()) {
                //deptname、location为SQL语句查询结果列的列名
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                out.print("				<tr>");
                out.print("					<td>部门编号</td>");
                out.print("					<td><input type='text' name='deptno' value='" + deptno + "' readonly/></td>");
                out.print("				</tr>");
                out.print("				<tr>");
                out.print("					<td>部门名称</td>");
                out.print("					<td><input type='text' name='deptname' value='" + deptname + "'/></td>");
                out.print("				</tr>");
                out.print("				<tr>");
                out.print("					<td>部门地址</td>");
                out.print("					<td><input type='text' name='location' value='" + location + "'/></td>");
                out.print("				</tr>");
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        out.print("				<tr>");
        out.print("					<td><input type='submit' value='修改部门'/></td>");
        out.print("				</tr>");
        out.print("			</table>");
        out.print("		</form>");
        out.print("	</body>");
        out.print("</html>");
    }

    private void doModify(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            String sql = "update dept set deptname = ? , location = ? where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptname);
            preparedStatement.setString(2, location);
            preparedStatement.setString(3, deptno);
            //执行SQL语句
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        }

        if (i == 1) {
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doDetail(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //设置响应内容类型
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        //获取部门编号
        String deptno = request.getParameter("deptno");
        //获取webapp的根路径
        String contextPath = request.getContextPath();

        out.print("<!DOCTYPE html>");
        out.print("<html>");
        out.print(" <head>");
        out.print("     <meta charset='utf-8'>");
        out.print("     <title>部门详情</title>");
        out.print("</head>");
        out.print("<body>");
        out.print(" <h1>部门详情</h1>");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select * from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, deptno);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集(deptno为主键,不可重复,所以此结果集只有一条记录)
            while (resultSet.next()) {
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");

                out.print(" <h4>部门编号:" + deptno + "</h4>");
                out.print(" <h4>部门名称:" + deptname + "</h4>");
                out.print(" <h4>部门地址:" + location + "</h4>");

            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }

        out.print(" <a href='" + contextPath + "/list" + "'>返回上一级</a>");
        out.print("</body>");
        out.print("</html>");
    }
}
JSP
JSP原理剖析
JSP引出
1、Servlet中编写html、css、javascript前端代码，存在什么问题？

(1)java程序中编写前端代码,编写难度大,难于发现错误
(2)java程序中编写前端代码,程序的耦合度高
(3)java程序中编写前端代码,代码不美观
(4)java程序中编写前端代码,难以维护
(5)修改java程序中的前端代码,若有改动则需重新编译生成class字节码文件
2、如何解决以上问题？

程序员无需编写Servlet(java程序),机器自动生成。
程序员只需编写Servlet(java程序)中的前端代码,机器自动将程序员编写的前端代码翻译生成为Servlet(java程序)中的前端代码
机器自动将Servlet(java程序)翻译生成class字节码文件
3、机器自动将前端代码翻译生成为Servlet（java程序）中的前端代码

<html>
    <head>
    </head>
</html>

自动翻译生成为:

out.print("<html>");
    out.print("<head>");
    out.print("</head>");
out.print("</html>");
JSP原理（重要！！）
1、web应用根路径下创建index.jsp文件，index.jsp文件中无任何内容。

2、部署项目后，启动Tomcat服务器，打开浏览器地址栏输入：http://localhost:8080/jsp/index.jsp，浏览器显示空白

(1)实际上，访问index.jsp文件，底层执行index_jsp.class
(2)index.jsp被Tomcat服务器翻译生成index_jsp.java文件，Tomcat服务器又将index_jsp.java文件编译生成index_jsp.class文件
3、JSP实际上就是一个Servlet

(1)访问index.jsp文件时，Tomcat服务器自动翻译生成index_jsp.java文件，Tomcat服务器将index_jsp.java文件自动编译生成index_jsp.class文件。
(2)index_jsp就是一个类，index_jsp继承HttpJspBase，HttpJspBase继承HttpServlet。所以index_jsp类为Servlet类
(3)jsp的生命周期和Servlet的生命周期完全相同
4、jsp文件为何第一次访问比较缓慢？

第一次访问jsp文件:
Tomcat服务器将jsp文件翻译生成java文件
Tomcat服务器再将java文件编译生成class字节码文件
通过反射机制创建Servlet对象
调用Servlet对象的init方法
调用Servlet对象的service方法

第二次访问jsp文件:
调用单例Servlet对象的service方法
5、何为JSP？

(1)JSP是java程序
(2)JSP:JavaServer Pages,基于java语言实现的服务器端的页面
(3)Servlet为JavaEE的13个子规范之一;JSP也为JavaEE的13个子规范之一
(4)JSP是一套规范,所有的Web服务器都遵循该规范进行翻译生成
(5)每一Web服务器都会内置一个JSP翻译引擎
(6)JSP翻译引擎根据不同的符号翻译到不同的位置
6、JSP本质上为Servlet，JSP和Servlet有何区别？

(1)职责不同
(2)JSP职责:展示数据(显示数据)
(3)Servlet职责:收集数据(逻辑处理、业务处理、连接数据库、获取数据)
7、对JSP进行错误调试时，直接打开JSP文件对应的java文件，检查java代码

8、开发JSP的最高境界：眼前为JSP代码，脑袋中呈现java代码

JSP语法详解
1、JSP基础语法

(1)JSP文件中编写文字,文字会被自动翻译到Servlet类中的service方法的out.write("文字"),当作普通字符串打印输出到浏览器
(2)JSP文件中编写的html、css、javascript代码,这些代码对于JSP来说为一个普通的字符串。但JSP将这个普通的字符串输出到浏览器,浏览器将会对html、css、javascript代码进行解释执行,展现效果
(3)JSP的page指令,解决响应时的中文乱码问题。通过page指令设置响应的内容类型以及字符集(<%@page contentType="text/html;charset=UTF-8" %>),表示相应内容类型为text/html,字符集为UTF-8
2、service方法中编写java程序

(1)<% java语句 %>
(2)<%%>符号中编写的视为java程序,被翻译到Servlet类的service方法内部
(3)<%%>符号中编写的java程序会被Tomcat服务器翻译生成到Servlet类中的service方法中
(4)service方法中编写的代码遵循自上而下的顺序依次逐行执行
(5)service方法中不可编写静态代码块、不可编写方法、不可定义成员变量...
3、service方法外编写java程序

(1)<%! java语句 %>
(2)<%!%>符号中编写的视为java程序,被翻译到Servlet类的service方法外部
(3)<%!%>符号中可以编写静态代码块、可以编写方法、可以定义成员变量...
(4)<%!%>符号很少使用,因为在service方法外定义静态变量和实例变量会存在线程安全问题
(5)JSP为Servlet类,Servlet类为单例的,多线程并发的环境下,静态变量和实例变量一旦存在修改操作则必然发生线程安全问题
4、JSP中注释

<!-- -->:此注释不专业,会被Tomcat服务器翻译到java源代码中,JSP中不使用此注释
<%-- --%>:JSP专业注释,不会被Tomcat服务器翻译到java源代码中
5、JSP输出语法

(1)使用JSP九大内置对象之一out输出
<%
    String name = "jxs";
    out.write("name=" + name);
%>
out为JSP的九大内置对象之一,可以在service方法内部直接使用

(2)若输出内容无java代码,例:输出"jxs"固定的字符串,无需写入到<% java语句 %>

(3)
若输出内容存在java代码,可使用语法格式:<%= %>,=后编写输出内容。
<%= %>符号被翻译到service方法中,翻译为out.print();
输出的内容含有java变量,输出的内容为一个动态的内容,输出的内容不为字符串时使用<%= %>符号。若输出的内容为一个字符串,则直接在JSP文件中编写即可。
6、JSP语法案例演示

<%-- page指令设置响应的内容类型以及字符集 --%>
<%@page contentType="text/html;charset=UTF-8" %>

<%-- <%%>中编写java语句 --%>
<% System.out.println("Hello JXS");%>

<%--
    service方法中定义变量不可使用访问修饰符
    private int i;

    service方法中不可编写静态代码块
    static {
        System.out.println("静态代码块");
    }

    service方法中不可编写方法
    public static void method() {
        System.out.println("method execute");
    }
--%>

<% int i = 100; %>
<% System.out.println(i); %>

<% System.out.println("Hello Servlet"); %>
<%--
类体中不可直接打印输出
<%! System.out.println("Hello Servlet"); %>
--%>

<% System.out.println(j); %>
<%!
    //service方法外定义成员变量、静态代码块、方法
    private int j = 200;

    static {
        System.out.println("静态代码块");
    }

    public static void method() {
        System.out.println("method execute");
    }
%>

<%
    //使用JSP九大内置对象之一out输出变量
    String name = "jxs";
    out.write("name=" + name);
%>

<%--
将<%= 100 + 200%>翻译到index_jsp.java中为out.print(100 + 200);
<%= %>符号翻译为out.print();
--%>
<%= 100 + 200%>

<%
    int a = 100;
    int b = 200;
%>
<%--翻译为out.print(a + b);--%>
<%= a + b%>
JSP总结（精华！！）
1、JSP：JavaServer Pages，基于Java语言实现的服务器端的页面。JSP属于JavaEE的13个子规范之一。每一Web服务器都会内置一个JSP翻译引擎。

2、

访问index.jsp文件时，Tomcat服务器将index.jsp文件中的内容翻译生成为index_jsp.java文件，Tomcat服务器又将index_jsp.java文件编译生成index_jsp.class文件。index_jsp为一个类，index_jsp类继承HttpJspBase类，HttpJspBase类继承HttpServlet类，即index_jsp为Servlet类。

3、

JSP中编写文字，文字会被自动翻译到Servlet类中的service方法中，当作普通字符串打印输出到浏览器；

JSP中编写HTML、CSS、JavaScript代码，HTML、CSS、JavaScript代码会被自动翻译到Servlet类中的service方法中，当作普通字符串打印输出到浏览器，浏览器对HTML、CSS、JavaScript代码进行解释执行；

JSP中<% java语句 %>符号中编写的内容视为java程序，会被自动翻译到Servlet类中的service方法中，JSP中<%! java语句 %>符号中编写的内容视为java程序，会被自动翻译到Servlet类中的service方法外。

4、JSP与Servlet区别：JSP与Servlet职责不同。JSP负责展示数据；Servlet负责收集数据

5、JSP输出语法：使用JSP九大内置对象之一out输出；使用<%= %>符号，<%= %>翻译为out.print();，翻译到Servlet类中的service方法中。

Servlet和JSP改造crud项目
1、改造步骤

(1)
将html原型文件修改为jsp文件,每个jsp文件头部添加
<%@page contentType="text/html;charset=UTF-8" %>
防止中文乱码问题。将所有jsp文件拷贝到webapp的根路径下

(2)
修改超链接的请求路径,完成所有页面的正常跳转
<% String contextPath = request.getContextPath(); %>
<a href = "<%= contextPath%>/list.jsp"></a>
JSP中动态的获取webapp的根路径

(3)
Servlet中连接数据库,获取所有部门信息,遍历结果集
遍历结果集,取出部门编号,部门名称、部门地址,封装成Dept对象实例
将Dept对象实例存放到List集合中
将List集合存放到request请求域中
转发到list.jsp

(4)
JSP中从request请求域中取出集合List
遍历集合,取出每一个Dept对象实例
动态生成tr
2、若只使用JSP技术，是否可以开发web应用

(1)可以！

(2)
JSP本质就是一个Servlet,<% java语句 %>符号中的内容会自动翻译到Servlet类中的service方法中,在JSP中<% java语句 %>符号中编写JDBC代码,连接数据库,获取数据。

(3)
虽然JSP技术可以完成web应用,但是单纯使用JSP开发web应用职责不明确！
还是建议采用Servlet+JSP的方式进行开发,Servlet负责处理业务逻辑、连接数据库、获取数据;JSP负责显示数据。职责分明！
3、JSP文件扩展名必须为.jsp吗？

(1)JSP文件扩展名是可以配置的,不是固定的
(2)CATALINA_HOME/conf/web.xml文件中配置JSP文件扩展名
(3)JSP文件对于Tomcat服务器只是一个普通的文本文件,Tomcat服务器将xxx.jsp文件翻译为xxx_jsp.java文件,Tomcat服务器再将xxx_jsp.class文件。最终执行的是xxx_jsp类中的方法,和xxx.jsp文件无关。
<servlet-mapping>
    <servlet-name>jsp</servlet-name>
    <url-pattern>*.jsp</url-pattern>
    <url-pattern>*.jspx</url-pattern>
</servlet-mapping>
4、包名bean什么意思？

(1)java的logo是一杯热气腾腾的的咖啡,javabean被翻译为咖啡豆
(2)咖啡由一粒一粒咖啡豆研磨而成,java由众多javabean组成
(3)javabean即符合某种规范的java类
	提供无参构造方法
	属性私有化
	对外提供共有的getter、setter方法
	重写toString方法
	重写hashCode、equals方法
	实现java.io.Serializable接口(序列化、反序列化)
(4)javabean即java中的实体类,负责数据的封装
5、学习目标

(1)Servlet+JSP
	session
	cookie
	EL表达式
	JSTL标签
	Filter
	Listener
(2)AJAX
(3)jQuery
(4)Vue
(5)MVC架构模式
(6)连接池
(7)SSM
(8)Maven
(9)git
index.jsp
<%@ page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>欢迎页</title>
    </head>
    <body>
        <%--
        (1)<% java语句 %>符号内编写的java语句翻译到Servlet类中的service方法中
        (2)调用JSP九大内置对象之一request的getContextPath方法获取webapp的根路径
        (3)前端发送请求路径时以"/项目名"开始
        (4)<%= contextPath%>翻译为out.print(contextPath),即out.print(/crud)
        (5)执行Servlet,连接数据库,查询数据、收集数据
        (6)JSP展示数据
        --%>
        <a href="<%= request.getContextPath()%>/list">部门列表</a>
    </body>
</html>
list.jsp
<%@ page import="java.util.List" %>
<%@ page import="bean.Dept" %>
<%@ page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>部门列表页面</title>
    </head>

    <body>
        <script type="text/javascript">
            function del(deptno) {
                var result = window.confirm("确认删除？");
                if (result) {
                    <% String contextPath = request.getContextPath(); %>
                    document.location.href = "<%= contextPath%>/delete?deptno=" + deptno;
                }
            }
        </script>
        <form>
            <table>
                <tr>
                    <td>部门编号</td>
                    <td>部门名称</td>
                    <td>部门地址</td>
                    <td>部门操作</td>
                </tr>

                <%
                    //request请求域中获取数据
                    List<Dept> deptList = (List<Dept>)request.getAttribute("deptList");
                    //遍历List集合
                    for (Dept dept : deptList) {
                        String deptno = dept.getDeptno();
                        String deptname = dept.getDeptname();
                        String location = dept.getLocation();
                %>

                <tr>
                    <td><%= deptno%></td>
                    <td><%= deptname%></td>
                    <td><%= location%></td>
                    <td>
                        <a href="javascript:void(0)" onclick="del(<%= deptno%>)">删除</a>
                        <a href="<%= contextPath%>/edit?deptno=<%= deptno%>">修改</a>
                        <a href="<%= contextPath%>/detail?deptno=<%= deptno%>">详情</a>
                    </td>
                </tr>

                <%
                    }
                %>

            </table>
            <a href="<%= contextPath%>/add.jsp">新增部门</a>
        </form>
    </body>
</html>
detail.jsp
<%@ page import="java.util.List" %>
<%@ page import="bean.Dept" %>
<%@page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>部门详情</title>
    </head>
    <body>
        <%--获取webapp的根路径--%>
        <% String contextPath = request.getContextPath(); %>

        <%
            //request请求域中获取List集合
            List<Dept> deptList = (List<Dept>)request.getAttribute("deptList");
            //遍历List集合
            for (Dept dept : deptList) {
                String deptno = dept.getDeptno();
                String deptname = dept.getDeptname();
                String location = dept.getLocation();
        %>

        <h1>部门详情</h1>
        <h4>部门编号:<%= deptno%></h4>
        <h4>部门名称:<%= deptname%></h4>
        <h4>部门地址:<%= location%></h4>

        <%
            }
        %>

        <a href="<%= contextPath%>/list">返回上一级</a>
    </body>
</html>
add.jsp
<%@page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>新增部门</title>
    </head>
    <body>
        <% String contextPath = request.getContextPath(); %>
        <form action="<%= contextPath%>/add" method="get">
            <table>
                <tr>
                    <td>部门编号</td>
                    <td><input type="text" name="deptno"/></td>
                </tr>
                <tr>
                    <td>部门名称</td>
                    <td><input type="text" name="deptname"/></td>
                </tr>
                <tr>
                    <td>部门地址</td>
                    <td><input type="text" name="location"/></td>
                </tr>
                <tr>
                    <td><input type="submit" value="新增部门"/></td>
                </tr>
            </table>
        </form>
    </body>
</html>
edit.jsp
<%@ page import="java.util.List" %>
<%@ page import="bean.Dept" %>
<%@page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>修改部门</title>
    </head>
    <body>
        <%
            //获取webapp的根路径
            String contextPath = request.getContextPath();

            //request请求域中获取List集合
            List<Dept> deptList = (List<Dept>)request.getAttribute("deptList");
            //遍历List集合
            for (Dept dept : deptList) {
                String deptno = dept.getDeptno();
                String deptname = dept.getDeptname();
                String location = dept.getLocation();
        %>

        <form action="<%= contextPath%>/modify" method="get">
            <table>
                <tr>
                    <td>部门编号</td>
                    <td><input type="text" name="deptno" value="<%= deptno%>" readonly/></td>
                </tr>
                <tr>
                    <td>部门名称</td>
                    <td><input type="text" name="deptname" value="<%= deptname%>"/></td>
                </tr>
                <tr>
                    <td>部门地址</td>
                    <td><input type="text" name="location" value="<%= location%>"/></td>
                </tr>
                <tr>
                    <td><input type="submit" value="修改部门"/></td>
                </tr>
            </table>
        </form>

    <%
        }
    %>
    </body>
</html>
Dept实体类
/**
 * 普通的java类,封装零散的数据
 * 一个Dept类对象实例代表一个部门对象
 */
public class Dept {
    private String deptno;
    private String deptname;
    private String location;

    public Dept() { }

    public String getDeptno() {
        return deptno;
    }
    public void setDeptno(String deptno) {
        this.deptno = deptno;
    }
    public String getDeptname() {
        return deptname;
    }
    public void setDeptname(String deptname) {
        this.deptname = deptname;
    }
    public String getLocation() {
        return location;
    }
    public void setLocation(String location) {
        this.location = location;
    }

    @Override
    public String toString() {
        return "Dept{" +
                "deptno='" + deptno + '\'' +
                ", deptname='" + deptname + '\'' +
                ", location='" + location + '\'' +
                '}';
    }
}
DeptServlet
/**
 * 模板类
 */
@WebServlet({"/list", "/detail", "/edit", "/delete", "/add", "/modify"})
public class DeptServlet extends HttpServlet {
    @Override
    protected void service(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取Servlet类对应的请求路径
        String servletPath = request.getServletPath();

        //if判断
        if ("/list".equals(servletPath)) {
            doList(request, response);
        } else if ("/detail".equals(servletPath)) {
            doDetail(request, response);
        } else if ("/edit".equals(servletPath)) {
            doEdit(request, response);
        } else if ("/delete".equals(servletPath)) {
            doDel(request, response);
        } else if ("/add".equals(servletPath)) {
            doAdd(request, response);
        } else if ("/modify".equals(servletPath)) {
            doModify(request, response);
        }
    }

    private void doModify(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号、部门名称、部门地址
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "update dept set deptname = ?,location = ? where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句问号赋值
            preparedStatement.setString(1, deptname);
            preparedStatement.setString(2, location);
            preparedStatement.setString(3, deptno);
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, null);
        }
        if (i == 1) {
            //重定向
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doAdd(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号、部门名称、部门地址
        String deptno = request.getParameter("deptno");
        String deptname = request.getParameter("deptname");
        String location = request.getParameter("location");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "insert into dept values (?,?,?)";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句问号赋值
            preparedStatement.setString(1, deptno);
            preparedStatement.setString(2, deptname);
            preparedStatement.setString(3, location);
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, null);
        }
        if (i == 1) {
            //重定向
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doDel(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        int i = 0;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "delete from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句第一次问号赋值
            preparedStatement.setString(1, deptno);
            //执行SQL语句
            i = preparedStatement.executeUpdate();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, null);
        }
        if (i == 1) {
            //重定向
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }

    private void doEdit(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        List<Dept> deptList = new ArrayList<>();

        //获取部门编号
        String deptno = request.getParameter("deptno");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select * from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句第一次问号赋值
            preparedStatement.setString(1, deptno);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");
                //将零散的数据封装至Dept对象实例
                Dept dept = new Dept();
                dept.setDeptno(deptno);
                dept.setDeptname(deptname);
                dept.setLocation(location);
                //将Dept对象实例存储至List集合
                deptList.add(dept);
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }
        //将List集合存储至request请求域
        request.setAttribute("deptList", deptList);
        //转发
        request.getRequestDispatcher("/edit.jsp").forward(request, response);
    }

    /**
     * @param request
     * @param response
     * @throws ServletException
     * @throws IOException
     */
    private void doDetail(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取部门编号
        String deptno = request.getParameter("deptno");
        //准备List集合存储Dept对象实例
        List<Dept> deptList = new ArrayList<>();

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select * from dept where deptno = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //为SQL语句第一次问号赋值
            preparedStatement.setString(1, deptno);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");
                //将零散的数据封装到Dept对象实例中
                Dept dept = new Dept();
                dept.setDeptno(deptno);
                dept.setDeptname(deptname);
                dept.setLocation(location);
                deptList.add(dept);
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            DBUtils.close(connection, preparedStatement, resultSet);
        }
        //将List集合存放至request请求域
        request.setAttribute("deptList", deptList);
        //转发
        request.getRequestDispatcher("/detail.jsp").forward(request, response);
    }

    /**
     * Servlet负责连接数据库,查询所有部门信息
     * 收集所有部门信息后跳转到list.jsp
     * JSP负责展示数据
     *
     * @param request
     * @param response
     * @throws ServletException
     * @throws IOException
     */
    private void doList(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //准备List集合存放Dept对象实例
        List<Dept> deptList = new ArrayList<>();

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            //SQL语句
            String sql = "select * from dept";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            //执行SQL语句
            resultSet = preparedStatement.executeQuery();
            //处理结果集
            while (resultSet.next()) {
                //从结果集中取出数据,将数据封装到Dept对象实例中
                String deptno = resultSet.getString("deptno");
                String deptname = resultSet.getString("deptname");
                String location = resultSet.getString("location");
                //将以上零散的数据封装为Dept对象
                Dept dept = new Dept();
                dept.setDeptno(deptno);
                dept.setDeptname(deptname);
                dept.setLocation(location);
                //将Dept对象实例存放至List集合中
                deptList.add(dept);
            }
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }
        //将List集合存放至request请求域
        request.setAttribute("deptList", deptList);
        //转发
        request.getRequestDispatcher("/list.jsp").forward(request, response);
    }
}
JSP指令
1、JSP指令基本介绍

(1)指导JSP翻译引擎如何翻译JSP文件
(2)JSP指令包括
	include指令:包含指令,JSP中完成静态包含
	taglib指令:引入标签库指令
	page指令
(3)指令使用语法:<%@ 指令名 属性名=属性值 属性名=属性值 属性名=属性值... %>
2、page指令

(1)<%@ page session="false/true" %>:true表示启用JSP内置对象session、false表示不启用JSP内置对象session,若未设置默认为true
(2)<%@ page contentType="text/html" %>:设置响应内容类型
(3)<%@ page pageEncoding="UTF-8" %>:设置响应内容字符集 
(4)<%@ page import="java.util.*" %>:导包
(5)<%@ page errorPage="/xxx.jsp" %>:设置出现异常后跳转的页面
(6)<%@ page isErrorPage="true" %>:启用JSP九大内置对象之一exception,若未设置默认为false
JSP九大内置对象
1、jakarta.servlet.jsp.PageContext pageContext 页面域

2、jakarta.servlet.http.HttpServletRequest request 请求域

3、jakarta.servlet.http.HttpSession session 会话域

4、jakarta.servlet.ServletContext application 应用域

(1)作用域范围:pageContext < request < session < application
(2)四个作用域都有setAttribute、getAttribute、removeAttribute方法
(3)以上作用域使用原则:尽可能使用小的作用域
5、java.lang.Throwable exception

6、jakarta.servlet.ServletConfig config

7、java.lang.Object page

(1)即this,当前的Servlet对象
8、jakarta.servlet.jsp.JspWriter out

9、jakarta.servlet.http.HttpServletResponse response

(1)out负责输出
(2)response负责响应
session
crud项目实现用户登录功能
1、当前crud项目存在问题？

(1)任意用户可以访问此系统,都可对当前系统中的数据进行增删改操作
(2)设计用户登录功能实现合法的用户可以登录系统,不合法的用户不可以登录系统
(3)crud项目添加登录功能,登录成功可以访问该系统,登录失败不可以访问该系统
2、登录功能实现步骤

(1)创建index.jsp登录页面,index.jsp登录页面设置表单
(2)表单中设置文本框、密码框,用户点击提交按钮以post方式提交数据
(3)数据库新建用户表,存储用户的用户名、密码(密码在数据库中存储的为密文,一般不以明文的形式存储)
(4)后台Servlet处理登录请求
	登录成功跳转部门列表页面
	登录失败跳转登录失败页面
DROP TABLE IF EXISTS `user`;

CREATE TABLE `user`(
id INT PRIMARY KEY,
username VARCHAR(255),
`password` VARCHAR(255));

INSERT INTO user VALUES (1,"jxs","123456"),(2,"dwy","123456");
3、index.jsp登录页面，以post方式提交数据至/login请求路径对应的Servlet类，进行逻辑处理

<%@ page contentType="text/html;charset=UTF-8" %>

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>登陆页面</title>
    </head>
    <body>
        <h1>用户登录</h1>
        <%--
        (1)<% java语句 %>符号内编写的java语句翻译到Servlet类中的service方法中
        (2)调用JSP九大内置对象之一request的getContextPath方法获取webapp的根路径
        (3)前端发送请求路径时以"/项目名"开始
        (4)<%= contextPath%>翻译为out.print(contextPath),即out.print(/crud)
        (5)执行Servlet,连接数据库,查询数据、收集数据
        (6)JSP展示数据
        --%>
        <% String contextPath = request.getContextPath(); %>

        <form action="<%= contextPath%>/login" method="post">
            <table>
                <tr>
                    <td>用户名</td>
                    <td><input type="text" name="username"></td>
                </tr>
                <tr>
                    <td>密码</td>
                    <td><input type="password" name="password"></td>
                </tr>
                <tr>
                    <td><input type="submit" value="登录"></td>
                </tr>
            </table>
        </form>
    </body>
</html>
4、DeptServlet模板类中doLogin方法，获取用户提交的数据，将获取的数据与数据库中的数据进行比对，登录成功则重定向至部门列表页面。

private void doLogin(HttpServletRequest request, HttpServletResponse response)
    throws ServletException, IOException {
    /*
        Web前端用户以post方式提交的数据存储至Http请求协议中的请求体中
        Http请求协议中的数据存储至request请求域中
        获取前端用户提交的用户名、密码
         */
    String username = request.getParameter("username");
    String password = request.getParameter("password");

    Connection connection = null;
    PreparedStatement preparedStatement = null;
    ResultSet resultSet = null;

    try {
        //获取数据库连接对象
        connection = DBUtils.getConnection();
        String sql = "select * from user where username = ? and password = ?";
        //获取数据库操作对象
        preparedStatement = connection.prepareStatement(sql);
        preparedStatement.setString(1, username);
        preparedStatement.setString(2, password);
        //获取结果集
        resultSet = preparedStatement.executeQuery();
    } catch (Exception exception) {
        System.out.println(exception.getMessage());
    } finally {
        //释放资源
        DBUtils.close(connection, preparedStatement, resultSet);
    }
    /*
        处理结果集
        结果集中最多只有一条数据
         */
    if (resultSet != null) {
        //重定向
        response.sendRedirect(request.getContextPath() + "/list");
    }
}
5、crud项目仍存在什么问题？

(1)登录功能虽然实现了,但无任何作用
(2)用户只要知道部门列表的请求路径,在不使用登录功能的情况下仍可以访问用户列表
(3)此登录功能无拦截作用
session机制
1、何为session？

(1)session:会话
(2)一次会话:用户打开浏览器,进行一系列操作,最终关闭浏览器的整个过程
(3)一次请求:用户打开浏览器,地址栏输入URL回车、点击一个超链接、点击一个按钮的操作
(4)请求对应的服务器的java对象:request;会话对应的服务器的java对象:session
(5)一次会话对应N次请求
(6)Servlet规范中,session对应的类名:jarkata.servlet.http.HttpSession
(7)session机制属于B/S结构一部分,session机制是一种规范,不同的语言对于session机制有不同的实现
(8)session对象作用:保存会话状态
	例:用户登录网站成功后为网站登录成功状态,使用session对象可以保存会话状态
(9)为何需要session对象来保存会话状态
	9.1、HTTP协议为无状态协议
	9.2、无状态协议:用户发送请求时,Browser端与Server端是连接的;页面展示完毕,请求结束后,Browser端与Server端断开连接
	9.3、HTTP协议为何为无状态协议:用户发送请求至服务器,服务器响应数据至浏览器,浏览器页面展示完毕,浏览器与服务器断开连接,此操作可以降低服务器压力
	9.4、用户发送请求至服务器,服务器响应数据至浏览器,浏览器页面展示完毕后,浏览器与服务器断开连接,用户关闭浏览器后,服务器不知道浏览器关闭
2、为何不使用request对象保存会话状态？为何不使用ServletContext对象保存会话状态？

(1)
request.setAttribute(String name,Object obj)             request请求域中绑定数据
request.getAttribute(String name)                        request请求域中获取数据
request.removeAttribute(String name)                     request请求域中删除数据
servletContext.setAttribute(String name,Object obj)      应用域中绑定数据
servletContext.getAttribute(String name)                 应用域中获取数据
servletContext.removeAttribute(String name)              应用域中删除数据

(2)
一次请求对应一个request对象
Tomcat服务器启动时创建servletContext对象,Tomcat服务器关闭时销毁servletContext对象

(3)
request请求域(HttpServletRequest对象)
session会话域(HttpSession对象)
application应用域(ServletContext对象)
作用域范围:request < session < application
3、request对象、session对象、application对象

(1)request对象
	用户向服务器端发送请求,服务器端响应数据至浏览器端,页面展示完毕后销毁request对象
	用户向服务器端发送新的请求,服务器端会创建新的request对象,该request对象与之前的request对象无关,因此无法获得之前的request对象中存放的任何数据。

(2)session对象
	同一个浏览器窗口中,用户无论向服务器端发送多少请求,session对象只有一个。
	只要浏览器不关闭,session对象就一直存在。

(3)application对象
	Tomcat服务器启动时创建application对象,Tomcat服务器关闭时销毁application对象
	Tomcat服务器运行过程中只存在一个application对象
session实现原理（重要！！）
1、session原理图

![](E:\Study\自学课程资料\Java\assets\session原理图.png)

2、用户第一次发送请求，Tomcat服务器创建session对象，并生成session对象对应的sessionId（特殊的Cookie—name为固定值JSESSIONID，value为session对象的ID）。Tomcat服务器将sessionId响应至浏览器，浏览器将sessionId保存至缓存中。

![](E:\Study\自学课程资料\Java\assets\服务器端响应sessionId至浏览器端.png)

3、用户第二次发送请求时，浏览器端自动将sessionId（特殊的Cookie—name为固定值JSESSIONID，value为session对象的ID）发送至服务器端，服务器端根据sessionId从session列表中获取对应的session对象。

![](E:\Study\自学课程资料\Java\assets\服务器端发送session对象至浏览器端.png)

4、sessionId为特殊的Cookie，name为固定值JSESSIONID，value为session对象的ID。sessionId保存在浏览器缓存中，浏览器关闭后sessionId销毁。

Cookie:JSESSIONID=session对象的ID
5、Cookie禁用

(1)服务器端发送Cookie至浏览器端,浏览器端拒绝接收

(2)用户发送第一次请求,服务器创建session对象并生成对应的sessionId(特殊的Cookie—name为固定值JSESSIONID,value为session对象的ID),服务器响应sessionId至浏览器,浏览器端拒绝接收Cookie。用户发送第二次请求,浏览器缓存中不存在Cookie,服务器端无法根据Cookie找到对应的session对象

(3)Cookie禁用后可通过URL重写机制实现session机制
URL重写机制格式:URL;JSESSIONID=session对象的ID
URL重写机制演示:http://localhost:8080/servlet13/sessionTest;JSESSIONID=685A00ED58B6CDC8B57069375D08D965
6、总结

(1)
一个request对象对应一个请求
一个session对象对应一个会话
一个会话包含N次请求

(2)
HttpSession session = request.getSession();
从Web服务器中获取session对象,若不存在则新建
HttpSession session = request.getSession(false);
从Web服务器中获取session对象,若不存在不会新建,返回null

(3)session实现原理
1.Web服务器中存在session列表,session列表类似于map集合
2.session列表中key为sessionId(特殊的Cookie—name为固定值JSESSIONID,value为session对象的ID)
3.session列表中value为session对象
4.用户发送第一次请求,服务器中创建session对象,同时生成session对象对应的编号sessionId。服务器将sessionId发送至浏览器,浏览器将sessionId保存至缓存中
5.用户发送第二次请求,浏览器自动将sessionId发送至服务器,服务器根据sessionId从session列表中获取对应的session对象
6.关闭浏览器,浏览器缓存中保存的sessionId销毁。重新打开浏览器时,无法根据缓存中保存的sessionId找到服务器中对应的session对象
7.session对象销毁方式
	超时销毁(浏览器关闭时.服务器无法检测浏览器是否关闭,用户超过30分钟没有与服务器交互,将超时销毁session对象)
	手动销毁(安全退出,清除服务器端session列表中的session对象,清除session对象中保存的用户状态)
session改造crud项目
1、改造步骤

(1)用户登录成功后将用户登录信息存储到session会话域中
(2)若session会话域中存在用户登录信息代表用户登录成功,反之登录失败跳转到登录页面
2、

UserServlet类中doLogin方法，用户输入用户名、密码，将输入的用户名、密码与数据库中的数据进行对比，若相同则登录成功。将登录信息存储至用户级别的session对象。

@WebServlet("/login")
public class UserServlet extends HttpServlet {
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        /*
        Web前端用户以post方式提交的数据存储至Http请求协议中的请求体中
        Http请求协议中的数据存储至request请求域中
        获取前端用户提交的用户名、密码
         */
        String username = request.getParameter("username");
        String password = request.getParameter("password");

        Connection connection = null;
        PreparedStatement preparedStatement = null;
        ResultSet resultSet = null;

        try {
            //获取数据库连接对象
            connection = DBUtils.getConnection();
            String sql = "select * from user where username = ? and password = ?";
            //获取数据库操作对象
            preparedStatement = connection.prepareStatement(sql);
            preparedStatement.setString(1, username);
            preparedStatement.setString(2, password);
            //获取结果集
            resultSet = preparedStatement.executeQuery();
        } catch (Exception exception) {
            System.out.println(exception.getMessage());
        } finally {
            //释放资源
            DBUtils.close(connection, preparedStatement, resultSet);
        }
        /*
        处理结果集
        结果集中最多只有一条数据
         */
        if (resultSet != null) {
            /*
            获取session对象
            用户发送第一次请求,服务器创建session对象并生成对应Cookie
            服务器将Cookie响应至浏览器
            用户发送第二次请求,服务器根据浏览器缓存中的Cookie在session列表中寻找对应session对象
             */
            HttpSession session = request.getSession();
            //session会话域中绑定数据
            session.setAttribute("username", username);
            //重定向
            response.sendRedirect(request.getContextPath() + "/list");
        }
    }
}
3、service方法，当用户访问登录页面以外的页面时，执行if判断，判断session对象中登录信息是否为空。若为空则跳转至登录页面，若不为空则说明登录成功，可以访问除登录页面外的页面。

@Override
protected void service(HttpServletRequest request, HttpServletResponse response)
    throws ServletException, IOException {
    //获取Servlet类对应的请求路径
    String servletPath = request.getServletPath();
    //获取session对象
    HttpSession session = request.getSession(false);
    /*
        判断session会话域中是否存在用户登录信息
        若不存在用户登录信息则跳转用户登录界面
        若存在用户登录信息则可跳转至其他界面
         */
    if (session != null && session.getAttribute("username") != null) {
        //if判断
        if ("/list".equals(servletPath)) {
            doList(request, response);
        } else if ("/detail".equals(servletPath)) {
            doDetail(request, response);
        } else if ("/edit".equals(servletPath)) {
            doEdit(request, response);
        } else if ("/delete".equals(servletPath)) {
            doDel(request, response);
        } else if ("/add".equals(servletPath)) {
            doAdd(request, response);
        } else if ("/modify".equals(servletPath)) {
            doModify(request, response);
        }
    } else {
        //重定向
        response.sendRedirect(request.getContextPath() + "/index.jsp");
    }
}
4、安全退出，部门列表页面加入安全退出超链接。UserServlet类中重写service方法，service方法中进行if判断，若请求路径为/login则执行doLogin方法，若请求路径为/exit则执行doExit方法。doExit方法中获取session对象，移除session会话域中的用户登录信息。

private void doExit(HttpServletRequest request, HttpServletResponse response)
    throws ServletException, IOException {
    HttpSession session = request.getSession(false);
    if (session != null) {
        //手动销毁session对象
        session.invalidate();
        response.sendRedirect(request.getContextPath() + "/index.jsp");
    }
}
Cookie
1、基本介绍

session实现原理中，用户第一次发送请求，服务器创建session对象，生成session对象对应的sessionId（特殊的Cookie—name为固定值JSESSIONID，value为session对象的ID）。服务器将sessionId响应至浏览器，浏览器将sessionId保存至运行内存中，只要浏览器不关闭，用户再次发送请求时，会自动将运行内存中的sessionId发送至服务器。

(1)服务器响应Cookie至浏览器,浏览器将Cookie保存至运行内存
Set-Cookie: JSESSIONID=40649D77878D7198CA9BA3F692F3569A; Path=/servlet13; HttpOnly

(2)
以下键值对数据即Cookie对象
JSESSIONID=40649D77878D7198CA9BA3F692F3569A

(3)对于seesion对象关联的Cookie来说,Cookie保存在浏览器运行内存中,用户再次发送请求时将浏览器运行内存中的Cookie发送至服务器
Cookie: JSESSIONID=40649D77878D7198CA9BA3F692F3569A

(4)服务器根据Cookie找到对应的session对象
2、Cookie保存在何处？

(1)Cookie最终保存在浏览器客户端
(2)Cookie可以保存在浏览器运行内存中(浏览器关闭后销毁)
(3)Cookie可以保存在硬盘文件中(永久保存)
3、Cookie作用？

(1)Cookie和session机制都是为了保存会话状态
(2)session对象将会话状态保存在服务器端(session对象是存储在服务器的session列表中)
(3)Cookie将会话状态保存在浏览器客户端上(Cookie数据存储在浏览器客户端上)
(4)为何存在session机制以及Cookie:Http协议是无状态、无连接协议,需要Cookie、seesion对象来保存会话状态
4、Cookie经典案例

(1)
京东商城中,在未登录的情况下,在购物车中添加商品,关闭京东商城,关闭浏览器。再次打开浏览器,访问京东商城,购物车中的商品仍存在。

将购物车中的商品编号存在至Cookie,将Cookie保存至硬盘文件中,如此即使关闭浏览器,硬盘上的Cookie仍存在。下一次打开京东商城,查看购物车时,会自动读取本地硬盘中存储的Cookie,根据Cookie中保存的商品编号动态的展示购物车中的商品。

(2)
126邮箱十天免登录

用户输入正确的用户名、密码,并选择十天内免登录。登录成功后,浏览器客户端将用户输入的用户名、密码保存在一个Cookie中,此Cookie保存在硬盘文件中,十天内有效。十天内用户再次访问126邮箱时,浏览器将自动提交Cookie至服务器,服务器接收Cookie后自动获取用户名、密码,验证成功后自动登录

Cookie如何失效:
(1)十天后Cookie自动失效
(2)修改密码,修改密码后,再次访问126邮箱时浏览器自动提交Cookie至服务器,服务器接收Cookie后自动获取用户名、密码,由于密码修改验证失败
(3)浏览器客户端清除Cookie
5、Cookie机制、session机制不属于Java中的机制，Cookie机制、session机制属于HTTP协议中的一部分。Web开发中不管任何编程语言都需要Cookie机制、session机制。

HTTP协议中规定：任意Cookie由name和value组成，name和value都为String类型。当浏览器发送请求时，根据URL携带Cookie数据至服务器。

6、在java的Servlet中对Cookie提供哪些支持？

(1)提供jarkata.servlet.http.Cookie类来表示Cookie数据
(2)java程序通过response.addCookie(cookie)方法将Cookie数据发送至浏览器
7、Cookie有效时间

(1)java程序设置Cookie有效时间
	cookie.setMaxAge(60 * 60):设置Cookie一小时后失效
(2)若没有设置Cookie有效时间则默认Cookie存储至浏览器运行内存中
(3)只要设置Cookie有效时间大于0,此Cookie一定存储至硬盘文件中
(4)设置Cookie有效时间等于0,表示删除此Cookie(主要应用于删除浏览器上的同名Cookie)
(5)设置Cookie有效时间小于0,表示此Cookie不会被存储至硬盘文件中,而是存储至浏览器运行内存中,和不调用setMaxAge方法同一效果
8、Cookie关联路径

(1)浏览器端用户发送第一次请求"http://localhost:8080/servlet14/cookie/generate",服务器端生成Cookie对象(name为product,value为123456),若Cookie对象没有设置path则默认为"http://localhost:8080/servlet14/cookie"路径以及此路径下的子路径。即当浏览器的请求路径为"http://localhost:8080/servlet14/cookie/generate"路径以及此路径的子路径时,浏览器端自动发送Cookie对象至服务器端

(2)手动设置Cookie对象的path(cookie.setPath("/servlet14");)
表示只要为servlet14项目的请求路径都会提交Cookie对象至服务器端
Cookie案例演示
1、index.jsp文件

<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<html>
    <head>
        <title>cookie</title>
    </head>
    <body>
        <a href="<%= request.getContextPath()%>/cookie/generate">
            服务器生成cookie并将cookie响应至浏览器,
            浏览器接收cookie,
            将cookie存放至浏览器客户端。
        </a>
        <a href="<%= request.getContextPath()%>/sendCookie">
            浏览器发送cookie至服务器
        </a>
    </body>
</html>
2、点击<a href="<%= request.getContextPath()%>/cookie/generate">超链接，执行对应的Servlet类，服务器创建Cookie对象并将Cookie对象响应至浏览器端，浏览器端接收Cookie对象并将Cookie对象存放至缓存。

@WebServlet(urlPatterns = "/cookie/generate")
public class GenerateCookieServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //创建Cookie对象
        Cookie cookie01 = new Cookie("product", "123456");
        Cookie cookie02 = new Cookie("username", "123456");
        //设置Cookie一小时后失效
        cookie01.setMaxAge(60 * 60);
        cookie02.setMaxAge(60 * 60);
        //设置Cookie对象的path
        cookie01.setPath(request.getContextPath());
        cookie02.setPath(request.getContextPath());
        //将Cookie响应至浏览器
        response.addCookie(cookie01);
        response.addCookie(cookie02);
    }
}
3、点击<a href="<%= request.getContextPath()%>/sendCookie">超链接，浏览器端自动将Cookie对象发送至服务器端，服务器端通过request对象的getCookies方法获取Cookie对象

@WebServlet(urlPatterns = "/sendCookie")
public class SendCookieServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        /*
        通过request对象的getCookies方法接收浏览器端发送的Cookie对象
        浏览器端可能提交多个Cookie对象至服务器端,所以返回值为Cookie数组
        当浏览器端没有提交Cookie对象至服务器端则返回null,并不是返回长度为0的数组
         */
        Cookie[] cookies = request.getCookies();
        //判断Cookie数组是否为空
        if (cookies != null) {
            //遍历Cookie数组
            for (Cookie cookie : cookies) {
                String name = cookie.getName();
                String value = cookie.getValue();
                System.out.println(name + "=" + value);
            }
        }
    }
}
Cookie实现十天内免登录
1、实现十天内免登录步骤

(1)实现登录功能
	登录成功重定向至部门列表页面
(2)登录页面添加十天内免登录复选框
	用户选择复选框则支持十天内免登录
	用户未选择复选框则不支持十天内免登录
(3)修改UserServlet类中的doLogin方法
	用户选择十天内免登录功能则在UserServlet类中的doLogin方法中创建Cookie对象,用于存储用户名、密码,并设置Cookie对象的有效期限,将Cookie对象响应至浏览器端,浏览器端接收Cookie对象后自动将Cookie对象保存至硬盘文件中
(4)用户访问欢迎页时存在两种情况
	跳转到部门列表页面
	跳转到登录页面
2、web.xml文件中配置欢迎页

<?xml version="1.0" encoding="UTF-8"?>
<web-app xmlns="https://jakarta.ee/xml/ns/jakartaee"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="https://jakarta.ee/xml/ns/jakartaee https://jakarta.ee/xml/ns/jakartaee/web-app_5_0.xsd"
         version="5.0">

    <!--配置欢迎页面-->
    <welcome-file-list>
        <welcome-file>welcome</welcome-file>
    </welcome-file-list>

</web-app>
3、用户发送http://localhost:8080/crud请求，自动跳转到欢迎页，用户访问欢迎页时存在两种情况：跳转到部门列表页面；跳转到登陆页面

@WebServlet(urlPatterns = "/welcome")
public class WelcomeServlet extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        /*
        获取Cookie
        浏览器端可能提交多个Cookie对象至服务器端,所以返回值为Cookie数组
        当浏览器端没有提交Cookie对象至服务器端则返回null,并不是返回长度为0的数组
         */
        Cookie[] cookies = request.getCookies();

        String username = null;
        String password = null;

        if (cookies != null) {
            for (Cookie cookie : cookies) {
                String name = cookie.getName();
                if (name.equals("username")) {
                    username = cookie.getValue();
                } else if (name.equals("password")) {
                    password = cookie.getValue();
                }
            }
        }

        if (username != null && password != null) {
            //验证用户名、密码
            Connection connection = null;
            PreparedStatement preparedStatement = null;
            ResultSet resultSet = null;
            try {
                //获取数据库连接对象
                connection = DBUtils.getConnection();
                //SQL语句
                String sql = "select * from user where username = ? and password = ?";
                //获取数据库操作对象
                preparedStatement = connection.prepareStatement(sql);
                //为SQL语句第一个问号赋值
                preparedStatement.setString(1, username);
                //为SQL语句第二个问号赋值
                preparedStatement.setString(2, password);
                //获取结果集
                resultSet = preparedStatement.executeQuery();
            } catch (Exception exception) {
                System.out.println(exception.getMessage());
            } finally {
                //释放资源
                DBUtils.close(connection, preparedStatement, resultSet);
            }
            if (resultSet != null) {
                //获取session
                HttpSession session = request.getSession();
                //session会话域中绑定数据
                session.setAttribute("username", username);
                response.sendRedirect(request.getContextPath() + "/list");
            }
        } else {
            response.sendRedirect(request.getContextPath() + "/index.jsp");
        }
    }
}
4、index.jsp登录页面。用户选择十天内免登录后且登录成功后创建Cookie对象，将用户输入的用户名、密码封装到Cookie对象，设置Cookie对象的有效期限（有效期限大于0表示将Cookie对象存放至硬盘文件），设置Cookie对象的path，服务器端将Cookie对象响应至浏览器端，浏览器端接收Cookie对象后存放至缓存中。

protected void doLogin(HttpServletRequest request, HttpServletResponse response)
    throws ServletException, IOException {
    /*
        Web前端用户以post方式提交的数据存储至Http请求协议中的请求体中
        Http请求协议中的数据存储至request请求域中
        获取前端用户提交的用户名、密码
         */
    String username = request.getParameter("username");
    String password = request.getParameter("password");
    String flag = request.getParameter("flag");

    Connection connection = null;
    PreparedStatement preparedStatement = null;
    ResultSet resultSet = null;

    try {
        //获取数据库连接对象
        connection = DBUtils.getConnection();
        String sql = "select * from user where username = ? and password = ?";
        //获取数据库操作对象
        preparedStatement = connection.prepareStatement(sql);
        preparedStatement.setString(1, username);
        preparedStatement.setString(2, password);
        //获取结果集
        resultSet = preparedStatement.executeQuery();
    } catch (Exception exception) {
        System.out.println(exception.getMessage());
    } finally {
        //释放资源
        DBUtils.close(connection, preparedStatement, resultSet);
    }
    /*
        处理结果集
        结果集中最多只有一条数据
         */
    if (resultSet != null) {
        /*
            获取session对象
            用户发送第一次请求,服务器创建session对象并生成对应Cookie
            服务器将Cookie响应至浏览器
            用户发送第二次请求,服务器根据浏览器缓存中的Cookie在session列表中寻找对应session对象
             */
        HttpSession session = request.getSession();
        //session会话域中绑定数据
        session.setAttribute("username", username);

        //用户选择十天内免登录
        if ("1".equals(flag)) {
            //创建Cookie对象存储用户名、密码
            Cookie cookie01 = new Cookie("username", username);
            Cookie cookie02 = new Cookie("password", password);
            //设置Cookie对象有效期
            cookie01.setMaxAge(60 * 60 * 24 * 10);
            cookie02.setMaxAge(60 * 60 * 24 * 10);
            /*
                设置Cookie对象的path
                浏览器端只要发送crud项目的请求路径以及此路径的子路径则必须携带Cookie对象至服务器端
                 */
            cookie01.setPath(request.getContextPath());
            cookie02.setPath(request.getContextPath());
            /*
                服务器端将Cookie对象响应至浏览器端
                浏览器端接收Cookie对象后将Cookie对象存储至缓存
                 */
            response.addCookie(cookie01);
            response.addCookie(cookie02);
        }
        response.sendRedirect(request.getContextPath() + "/list");
    } else {
        response.sendRedirect(request.getContextPath() + "/index.jsp");
    }
}
session和Cookie区别
1、Cookie工作原理

(1)浏览器端用户发送第一次请求到服务器端
(2)服务器端创建Cookie(该Cookie中包含用户信息),然后将该Cookie发送至浏览器端
(3)浏览器端用户发送第二次请求到服务器端时携带服务器端创建的Cookie
(4)服务器端根据Cookie中包含的用户信息区分不同的用户
2、session工作原理

(1)浏览器端用户发送第一次请求到服务器端,服务器端创建session对象并生成session对象对应的sessionId(特殊的Cookie—name为固定值JSESSIONID,value为session对象的ID),然后将sessionId发送至浏览器端
(2)浏览器端用户发送第N次请求到服务器端,浏览器端自动将sessionId响应至服务器端,服务器端根据sessionId在session列表中寻找对应session对象从而区分不同用户
3、Cookie和session区别

(1)session数据保存在服务器端,Cookie数据保存在浏览器客户端
(2)Cookie不是很安全,session安全
(3)session数据保存在服务器端,当访问较多时会占用服务器性能,使用Cookie可减轻服务器性能
EL表达式
1、EL表达式基本介绍

(1)Expression Language(表达式语言)
(2)EL表达式可以代替JSP文件中的java代码,使JSP文件更加整洁美观
(3)JSP文件中夹杂java代码,例如<% java代码 %>、<%= %>等,导致JSP文件难以维护
(4)EL表达式可以算作JSP语法的一部分,EL表达式归属于JSP
2、EL表达式作用

(1)从某个作用域中取出数据,将其转换为字符串,再将其输出到浏览器
(2)EL表达式三大功效:
	从某个域中取出数据
	将数据转换为字符串
	将字符串输出到浏览器
3、EL表达式基本语法格式

(1)${表达式}
4、EL表达式基本案例演示

<%@ page contentType="text/html" pageEncoding="UTF-8" %>

<%-- 向request请求域中绑定数据 --%>
<%
    request.setAttribute("username","jxs");
%>

<%-- 使用java代码将request请求域中的数据取出 将数据输出到浏览器 --%>
<%
    String str = (String)request.getAttribute("username");
    out.print(str);
%>

<%-- 使用EL表达式将request请求域中的数据取出 将数据输出到浏览器 --%>
${username}
EL表达式的使用
EL表达式原理剖析
JSTL标签库
JSTL标签的使用
JSTL标签的原理剖析
Filter过滤器
过滤器的作用分析
过滤器的实现
责任链设计模式
过滤器在实际开发中的应用
Listener监听器
监听器的作用分析
监听器的实现
监听器有哪些
监听器设计模式
监听器在实际开发中的应用
AJAX（Asynchronous JavaScript And Xml）
传统请求及缺点
1、传统请求

(1)浏览器地址栏输入URL
(2)点击超链接
(3)提交form表单
(4)使用JS代码发送请求
window.open
document.location.href=url
window.location.href=url
2、传统请求缺点图解

![](E:\Study\自学课程资料\Java\assets\传统请求缺点图解.png)

3、传统请求缺点

(1)传统的请求响应方式,用户通过表单向服务器提交用户信息,服务器端处理接收到的信息,并把处理结果返回给用户,在这个过程中需要刷新整个页面才能得到服务器返回的结果。
AJAX概述
1、AJAX异步请求图解

![](E:\Study\自学课程资料\Java\assets\AJAX异步请求.png)

2、浏览器端发送AJAX请求至服务器，服务器响应3种数据：普通文本、XML字符串、JSON字符串。AJAX解析响应的数据，并将响应的数据渲染到div图层中，即完成页面局部刷新

3、AJAX（Asynchronous Javascript And Xml），即异步的JavaScript和Xml，浏览器需编写JS语法的代码发送AJAX请求至服务器，服务器响应XML字符串至浏览器

XMLHttpRequest对象
1、XMLHttpRequest对象为AJAX的核心对象，发送请求以及接收服务器返回的数据

2、浏览器中都内置了XMLHttpRequest对象

3、创建XMLHttpRequest对象

var xmlHttpRequest = new XMLHttpRequest()
4、XMLHttpRequest对象方法

方法	描述
open(method,url,async,user,pwd)	method：规定请求类型，async：true（异步）或false（同步）
send()	发送请求至服务器（GET请求）
send(String)	发送请求至服务器（POST请求）
setRequestHeader	向要发送的报头添加标签/键值对
abort()	取消当前请求
getAllResponseHeader()	返回头部信息
getResponseHeader()	返回特定头部信息
5、XMLHttpRequest对象属性

属性	描述
onreadystatechange	定义当readyState属性发送变化时被调用的函数
readyState	保存XMLHttpRequest状态。0：请求未初始化、1：服务器连接已建立、2：服务器已收到请求、3：服务器正在处理请求、4：服务器完成请求处理并且响应已就绪
responseText	以字符串返回响应数据
responseXML	以XML数据返回响应数据
status	返回请求状态号
statusText	返回状态文本
6、第一个AJAX请求详解

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>ajax GET请求</title>
</head>
<body>

<script type="text/javascript">
    window.onload = function () {
        //鼠标单击事件
        document.getElementById("button01").onclick = function () {
            /*
            发送ajax GET请求
            第一步:创建AJAX核心对象XMLHttpRequest
            第二步:注册回调函数
            第三步:开启通道建立连接
            第四步:发送ajax请求
            */
            var xmlHttpRequest = new XMLHttpRequest();
            //回调函数,当readyState状态值改变时被调用
            xmlHttpRequest.onreadystatechange = function () {
                console.log(xmlHttpRequest.readyState)
                //当readyState的值为4时表示服务器完成请求处理并且响应已就绪
                if (xmlHttpRequest.readyState == 4) {
                    console.log("响应结束")
                    /*
                    响应结束后会有HTTP状态码
                    常见的HTTP状态码:
                    成功:200
                    资源无法找到:404
                    服务器内部错误:500
                    */
                    if (xmlHttpRequest.status == 404) {
                        window.alert("请求资源不存在")
                    } else if (xmlHttpRequest.status == 500) {
                        window.alert("服务器内部错误")
                    } else if (xmlHttpRequest.status == 200) {
                        window.alert("响应成功")
                        //通过XMLHttpRequest对象的responseText属性获取响应信息
                        window.alert(xmlHttpRequest.responseText)
                        //将响应信息放至div图层中
                        document.getElementById("div01").innerHTML = xmlHttpRequest.responseText
                    }
                }
            }
            /*
            open(method,url,async,username,password)
            1.method:get请求或post请求
            2.url:请求地址
            3.async:true(异步)或false(同步)
            4.username:用户名  password:密码
            5.若想访问服务器上的资源,则需使用用户名和密码认证
            */
            xmlHttpRequest.open("GET", "/ajax02/ajaxRequest", true)
            xmlHttpRequest.send()
        }
    }
</script>

<!-- 定义按钮,用户点击按钮发送ajax请求 -->
<input type="button" value="点击我" id="button01">

<!-- div图层,浏览器发送ajax请求至服务器,服务器响应数据至此 -->
<div id="div01"></div>
</body>
</html>
@WebServlet("/ajaxRequest")
public class AjaxRequest extends HttpServlet {

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        PrintWriter out = response.getWriter();
        //XMLHttpRequest对象接收响应信息
        out.print("welcome to study ajax");
    }
}
AJAX GET请求
1、GET请求在“请求行”上提交数据，格式：url?name=value&name=value...

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>AJAX GET请求</title>
</head>
<body>
<script type="text/javascript">
    window.onload = function () {
        document.getElementById("submit01").onclick = function () {
            //创建AJAX核心对象XMLHttpRequest
            var xmlHttpRequest = new XMLHttpRequest();
            //注册回调函数
            xmlHttpRequest.onreadystatechange = function () {
                //readyState用于保存XMLHttpRequest对象状态
                if (xmlHttpRequest.readyState == 4) {
                    //status用于保存状态码
                    if (xmlHttpRequest.status == 200) {
                        /*
                        responseText获取服务器响应内容
                        以普通文本的形式获取响应内容
                        innerHTML设置元素内部的HTML代码,将后面的内容当作HTML代码解释执行
                        innerText将后面的内容当作普通文本解释执行
                        */
                        document.getElementById("app01").innerHTML
                            = xmlHttpRequest.responseText
                    }
                }
            }
            var username = document.getElementById("text01").value;
            var age = document.getElementById("text02").value;
            //开启通道
            xmlHttpRequest.open("get", "/ajax02/ajaxRequest02?username=" + username + "&age=" + age, true)
            //发送AJAX请求
            xmlHttpRequest.send()
        }
    }
</script>

用户名<input id="text01" type="text" name="username"><br>
年龄<input id="text02" type="text" name="age"><br>
<input type="submit" value="点击我" id="submit01">

<div id="app01"></div>
</body>
</html>
@WebServlet("/ajaxRequest02")
public class AJAXRequest02 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        //获取前端提交的数据
        String username = request.getParameter("username");
        String age = request.getParameter("age");
        //设置响应类型
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        out.print(username + "," + age);
    }
}
AJAX POST请求
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>AJAX POST请求</title>
</head>
<body>

<script type="text/javascript">
    window.onload = function () {
        document.getElementById("button01").onclick = function () {
            var xmlHttpRequest = new XMLHttpRequest();
            xmlHttpRequest.onreadystatechange = function () {
                if (xmlHttpRequest.readyState == 4) {
                    if (xmlHttpRequest.status == 200) {
                        document.getElementById("div01").innerHTML = xmlHttpRequest.responseText
                    }
                }
            }
            xmlHttpRequest.open("POST", "/ajax02/ajaxRequest03", true)

            //设置请求头的内容类型模拟AJAX提交form表单数据
            xmlHttpRequest.setRequestHeader("Content-Type", "application/x-www-form-urlencoded")
            //send()函数中传入实参,会自动在请求体中提交数据
            var username = document.getElementById("username").value;
            var password = document.getElementById("password").value;
            xmlHttpRequest.send("username=" + username + "&password=" + password)
        }
    }
</script>

用户名:<input type="text" id="username"><br>
密码:<input type="password" id="password"><br>

<button id="button01">发送AJAX POST请求</button>

<div id="div01"></div>
</body>
</html>
@WebServlet("/ajaxRequest03")
public class AJAXRequest03 extends HttpServlet {
    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        String username = request.getParameter("username");
        String password = request.getParameter("password");

        response.setContentType("text/html");
        PrintWriter out = response.getWriter();

        out.print(username + password);
    }
}
基于JSON的数据交换
1、Web前端中如何将json格式的字符串转换为json对象

var jsonStr = "{\"username\" : \"jxs\",\"age\" : 21}"
var jsonObj = JSON.parse(jsonStr)
console.log(jsonObj.username + jsonObj.age)
2、案例演示

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Title</title>
</head>
<body>

<script type="text/javascript">
    window.onload = function () {
        document.getElementById("button01").onclick = function () {
            var xmlHttpRequest = new XMLHttpRequest();
            xmlHttpRequest.onreadystatechange = function () {
                if (xmlHttpRequest.readyState == 4) {
                    if (xmlHttpRequest.status == 200) {
                        //将JSON格式的字符串转换为JSON对象
                        var jsonObjList = JSON.parse(xmlHttpRequest.responseText);
                        var html = "";
                        for (var i = 0; i < jsonObjList.length; i++) {
                            var student = jsonObjList[i];
                            html += "<tr>         "
                            html += "    <td>" + student.id + "</td>"
                            html += "    <td>" + student.name + "</td>"
                            html += "    <td>" + student.age + "</td>"
                            html += "    <td>" + student.address + "</td>"
                            html += "</tr>        "
                        }
                        document.getElementById("tbody01").innerHTML = html
                    }
                }
            }
            xmlHttpRequest.open("GET", "/ajax02/ajaxRequest04", true)
            xmlHttpRequest.send()
        }
    }
</script>

<input type="button" value="显示学员列表" id="button01">

<table>
    <thead>
    <tr>
        <td>序号</td>
        <td>姓名</td>
        <td>年龄</td>
        <td>住址</td>
    </tr>
    </thead>
    <tbody id="tbody01">
    </tbody>
</table>
</body>
</html>
@WebServlet("/ajaxRequest04")
public class AJAXRequest04 extends HttpServlet {
    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
            throws ServletException, IOException {
        response.setContentType("text/html");
        PrintWriter out = response.getWriter();
        String jsonStr = "[" +
                "{\"id\":1,\"name\":\"jxs\",\"age\":22,\"address\":\"南京市\"}," +
                "{\"id\":2,\"name\":\"dwy\",\"age\":22,\"address\":\"南京市\"}" +
                "]";
        out.print(jsonStr);
    }
}
3、fastjson


基于XML的数据交换
AJAX乱码问题
AJAX的异步同步
AJAX代码封装
AJAX实现省市联动
AJAX跨域问题
AJAX实现搜索联想 自动补全
Maven
Java框架
MyBatis
MyBatis简介
何为MyBatis
1、基本介绍

MyBatis本是Apache的一个开源项目iBatis
2010年6月这个项目由Apache Software Foundation迁移到Google Code
随着开发团队转投Google Code旗下,iBatis3.x正式更名为MyBatis
代码于2013年11月迁移到Github

iBatis来源于"internet"和"abatis"的组合,是一个基于Java的持久层框架。iBatis提供的持久层框架包括SQL Maps和Data Access Object(DAO 数据传输对象)
2、MyBatis特性

MyBatis 是一款优秀的持久层框架
它支持自定义 SQL、存储过程以及高级映射。
MyBatis 免除了几乎所有的 JDBC 代码以及设置参数和获取结果集的工作。
MyBatis 可以通过简单的 XML 或注解来配置和映射原始类型、接口和 Java POJO（Plain Old Java Objects，普通老式 Java 对象）为数据库中的记录。
3、MyBatis下载

Maven仓库

<dependency>
  <groupId>org.mybatis</groupId>
  <artifactId>mybatis</artifactId>
  <version>x.x.x</version>
</dependency>
Github:MyBatis下载地址:https://github.com/mybatis/
中文文档:https://mybatis.org/mybatis-3/zh/index.html
何为持久层
1、数据持久化

将程序的数据在持久状态和瞬时状态转化的过程

例:
数据库 数据持久化
IO流 文件持久化
生活中 冷藏、罐头 食物持久化
2、持久层?

(1)完成持久化工作的代码块
(2)层界限明显
3、为何需要MyBatis?

(1)帮助程序员将数据存入到数据库中以及从数据库中取出数据
(2)传统的JDBC操作,创建Driver类的对象实例、利用Driver类的对象实例获取连接、执行SQL指令、数据取出时进行封装,通过MyBatis可减少重复代码,提高开发效率
(3)MyBatis是一个半自动化的ORM框架 (Object Relationship Mapping) —> 对象关系映射
(4)所有的事情,不用Mybatis依旧可以做到,只是用了它,所有实现会更加简单！技术没有高低之分,只有使用这个技术的人有高低之别
MyBatis优点
(1)简单易学
(2)灵活
(3)sql和代码的分离，提高了可维护性。
(4)提供映射标签，支持对象与数据库的ORM字段关系映射。
(5)提供对象关系映射标签，支持对象关系组建维护。
(6)提供xml标签，支持编写动态sql
MyBatis和其它持久化层技术对比
1、JDBC  

(1)SQL夹杂在Java代码中耦合度高,导致硬编码内伤  
(2)维护不易且实际开发需求中SQL有变化,频繁修改的情况多见  
(3)代码冗长,开发效率低
2、Hibernate 和 JPA

(1)操作简便,开发效率高  
(2)程序中的长难复杂SQL需要绕过框架  
(3)内部自动生产的SQL,不容易做特殊优化  
(4)基于全映射的全自动框架,大量字段的POJO进行部分映射时比较困难。  
(5)反射操作太多,导致数据库性能下降
搭建MyBatis
搭建环境
1、思路

搭建环境 --> 导入依赖 --> 编写代码 --> 测试
2、搭建数据库

(1)创建数据库
CREATE DATABASE mybastis;

(2)创建表
CREATE TABLE `user`(
id INT PRIMARY KEY NOT NULL,
# 设置不为空,默认为''
name VARCHAR(32) NOT NULL DEFAULT '',
PASSWORD VARCHAR(32) NOT NULL DEFAULT '');

(3)插入数据
INSERT INTO `user` VALUES (1,'jxs','123'),(2,'dwy','123');
3、新建Maven项目，删除src目录，作为父工程统一管理依赖

4、pom.xml中导入依赖

<!--mysql驱动-->
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.30</version>
</dependency>

<!--mybatis-->
<dependency>
    <groupId>org.mybatis</groupId>
    <artifactId>mybatis</artifactId>
    <version>3.5.11</version>
</dependency>

<!--junit-->
<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.11</version>
    <scope>test</scope>
</dependency>
创建子模块
1、在父工程中新建module（子模块）

2、编写mybatis核心配置文件

<!--configuration核心配置文件-->
<configuration>
    <!--环境-->
    <environments default="development">
        <environment id="development">
            <!--事务管理-->
            <transactionManager type="JDBC"/>
            <!--数据源-->
            <dataSource type="POOLED">
                <!--属性-->
                <!--Driver驱动类
                统一资源定位符
                用户名
                密码-->
                <property name="driver" value="com.mysql.cj.jdbc.Driver"/>
                <!--serverTimezone=UTC 设置时区
                useSSL=true 进行安全验证
                useUnicode=true&amp;characterEncoding=UTF-8" 指定字符的编码、解码格式
                &amp 相当于 and-->
                <property name="url" value="jdbc:mysql://localhost:3306/mybatis?
                serverTimezone=UTC&amp;
                useSSL=true&amp;
                useUnicode=true&amp;
                characterEncoding=UTF-8"/>
                <property name="username" value="root"/>
                <property name="password" value="123456"/>
            </dataSource>
        </environment>
    </environments>

    <mappers>
        <!--每一个Mapper.xml文件都需在Mybatis核心配置文件中注册-->
        <mapper resource="com/jxs/dao/UserMapper.xml"/>
    </mappers>

</configuration>
3、编写myBatis工具类

/**
 * MyBatisUtils工具类
 */
public class MyBatisUtils {
    private static SqlSessionFactory sqlSessionFactory;

    static {
        try {
            //使用MyBatis第一步:获取sqlSessionFactory(SQL会话工厂)对象实例
            String resource = "mybatis-config.xml";
            InputStream inputStream = Resources.getResourceAsStream(resource);
            sqlSessionFactory = new SqlSessionFactoryBuilder().build(inputStream);
        } catch (IOException e) {
            e.printStackTrace();
        }
    }

    /*
    从 SqlSessionFactory 中获取 SqlSession
    可通过 SqlSession 对象实例来直接执行已映射的 SQL 语句 */
    public static SqlSession getSqlSession() {
        return sqlSessionFactory.openSession();
    }
}
编写代码
1、编写pojo实体类

public class User {
    private int id;
    private String name;
    private String password;

    public User() {
    }

    public User(int id, String name, String password) {
        this.id = id;
        this.name = name;
        this.password = password;
    }

    public int getId() {
        return id;
    }
    public void setId(int id) {
        this.id = id;
    }
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public String getPassword() {
        return password;
    }
    public void setPassword(String password) {
        this.password = password;
    }

    @Override
    public String toString() {
        return "User{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", password='" + password + '\'' +
                '}';
    }
}
2、Dao接口

public interface UserDao {
    List<User> getUserList();
}
3、接口实现类，由原来的UserDaoImplement实现类转变为Mapper配置文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Mapper 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<!--namespace标签:绑定一个对应的Dao/Mapper接口,就好比一个类实现了UserDao接口-->
<mapper namespace="com.jxs.dao.UserDao">
    <!--select查询语句
    id标签:UserDao接口的方法名,就好比一个类实现了UserDao接口并实现getUserList()方法
    resultType标签:返回结果类型,返回集合泛型的数据类型！
    -->
    <select id="getUserList" resultType="com.jxs.pojo.User">
        <!--执行SQL语句-->
        select * from mybatis.user;
    </select>
</mapper>
测试
1、junit测试

public class UserDaoTest {

    @Test
    public void test() {
        //获取sqlSession对象实例
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        //执行SQL
        UserDao mapper = sqlSession.getMapper(UserDao.class);
        List<User> userList = mapper.getUserList();
        for (User user : userList) {
            System.out.println(user);
        }
        sqlSession.close();
    }
}
注意事项
（1）每个Mapper.xml文件都需在核心配置文件中注册

<mappers>
    <!--每一个Mapper.xml文件都需在Mybatis核心配置文件中注册-->
    <mapper resource="com/jxs/dao/UserMapper.xml"/>
</mappers>
（2）资源过滤问题

父工程pom.xml中添加

<!--build中配置resources,防止资源导出失败问题-->
<build>
    <resources>

        <resource>
            <directory>src/main/resources</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>true</filtering>
        </resource>

        <resource>
            <directory>src/main/java</directory>
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>
            <filtering>true</filtering>
        </resource>

    </resources>
</build>
3、url中设置时区

serverTimezone=UTC 设置时区
总结（重要！！！！）
(1)创建数据库、表
(2)创建Maven工程,删除src目录,作为父工程统一管理依赖
(3)导入数据库驱动、mybatis、junit依赖
(4)父工程中新建子模块
(5)src/main/resources资源文件目录下新建mybatis-config.xml核心配置文件,包含从连接池获取数据库连接实例的数据源(dataSource)和决定事务作用域和控制方式的事务管理器
(6)编写MyBatisUtils工具类
Resources.getResourceAsStream("核心配置文件名"),将配置文件转换为字节输入流
new SqlSessionFactoryBuilder().builder(字节输入流),创建sqlSessionFactory(Sql会话工厂对象实例)
sqlSessionFactory.openSession(),获取sqlSession对象实例(就好比preparedstatement),sqlSession提供了数据库执行SQL命令所需的所有方法！
(7)编写数据库的表对应的pojo实体类
(8)定义Dao接口
(9)编写Mapper.xml文件,namespace标签绑定接口(就好比一个类实现了Dao接口),id标签绑定Dao接口的方法名(就好比一个类实现了Dao接口并实现Dao接口的方法)
标签解析
1、namespace:绑定对应的Mapper接口,且namespace中的包名和Mapper接口的包名一致
2、select:执行查询语句
3、id:namespace中绑定的接口的方法名
4、resultType:返回值类型
5、parameterType:参数类型
CRUD（看总结！！！！）
1、编写Mapper接口

public interface UserMapper {
    //查询全部用户
    List<User> getUserList();

    //根据ID查询用户
    User getUserById(int id);

    //插入用户数据
    int insertUser(User user);

    //修改用户数据
    int updateUser(User user);

    //删除用户数据
    int deleteUser(int id);
}
2、编写Mapper文件

<!--namespace标签:绑定一个对应的Dao/Mapper接口,就好比一个类实现了UserDao接口-->
<mapper namespace="com.jxs.dao.UserMapper">
    <!--select查询语句
    id标签:UserDao接口的方法名,就好比一个类实现了UserDao接口并实现getUserList()方法
    resultType标签:返回结果类型,返回集合泛型的数据类型！
    -->
    <select id="getUserList" resultType="com.jxs.pojo.User">
        <!--执行SQL语句-->
        select * from mybatis.user;
    </select>

    <select id="getUserById" resultType="com.jxs.pojo.User" parameterType="int">
        <!--#{}表示一个占位符号,相当于jdbc中的?符号
        #{}方式能够很大程度防止sql注入(安全),${}方式无法防止Sql注入-->
        select * from mybatis.user where id = #{id};
    </select>

    <insert id="insertUser" parameterType="com.jxs.pojo.User">
        <!--#{}占位符 #{id},#{name},#{password}分别对应传入的user对象的属性-->
        insert into mybatis.user values (#{id},#{name},#{password});
    </insert>

    <update id="updateUser" parameterType="com.jxs.pojo.User">
        update mybatis.user set name = #{name},password = #{password} where id = #{id};
    </update>

    <delete id="deleteUser" parameterType="int">
        delete from mybatis.user where id = #{id};
    </delete>
</mapper>
3、测试

public class UserDaoTest {

    @Test
    public void test1() {
        //获取sqlSession对象实例
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        //执行SQL
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        List<User> userList = mapper.getUserList();
        for (User user : userList) {
            System.out.println(user);
        }
        sqlSession.close();
    }

    @Test
    public void test2() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        //相当于UserMapper mapper = new UserMapperImplement();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User userById = mapper.getUserById(1);
        System.out.println(userById);
    }

    @Test
    public void test3() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User lzz = new User(3, "lzz", "123");
        int i = mapper.insertUser(lzz);
        //提交事务
        sqlSession.commit();
        sqlSession.close();
    }

    @Test
    public void test4() {
        //工厂中获取sqlSession对象实例
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        //相当于UserMapper mapper = new UserMapperImplement();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User user = new User(1,"蒋兴树","123");
        int i = mapper.updateUser(user);
        sqlSession.commit();
        System.out.println(i);
    }

    @Test
    public void test5() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        int i = mapper.deleteUser(1);
        sqlSession.commit();
        System.out.println(i);
    }
}
4、总结

(1)Mapper接口中编写增删改查对应的抽象方法
(2)编写Mapper文件,namespace标签绑定对应的Mapper接口,id标签绑定Mapper接口的方法名,编写SQL语句
(3)测试,通过MyBatis工具类获取SqlSession对象实例,sqlSession.getMapper(UserMapper.class)获取Mapper接口对应的Mapper文件,映射器通过命名空间和方法名找到对应的SQL语句(增删改须提交事务)
万能Map
1、编写Mapper接口

//万能Map之插入用户数据
int insertUserMethod(Map<String,Object> map);

//万能Map之根据ID查询用户
User getUserByIdMethod(Map<String,Object> map);

//万能Map之修改用户信息
int updateUserMethod(Map<String,Object> map);

//万能Map之删除用户信息
int deleteUserMethod(Map<String,Object> map);
2、编写Mapper文件

<insert id="insertUserMethod" parameterType="map">
    insert into mybatis.user (id,name,password) values (#{userid},#{username},#{password});
</insert>

<select id="getUserByIdMethod" resultType="com.jxs.pojo.User" parameterType="map">
    select * from mybatis.user where id = #{userid};
</select>

<update id="updateUserMethod" parameterType="map">
    update mybatis.user set name = #{username} where id = #{userid};
</update>

<delete id="deleteUserMethod" parameterType="map">
    delete from mybatis.user where id = #{userid};
</delete>
3、测试

@Test
public void test6() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    Map<String, Object> map = new HashMap<>();
    map.put("userid", 4);
    map.put("username", "zls");
    map.put("password", "123");
    int i = mapper.insertUserMethod(map);
    sqlSession.commit();
}

@Test
public void test7() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    Map<String, Object> map = new HashMap<>();
    map.put("userid",2);
    User user = mapper.getUserByIdMethod(map);
    System.out.println(user);
}

@Test
public void test8() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    Map<String,Object> map = new HashMap<>();
    map.put("userid",2);
    map.put("username","丁维一");
    int i = mapper.updateUserMethod(map);
    sqlSession.commit();
}

@Test
public void test9() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    Map<String,Object> map = new HashMap<>();
    map.put("userid",2);
    int i = mapper.deleteUserMethod(map);
    sqlSession.commit();
}
4、总结

(1)Map集合传递参数,直接在sql中取出key即可
(2)对象传递参数,直接在sql中取出对象的属性即可
(3)只有一个基本数据类型时,可直接在sql中取到
模糊查询
1、编写Mapper接口

//模糊查询
List<User> selectLike(String name);
2、编写Mapper文件

<select id="selectLike" resultType="com.jxs.pojo.User" parameterType="String">
    select * from mybatis.user where name like #{value};
</select>
3、测试

@Test
public void test10() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    List<User> users = mapper.selectLike("%l%");
    for (User user : users) {
        System.out.println(user);
    }
}
配置解析
核心配置文件
mybatis-config.xml包含了会深深影响 MyBatis 行为的设置和属性信息。 配置文档的顶层结构如下：

configuration（配置）
	properties（属性）
	settings（设置）
	typeAliases（类型别名）
	typeHandlers（类型处理器）
	objectFactory（对象工厂）
	plugins（插件）
	environments（环境配置）
		environment（环境变量）
			transactionManager（事务管理器）
			dataSource（数据源）
	databaseIdProvider（数据库厂商标识）
	mappers（映射器）
environments（环境配置）
1、MyBatis 可以配置成适应多种环境，尽管可以配置多个环境，但每个 SqlSessionFactory 实例只能选择一种环境。每个数据库对应一个 SqlSessionFactory 实例。

2、environments 元素定义了如何配置环境

<!--可修改默认环境-->
<environments default="development">
    
  <environment id="development">
      
    <!--事务管理器-->
    <transactionManager type="JDBC">
      <property name="..." value="..."/>
    </transactionManager>
    
    <!--数据源-->
    <dataSource type="POOLED">
      <property name="driver" value="${driver}"/>
      <property name="url" value="${url}"/>
      <property name="username" value="${username}"/>
      <property name="password" value="${password}"/>
    </dataSource>
      
  </environment>
    
</environments>
transactionManager
1、MyBatis中有两种类型的事务管理器，即JDBC、MANAGED

2、JDBC

(1)JDBC 配置使用了 JDBC 的提交和回滚功能,它依赖从数据源获得的连接来管理事务作用域。
(2)关闭连接时启用自动提交事务。
(3)"skipSetAutoCommitOnClose" 属性设置为 "true" 来跳过这个步骤
<transactionManager type="JDBC">
  <property name="skipSetAutoCommitOnClose" value="true"/>
</transactionManager>
3、MANAGED

(1)MANAGED配置几乎没有做什么
(2)它从不提交或回滚一个连接,而是让容器来管理事务的整个生命周期
(3)默认情况下它会关闭连接,将 closeConnection 属性设置为 false 来阻止默认的关闭行为
<transactionManager type="MANAGED">
  <property name="closeConnection" value="false"/>
</transactionManager>
dataSource
1、三种内建的数据源类型 UNPOOLED、POOLED、JNDI

2、UNPOOLED

(1)UNPOOLED数据源的实现会每次请求时打开和关闭连接。
(2)适合场景:对某些数据库来说,使用连接池并不重要
driver:这是 JDBC 驱动类的全类名
url:这是数据库的 JDBC URL 地址
username:登录数据库的用户名
password:登录数据库的密码
defaultTransactionIsolationLevel:默认的连接事务隔离级别。
defaultNetworkTimeout:等待数据库操作完成的默认网络超时时间（单位：毫秒）
3、POOLED

POOLED数据源的实现利用"池"的概念将 JDBC 连接对象组织起来,避免了创建新的连接实例时所必需的初始化和认证时间。 
4、JNDI

这个数据源实现是为了能在如 EJB 或应用服务器这类容器中使用,容器可以集中或在外部配置数据源,然后放置一个 JNDI 上下文的数据源引用。
properties（属性）
1、xml中，所有的标签都可以规定顺序

The content of element type "configuration" must match "(properties?,settings?,typeAliases?,typeHandlers?,objectFactory?,objectWrapperFactory?,reflectorFactory?,plugins?,environments?,databaseIdProvider?,mappers?)".

元素类型"configuration"的内容必须匹配(属性,设置,类型别名,类型处理程序,对象工厂,对象包装器工厂,反射器工厂,插件,环境,databaseIdProvider,映射器)
2、通过properties属性来实现引用配置文件，这些属性可以在外部进行配置，并可以进行动态替换。你既可以在典型的 Java 属性文件中配置这些属性，也可以在 properties 元素的子元素中设置。

3、编写一个配置文件 db.properties

driver=com.mysql.cj.jdbc.Driver
jdbc.url=jdbc:mysql://localhost:3306/mybatis?serverTimezone=UTC&useSSL=true&useUnicode=true&characterEncoding=UTF-8
4、修改核心配置文件

<!--configuration核心配置文件-->
<configuration>
    <!--引入外部配置文件-->
    <properties resource="db.properties">
        <!--在 properties 元素的子元素中设置属性-->
        <property name="username" value="root"/>
        <property name="password" value="123456"/>
    </properties>

    <!--环境-->
    <environments default="test">
        <environment id="test">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="${driver}"/>
                <property name="url" value="${jdbc.url}"/>
                <property name="username" value="${username}"/>
                <property name="password" value="${password}"/>
            </dataSource>
        </environment>
    </environments>

    <mappers>
        <!--每一个Mapper.xml文件都需在Mybatis核心配置文件中注册-->
        <mapper resource="com/jxs/dao/UserMapper.xml"/>
    </mappers>

</configuration>
5、总结

(1)可直接引入外部配置文件
(2)可在 properties 元素的子元素中设置属性
(3)若 外部配置文件 和 properties元素的子元素 有同一字段,优先使用外部配置文件字段。 
typeAliases（类型别名）
1、方式一：类型别名可为 Java 类型设置一个缩写名字。 它仅用于 XML 配置，意在降低冗余的全限定类名书写

<typeAliases>
    <typeAlias type="com.jxs.pojo.User" alias="User"/>
</typeAliases>
<!--User:别名-->
<select id="getUserList" resultType="User">
    <!--执行SQL语句-->
    select * from mybatis.user;
</select>
2、Configuration核心配置文件中的标签规定顺序：properties settings typeAliases

3、方式二：可以指定一个包名，MyBatis 会在包名下面搜索需要的 Java Bean，每一个在包中的 Java Bean，在没有注解的情况下，会使用 Bean 的首字母小写的非限定类名来作为它的别名。

<typeAliases>
    <package name="com.jxs.pojo"/>
</typeAliases>
<!--user/User:别名-->
<select id="getUserList" resultType="User">
    <!--执行SQL语句-->
    select * from mybatis.user;
</select>
4、常见的 Java 类型内建的类型别名。它们都是不区分大小写的，注意，为了应对原始类型的命名重复，采取了特殊的命名风格。

别名	映射的类型
_byte	byte
_char (since 3.5.10)	char
_character (since 3.5.10)	char
_long	long
_short	short
_int	int
_integer	int
_double	double
_float	float
_boolean	boolean
string	String
byte	Byte
char (since 3.5.10)	Character
character (since 3.5.10)	Character
long	Long
short	Short
int	Integer
integer	Integer
double	Double
float	Float
boolean	Boolean
date	Date
decimal	BigDecimal
bigdecimal	BigDecimal
biginteger	BigInteger
object	Object
date[]	Date[]
decimal[]	BigDecimal[]
bigdecimal[]	BigDecimal[]
biginteger[]	BigInteger[]
object[]	Object[]
map	Map
hashmap	HashMap
list	List
arraylist	ArrayList
collection	Collection
iterator	Iterator
5、总结

(1)实体类少时使用第一种方式;实体类多时使用第二种方式
(2)第一种方式可以自定义别名;第二种方式不可自定义别名;若有注解,则别名为其注解值
//自定义pojo实体类User别名为hello
@Alias("hello")
public class User {
    ...
}
settings（设置 重点！！）
1、这是 MyBatis 中极为重要的调整设置，它们会改变 MyBatis 的运行时行为。 

2、各项设置的含义、默认值等。

设置名	描述	有效值	默认值
cacheEnabled	全局性地开启或关闭所有映射器配置文件中已配置的任何缓存。	true | false	true
lazyLoadingEnabled	延迟加载的全局开关。当开启时，所有关联对象都会延迟加载。 特定关联关系中可通过设置 fetchType 属性来覆盖该项的开关状态。	true | false	false
useGeneratedKeys	允许 JDBC 支持自动生成主键，需要数据库驱动支持。如果设置为 true，将强制使用自动生成主键。尽管一些数据库驱动不支持此特性，但仍可正常工作（如 Derby）。	true | false	false
mapUnderscoreToCamelCase	是否开启驼峰命名自动映射，即从经典数据库列名 A_COLUMN 映射到经典 Java 属性名 aColumn。	true | false	False
logImpl	指定 MyBatis 所用日志的具体实现，未指定时将自动查找。	SLF4J | LOG4J（3.5.9 起废弃） | LOG4J2 | JDK_LOGGING | COMMONS_LOGGING | STDOUT_LOGGING | NO_LOGGING	未设置
mappers（映射器）
1、Mapper文件中定义SQL语句，并告诉 MyBatis 到哪里去找到这些语句。 

2、在自动查找资源方面，Java 并没有提供一个很好的解决方案，所以最好的办法是直接告诉 MyBatis 到哪里去找映射文件。 

3、可以使用相对于类路径的资源引用，完全限定资源定位符、类名、包名等。

4、方式一：

<!-- 使用相对于类路径的资源引用 -->
<mappers>
    <mapper resource="com/jxs/dao/UserMapper.xml"/>
</mappers>
5、方式二：

<!-- 使用映射器接口实现类的完全限定类名 -->
<mappers>
    <mapper class="com.jxs.dao.UserMapper"/>
</mappers>
方式二注意点:
(1)Mapper接口和Mapper文件必须同名
(2)Mapper接口和Mapper文件必须同包
6、方式三：

<!-- 将包内的映射器接口全部注册为映射器 -->
<mappers>
    <package name="com.jxs.dao"/>
</mappers>
方式三注意点:
(1)Mapper接口和Mapper文件必须同名
(2)Mapper接口和Mapper文件必须同包
总结（精辟！！）
(1)核心配置文件:从连接池中获取数据库的连接
(2)MyBatis工具类:获取SqlSessionFactory对象实例(每个数据库对应一个SqlSessionFactory对象实例),再创建可执行SQL语句的SqlSession对象实例
(3)定义pojo实体类,实体类的每个对象实例对应数据库表中每一行记录
(4)定义Mapper接口,定义Mapper文件,Mapper文件中自定义SQL语句
(5)核心配置文件中定义映射器,传入Mapper文件的全类名
作用域和生命周期
1、不同作用域和生命周期类别是至关重要的，因为错误的使用会导致非常严重的并发问题。

2、SqlSessionFactoryBuilder

(1)SqlSessionFactoryBuilder类可以被实例化、使用、丢弃，一旦创建了 SqlSessionFactory，就不再需要它了
(2) SqlSessionFactoryBuilder 实例的最佳作用域是方法作用域（也就是局部方法变量）
3、SqlSessionFactory

(1)SqlSessionFactory可以想象为数据库连接池
(2)SqlSessionFactory 一旦被创建就应该在应用的运行期间一直存在，没有任何理由丢弃它或重新创建另一个实例。 
(3)使用 SqlSessionFactory 的最佳实践是在应用运行期间不要重复创建多次,多次重建 SqlSessionFactory 被视为一种代码“坏习惯”。因此 SqlSessionFactory 的最佳作用域是应用作用域。 (4)最简单的就是使用单例模式或者静态单例模式。
4、SqlSession

(1)SqlSession可以想象为(connection+preparedstatement,从连接池获取连接并获取执行SQL语句的对象)
(2)SqlSession 的实例不是线程安全的,因此是不能被共享的,所以它的最佳的作用域是请求或方法作用域。
(3)SqlSession 实例使用完毕后需要立即关闭(可以想象为将连接放回连接池),否则资源被占用。
ResultMap（最重要！！）
1、解决pojo实体类属性名和数据库中表的字段名不一致问题

2、pojo实体类

public class User {
    private int id;
    private String name;
    private String pwd;

    public User() {
    }

    public User(int id, String name, String pwd) {
        this.id = id;
        this.name = name;
        this.pwd = pwd;
    }

    public int getId() {return id;}
    public void setId(int id) {this.id = id;}
    public String getName() {return name;}
    public void setName(String name) {this.name = name;}
    public String getPwd() {return pwd;}
    public void setPwd(String pwd) {this.pwd = pwd;}

    @Override
    public String toString() {
        return "User{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", pwd='" + pwd + '\'' +
                '}';
    }
}
3、数据库表

id	name	password
3	lzz	123
4	zls	123
4、Mapper接口

public interface UserMapper {
    //根据ID查询用户
    User getUserById(int id);
}
5、Mapper文件

<mapper namespace="com.jxs.dao.UserMapper">

    <select id="getUserById" resultType="com.jxs.pojo.User" parameterType="int">
        select * from mybatis.user where id = #{id};
    </select>

</mapper>
6、测试

public class UserDaoTest {

    @Test
    public void test1() {
        //获取sqlSession对象实例
        SqlSession sqlSession = MyBatisUtils.getSqlSession();

        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User user = mapper.getUserById(3);
        System.out.println(user);
        sqlSession.close();
    }
}

//测试结果:User{id=3, name='lzz', pwd='null'}
7、pojo类的属性名和数据库表的字段名不对应造成

select * from mybatis.user where id = #{id};

select id,name,password from mybatis.user where id = #{id};
8、解决方案

(1)别名as(select id,name,password as pwd from mybatis.user where id = #{id};)
(2)resultMap
9、结果集映射简单使用

<mapper namespace="com.jxs.dao.UserMapper">

    <resultMap id="UserMap" type="User">
        <result column="id" property="id"/>
        <result column="name" property="name"/>
        <result column="password" property="pwd"/>
    </resultMap>

    <select id="getUserById" resultMap="UserMap">
        select * from mybatis.user where id = #{id};
    </select>

</mapper>
10、ResultMap基本介绍

(1)resultMap元素是MyBatis中最重要最强大的元素
(2)ResultMap的设计思想是对于简单的语句根本不需要配置显示的结果映射,而对于复杂的语句只需描述他们之间的关系
(3)ResultMap最优秀的地方在于虽然你已经对他相当了解,但是根本不需显示调用他们
<mapper namespace="com.jxs.dao.UserMapper">

    <resultMap id="UserMap" type="User">
        <result column="password" property="pwd"/>
    </resultMap>

    <select id="getUserById" resultMap="UserMap">
        select * from mybatis.user where id = #{id};
    </select>

</mapper>
日志
日志工厂
1、基本介绍

(1)若数据库操作出现异常,日志就是最好的排错助手
(2)Mybatis 通过使用内置的日志工厂提供日志功能。
(3)logImpl 可选的值有:
LOG4J、STDOUT_LOGGING(掌握)
SLF4J、LOG4J2、JDK_LOGGING、COMMONS_LOGGING、NO_LOGGING(了解)
2、settings中配置日志实现

<settings>
	<!--STDOUT_LOGGING标准日志输出-->
	<setting name="logImpl" value="STDOUT_LOGGING"/>
</settings>
3、STDOUT_LOGGING日志分析

![](E:\Study\自学课程资料\Java\assets\日志分析.png)

LOG4J
1、基本介绍

(1)Log4j是Apache的一个开源项目,通过使用Log4j,我们可以控制日志信息输送的目的地是控制台、文件、GUI组件,甚至是套接口服务器、NT的事件记录器、UNIX Syslog守护进程等
(2)可控制每一条日志的输出格式
(3)通过定义每一条日志信息的级别,我们能够更加细致地控制日志的生成过程
(4)可通过一个配置文件来灵活地进行配置,而不需要修改应用的代码。
2、导入log4j依赖

<dependency>
    <groupId>log4j</groupId>
    <artifactId>log4j</artifactId>
    <version>1.2.17</version>
</dependency>
3、src/main/resources目录下创建log4j配置文件log4j.properties

#将等级为DEBUG的日志信息输出到console(控制台)和file(文件)
log4j.rootLogger=DEBUG,console,file

#控制台输出的相关设置
log4j.appender.console = org.apache.log4j.ConsoleAppender
log4j.appender.console.Target = System.out
log4j.appender.console.Threshold=DEBUG
log4j.appender.console.layout = org.apache.log4j.PatternLayout
log4j.appender.console.layout.ConversionPattern=[%c]-%m%n

#文件输出的相关设置
log4j.appender.file = org.apache.log4j.RollingFileAppender
log4j.appender.file.File=./log/logFile.log
log4j.appender.file.MaxFileSize=10mb
log4j.appender.file.Threshold=DEBUG
log4j.appender.file.layout=org.apache.log4j.PatternLayout
log4j.appender.file.layout.ConversionPattern=[%p][%d{yy-MM-dd}][%c]%m%n

#日志输出级别
log4j.logger.org.mybatis=DEBUG
log4j.logger.java.sql=DEBUG
log4j.logger.java.sql.Statement=DEBUG
log4j.logger.java.sql.ResultSet=DEBUG
log4j.logger.java.sql.PreparedStatement=DEBUG
4、设置log4j为日志的实现

<settings>
    <setting name="logImpl" value="LOG4J"/>
</settings>
5、LOG4J日志分析

![](E:\Study\自学课程资料\Java\assets\LOG4J日志分析.png)

LOG4J简单使用
1、加载日志对象，参数为当前类的Class对象

Logger logger = Logger.getLogger(UserDaoTest.class);
2、测试

public class UserDaoTest {

    static Logger logger = Logger.getLogger(UserDaoTest.class);

    @Test
    public void testLog4j() {
        logger.info("info:进入了testLog4j()方法");
        logger.debug("debug:进入了testLog4j()方法");
        logger.error("debug:进入了testLog4j()方法");
    }
}
3、测试成功后子工程目录下生成log目录，log目录下生成logFile.log日志文件

分页
Limit分页
1、为何分页

(1)减少数据处理量
2、limit分页基本使用

# start从0开始计算,从start+1行开始取,取出rows行
select * from 表名 limit start,rows
3、Mapper接口（limit分页）

public interface UserMapper {
    //Limit分页查询用户
    List<User> getUserByLimit(Map<String, Object> map);
}
4、Mapper文件

<mapper namespace="com.jxs.dao.UserMapper">

    <select id="getUserByLimit" resultMap="UserMap" parameterType="map">
        select * from mybatis.user limit #{startIndex},#{pageSize};
    </select>

</mapper>
5、测试

@Test
public void testLimit() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();
    UserMapper mapper = sqlSession.getMapper(UserMapper.class);
    Map<String,Object> map = new HashMap<>();
    map.put("startIndex",0);
    map.put("pageSize",2);
    List<User> userByLimit = mapper.getUserByLimit(map);
    for (User user : userByLimit) {
        System.out.println(user);
    }
    sqlSession.close();
}
RowBounds分页
1、RowBounds不再使用SQL实现分页

2、Mapper接口

public interface UserMapper {
	//RowBounds分页查询用户
    List<User> getUserByRowBounds();
}
3、Mapper文件

<mapper namespace="com.jxs.dao.UserMapper">

    <select id="getUserByRowBounds" resultMap="UserMap">
        select * from mybatis.user;
    </select>

</mapper>
4、测试

@Test
public void testRowBounds() {
    SqlSession sqlSession = MyBatisUtils.getSqlSession();

    //通过RowBounds实现
    RowBounds rowBounds = new RowBounds(0, 2);

    //通过java代码层面实现
    List<Object> userList = sqlSession.selectList("com.jxs.dao.UserMapper.getUserByRowBounds",0,rowBounds);
    for (Object o : userList) {
        User user = (User) o;
        System.out.println(user);
    }
}
分页插件PageHelper（了解即可）
1、文档地址

https://pagehelper.github.io/
注解
面向接口编程
1、使用原因

(1)解耦、可扩展、复用性高
(2)分层开发中,上层不管具体的实现,大家都遵守共同的标准,使开发更具规范性
2、接口的理解

(1)接口:定义(规范、约束)与实现(名实分离原则)的分离
(2)接口本身反映了系统设计人员对系统的抽象理解
(3)接口有两类:(1)对个体的抽象,可对应为一个抽象体(2)对某一方面的抽象,可形成一个抽象面
使用注解开发
1、注解在Mapper接口上实现

public interface UserMapper {

    @Select("select id,name,password as pwd from user")
    List<User> getUsers();

}
2、在MyBatis核心配置文件绑定Mapper接口

<mappers>
    <mapper class="com.jxs.dao.UserMapper"/>
</mappers>
3、测试

public class UserDaoTest {

    @Test
    public void getUsersTest() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        List<User> users = mapper.getUsers();
        for (User user : users) {
            System.out.println(user);
        }
    }
}
4、本质

(1)本质:反射机制
(2)底层:动态代理
代理模式
1、静态代理理解

静态代理中,我们对目标对象的每个方法的增强都是手动完成的,非常不灵活(比如:接口一旦新增方法,目标对象和代理对象都要进行修改)且麻烦(需要对每个目标类都单独写一个代理类),从 JVM 层面来说,静态代理在编译时就将接口、实现类、代理类这些都变成了一个个实际的 class 文件
2、静态代理实现步骤

1.定义一个接口及其实现类
2.创建一个代理类同样实现这个接口
3.将目标对象注入进代理类,然后在代理类的对应方法调用目标类中的对应方法。如此就可以通过代理类屏蔽对目标对象的访问,并且可以在目标方法执行前后做一些自己想做的事情。
3、接口

#定义发送短信的接口
public interface SmsService {
    String send(String message);
}
4、接口实现类

public class SmsServiceImpl implements SmsService {
    public String send(String message) {
        System.out.println("send message:" + message);
        return message;
    }
}
5、代理类

public class SmsProxy implements SmsService {

    private final SmsService smsService;

    public SmsProxy(SmsService smsService) {
        this.smsService = smsService;
    }

    @Override
    public String send(String message) {
        //调用方法之前，我们可以添加自己的操作
        System.out.println("before method send()");
        smsService.send(message);
        //调用方法之后，我们同样可以添加自己的操作
        System.out.println("after method send()");
        return null;
    }
}
6、实际使用

public class Main {
    public static void main(String[] args) {
        SmsService smsService = new SmsServiceImpl();
        SmsProxy smsProxy = new SmsProxy(smsService);
        smsProxy.send("java");
    }
}

/*
输出结果：
before method send()
send message:java
after method send()
*/
MyBatis执行流程剖析（重要！！！）
1、编写核心配置文件mybatis-config.xml

2、Resources获取核心配置文件（InputStream inputStream = Resources.getResourceAsStream(mybatis-config.xml);）

3、创建SqlSessionFactoryBuilder对象实例（SqlSessionFactoryBuilder sqlSessionFactoryBuilder = new SqlSessionFactoryBuilder();）

4、解析配置文件流，返回XMLConfigBuilder对象实例（XMLConfigBuilder parser = new XMLConfigBuilder(inputStream, environment, properties);）

5、将所有配置信息存放在Configuration对象实例中

6、build()方法中传入Configuration对象实例，返回SqlSessionFactory对象实例（SqlSessionFactory sqlSessionFactory = sqlSessionFactoryBuilder.build(inputStream);）

public SqlSessionFactory build(Configuration config) {
    return new DefaultSqlSessionFactory(config);
}
7、transactional事务管理器

8、创建executor执行器

9、创建SqlSession对象实例（SqlSession sqlSession = sqlSessionFactory.openSession();）

10、实现CRUD

CRUD
1、MyBatis工具类实现自动提交事务

public static SqlSession getSqlSession() {
    /*
    参数设置为true,实现自动提交事务
    public SqlSession openSession(boolean autoCommit) {
    	return this.openSessionFromDataSource(this.configuration.getDefaultExecutorType(), (TransactionIsolationLevel)null, autoCommit);
    }
    */
    return sqlSessionFactory.openSession(true);
}
2、Mapper接口，增加注解，将接口绑定到核心配置文件中

public interface UserMapper {

    @Select("select id,name,password as pwd from user")
    List<User> getUsers();

    //方法中存在多个参数,所有参数前必须加上@Param注解
    @Select("select id,name,password as pwd from user where id = #{id} and name = #{name}")
    User getUserById(@Param("id") int id, @Param("name") String name);

    @Insert("insert into user (id,name,password) values (#{id},#{name},#{pwd})")
    int insertUser(User user);

    @Delete("delete from user where id = #{id}")
    int deleteUser(@Param("id") int id);

    @Update("update user set name = #{name} where id = #{id}")
    int updateUser(@Param("name") String name, @Param("id") int id);
}
3、测试

public class UserDaoTest {

    @Test
    public void getUsersTest() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        List<User> users = mapper.getUsers();
        for (User user : users) {
            System.out.println(user);
        }
    }

    @Test
    public void getUserById() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User userById = mapper.getUserById(3,"zls");
        System.out.println(userById);
    }

    @Test
    public void insertUser() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        int i = mapper.insertUser(new User(2, "dwy", "123"));

        List<User> users = mapper.getUsers();
        for (User user : users) {
            System.out.println(user);
        }
    }

    @Test
    public void deleteUser() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        int i = mapper.deleteUser(6);

        List<User> users = mapper.getUsers();
        for (User user : users) {
            System.out.println(user);
        }
    }

    @Test
    public void updateUser() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        int i = mapper.updateUser("jxj", 5);

        List<User> users = mapper.getUsers();
        for (User user : users) {
            System.out.println(user);
        }
    }
}
@Param(String value)注解
(1)Mapper接口的方法的形参列表中存在基本数据类型或String类型必须加上@Param()注解
(2)Mapper接口的方法的形参列表中为引用类型不需要加上@Param()注解
(3)Mapper接口的方法的形参列表中只存在一个基本数据类型,可以忽略@Param()注解,但建议都加上@Param()注解
(4)SQL中的引用即@Param(String value)中的value属性名
Lombok（偷懒神器）
1、基本介绍

Project Lombok is a java library that automatically plugs into your editor and build tools, spicing up your java.
Never write another getter or equals method again, with one annotation your class has a fully featured builder, Automate your logging variables, and much more.

Project Lombok 是一个 Java 库，它会自动插入编辑器和构建工具，为您的 Java 增添趣味。
永远不要再写另一个 getter 或 equals 方法，使用一个注释，您的类有一个功能齐全的构建器，自动化您的日志记录变量等等。
2、安装Lombok插件

3、项目中导入lombok依赖包

<dependency>
    <groupId>org.projectlombok</groupId>
    <artifactId>lombok-maven-plugin</artifactId>
    <version>1.18.20.0</version>
</dependency>
4、lombok注解

@Getter and @Setter
@FieldNameConstants
@ToString
@EqualsAndHashCode
@AllArgsConstructor, @RequiredArgsConstructor and @NoArgsConstructor
@Log, @Log4j, @Log4j2, @Slf4j, @XSlf4j, @CommonsLog, @JBossLog, @Flogger, @CustomLog
@Data
@Builder
@SuperBuilder
@Singular
@Delegate
@Value
@Accessors
@Wither
@With
@SneakyThrows
@val
@var
experimental @var
@UtilityClass
Lombok config system
5、@Data：为pojo实体类生成无参构造、get()、set()、toString()、hashcode()、equals()方法

@Data
public class User {
    private int id;
    private String name;
    private String pwd;
}
6、@AllArgsConstructor：为pojo实体类生成有参构造

@Data
@AllArgsConstructor
public class User {
    private int id;
    private String name;
    private String pwd;
}
7、@NoArgsConstructor：为pojo实体类生成无参构造

@Data
@AllArgsConstructor
@NoArgsConstructor
public class User {
    private int id;
    private String name;
    private String pwd;
}
8、@ToString：为pojo实体类生成toString()方法

@ToString
public class User {
    private int id;
    private String name;
    private String pwd;
}
9、@EqualsAndHashCode：为pojo实体类生成equals()、hashcode()方法

@EqualsAndHashCode
public class User {
    private int id;
    private String name;
    private String pwd;
}
10、Lombok优缺点

优点:
(1)通过注解的形式自动生成构造器、getter、setter、equals、hashcode、toString等方法,提高开发效率
(2)简洁代码
(3)属性修改后,也简化了维护这些属性所生成的getter()、setter()方法等

缺点:
(1)不支持多种参数构造器的重载
(2)降低代码的可读性以及完整性,降低阅读代码的舒适度
多对一处理（难点重点）
1、概念理解

一位老师教导多位学生

对于学生:多位学生关联一位老师(关联)
对于老师:一位老师包含多位学生(集合)
2、数据库中新建表

CREATE TABLE teacher(
id INT PRIMARY KEY,
`name` VARCHAR(32));

INSERT INTO teacher VALUES (1,'jxs');

CREATE TABLE student(
id INT PRIMARY KEY,
`name` VARCHAR(32),
teacher_id INT,
FOREIGN KEY (teacher_id) REFERENCES teacher(id));

INSERT INTO student VALUES (1,'dwy',1);
INSERT INTO student VALUES (2,'zls',1);
INSERT INTO student VALUES (3,'lzz',1);
INSERT INTO student VALUES (4,'tyh',1);
INSERT INTO student VALUES (5,'jxj',1);
3、模型图

![](E:\Study\自学课程资料\Java\assets\多对一模型图.png)

测试环境搭建
1、新建Maven工程

2、导入log4j日志、lombok依赖包

3、核心配置文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-config.dtd">

<!--configuration核心配置文件-->
<configuration>

    <!--引入外部配置文件-->
    <properties resource="db.properties">
        <!--在 properties 元素的子元素中设置属性-->
        <property name="username" value="root"/>
        <property name="password" value="123456"/>
    </properties>

    <!--日志-->
    <settings>
        <setting name="logImpl" value="LOG4J"/>
    </settings>

    <!--别名-->
    <typeAliases>
        <package name="com.jxs.pojo"/>
    </typeAliases>

    <!--环境-->
    <environments default="test">
        <environment id="test">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="${driver}"/>
                <property name="url" value="${jdbc.url}"/>
                <property name="username" value="${username}"/>
                <property name="password" value="${password}"/>
            </dataSource>
        </environment>
    </environments>

</configuration>
4、新建pojo实体类

@Data
public class Student {
    private int id;
    private String name;
    //关联一位老师
    private Teacher teacher;
}
@Data
public class Teacher {
    private int id;
    private String name;
}
5、新建Mapper接口

public interface StudentMapper {
}
public interface TeacherMapper {
    //查询所有教师
    List<Teacher> getTeachers();
}
6、新建Mapper文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.StudentMapper">
    
</mapper>
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.TeacherMapper">

    <select id="getTeachers" resultType="com.jxs.pojo.Teacher">
        select * from mybatis.teacher;
    </select>

</mapper>
7、核心配置文件中绑定注册

<mappers>
    <mapper class="com.jxs.dao.StudentMapper"/>
    <mapper class="com.jxs.dao.TeacherMapper"/>
</mappers>
8、测试

public class StudentMapperTest {
}
public class TeacherMapperTest {

    @Test
    public void testGetTeachers() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        TeacherMapper mapper = sqlSession.getMapper(TeacherMapper.class);
        List<Teacher> teachers = mapper.getTeachers();
        for (Teacher teacher : teachers) {
            System.out.println(teacher);
        }
        sqlSession.close();
    }
}
根据查询嵌套处理
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">


<!--绑定StudentMapper接口-->
<mapper namespace="com.jxs.dao.StudentMapper">
    <!--
    思路:
    查询所有学生信息
    根据查询出的teacher_id寻找对应教师
    -->
    <resultMap id="StudentMap01" type="Student">
        <result property="id" column="id"/>
        <result property="name" column="name"/>
        <!--复杂的属性单独处理,对象:association、集合:collection-->
        <!--
        将Student类teacher属性对应数据库student表teacher_id字段
        设置teacher属性为Teacher类型
        创建表时设置student表teacher_id字段为teacher表id字段外键
        查询teacher表时将student.teacher_id=teacher.id的数据查询出来
        -->
        <association property="teacher" column="teacher_id" javaType="Teacher" select="getTeachers"/>
    </resultMap>

    <select id="getStudents01" resultMap="StudentMap01">
        select * from mybatis.student;
    </select>

    <select id="getTeachers" resultType="teacher">
        select * from mybatis.teacher where id = #{teacher_id};
    </select>
</mapper>
按照结果嵌套处理
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">


<!--绑定StudentMapper接口-->
<mapper namespace="com.jxs.dao.StudentMapper">
	<resultMap id="StudentMap02" type="Student">
        <result property="id" column="s_id"/>
        <result property="name" column="s_name"/>
        <association property="teacher" javaType="Teacher">
            <result property="id" column="s_id"/>
            <result property="name" column="t_name"/>
        </association>
    </resultMap>

    <select id="getStudents02" resultMap="StudentMap02">
        select student.id as s_id,student.name as s_name,teacher.name t_name
        from mybatis.student,mybatis.teacher
        where student.teacher_id = teacher.id
    </select>
</mapper>
总结
1、MySQL多对一查询方式

(1)子查询
(2)联表查询
一对多处理
测试环境搭建
1、新建Maven工程

2、导入log4j日志、lombok依赖包

3、核心配置文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-config.dtd">

<!--configuration核心配置文件-->
<configuration>

    <!--引入外部配置文件-->
    <properties resource="db.properties">
        <!--在 properties 元素的子元素中设置属性-->
        <property name="username" value="root"/>
        <property name="password" value="123456"/>
    </properties>

    <!--日志-->
    <settings>
        <setting name="logImpl" value="LOG4J"/>
    </settings>

    <!--别名-->
    <typeAliases>
        <package name="com.jxs.pojo"/>
    </typeAliases>

    <!--环境-->
    <environments default="test">
        <environment id="test">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="${driver}"/>
                <property name="url" value="${jdbc.url}"/>
                <property name="username" value="${username}"/>
                <property name="password" value="${password}"/>
            </dataSource>
        </environment>
    </environments>

</configuration>
4、新建pojo实体类

@Data
public class Student {
    private int id;
    private String name;
    private int teacher_id;
}
@Data
public class Teacher {
    private int id;
    private String name;
    //一位教师包含多位学生
    private List<Student> students;
}
5、新建Mapper接口

public interface StudentMapper {
}
public interface TeacherMapper {
    List<Teacher> getTeachers01();
}
6、新建Mapper文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.StudentMapper">

</mapper>
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.TeacherMapper">

    <select id="getTeachers01" resultType="Teacher">
        select * from mybatis.teacher;
    </select>
    
</mapper>
7、核心配置文件中绑定注册

<mappers>
    <mapper class="com.jxs.dao.StudentMapper"/>
    <mapper class="com.jxs.dao.TeacherMapper"/>
</mappers>
8、测试

public class StudentMapperTest {
}
public class TeacherMapperTest {
    @Test
    public void testGetTeachers01() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        TeacherMapper mapper = sqlSession.getMapper(TeacherMapper.class);
        List<Teacher> teacherList = mapper.getTeachers01();
        for (Teacher teacher : teacherList) {
            System.out.println(teacher);
        }
    }
}
按照结果嵌套查询
1、Mapper接口

public interface TeacherMapper {
    //获取指定教师下的学生和教师信息
    //SQL中的引用即@Param(String value)中的value属性名
    Teacher getTeachers02(@Param("t_id") int id);
}
2、Mapper文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.TeacherMapper">

    <resultMap id="TeacherMap01" type="Teacher">
        <result property="id" column="t_id"/>
        <result property="name" column="t_name"/>
        <!--
        javaType 指定属性的数据类型
        ofType 集合中泛型的数据类型
        -->
        <collection property="students" ofType="Student">
            <result property="id" column="s_id"/>
            <result property="name" column="s_name"/>
            <result property="teacher_id" column="t_id"/>
        </collection>
    </resultMap>

    <select id="getTeachers02" resultMap="TeacherMap01" parameterType="int">
        select student.id as s_id,student.name as s_name,
        teacher.id as t_id,teacher.name as t_name
        from mybatis.student,mybatis.teacher
        where student.teacher_id = teacher.id and teacher.id = #{t_id};
    </select>

</mapper>
按照查询嵌套查询
1、Mapper接口

public interface TeacherMapper {
    //获取指定教师下的学生和教师信息
    Teacher getTeachers02(@Param("t_id") int id);
}
2、Mapper文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.TeacherMapper">

    <select id="getTeachers02" resultMap="TeacherMap" parameterType="int">
        select id,name from mybatis.teacher where id = #{t_id};
    </select>

    <resultMap id="TeacherMap" type="Teacher">
        <result property="id" column="id"/>
        <result property="name" column="name"/>
        <collection property="students" javaType="ArrayList" ofType="Student" column="id" select="getStudents"/>
    </resultMap>

    <select id="getStudents" resultType="Student">
        select * from mybatis.Student where teacher_id = #{t_id};
    </select>

</mapper>
总结
1、关联（association）：多对一；集合（collection）：一对多

2、javaType：指定实体类中属性的数据类型；ofType：指定映射到List或集合中的pojo类型，即泛型中的数据类型

动态SQL
搭建环境
1、数据库创建表

CREATE TABLE blog(
id VARCHAR(32) COMMENT '博客id',
title VARCHAR(32) COMMENT '博客标题',
author VARCHAR(32) COMMENT '博客作者',
create_time DATETIME COMMENT '博客创建时间',
views int(30) COMMENT '博客浏览量');
2、创建Maven工程

3、新建核心配置文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-config.dtd">

<!--configuration核心配置文件-->
<configuration>

    <!--引入外部配置文件-->
    <properties resource="db.properties">
        <!--在 properties 元素的子元素中设置属性-->
        <property name="username" value="root"/>
        <property name="password" value="123456"/>
    </properties>

    <!--设置-->
    <settings>
        <setting name="mapUnderscoreToCamelCase" value="true"/>
    </settings>

    <!--类别名-->
    <typeAliases>
        <typeAlias type="com.jxs.pojo.Blog" alias="blog"/>
    </typeAliases>

    <!--环境-->
    <environments default="test">
        <environment id="test">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="${driver}"/>
                <property name="url" value="${jdbc.url}"/>
                <property name="username" value="${username}"/>
                <property name="password" value="${password}"/>
            </dataSource>
        </environment>
    </environments>

</configuration>
4、MyBatis工具类、ID工具类

/**
 * MyBatisUtils工具类
 */
public class MyBatisUtils {
    private static SqlSessionFactory sqlSessionFactory;

    static {
        try {
            //使用MyBatis第一步:获取sqlSessionFactory(SQL会话工厂)对象实例
            String resource = "mybatis-config.xml";
            InputStream inputStream = Resources.getResourceAsStream(resource);
            SqlSessionFactoryBuilder sqlSessionFactoryBuilder = new SqlSessionFactoryBuilder();
            sqlSessionFactory = sqlSessionFactoryBuilder.build(inputStream);

        } catch (IOException e) {
            e.printStackTrace();
        }
    }


    public static SqlSession getSqlSession() {
        /*
        参数设置为true,实现自动提交事务
        public SqlSession openSession(boolean autoCommit) {
            return this.openSessionFromDataSource(this.configuration.getDefaultExecutorType(), (TransactionIsolationLevel)null, autoCommit);
        }
        */
        return sqlSessionFactory.openSession(true);
    }
}
public class IDUtils {

    public static String getId() {
        return UUID.randomUUID().toString().replace("-","");
    }
}
5、新建pojo实体类

@Data
@AllArgsConstructor
public class Blog {
    private String id;
    private String title;
    private String author;
    private Date createTime;
    private int views;
}
6、新建Mapper接口、Mapper文件

public interface BlogMapper {
    //插入数据
    int insertBlog(Blog blog);
}
<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.BlogMapper">

    <insert id="insertBlog" parameterType="blog">
        insert into mybatis.blog
        values (#{id},#{title},#{author},#{createTime},#{views})
    </insert>
</mapper>
7、核心配置文件中添加Mapper映射

<mappers>
    <mapper class="com.jxs.dao.BlogMapper"/>
</mappers>
8、测试

public class BlogMapperTest {
    @Test
    public void testInsertBlog() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        Blog blog = new Blog(IDUtils.getId(),"MyBatis如此简单","jxs",new Date(),99);
        Blog blog1 = new Blog(IDUtils.getId(),"Java如此简单","jxs",new Date(),99);
        Blog blog2 = new Blog(IDUtils.getId(),"Spring如此简单","jxs",new Date(),99);
        int i = mapper.insertBlog(blog);
        int i1 = mapper.insertBlog(blog1);
        int i2 = mapper.insertBlog(blog2);
        sqlSession.close();
    }
}
动态SQL之IF语句
1、官方案例

<select id="findActiveBlogWithTitleLike"
     resultType="Blog">
  SELECT * FROM BLOG
  WHERE state = ‘ACTIVE’
  <if test="title != null">
    AND title like #{title}
  </if>
</select>
这条语句提供了可选的查找文本功能。
若不传入 “title”，那么所有处于 “ACTIVE” 状态的 BLOG 都会返回
若传入了 “title” 参数，那么就会对 “title” 一列进行模糊查找并返回对应的 BLOG 结果
2、Mapper接口

public interface BlogMapper {
    //查询blog
    List<Blog> queryBlogIf(Map map);
}
3、Mapper文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE mapper
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-mapper.dtd">

<mapper namespace="com.jxs.dao.BlogMapper">
    <select id="queryBlogIf" parameterType="map" resultType="blog">
        select * from mybatis.blog where 1 = 1
        <if test="title != null">
            and title = #{title}
        </if>
        <if test="author != null">
            and author = #{author}
        </if>
    </select>
</mapper>
4、测试

public class BlogMapperTest {

    @Test
    public void testQueryBlogIf() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        HashMap hashMap = new HashMap();
        hashMap.put("title","MyBatis如此简单");
        hashMap.put("author","dwy");
        List<Blog> blogs = mapper.queryBlogIf(hashMap);
        for (Blog blog : blogs) {
            System.out.println(blog);
        }
        sqlSession.close();
    }
}
动态SQL之trim、where、set
where
1、where官方案例

(1)
<select id="findActiveBlogLike"
     resultType="Blog">
  SELECT * FROM BLOG
  WHERE
  <if test="state != null">
    state = #{state}
  </if>
  <if test="title != null">
    AND title like #{title}
  </if>
  <if test="author != null and author.name != null">
    AND author_name like #{author.name}
  </if>
</select>

(2)
若没有匹配的条件会怎么样？最终 SQL 语句会变成这样:
SELECT * FROM BLOG
WHERE
导致查询失败。

(3)
若匹配的只是第二个条件又会怎样？这条 SQL 会是这样:
SELECT * FROM BLOG
WHERE
AND title like ‘someTitle’
这个查询也会失败。这个问题不能简单地用条件元素来解决。

(4)
MyBatis 有一个简单且适合大多数场景的解决办法。而在其他场景中，可以对其进行自定义以符合需求。
<select id="findActiveBlogLike"
     resultType="Blog">
  SELECT * FROM BLOG
  <where>
    <if test="state != null">
         state = #{state}
    </if>
    <if test="title != null">
        AND title like #{title}
    </if>
    <if test="author != null and author.name != null">
        AND author_name like #{author.name}
    </if>
  </where>
</select>
where 元素只会在子元素返回任何内容的情况下才插入 “WHERE” 子句。
而且,若子句的开头为 “AND” 或 “OR”，where 元素也会将它们去除。
2、Mapper接口

public interface BlogMapper {
    //查询blog
    List<Blog> queryBlogWhere(Map map);
}
3、Mapper文件

<mapper namespace="com.jxs.dao.BlogMapper">
    
    <select id="queryBlogWhere" parameterType="map" resultType="blog">
        select * from mybatis.blog
        <where>
            <if test="title != null">
                title = #{title}
            </if>
            <if test="author != null">
                and author = #{author}
            </if>
        </where>
    </select>
    
</mapper>
4、测试

public class BlogMapperTest {
    @Test
    public void testQueryBlogWhere() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        HashMap hashMap = new HashMap();
        hashMap.put("title","MyBatis如此简单");
        hashMap.put("author","jxs");
        List<Blog> blogs = mapper.queryBlogWhere(hashMap);
        for (Blog blog : blogs) {
            System.out.println(blog);
        }
        sqlSession.close();
    }
}
set
1、set官方案例

用于动态更新语句的类似解决方案叫做 set。set 元素可以用于动态包含需要更新的列，忽略其它不更新的列。
<update id="updateAuthorIfNecessary">
  update Author
    <set>
      <if test="username != null">username=#{username},</if>
      <if test="password != null">password=#{password},</if>
      <if test="email != null">email=#{email},</if>
      <if test="bio != null">bio=#{bio}</if>
    </set>
  where id=#{id}
</update>
这个例子中，set 元素会动态地在行首插入 SET 关键字，并会删掉额外的逗号（这些逗号是在使用条件语句给列赋值时引入的）。
2、Mapper接口

public interface BlogMapper {
    //更新博客
    int updateBlogSet(Map map);
}
3、Mapper文件

<mapper namespace="com.jxs.dao.BlogMapper">   
    <update id="updateBlogSet" parameterType="map">
        update mybatis.blog
        <set>
            <if test="title != null">
                title = #{title},
            </if>
            <if test="author != null">
                author = #{author},
            </if>
        </set>
        <where>
            id = #{id}
        </where>
    </update>
</mapper>
4、测试

public class BlogMapperTest {    
    @Test
    public void testUpdateBlogSet() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        HashMap hashMap = new HashMap();
        hashMap.put("title","MySQL如此简单");
        hashMap.put("author","jxs");
        hashMap.put("id","5c1361ad69de49f09ff90d935c99515c");
        mapper.updateBlogSet(hashMap);
        sqlSession.close();
    }
}
trim
1、官方案例

<trim prefix="WHERE" prefixOverrides="AND |OR ">
  ...
</trim>

<trim prefix="SET" suffixOverrides=",">
  ...
</trim>

prefixOverrides 属性会忽略通过管道符分隔的文本序列（注意此例中的空格是必要的）。
上述例子会移除所有 prefixOverrides 属性中指定的内容，并且插入 prefix 属性中指定的内容。
动态SQL之choose、when、otherwise
1、choose官方案例

<select id="findActiveBlogLike"
     resultType="Blog">
  SELECT * FROM BLOG WHERE state = ‘ACTIVE’
  <choose>
    <when test="title != null">
      AND title like #{title}
    </when>
    <when test="author != null and author.name != null">
      AND author_name like #{author.name}
    </when>
    <otherwise>
      AND featured = 1
    </otherwise>
  </choose>
</select>
有时候，我们不想使用所有的条件，而只是想从多个条件中选择一个使用。针对这种情况，MyBatis 提供了 choose 元素，它有点像 Java 中的 switch 语句。

还是上面的例子，但是策略变为：传入了 “title” 就按 “title” 查找，传入了 “author” 就按 “author” 查找的情形。若两者都没有传入，就返回标记为 featured 的 BLOG
2、Mapper接口

public interface BlogMapper {
    //查询blog
    List<Blog> queryBlogChoose(Map map);
}
3、Mapper文件

<mapper namespace="com.jxs.dao.BlogMapper">    
    <select id="queryBlogChoose" resultType="blog" parameterType="map">
        select * from mybatis.blog
        <where>
            <choose>
                <!--多个条件中选择一个使用
                只执行一个when标签中的内容
                相当于switch case用法-->
                <when test="title != null">
                    title = #{title}
                </when>
                <when test="author != null">
                    and author = #{author}
                </when>
                <!--若两个when标签中的条件都不满足,就返回满足views = #{views}的数据-->
                <otherwise>
                    and views = #{views}
                </otherwise>
            </choose>
        </where>
    </select>
</mapper>
4、测试

public class BlogMapperTest {
    @Test
    public void testQueryBlogChoose() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        HashMap hashMap = new HashMap();
        //hashMap.put("title","MyBatis如此简单");
        hashMap.put("author","jxs");
        //hashMap.put("views","99");
        List<Blog> blogs = mapper.queryBlogChoose(hashMap);
        for (Blog blog : blogs) {
            System.out.println(blog);
        }
    }
}
动态SQL之foreach
SQL片段
1、基本介绍

(1)使用SQL标签抽取公共部分
(2)在需要使用的地方使用include标签引用
2、Mapper接口

public interface BlogMapper {
    //查询blog
    List<Blog> queryBlogIf(Map map);
}
3、Mapper文件

<mapper namespace="com.jxs.dao.BlogMapper">

    <sql id="if-title-author">
        <if test="title != null">
            title = #{title}
        </if>
        <if test="author != null">
            and author = #{author}
        </if>
    </sql>

    <!--=========================================================-->

    <select id="queryBlogIf" parameterType="map" resultType="blog">
        select * from mybatis.blog
        <where>
            <include refid="if-title-author"></include>
        </where>
    </select>

</mapper>
4、测试

public class BlogMapperTest {
    @Test
    public void testQueryBlogIf() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        HashMap hashMap = new HashMap();
        hashMap.put("title","MyBatis如此简单");
        hashMap.put("author","dwy");
        List<Blog> blogs = mapper.queryBlogIf(hashMap);
        for (Blog blog : blogs) {
            System.out.println(blog);
        }
        sqlSession.close();
    }
}
5、注意事项

(1)基于单表定义SQL片段
(2)SQL片段中不可存在Where标签
(3)
foreach
1、官方案例

<select id="selectPostIn" resultType="domain.blog.Post">
  SELECT *
  FROM POST P
  <where>
    <foreach item="item" index="index" collection="list"
        open="ID in (" separator="," close=")" nullable="true">
          #{item}
    </foreach>
  </where>
</select>
(1)foreach 元素的功能非常强大，允许指定一个集合
(2)声明可以在元素体内使用的集合项（item）和索引（index）变量
(3)它也允许你指定开头与结尾的字符串以及集合项迭代之间的分隔符。
(4)foreach 元素不会错误地添加多余的分隔符
2、注意事项

可以将任何可迭代对象(如List、Set等)、Map对象或者数组对象作为集合参数传递给foreach。
当使用可迭代对象或者数组时,index是当前迭代的序号,item的值是本次迭代获取到的元素
当使用Map对象(或者Map.Entry对象的集合)时,index是键,item是值。
3、Mapper接口

public interface BlogMapper {
    //查询1、2、3号记录的博客
    List<Blog> queryBlogForeach(Map map);
}
4、Mapper文件

<mapper namespace="com.jxs.dao.BlogMapper">   
    
    <select id="queryBlogForeach" parameterType="map" resultType="blog">
        select * from mybatis.blog
        <where>
            <foreach collection="ids" item="id" open="and (" close=")" separator="or">
                id = #{id}
            </foreach>
        </where>
    </select>
    
</mapper>
5、测试

public class BlogMapperTest {
    @Test
    public void testQueryBlogForeach() {
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        BlogMapper mapper = sqlSession.getMapper(BlogMapper.class);
        
        ArrayList<Integer> ids = new ArrayList<>();
        HashMap hashMap = new HashMap();
        hashMap.put("ids", ids);
        
        List<Blog> blogs = mapper.queryBlogForeach(hashMap);
        for (Blog blog : blogs) {
            System.out.println(blog);
        }
        sqlSession.close();
    }
}
动态SQL总结
(1)何为动态SQL:动态SQL指根据不同的条件生成不同的SQL语句
(2)动态SQL的本质还是SQL语句,只是可以在SQL层面执行一个逻辑代码
(3)动态SQL即拼接SQL语句,只要保证SQL的正确性,按照SQL的格式进行排列组合即可
缓存
简介
1、缓存个人理解

(1)进行每次查询都连接数据库,耗资源
(2)一次查询的结果暂存在内存中,再次查询相同的数据时,直接走缓存
2、基本介绍

何为缓存:
(1)存储在内存中的临时数据
(2)将用户经常查询的数据存放在缓存(内存)中,用户查询数据时就不再从磁盘上(关系型数据库数据文件)查询,而是从缓存(内存)中查询,提高查询效率,解决高并发系统的性能问题。

为何使用缓存:
(1)减少与数据库交互的次数
(2)减少系统开销
(3)提高系统效率

何时使用缓存:
(1)经常查询且不经常改变的数据
MyBatis缓存
(1)MyBatis包含一个非常强大的查询缓存特性,可以非常方便的定制和配置缓存,缓存可以极大的提升查询效率。
(2)MyBatis系统中默认定义了两级缓存:一级缓存、二级缓存
(3)默认情况下,只有一级缓存开启(SqlSession级别的缓存,也称为本地缓存)
(4)二级缓存需手动开启和配置(namespace级别的缓存)
(5)为提高扩展性,MyBatis定义了缓存接口Cache,我们可以通过Cache接口来自定义二级缓存
一级缓存
1、配置日志

(1)导入日志依赖
(2)创建日志配置文件
(3)MyBatis核心配置文件中设置日志实现
2、Mapper接口

public interface UserMapper {
    User getUserById(int id);
}
3、Mapper文件

<mapper namespace="com.jxs.dao.UserMapper">
    <select id="getUserById" resultType="user" parameterType="int">
        select * from user where id = #{id};
    </select>
</mapper>
4、测试在一个sqlSession中查询两次相同记录

public class TestUserMapper {
    @Test
    public void testGetUsers() {
        //一级缓存
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User user1 = mapper.getUserById(1);
        User user2 = mapper.getUserById(1);
        /*
        [org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Opening JDBC Connection
        [org.apache.ibatis.datasource.pooled.PooledDataSource]-Created connection 1132307065.
        [com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
        [com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
        [com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
        true
        [org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@437da279]
        [org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1132307065 to pool.
        */
        System.out.println(user1 == user2);
        sqlSession.close();
    }
}
5、何时缓存

(1)映射语句文件中的所有 select 语句的结果将会被缓存。
(2)映射语句文件中的所有 insert、update 和 delete 语句会刷新缓存。
(3)缓存会使用最近最少使用算法（LRU, Least Recently Used）算法来清除不需要的缓存。
(4)缓存不会定时进行刷新（也就是说，没有刷新间隔）。
(5)缓存会保存列表或对象（无论查询方法返回哪种）的 1024 个引用。
(6)缓存会被视为读/写缓存，这意味着获取到的对象并不是共享的，可以安全地被调用者修改，而不干扰其他调用者或线程所做的潜在修改。
6、缓存失效

(1)映射语句文件中查询不同的记录
(2)增删改操作后刷新缓存
(3)手动清理缓存
public class TestUserMapper {
    @Test
    public void testGetUsers() {
        //一级缓存
        SqlSession sqlSession = MyBatisUtils.getSqlSession();
        UserMapper mapper = sqlSession.getMapper(UserMapper.class);
        User user1 = mapper.getUserById(1);

        HashMap<String, Object> hashMap = new HashMap<>();
        hashMap.put("id", 1);
        hashMap.put("name", "蒋兴树");
        hashMap.put("password", "123456");
        int i = mapper.updateUser(hashMap);

        //映射语句文件中的所有 insert、update 和 delete 语句会刷新缓存。
        User user2 = mapper.getUserById(1);

        /*
        [org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Opening JDBC Connection
        [org.apache.ibatis.datasource.pooled.PooledDataSource]-Created connection 1132307065.
        [com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
        [com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
        [com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
        [com.jxs.dao.UserMapper.updateUser]-==>  Preparing: update user set name = ?,password = ? where id = ?;
        [com.jxs.dao.UserMapper.updateUser]-==> Parameters: 蒋兴树(String), 123456(String), 1(Integer)
        [com.jxs.dao.UserMapper.updateUser]-<==    Updates: 1
        [com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
        [com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
        [com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
        false
        [org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@437da279]
        [org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1132307065 to pool.
        */
        System.out.println(user1 == user2);


        //缓存失效:手动清理缓存
        User user3 = mapper.getUserById(2);
        sqlSession.clearCache();
        /*
        [com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
        [com.jxs.dao.UserMapper.getUserById]-==> Parameters: 2(Integer)
        [com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
        [com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
        [com.jxs.dao.UserMapper.getUserById]-==> Parameters: 2(Integer)
        [com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
        [org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@437da279]
        [org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1132307065 to pool.
        */
        User user4 = mapper.getUserById(2);
        sqlSession.close();
    }
}
7、总结

(1)一级缓存默认开启,只在一次sqlSession中有效,即拿到数据库连接到关闭数据库连接区间段
二级缓存（看总结！！！）
1、基本介绍

(1)二级缓存也叫全局缓存,一级缓存作用域在会话开启和关闭期间
(2)二级缓存,基于namespace级别的缓存,一个命名空间对应一个二级缓存
2、工作机制

(1)一个会话查询一条数据,此数据会被存放在当前会话的一级缓存中
(2)若当前会话关闭,此会话对应的一级缓存就不存在
(3)若想要会话关闭后,一级缓存中的数据被保存到二级缓存中
(4)新的会话查询信息,可以从二级缓存中获取内容
3、二级缓存步骤

(1)核心配置文件中显示开启全局缓存(二级缓存)
<settings>
    <!--显示开启全局缓存-->
    <setting name="cacheEnabled" value="true"/>
</settings>
(2)在Mapper文件中使用二级缓存
<!--
1.创建了一个 FIFO 缓存
2.每隔 60 秒刷新
3.最多可以存储结果对象或列表的 512 个引用
4.返回的对象被认为是只读的
-->
<cache eviction="FIFO"
       flushInterval="60000"
       size="512"
       readOnly="true"/>
可用的清除策略有:
	LRU – 最近最少使用:移除最长时间不被使用的对象。
	FIFO – 先进先出:按对象进入缓存的顺序来移除它们。
    SOFT – 软引用:基于垃圾回收器状态和软引用规则移除对象。
    WEAK – 弱引用:更积极地基于垃圾收集器状态和弱引用规则移除对象。
    默认的清除策略是 LRU。
4、测试

public class TestUserMapper01 {
    @Test
    public void testGetUserById() {
        SqlSession sqlSession1 = MyBatisUtils.getSqlSession();
        UserMapper mapper1 = sqlSession1.getMapper(UserMapper.class);
        User user1 = mapper1.getUserById(1);
        sqlSession1.close();

        SqlSession sqlSession2 = MyBatisUtils.getSqlSession();
        UserMapper mapper2 = sqlSession2.getMapper(UserMapper.class);
        User user2 = mapper2.getUserById(1);
        sqlSession2.close();
    }
}
5、不使用二级缓存

[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Opening JDBC Connection
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Created connection 1132307065.
[com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
[com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
[com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@437da279]
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1132307065 to pool.
[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Opening JDBC Connection
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Checked out connection 1132307065 from pool.
[com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
[com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
[com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@437da279]
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1132307065 to pool.
6、使用二级缓存

[com.jxs.dao.UserMapper]-Cache Hit Ratio [com.jxs.dao.UserMapper]: 0.0
[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Opening JDBC Connection
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Created connection 1420232606.
[com.jxs.dao.UserMapper.getUserById]-==>  Preparing: select * from user where id = ?;
[com.jxs.dao.UserMapper.getUserById]-==> Parameters: 1(Integer)
[com.jxs.dao.UserMapper.getUserById]-<==      Total: 1
[org.apache.ibatis.transaction.jdbc.JdbcTransaction]-Closing JDBC Connection [com.mysql.cj.jdbc.ConnectionImpl@54a7079e]
[org.apache.ibatis.datasource.pooled.PooledDataSource]-Returned connection 1420232606 to pool.
[com.jxs.dao.UserMapper]-Cache Hit Ratio [com.jxs.dao.UserMapper]: 0.5
7、注意事项

(1)将pojo实体类序列化
8、总结

一个会话查询一条数据,此数据会被存放在当前会话对应的一级缓存中,若Mapper文件中开启二级缓存且关闭该会话(或提交会话),该会话对应的一级缓存中的数据会被保存到二级缓存中,若同一个Mapper下新的会话查询信息,可以从二级缓存中获取内容
缓存原理图
![](E:\Study\自学课程资料\Java\assets\缓存原理图.png)

自定义缓存（ehcache）
1、基本介绍

Ehcache是一种广泛使用的开源Java分布式缓存,主要面向通用缓存
2、导入ehcache依赖

<dependency>
    <groupId>org.mybatis.caches</groupId>
    <artifactId>mybatis-ehcache</artifactId>
    <version>1.2.2</version>
</dependency>
3、Mapper文件中自定义二级缓存

<cache type="org.mybatis.caches.ehcache.EhcacheCache"/>
4、创建ehcache.xml配置文件

<?xml version="1.0" encoding="UTF-8"?>
<ehcache xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:noNamespaceSchemaLocation="http://ehcache.org/ehcache.xsd"
         updateCheck="false">

    <!--
       diskStore：为缓存路径，ehcache分为内存和磁盘两级，此属性定义磁盘的缓存位置。参数解释如下:
       user.home – 用户主目录
       user.dir  – 用户当前工作目录
       java.io.tmpdir – 默认临时文件路径
     -->
    <diskStore path="java.io.tmpdir/Tmp_EhCache"/>

    <!--
       defaultCache：默认缓存策略，当ehcache找不到定义的缓存时，则使用这个缓存策略。只能定义一个。
     -->
    <!--
      name:缓存名称。
      maxElementsInMemory:缓存最大数目
      maxElementsOnDisk：硬盘最大缓存个数。
      eternal:对象是否永久有效，一但设置了，timeout将不起作用。
      overflowToDisk:是否保存到磁盘，当系统当机时
      timeToIdleSeconds:设置对象在失效前的允许闲置时间（单位：秒）。仅当eternal=false对象不是永久有效时使用，可选属性，默认值是0，也就是可闲置时间无穷大。
      timeToLiveSeconds:设置对象在失效前允许存活时间（单位：秒）。最大时间介于创建时间和失效时间之间。仅当eternal=false对象不是永久有效时使用，默认是0.，也就是对象存活时间无穷大。
      diskPersistent：是否缓存虚拟机重启期数据 Whether the disk store persists between restarts of the Virtual Machine. The default value is false.
      diskSpoolBufferSizeMB：这个参数设置DiskStore（磁盘缓存）的缓存区大小。默认是30MB。每个Cache都应该有自己的一个缓冲区。
      diskExpiryThreadIntervalSeconds：磁盘失效线程运行时间间隔，默认是120秒。
      memoryStoreEvictionPolicy：当达到maxElementsInMemory限制时，Ehcache将会根据指定的策略去清理内存。默认策略是LRU（最近最少使用）。你可以设置为FIFO（先进先出）或是LFU（较少使用）。
      clearOnFlush：内存数量最大时是否清除。
      memoryStoreEvictionPolicy:可选策略有：LRU（最近最少使用，默认策略）、FIFO（先进先出）、LFU（最少访问次数）。
      FIFO，first in first out，这个是大家最熟的，先进先出。
      LFU， Less Frequently Used，就是上面例子中使用的策略，直白一点就是讲一直以来最少被使用的。如上面所讲，缓存的元素有一个hit属性，hit值最小的将会被清出缓存。
      LRU，Least Recently Used，最近最少使用的，缓存的元素有一个时间戳，当缓存容量满了，而又需要腾出地方来缓存新的元素的时候，那么现有缓存元素中时间戳离当前时间最远的元素将被清出缓存。
   -->
    <defaultCache
            eternal="false"
            maxElementsInMemory="10000"
            overflowToDisk="false"
            diskPersistent="false"
            timeToIdleSeconds="1800"
            timeToLiveSeconds="259200"
            memoryStoreEvictionPolicy="LRU"/>

    <cache
            name="cloud_user"
            eternal="false"
            maxElementsInMemory="5000"
            overflowToDisk="false"
            diskPersistent="false"
            timeToIdleSeconds="1800"
            timeToLiveSeconds="1800"
            memoryStoreEvictionPolicy="LRU"/>
</ehcache>
Spring
1、基本介绍

(1)spring框架,整合其他框架的框架,核心为IOC和AOP
(2)spring框架由20多个模块组成,在很多领域都提供优秀的解决方案
(3)spring springMVC springboot springcloud
核心容器
IoC/DI
1、问题分析

public interface BookService {
    void save();
}
public class BookServiceImplement implements BookService {
    BookDao bookDao = new BookDaoImplement();
    @Override
    public void save() {
        bookDao.save();
    }
}
public interface BookDao {
    void save();
}
public class BookDaoImplement implements BookDao {
    @Override
    public void save() {
        System.out.println("book dao save");
    }
}
(1)耦合度偏高
    解决方案:使用对象时,在程序中不主动使用new关键字创建对象实例,转换为由外部提供对象
2、IoC（Inversion of Control）控制反转

使用对象时,由主动new创建对象转换为由外部提供对象,创建对象的控制权由程序转移到外部,即控制反转
3、Spring技术实现IoC思想

(1)Spring提供了一个容器,称为IoC容器,IoC容器用于充当IoC思想中的"外部"
(2)IoC容器负责创建对象、初始化等一系列工作,被创建或被管理的对象在IoC容器中统称为Bean
4、DI（Dependency Injection）依赖注入

(1)在容器中建立bean与bean之间的依赖关系的整个过程称为依赖注入
5、充分解耦

(1)使用IoC容器管理bean(IoC-控制反转)
(2)在IoC容器内将存在依赖关系的bean进行关系绑定(DI-依赖注入)
6、最终效果

使用的对象不仅可直接从IoC容器中获取,而且获取到的bean已经绑定了所有的依赖关系
7、IoC入门案例思路分析

(1)管理什么?bean
(2)如何将被管理的对象告知IoC容器?配置
(3)被管理的对象交给IoC容器,如何获取IoC容器?接口
(4)得到IoC容器后如何从容器中获取bean?接口方法
(5)使用Spring导入哪些坐标?pom.xml
8、IoC入门案例

(1)导入依赖包
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
    <version>5.2.10.RELEASE</version>
</dependency>
    
(2)配置文件多行注释(Ctrl+Shift+/) 配置文件单行注释(Ctrl+/)
    
(3)src/main/resources资源文件目录下新建配置文件XML Configuration File -> Spring Config
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!-- 1.导入spring依赖spring-context,对应版本是5.2.10.RELEASE -->
    <!-- 2.配置bean
    bean标签表示配置bean
    id表示为bean起名
    class表示为bean定义类型-->
    <bean id="bookServiceImplement" class="service.implement.BookServiceImplement"/>
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement"/>
</beans>
        
(4)
public class App2 {
    public static void main(String[] args) {
        //3.获取IoC容器
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        //4.获取bean,得到Object类型对象,向下转型
        BookDao bookDao = (BookDao) applicationContext.getBean("bookDao");
        bookDao.save();
        BookService bookService = (BookService) applicationContext.getBean("bookService");
        bookService.save();
    }
}
9、总结

(1)导入Spring依赖包
(2)创建Spring配置文件applicationContext,配置bean
(3)通过配置文件初始化IoC容器,通过容器获取bean
	ApplicationContext applicationContext = new ClassPathXmlApplicationContext(配置文件路径)
10、DI入门案例思路分析

(1)基于IoC管理bean
(2)Service中使用new形式创建的Dao对象是否保留?(存在耦合,不保留)
(3)Service中需要Dao对象如何进入Service中?(提供方法)
(4)Service与Dao之间的关系如何描述?(配置)
11、DI入门案例

public class BookServiceImplement implements BookService {
    //5.删除业务逻辑层中使用new方式创建的dao对象
    private BookDao bookDao;

    //6.提供对应的set方法
    public void setBookDao(BookDao bookDao) {
        this.bookDao = bookDao;
    }

    public void save() {
        System.out.println("book service save");
        bookDao.save();
    }
}
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!-- 1.导入spring的坐标spring-context,对应版本是5.2.10.RELEASE -->

    <!-- 2.配置bean
    bean标签表示配置bean
    id表示为bean起名
    class表示为bean定义类型-->
    <bean id="bookServiceImplement" class="service.implement.BookServiceImplement">
        <!--7.配置Service和Dao的关系-->
        <!--
        property标签表示配置当前bean的属性
        name标签表示一个具体的属性名
        ref标签表示参照哪一个bean
        BookServiceImplement中属性bookDao参照bean id="bookDaoImplement"-->
        <property name="bookDao" ref="bookDaoImplement"/>
    </bean>
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement"/>
</beans>
12、总结

(1)删除使用new的形式创建对象的代码
(2)提供依赖对象对应的set()方法
(3)配置文件中配置service和dao之间的关系
bean配置
1、bean基础配置

(1)名称:bean
(2)类型:标签
(3)所属:beans
(4)功能:定义Spring核心容器管理的对象
(5)格式:
<beans>
    <bean/>
    <bean></bean>
</beans>
(6)属性列表:
	id:bean的id,使用容器可以通过id值获取对应的bean,在一个容器中id唯一
	class:bean的类型,配置bean的全路径类名
(7)范例:
<bean id="bookServiceImplement" class="service.implement.BookServiceImplement"/>
<bean id="bookDaoImplement" class="dao.implement.BookDaoImplement"/>
2、bean别名配置

(1)名称:name
(2)类型:属性
(3)所属:bean标签
(4)功能:定义bean的别名,可定义多个别名,使用逗号,分号,空格分隔
(5)范例:
<bean id="bookDaoImplement" name="bookDaoEnterpriseBusinessInterface" class="dao.implement.BookDaoImplement"/>
(6)注意事项:
无名为bookDaoEnterpriseBusinessInterface1的bean可用
NoSuchBeanDefinitionException: No bean named 'bookDaoEnterpriseBusinessInterface1' available
注:定义bean时输入的id或name和获取bean时输入的id或name不一致
3、bean别名配置测试

<bean id="bookDaoImplement" name="bookDaoEnterpriseBusinessInterface" class="dao.implement.BookDaoImplement"/>
public class App2 {
    public static void main(String[] args) {
        //3.获取IoC容器
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        //4.获取bean,得到Object类型对象,向下转型
        BookDao bookDao = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        bookDao.save();
    }
}
4、bean作用范围配置

(1)名称:scope
(2)类型:属性
(3)所属:bean标签
(4)功能:
定义bean的作用范围
	singleton:单例(默认)
	prototype:非单例
(5)范例:
<bean id="bookDaoImplement" name="bookDaoEnterpriseBusinessInterface" class="dao.implement.BookDaoImplement" scope="prototype"/>
5、bean作用范围为prototype测试

<bean id="bookDaoImplement" name="bookDaoEnterpriseBusinessInterface" class="dao.implement.BookDaoImplement" scope="prototype"/>
public class App2 {
    public static void main(String[] args) {
        //3.获取IoC容器
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        //4.获取bean,得到Object类型对象,向下转型
        BookDao bookDao1 = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        BookDao bookDao2 = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        System.out.println(bookDao1);
        System.out.println(bookDao2);
    }
}

/*
输出结果:
dao.implement.BookDaoImplement@25bbe1b6
dao.implement.BookDaoImplement@5702b3b1
*/
6、bean作用范围为默认测试

<bean id="bookDaoImplement" name="bookDaoEnterpriseBusinessInterface" class="dao.implement.BookDaoImplement"/>
public class App2 {
    public static void main(String[] args) {
        //3.获取IoC容器
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        //4.获取bean,得到Object类型对象,向下转型
        BookDao bookDao1 = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        BookDao bookDao2 = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        System.out.println(bookDao1);
        System.out.println(bookDao2);
    }
}

/*
输出结果:
dao.implement.BookDaoImplement@25bbe1b6
dao.implement.BookDaoImplement@25bbe1b6
*/
7、bean作用范围说明

(1)适合交给容器进行管理的bean
	表现层对象(controller)
	业务层对象(service)
	数据层对象(dao)
	工具类对象(util)
(2)不合适交给容器进行管理的bean
	domain实体类对象实例
bean实例化
实例化bean的三种方式—无参构造方法
1、接口实现类

public class BookDaoImplement implements BookDao {

    private BookDaoImplement() {
        System.out.println("book dao constructor is running");
    }

    @Override
    public void save() {
        System.out.println("book dao save");
    }
}
2、测试

public class App2 {
    public static void main(String[] args) {
        //获取IoC容器
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        //获取bean,得到Object类型对象,向下转型
        BookDao bookDao = (BookDao) applicationContext.getBean("bookDaoEnterpriseBusinessInterface");
        System.out.println(bookDao);
    }
}

/*
输出结果:
book dao constructor is running
dao.implement.BookDaoImplement@25bbe1b6
*/
3、注意事项

(1)若无参构造方法不存在,将抛出异常.BeanInstantiationException
Caused by: java.lang.NoSuchMethodException: dao.implement.BookDaoImplement.<init>()

Caused by: org.springframework.beans.BeanInstantiationException: Failed to instantiate [dao.implement.BookDaoImplement]: No default constructor found; nested exception is java.lang.NoSuchMethodException: dao.implement.BookDaoImplement.<init>()

Caused by: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'bookDaoImplement' defined in class path resource [applicationContext.xml]: Instantiation of bean failed; nested exception is org.springframework.beans.BeanInstantiationException: Failed to instantiate [dao.implement.BookDaoImplement]: No default constructor found; nested exception is java.lang.NoSuchMethodException: dao.implement.BookDaoImplement.<init>()
实例化bean的三种方式—静态工厂
1、接口

public interface OrderDao {
    void save();
}
2、接口实现类

public class OrderDaoImplement implements OrderDao {
    @Override
    public void save() {
        System.out.println("order dao save");
    }
}
3、静态工厂

public class OrderDaoFactory {
    public static OrderDao getOrderDao() {
        return new OrderDaoImplement();
    }
}
4、配置

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="orderDaoImplement" class="factory.OrderDaoFactory" factory-method="getOrderDao"/>
</beans>
5、测试

public class AppForInstanceOrder {
    public static void main(String[] args) {
        //通过静态工厂创建对象
        //OrderDao orderDao = OrderDaoFactory.getOrderDao();
        //orderDao.save();
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        OrderDao orderDao = (OrderDao) applicationContext.getBean("orderDaoImplement");
        orderDao.save();
    }
}
实例化bean的三种方式—实例工厂
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
3、实例工厂

public class UserDaoFactory {
    public UserDao getUserDao() {
        return new UserDaoImplement();
    }
}
4、配置

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="userDaoFactory" class="factory.UserDaoFactory"/>
    <!--
    factory-bean:指定工厂方法所在的工厂类实例(即工厂方法bean的id,用法与ref类似)
    factory-method:还是指定工厂方法名
    -->
    <bean id="userDaoImplement" factory-bean="userDaoFactory" factory-method="getUserDao"/>
</beans>
5、测试

public class AppForInstanceUser {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoImplement");
        userDao.save();
    }
}
实例化bean的最重要方式—FactoryBean
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
3、工厂

public class UserDaoFactoryBean implements FactoryBean<UserDao> {
    //使用FactoryBean创建Bean
    @Override
    public UserDao getObject() throws Exception {
        return new UserDaoImplement();
    }

    //创建Bean的数据类型为UserDao
    @Override
    public Class<?> getObjectType() {
        return UserDao.class;
    }

    //单例、非单例
    @Override
    public boolean isSingleton() {
        return false;
    }
}
4、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="userDaoImplement" class="factory.UserDaoFactoryBean"/>
</beans>
5、测试

public class AppForInstanceUser {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoImplement");
        userDao.save();
    }
}
bean生命周期
配置控制
1、基本介绍

生命周期:从创建到消亡的完整过程
bean生命周期:bean从创建到消亡的完整过程
bean生命周期控制:在bean创建后到消亡前执行的操作
2、接口

public interface UserDao {
    void save();
}
3、接口实现类

public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("蒋兴树");
    }
}
4、工厂

public class UserDaoFactoryBean implements FactoryBean<UserDao> {
    @Override
    public UserDao getObject() throws Exception {
        return new UserDaoImplement();
    }

    @Override
    public Class<?> getObjectType() {
        return UserDao.class;
    }

    @Override
    public boolean isSingleton() {
        return true;
    }


    public void init() {
        System.out.println("初始化");
    }

    public void destory() {
        System.out.println("消亡");
    }
}
5、配置

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
    <!--
    IoC容器中管理的bean的id
    IoC容器中管理的bean的别名
    初始化方法:init-method
    消亡方法:destroy-method
    -->
    <bean class="factory.UserDaoFactoryBean"
          id="userDaoFactoryBean"
          init-method="init"
          destroy-method="destory"/>
</beans>
6、测试

public class UserDaoTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoFactoryBean");
        userDao.save();
    }
}
接口控制
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("蒋兴树");
    }
}
3、工厂

/**
 * FactoryBean:Bean工厂
 * InitializingBean:初始化Bean接口
 * DisposableBean:消亡Bean接口
 */
public class UserDaoFactoryBean implements FactoryBean<UserDao>, InitializingBean, DisposableBean {
    @Override
    public UserDao getObject() throws Exception {
        return new UserDaoImplement();
    }

    @Override
    public Class<?> getObjectType() {
        return UserDao.class;
    }

    @Override
    public boolean isSingleton() {
        return true;
    }

    @Override
    public void destroy() throws Exception {
        System.out.println("消亡");
    }

    @Override
    public void afterPropertiesSet() throws Exception {
        System.out.println("初始化");
    }
}
4、配置

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
    <!--
    IoC容器中管理的bean的id
    IoC容器中管理的bean的别名
    初始化方法:init-method
    消亡方法:destroy-method
    -->
    <bean class="factory.UserDaoFactoryBean"
          id="userDaoFactoryBean"/>
</beans>
5、测试

public class UserDaoTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("applicationContext.xml");
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoFactoryBean");
        userDao.save();

        //IoC容器关闭时bean消亡
        ClassPathXmlApplicationContext classPathXmlApplicationContext
                = (ClassPathXmlApplicationContext) applicationContext;
        classPathXmlApplicationContext.close();
    }
}
bean生命周期经历阶段
(1)初始化容器
	执行构造器方法,创建bean对象实例
	执行属性注入
	执行bean初始化方法
(2)使用bean
	执行业务操作
(3)关闭容器
	执行bean消亡方法
bean销毁时机
(1)IoC容器关闭前触发bean的消亡
(2)关闭容器方式:
	手动关闭容器:ConfigurableApplicationContext接口close()方法
	注册关闭钩子:ConfigurableApplicationContext接口registerShutdownHook()方法
依赖注入方式
1、向一个类中传递数据的方式

(1)set()方法
(2)构造方法
2、依赖注入描述了容器中建立bean与bean之间依赖关系的过程，若bean运行所需的为数据或字符串

(1)引用类型
(2)普通类型(基本数据类型、String)
3、依赖注入方式

(1)setter注入
	简单类型
	引用类型
(2)构造器注入
	简单类型
	引用类型
setter注入
1、接口

public interface BookDao {
    void save();
}
public interface UserDao {
    void save();
}
2、依赖接口

public interface UserService {
    void save();
}
3、接口实现类

public class BookDaoImplement implements BookDao {
    private int connectionNum;
    private String databaseName;

    public void setConnectionNum(int connectionNum) {
        this.connectionNum = connectionNum;
    }

    public void setDatabaseName(String databaseName) {
        this.databaseName = databaseName;
    }

    @Override
    public void save() {
        System.out.println("book dao save" + connectionNum + databaseName);
    }
}
public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
4、依赖接口实现类

public class UserServiceImplement implements UserService {
    private UserDao userDao;
    private BookDao bookDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    public void setBookDao(BookDao bookDao) {
        this.bookDao = bookDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
        bookDao.save();
    }
}
5、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="userServiceImplement" class="service.implement.UserServiceImplement">
        <property name="userDao" ref="userDaoImplement"/>
        <property name="bookDao" ref="bookDaoImplement"/>
    </bean>

    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement"/>
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement">
        <property name="connectionNum" value="1"/>
        <property name="databaseName" value="my_database"/>
    </bean>
</beans>
6、测试

public class UserServiceTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("spring-config.xml");
        UserService userService = (UserService) applicationContext.getBean("userServiceImplement");
        userService.save();
    }
}
构造器注入
1、接口

public interface BookDao {
    void save();
}
public interface UserDao {
    void save();
}
2、依赖接口

public interface UserService {
    void save();
}
3、接口实现类

public class BookDaoImplement implements BookDao {
    private int connectionNum;
    private String databaseName;

    public BookDaoImplement(int connectionNum, String databaseName) {
        this.connectionNum = connectionNum;
        this.databaseName = databaseName;
    }

    @Override
    public void save() {
        System.out.println("book dao save" + connectionNum + databaseName);
    }
}
public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
4、依赖接口实现类

public class UserServiceImplement implements UserService {
    private UserDao userDao;
    private BookDao bookDao;

    public UserServiceImplement(UserDao userDao, BookDao bookDao) {
        this.userDao = userDao;
        this.bookDao = bookDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
        bookDao.save();
    }
}
5、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!--标准写法-->
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement">
        <!--
        name标签为BookDaoImplement中构造器中的形参名
        若构造器中的形参名修改,name标签也需修改,耦合度高
        -->
        <constructor-arg name="connectionNum" value="10"/>
        <constructor-arg name="databaseName" value="my_database"/>
    </bean>
    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement"/>
    
    <bean id="userServiceImplement" class="service.implement.UserServiceImplement">
        <constructor-arg name="bookDao" ref="bookDaoImplement"/>
        <constructor-arg name="userDao" ref="userDaoImplement"/>
    </bean>
</beans>
6、测试

public class UserServiceTest {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext classPathXmlApplicationContext = new ClassPathXmlApplicationContext("spring-02.xml");
        UserService userService = (UserService)classPathXmlApplicationContext.getBean("userServiceImplement");
        userService.save();
    }
}
7、配置文件优化

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!--解决name标签与构造器中形参名耦合度过高问题-->
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement">
        <constructor-arg type="int" value="10"/>
        <constructor-arg type="java.lang.String" value="my_database"/>
    </bean>
    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement"/>

    <bean id="userServiceImplement" class="service.implement.UserServiceImplement">
        <constructor-arg name="bookDao" ref="bookDaoImplement"/>
        <constructor-arg name="userDao" ref="userDaoImplement"/>
    </bean>
</beans>
8、配置文件再优化

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!--解决参数类型重复问题,使用索引位置解决参数匹配-->
    <bean id="bookDaoImplement" class="dao.implement.BookDaoImplement">
        <constructor-arg index="0" value="10"/>
        <constructor-arg index="1" value="my_database"/>
    </bean>
    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement"/>

    <bean id="userServiceImplement" class="service.implement.UserServiceImplement">
        <constructor-arg name="bookDao" ref="bookDaoImplement"/>
        <constructor-arg name="userDao" ref="userDaoImplement"/>
    </bean>
</beans>
9、依赖注入方式选择

(1)强制依赖使用构造器注入,使用setter注入有概率不进行注入,导致null对象出现
(2)可选依赖使用setter注入,灵活性强
(3)Spring框架倡导使用构造器注入,第三方框架内部大多数采用构造器注入的形式进行数据的初始化，相对严谨。
(4)若有必要可以同时使用两种注入,使用构造器注入完成强制依赖注入,使用setter注入完成可选依赖注入。
(5)实际开发过程中根据实际情况分析,若受控对象没有提供setter方法就必须使用构造器注入
(6)自己开发的模块推荐使用setter注入
依赖自动装配
1、基本介绍

IoC容器根据bean所依赖的资源在容器中自动查找并注入到bean中的过程称为自动装配
2、自动装配方式

(1)按类型
(2)按名称
(3)按构造方法
3、接口

public interface UserDao {
    void save();
}
4、接口实现类

public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
5、依赖接口

public interface UserService {
    void save();
}
6、依赖接口实现类

public class UserServiceImplement implements UserService {
    private UserDao userDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
    }
}
7、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement"/>

    <!--autowire:按类型进行依赖自动装配-->
    <bean id="userServiceImplement" class="service.implement.UserServiceImplement" autowire="byType"/>
</beans>
8、测试

public class UserServiceTest {
    public static void main(String[] args) {
        ClassPathXmlApplicationContext classPathXmlApplicationContext = new ClassPathXmlApplicationContext("spring-03.xml");
        UserService userService = (UserService)classPathXmlApplicationContext.getBean("userServiceImplement");
        userService.save();
    }
}
9、依赖自动装配特征

(1)自动装配用于引用类型依赖注入,不可对简单类型进行操作
(2)使用按类型进行依赖自动装配时必须保障容器中相同类型的bean唯一,推荐使用
(3)使用按名称进行依赖自动装配时必须保障容器中具有指定名称的bean,变量名和配置耦合,不推荐使用
(4)自动装配优先级低于setter注入与构造器注入,同时出现时自动装配失效
集合注入
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

public class UserDaoImplement implements UserDao {
    private int[] array;
    private List<String> list;
    private Set<String> set;
    private Map<String,String> map;
    private Properties properties;

    public void setArray(int[] array) {
        this.array = array;
    }
    public void setList(List<String> list) {
        this.list = list;
    }
    public void setSet(Set<String> set) {
        this.set = set;
    }
    public void setMap(Map<String, String> map) {
        this.map = map;
    }
    public void setProperties(Properties properties) {
        this.properties = properties;
    }

    @Override
    public void save() {
        System.out.println("user dao save");
        System.out.println(Arrays.toString(array));
        System.out.println(list);
        System.out.println(set);
        System.out.println(map);
        System.out.println(properties);
    }
}
3、依赖接口

public interface UserService {
    void save();
}
4、依赖接口实现类

public class UserServiceImplement implements UserService {
    private UserDao userDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
    }
}
5、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <bean id="userDaoImplement" class="dao.implement.UserDaoImplement">
        <property name="array">
            <array>
                <value>1</value>
                <value>2</value>
                <value>3</value>
            </array>
        </property>

        <property name="list">
            <list>
                <value>jxs</value>
                <value>dwy</value>
                <value>jxs</value>
                <value>dwy</value>
            </list>
        </property>

        <property name="set">
            <set>
                <value>jxs</value>
                <value>jxs</value>
                <value>dwy</value>
                <value>dwy</value>
            </set>
        </property>

        <property name="map">
            <map>
                <entry key="1" value="jxs"/>
                <entry key="2" value="dwy"/>
            </map>
        </property>

        <property name="properties">
            <props>
                <prop key="1">jxs</prop>
                <prop key="2">dwy</prop>
            </props>
        </property>
    </bean>

    <bean id="userServiceImplement" class="service.implement.UserServiceImplement">
        <property name="userDao" ref="userDaoImplement"/>
    </bean>
</beans>
6、测试

public class UserServiceTest {
    public static void main(String[] args) {
        //获取IoC容器,向上转型
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("spring-04.xml");
        //获取IoC容器中管理的bean对象,向下转型
        UserService userService = (UserService) applicationContext.getBean("userServiceImplement");
        userService.save();
    }
}

/*
输出结果:
user service save
user dao save
[1, 2, 3]
[jxs, dwy, jxs, dwy]
[jxs, dwy]
{1=jxs, 2=dwy}
{2=dwy, 1=jxs}
*/
数据源对象管理
第三方数据源对象配置管理
1、导入依赖

<dependency>
    <groupId>com.alibaba</groupId>
    <artifactId>druid</artifactId>
    <version>1.2.15</version>
</dependency>
2、配置bean

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">

    <!--德鲁伊连接池-->
    <bean id="druidDataSource" class="com.alibaba.druid.pool.DruidDataSource">
        <!--数据库驱动-->
        <property name="driverClassName" value="com.mysql.cj.jdbc.Driver"/>
        <property name="url" value="jdbc:mysql://localhost:3306/spring"/>
        <property name="username" value="root"/>
        <property name="password" value="123456"/>
        <!--
        初始化连接数
        最小空闲数
        最大连接数
        获取连接时最大等待时间
        -->
        <property name="initialSize" value="10"/>
        <property name="minIdle" value="5"/>
        <property name="maxActive" value="10"/>
        <property name="maxWait" value="3000"/>
    </bean>
</beans>
加载Properties文件
1、配置文件

driver=com.mysql.cj.jdbc.Driver
url=jdbc:mysql://localhost:3306/spring
username=root
password=123456
2、开启名为context的xmlns命名空间

![](E:\Study\自学课程资料\Java\assets\开启名为context的xmlns命名空间.png)

3、使用context命名空间加载properties文件

<!--
database.properties配置文件中存在属性username
windows系统变量中的username和database.properties中属性username冲突
优先读取windows系统变量中的username
system-properties-mode="NEVER":不加载系统属性
-->
<context:property-placeholder location="database.properties" system-properties-mode="NEVER"/>
4、使用${}占位符读取properties文件中的属性

<bean id="druidDataSource" class="com.alibaba.druid.pool.DruidDataSource">
    <property name="driverClassName" value="${driver}"/>
    <property name="url" value="${url}"/>
    <property name="username" value="${username}"/>
    <property name="password" value="${password}"/>
</bean>
5、加载多个properties文件

<context:property-placeholder location="database.properties,database01.properties"/>
6、加载所有properties文件

<context:property-placeholder location="*.properties"/>
7、加载properties文件标准格式

<context:property-placeholder location="classpath:*.properties"/>
8、从类路径或jar包中搜索并加载properties文件

<context:property-placeholder location="classpath*:*.properties"/>
容器
创建容器
public class DruidTest {
    public static void main(String[] args) {
        //创建容器方式一:加载类路径下的配置文件
        ApplicationContext applicationContext1 = new ClassPathXmlApplicationContext("spring-05.xml");
        DataSource dataSource1 = (DataSource) applicationContext1.getBean("druidDataSource");
        System.out.println(dataSource1);

        //创建容器方式二:文件路径下加载配置文件
        String srcPath = "E:\\Software Development Kit\\Maven\\workspace\\Spring\\spring-05\\src\\main\\resources\\spring-05.xml";
        ApplicationContext applicationContext2 = new FileSystemXmlApplicationContext(srcPath);
        DataSource dataSource2 = applicationContext2.getBean("druidDataSource",DataSource.class);
        System.out.println(dataSource2);
        //IoC容器获取管理的bean对象时形参列表中指定数据类型后无需向下转型

        //加载多个配置文件
        //创建容器方式一:加载类路径下的配置文件
        ApplicationContext applicationContext3 = new ClassPathXmlApplicationContext("spring-05.xml","spring-06.xml");
    }
}
获取bean
public class DruidTest {
    public static void main(String[] args) {
        //创建IoC容器
        ApplicationContext applicationContext1 = new ClassPathXmlApplicationContext("spring-05.xml");
        //获取bean方式一:使用bean的id获取
        DataSource dataSource1 = (DataSource) applicationContext1.getBean("druidDataSource");
        //获取bean方式二:使用bean的id以及指定数据类型获取
        DataSource dataSource2 = applicationContext1.getBean("druidDataSource", DataSource.class);
        //获取bean方式三:使用bean类型获取
        DataSource dataSource3 = applicationContext1.getBean(DataSource.class);
        System.out.println(dataSource1);
        System.out.println(dataSource2);
        System.out.println(dataSource3);
    }
}
容器类层次结构
![](E:\Study\自学课程资料\Java\assets\容器类层次结构.png)

BeanFactory初始化
1、类路径加载配置文件

public class DruidTest {
    public static void main(String[] args) {
        Resource resource = new ClassPathResource("spring-05.xml");
        BeanFactory beanFactory = new XmlBeanFactory(resource);
        UserDao userDao = beanFactory.getBean("userDaoImplement", UserDao.class);
        userDao.save();
    }
}
2、BeanFactory创建完毕后所有的bean均为延迟加载

核心容器总结
1、容器相关

(1)BeanFactory接口:IoC容器顶层接口,初始化BeanFactory对象时,加载的bean延迟加载
(2)ApplicationContext接口:Spring容器核心接口,初始化bean立即加载
(3)ApplicationContext接口:提供基础的bean操作相关方法,通过其他接口扩展功能
(4)ApplicationContext接口常用初始化类:ClassPathXmlApplicationContext、FileSystemXmlApplicationContext
2、bean相关

<bean
    <!--bean的id-->
    id="userDao"
    
    <!--bean的别名-->
    name="userDaoEnterpriseBusinessInterface"
    
    <!--bean的数据类型-->
    class="dao.implement.UserDaoImplement"
    
    <!--控制bean为单例/非单例-->
    scope="singleton"
    
    <!--生命周期初始化方法-->
    init-method="init"
    
    <!--生命周期消亡方法-->
    destroy-method="destroy"
    
    <!--自动装配类型-->
    autowire="byType"
    
    <!--bean工厂方法-->
    factory-method="getInstance"
    
    <!--实例工厂bean-->
    factory-bean="factory.UserDaoFactory"
    
    <!--控制bean延迟加载-->
    lazy-init="true"
    />
注解
注解开发bean
注解开发定义bean
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

@Component("userDaoImplement")
public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
3、依赖接口

public interface UserService {
    void save();
}
4、依赖接口实现类

@Component("userServiceImplement")
public class UserServiceImplement implements UserService {
    private UserDao userDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
    }
}
5、配置文件

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="
       http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context.xsd
       ">

    <!--组件扫描-->
    <context:component-scan base-package="dao.implement"/>
    <context:component-scan base-package="service.implement"/>

</beans>
6、测试

public class UserServiceTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("spring-06.xml");
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoImplement");
        UserService userService  = (UserService) applicationContext.getBean("userServiceImplement");
        System.out.println(userDao);
        System.out.println(userService);
    }
}
@Component注解衍生注解
1、基本介绍

(1)@Controller:表现层bean定义
(2)@Service:业务层bean定义
(3)@Repository:数据层bean定义
2、案例演示

@Repository("userDaoImplement")
public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
@Service("userServiceImplement")
public class UserServiceImplement implements UserService {
    private UserDao userDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
    }
}
纯注解开发bean
1、基本介绍

(1)Spring3.0开启纯注解开发模式,使用Java的配置类替代配置文件,开启Spring快速开发通道
2、Java的配置类替代配置文件

/**
 * @Configuration 此注解用于设定当前类为配置类
 * @ComponentScan 此注解用于设定扫描路径,此注解只可添加1次,多个数据采用数组格式
 */
@Configuration
@ComponentScan({"dao.implement","service.implement"})
public class SpringConfig {
}
3、测试

/**
 * Annotation 注解
 * Config 配置
 * Application 应用
 * Context 上下文
 */
public class UserServiceTest {
    public static void main(String[] args) {
        //读取Spring核心配置文件初始化容器对象切换为读取Java配置类初始化容器对象
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        UserDao userDao = (UserDao) applicationContext.getBean("userDaoImplement");
        UserService userService = (UserService) applicationContext.getBean("userServiceImplement");
        System.out.println(userDao);
        System.out.println(userService);
    }
}
注解开发bean作用范围、生命周期
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

@Repository("userDaoImplement")
public class UserDaoImplement implements UserDao {
    @Override
    public void save() {
        System.out.println("user dao save");
    }
}
3、依赖接口

public interface UserService {
    void save();
}
4、依赖接口实现类

/**
 * @Service 使用注解定义bean
 * @Scope 使用注解定义单例/非单例
 * @PostConstruct 生命周期初始化
 * @PreDestroy 生命周期消亡
 */
@Service("userServiceImplement")
@Scope("singleton")
public class UserServiceImplement implements UserService {
    @Override
    public void save() {
        System.out.println("user service save");
    }

    @PostConstruct
    public void init() {
        System.out.println("init");
    }

    @PreDestroy
    public void destroy() {
        System.out.println("destroy");
    }
}
5、配置类

@Configuration
@ComponentScan({"dao.implement","service.implement"})
public class SpringConfig {
}
6、测试类

public class UserServiceTest {
    public static void main(String[] args) {
        AnnotationConfigApplicationContext annotationConfigApplicationContext= new AnnotationConfigApplicationContext(SpringConfig.class);
        UserDao userDao = (UserDao) annotationConfigApplicationContext.getBean("userDaoImplement");
        UserService userService = (UserService) annotationConfigApplicationContext.getBean("userServiceImplement");
        System.out.println(userDao);
        System.out.println(userService);
        annotationConfigApplicationContext.close();
    }
}
7、@Scope注解：定义IoC容器管理的bean对象为单例/非单例

@Service("userServiceImplement")
@Scope("singleton")
public class UserServiceImplement implements UserService {
    @Override
    public void save() {
        System.out.println("user service save");
    }
}
8、@PostConstruct、@PreDestroy定义IoC容器管理的bean对象生命周期的初始化、消亡

@Service("userServiceImplement")
@Scope("singleton")
public class UserServiceImplement implements UserService {
    @Override
    public void save() {
        System.out.println("user service save");
    }

    @PostConstruct
    public void init() {
        System.out.println("init");
    }

    @PreDestroy
    public void destroy() {
        System.out.println("destroy");
    }
}
注解开发依赖注入
1、接口

public interface UserDao {
    void save();
}
2、接口实现类

@Repository("userDaoImplement")
public class UserDaoImplement implements UserDao {
    /*
    @Value 实现外部配置文件中简单数据类型的注入
    */
    @Value("${name}")
    private String name;

    @Override
    public void save() {
        System.out.println("user dao save" + name);
    }
}
3、依赖接口

public interface UserService {
    void save();
}
4、依赖接口实现类

@Service("userServiceImplement")
public class UserServiceImplement implements UserService {
    /*
    @Autowired 自动注入指定数据类型依赖bean
    @Qualifier 自动注入指定id依赖bean,@Qualifier依赖@Autowired
    */
    @Autowired
    @Qualifier("userDaoImplement")
    private UserDao userDao;

    public void setUserDao(UserDao userDao) {
        this.userDao = userDao;
    }

    @Override
    public void save() {
        System.out.println("user service save");
        userDao.save();
    }
}
5、配置类

@Configuration
@ComponentScan({"dao.implement","service.implement"})
//PropertySource 加载外部配置文件
@PropertySource("name.properties")
public class SpringConfig {
}
6、测试类

public class UserServiceTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        UserService userService = (UserService) applicationContext.getBean("userServiceImplement");
        userService.save();
    }
}
7、总结

(1)使用@Autowired注解开启按类型自动装配模式。
(2)自动装配基于反射创建对象实例并反射爆破私有属性进行初始化数据,因此无需提供setter方法。
(3)自动装配建议使用无参构造方法创建对象实例,若不提供对应构造方法,则提供唯一的构造方法。
(4)使用@Qualifier注解开启指定名称装配bean。@Qualifier注解无法单独使用,必须配合@Autowired注解使用
(5)使用@PropertiesSource注解加载properties文件,加载多个外部配置文件使用数组格式
注解开发管理第三方bean
1、JDBC配置类

public class JdbcConfig {
    //1.定义方法获取管理对象,将方法返回值定义为bean
    @Bean()
    public DataSource dataSource() {
        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName("com.mysql.cj.jdbc.Driver");
        druidDataSource.setUrl("jdbc:mysql://localhost:3306/spring");
        druidDataSource.setName("root");
        druidDataSource.setPassword("123456");
        return druidDataSource;
    }
}
2、Spring配置类

@Configuration
//@Import 导入配置类
@Import(JdbcConfig.class)
public class SpringConfig {
}
3、测试类

public class DruidTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        DataSource bean = applicationContext.getBean(DataSource.class);
        System.out.println(bean);
    }
}
4、总结

(1)@Import注解手动加入配置类到核心配置类中,此注解只可添加一次,多个配置类使用数组格式添加。
注解开发管理第三方bean注入资源
1、JDBC配置类

public class JdbcConfig {
    @Value("com.mysql.cj.jdbc.Driver")
    private String driverClassName;
    @Value("jdbc:mysql://localhost:3306/spring")
    private String url;
    @Value("root")
    private String name;
    @Value("123456")
    private String password;

    //1.定义方法获取管理对象,将方法返回值定义为bean
    @Bean()
    public DataSource dataSource(BookDao bookDao) {
        System.out.println(bookDao);

        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName(driverClassName);
        druidDataSource.setUrl(url);
        druidDataSource.setName(name);
        druidDataSource.setPassword(password);
        return druidDataSource;
    }
}
2、资源类

public interface BookDao {
    void save();
}


@Repository("bookDaoImplement")
public class BookDaoImplement implements BookDao {
    @Override
    public void save() {
        System.out.println("book dao save");
    }
}
3、Spring配置类

@Configuration
//@Import 导入配置类
@Import(JdbcConfig.class)
@ComponentScan("dao.implement")
public class SpringConfig {
}
4、测试类

public class DruidTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        DataSource bean = applicationContext.getBean(DataSource.class);
        System.out.println(bean);
    }
}
5、总结

(1)引用类型注入只需为bean定义方法设置形参即可,容器会根据类型自动装配对象。
注解开发总结
1、XML配置与注解配置对比

功能	XML配置	注解
定义bean	bean标签（id属性、class属性）	@Component（@Controller、@Service、@Repository）、@ComponentScan
设置依赖注入	setter注入、构造器注入	@Autowired（@Qualifier）、@Value
配置第三方bean	bean标签（静态工厂、实例工厂、FactoryBean）	@Bean
作用范围	scope属性	@Scope
生命周期	标准接口（init-method、destroy-method）	@PostConstructor、@PreDestroy
整合
Spring整合MyBatis（重要！！）
MyBatis基础框架
1、创建数据库

CREATE TABLE account(
id INT PRIMARY KEY,
name VARCHAR(32),
money VARCHAR(32));

INSERT INTO account VALUES (1,'jxs','10000'),(2,'dwy','15000');
2、创建Maven工程，导入依赖

<dependencies>
    <!--mysql驱动-->
    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <version>8.0.30</version>
    </dependency>

    <!--mybatis-->
    <dependency>
        <groupId>org.mybatis</groupId>
        <artifactId>mybatis</artifactId>
        <version>3.5.11</version>
    </dependency>

    <!--junit-->
    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.11</version>
        <scope>test</scope>
    </dependency>

</dependencies>
3、数据库外部配置文件

driver=com.mysql.cj.jdbc.Driver
url=jdbc:mysql://localhost:3306/spring
username=root
password=123456
4、MyBatis核心配置文件

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-config.dtd">

<!--核心配置文件-->
<configuration>

    <properties resource="database.properties"/>

    <!--环境选择-->
    <environments default="development">
        <environment id="development">
            <transactionManager type="JDBC"/>
            <dataSource type="POOLED">
                <property name="driver" value="${driver}"/>
                <property name="url" value="${url}"/>
                <property name="username" value="${username}"/>
                <property name="password" value="${password}"/>
            </dataSource>
        </environment>
    </environments>

    <mappers>
        <mapper class="dao.AccountMapper"/>
    </mappers>

</configuration>
5、数据库表对应pojo实体类

public class Account {
    private int id;
    private String name;
    private  String money;

    public Account(int id, String name, String money) {
        this.id = id;
        this.name = name;
        this.money = money;
    }

    public int getId() { return id; }
    public void setId(int id) { this.id = id; }
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    public String getMoney() { return money; }
    public void setMoney(String money) { this.money = money; }

    @Override
    public String toString() {
        return "Account{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", money='" + money + '\'' +
                '}';
    }
}
6、Mapper接口

public interface AccountMapper {
    @Select("select * from account")
    List<Account> getAccounts();
}
7、测试类

public class AccountTest {
    public static void main(String[] args) throws Exception {
        //创建SqlSessionFactoryBuilder对象实例
        SqlSessionFactoryBuilder sqlSessionFactoryBuilder = new SqlSessionFactoryBuilder();
        //加载MyBatis核心配置文件
        InputStream inputStream = Resources.getResourceAsStream("mybatis.xml");
        //创建SqlSessionFactory对象实例
        SqlSessionFactory sqlSessionFactory = sqlSessionFactoryBuilder.build(inputStream);
        //创建SqlSession对象实例
        SqlSession sqlSession = sqlSessionFactory.openSession();
        //SqlSession对象实例执行SQL语句,获取结果集accounts
        AccountMapper mapper = sqlSession.getMapper(AccountMapper.class);
        List<Account> accounts = mapper.getAccounts();
        //增强for遍历结果集
        for (Account account : accounts) {
            System.out.println(account);
        }
        sqlSession.close();
    }
}
整合MyBatis
1、概述

(1)MyBatis 与 Spring 进行整合,即将 SqlSessionFactory 对象交由 Spring IoC 容器管理。
(2)将 SqlSessionFactory 的对象生成器 SqlSessionFactoryBean 注册在 Spring IoC 容器中。
2、整合步骤

(1)创建Maven工程
(2)添加依赖
(3)MyBatis核心配置文件
(4)Spring配置文件
(5)将德鲁伊连接池数据源交由Spring管理
3、添加依赖

<dependencies>

    <!--Spring-->
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-jdbc</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>

    <!--mybatis-->
    <dependency>
        <groupId>org.mybatis</groupId>
        <artifactId>mybatis</artifactId>
        <version>3.5.11</version>
    </dependency>

    <!--mysql驱动-->
    <dependency>
        <groupId>mysql</groupId>
        <artifactId>mysql-connector-java</artifactId>
        <version>8.0.31</version>
    </dependency>

    <!--德鲁伊连接池-->
    <dependency>
        <groupId>com.alibaba</groupId>
        <artifactId>druid</artifactId>
        <version>1.2.15</version>
    </dependency>

    <!--junit-->
    <dependency>
        <groupId>junit</groupId>
        <artifactId>junit</artifactId>
        <version>4.12</version>
    </dependency>

    <!--MyBatis-Spring模块-->
    <dependency>
        <groupId>org.mybatis</groupId>
        <artifactId>mybatis-spring</artifactId>
        <version>1.3.0</version>
    </dependency>

</dependencies>
Spring配置文件中配置数据源
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="
       http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context.xsd
       ">

    <!--引入外部资源文件-->
    <context:property-placeholder location="classpath:database.properties"/>

    <!--配置德鲁伊数据源-->
    <bean id="druidDataSource" class="com.alibaba.druid.pool.DruidDataSource">
        <!--注入属性-->
        <property name="driverClassName" value="${jdbc.driver}"/>
        <property name="url" value="${jdbc.url}"/>
        <property name="username" value="${jdbc.username}"/>
        <property name="password" value="${jdbc.password}"/>
    </bean>
</beans>
注解开发注册数据源
@Configuration
@PropertySource("classpath:database.properties")
public class DataSourceConfig {
    @Value("${jdbc.driver}}")
    private String driver;
    @Value("${jdbc.url}}")
    private String url;
    @Value("${jdbc.username}}")
    private String username;
    @Value("${jdbc.password}}")
    private String password;

    @Bean
    public DataSource getDataSource() {
        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName(driver);
        druidDataSource.setUrl(url);
        druidDataSource.setUsername(username);
        druidDataSource.setPassword(password);
        return druidDataSource;
    }
}
Spring配置文件中配置SqlSessionFactory
1、MyBatis完全交由Spring管理，MyBatis核心配置文件中内容全部删除，只留下根节点

<?xml version="1.0" encoding="UTF-8" ?>
<!DOCTYPE configuration
        PUBLIC "-//mybatis.org//DTD Config 3.0//EN"
        "https://mybatis.org/dtd/mybatis-3-config.dtd">

<configuration>

</configuration>
2、Spring配置文件中配置SqlSessionFactory

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="
       http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context.xsd
       ">

    <!--引入外部资源文件-->
    <context:property-placeholder location="classpath:database.properties"/>

    <!--配置德鲁伊数据源-->
    <bean id="druidDataSource" class="com.alibaba.druid.pool.DruidDataSource">
        <!--注入属性-->
        <property name="driverClassName" value="${jdbc.driver}"/>
        <property name="url" value="${jdbc.url}"/>
        <property name="username" value="${jdbc.username}"/>
        <property name="password" value="${jdbc.password}"/>
    </bean>

    <!--配置SqlSessionFactory-->
    <bean id="sqlSessionFactory" class="org.mybatis.spring.SqlSessionFactoryBean">
        <!--注入数据源-->
        <property name="dataSource" ref="druidDataSource"/>
        <!--settings-->
        <!--别名-->
        <property name="typeAliases" value="pojo.Account"/>
        <!--注册映射文件-->
        <property name="mapperLocations" value="AccountMapper.xml"/>
    </bean>
</beans>
测试
public class AccountServiceTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new ClassPathXmlApplicationContext("spring-config.xml");
        SqlSessionFactory bean = applicationContext.getBean(SqlSessionFactory.class);
        SqlSession sqlSession = bean.openSession();
        AccountMapper mapper = sqlSession.getMapper(AccountMapper.class);
        List<Account> accounts = mapper.selectAccounts();
        for (Account account : accounts) {
            System.out.println(account);
        }
    }
}
Spring配置文件中配置代理Mapper
1、定义Mapper接口

public interface AccountMapper {
    List<Account> selectAccounts();
}
2、定义Mapper接口对应的Mapper文件

<mapper namespace="dao.AccountMapper">

    <select id="selectAccounts" resultType="pojo.Account">
        select * from account;
    </select>

</mapper>
3、将Mapper接口、Mapper文件存放同一包中且接口名、文件名一致

4、修改Spring配置文件中配置内容

<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xmlns:context="http://www.springframework.org/schema/context"
       xsi:schemaLocation="
       http://www.springframework.org/schema/beans
       http://www.springframework.org/schema/beans/spring-beans.xsd
       http://www.springframework.org/schema/context
       http://www.springframework.org/schema/context/spring-context.xsd
       ">

    <!--引入外部资源文件-->
    <context:property-placeholder location="classpath:database.properties"/>

    <!--配置德鲁伊数据源-->
    <bean id="druidDataSource" class="com.alibaba.druid.pool.DruidDataSource">
        <!--注入属性-->
        <property name="driverClassName" value="${jdbc.driver}"/>
        <property name="url" value="${jdbc.url}"/>
        <property name="username" value="${jdbc.username}"/>
        <property name="password" value="${jdbc.password}"/>
    </bean>

    <!--配置SqlSessionFactory-->
    <bean id="sqlSessionFactory" class="org.mybatis.spring.SqlSessionFactoryBean">
        <!--注入数据源-->
        <property name="dataSource" ref="druidDataSource"/>
        <!--settings-->
        <!--别名-->
        <property name="typeAliases" value="pojo.Account"/>
    </bean>

    <!--配置自动扫描的映射类-->
    <bean class="org.mybatis.spring.mapper.MapperScannerConfigurer">
        <!--注入sqlSessionFactory的id-->
        <property name="sqlSessionFactoryBeanName" value="sqlSessionFactory"/>
        <!--注入Mapper文件、Mapper接口所在包名-->
        <property name="basePackage" value="dao"/>
    </bean>
</beans>
5、代理Mapper注意事项

(1)Mapper接口、Mapper文件在同一包中
(2)Mapper文件namespace必须为接口的全限定类名
(3)Mapper接口的每个方法在Mapper文件中都必须有对应的sql语句
(4)Mapper文件sql语句的id必须与Mapper接口中的方法名一致
资源文件无法加载异常处理
1、异常

![](E:\Study\自学课程资料\Java\assets\资源文件无法加载异常处理1.png)

2、映射文件无法找到

![](E:\Study\自学课程资料\Java\assets\资源文件无法加载异常处理2.png)

3、原因

Maven工程结构中,默认所有的资源文件在src/resources目录下,当将资源文件存放在src/main/java目录下时,Maven不会将这些资源文件打包到输出目录下
4、调整方案

通过配置告知Maven将src/main/java目录下的资源文件也打包到输出目录下
5、pom.xml添加如下配置

<build>
    <!--配置Maven 对resource文件 过滤 -->
    <resources>

        <resource>
            <directory>src/main/resources</directory>
            <!--resources目录下包含的资源文件加载到classes下-->
            <includes>
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>

            <!--resources目录下排除的资源文件不加载到classes下-->
            <excludes>
            </excludes>

            <filtering>true</filtering>
        </resource>

        <resource>
            <directory>src/main/java</directory>
            <includes>
                <!--java目录下包含的资源文件加载到classes下-->
                <include>**/*.properties</include>
                <include>**/*.xml</include>
            </includes>

            <filtering>true</filtering>
        </resource>
    </resources>
</build>
注解配置代理Mapper
1、添加主配置类

@Configuration
@ComponentScan({"config"})
public class SpringConfig {
}
2、数据源配置类

@Configuration
@PropertySource(value = "classpath:spring_database.properties")
public class DataSourceConfig {
    @Value("${jdbc.driver}")
    private String driver;

    @Value("${jdbc.url}")
    private String url;

    @Value("${jdbc.username}")
    private String username;

    @Value("${jdbc.password}")
    private String password;

    @Bean
    public DataSource getDataSource() {
        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName(driver);
        druidDataSource.setUrl(url);
        druidDataSource.setUsername(username);
        druidDataSource.setPassword(password);
        return druidDataSource;
    }
}
3、MyBatis配置类

@Configuration
public class MyBatisConfig {
    @Bean
    public SqlSessionFactory getSqlSessionFactory() throws Exception {
        SqlSessionFactoryBean sqlSessionFactoryBean = new SqlSessionFactoryBean();
        sqlSessionFactoryBean.setTypeAliasesPackage("pojo");
        DataSourceConfig dataSourceConfig = new DataSourceConfig();
        sqlSessionFactoryBean.setDataSource(dataSourceConfig.getDataSource());
        return sqlSessionFactoryBean.getObject();
    }

    @Bean
    public MapperScannerConfigurer getMapperScannerConfigurer() {
        MapperScannerConfigurer mapperScannerConfigurer = new MapperScannerConfigurer();
        mapperScannerConfigurer.setBasePackage("dao");
        return mapperScannerConfigurer;
    }
}
4、测试类

public class AccountServiceTest {
    @Test
    public void testSpringMyBatisAnnotation() {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        AccountMapper bean = applicationContext.getBean(AccountMapper.class);
        List<Account> accounts = bean.selectAccounts();
        for (Account account : accounts) {
            System.out.println(account);
        }
    }
}
Spring整合JUnit
1、导入依赖

<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.12</version>
    <scope>test</scope>
</dependency>

<dependency>
    <groupId>junit</groupId>
    <artifactId>junit</artifactId>
    <version>4.12</version>
    <scope>compile</scope>
</dependency>

<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-test</artifactId>
    <version>5.2.10.RELEASE</version>
</dependency>
2、测试类

@RunWith(SpringJUnit4ClassRunner.class)
@ContextConfiguration(classes = SpringConfig.class)
public class AccountServiceTest {
    @Autowired
    private AccountService accountService;

    @Test
    public void testSave() {
        accountService.save();
    }
}
AOP
1、AOP简介

(1)AOP(Aspect Oriented Programming)面向切面编程,一种编程思想,指导开发者如何组织程序结构
(2)作用:不惊动原始设计的基础上进行功能的增强
(3)Spring理念:无入侵式编程
2、AOP核心概念

(1)连接点:程序执行过程中的任意位置,粒度为执行方法、抛出异常、设置变量等。在SpringAOP中理解为方法的执行
(2)切入点:匹配连接点的式子。在SpringAOP中,一个切入点可以只描述一个具体方法,也可匹配多个方法
(3)通知:切入点处执行的操作,即共性功能。在SpringAOP中,功能最终以方法的形式呈现。
(4)通知类:定义通知的类
(5)切面:描述通知与切入点的对应关系
AOP入门案例
1、思路分析

(1)案例设定:测定接口执行效率
(2)简化设定:接口执行前输出当前系统时间
(3)开发模式:XML 或 注解
(4)思路分析:
	导入依赖
	制作连接点方法
	制作共性功能(通知类、通知)
	定义切入点
	绑定切入点与通知关系(切面)
2、导入依赖

<dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-jdbc</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>
    
    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjweaver</artifactId>
        <version>1.9.9</version>
    </dependency>
</dependencies>
3、通知类

/*
@Component:定义通知类受Spring容器管理
@Aspect:定义通知类为切面类
 */
@Component
@Aspect
public class MyAdvice {

    //切入点,切入点依托一个不具实际意义的方法进行,既无参数、无返回值、方法体无实际逻辑
    @Pointcut("execution(void dao.BookDao.update())")
    private void pt() { }

    //通知,绑定切入点与通知关系,并指定通知添加到原始连接点的具体执行位置
    @Before("pt()")
    public void method01() {
        System.out.println(System.currentTimeMillis());
    }
}
4、Spring配置类

//@EnableAspectJAutoProxy 开启Spring对AOP注解驱动支持
@Configuration
@ComponentScan({"dao.implement","aop"})
@EnableAspectJAutoProxy
public class SpringConfig {
}
AOP工作流程
1、Spring容器启动

2、读取所有切面配置中的切入点

3、初始化bean，判定bean对应的类中的方法是否匹配到任意切入点

(1)匹配失败,创建对象
(2)匹配成功,创建原始对象的代理对象
4、获取bean执行方法

(1)获取bean,调用方法并执行,完成操作。
(2)获取bean为代理对象时,根据代理对象的运行模式运行原始方法与增强的内容,完成操作。
AOP切入点表达式
1、场景

public interface BookDao {
    void update();
}


@Repository("bookDaoImplement")
public class BookDaoImplement implements BookDao {
    @Override
    public void update() {
        System.out.println("book dao update");
    }
}
2、描述方式

(1)@Pointcut("execution(void dao.BookDao.update())")

(2)@Pointcut("execution(void dao.implement.BookDaoImplement.update())")
3、切入点表达式格式

@Pointcut("动作关键字(访问修饰符 返回值 包名.类名/接口名.方法名(参数) 异常名)")
4、通配符

(1)* :单个独立的任意符号,可以独立出现,也可作为前缀或者后缀的匹配符出现
@Pointcut("execution(public * dao.implement.*.update*())")
匹配dao.implement包下任意类以update开头的方法

(2).. :多个连续的任意符号,可独立出现,常用于简化包名与参数的书写
@Pointcut("execution(public void dao..update())")
匹配dao包下任意包中类或接口中所有名称为update的方法

(3)+ :专用于匹配子类类型
@Pointcut("execution(* *..*Dao+.*())")
匹配返回值任意、任意包下以Dao结尾的子类类型的所有方法
5、书写技巧

(1)所有代码按照标准规范开发,否则以下技巧全部失效
(2)描述切入点时通常描述接口,而不描述实现类
(3)访问修饰符针对接口开发均采用public描述
(4)返回值类型对于增删改类使用精准类型加速匹配,对于查询类使用*通配符快速描述
(5)包名书写尽量不使用..匹配,效率过低,常用*做单个包描述匹配或精准匹配
(6)接口名/类名书写名称与模块相关的采用*匹配,例如UserService书写成*Service
(7)方法名书写以动词进行精准匹配,名词采用*匹配,例如getById书写成getBy*
(8)参数规则较为复杂,根据业务方法灵活调整
(9)通常不使用异常作为匹配规则
AOP通知类型
1、基本介绍

AOP通知描述了抽取的共性功能,根据共性功能抽取的位置不同,最终运行代码时要将其加入到合理位置
2、通知类型

(1)前置通知
(2)后置通知
(3)环绕通知(重点)
(4)返回后通知(了解)
(5)抛出异常后通知(了解)
3、案例演示

/*
@Component:定义通知类受Spring容器管理
@Aspect:定义通知类为切面类
 */
@Component
@Aspect
public class MyAdvice {

    //切入点,切入点依托一个不具实际意义的方法进行,既无参数、无返回值、方法体无实际逻辑
    @Pointcut("execution(void dao.BookDao.update())")
    private void entryPoint1() { }

    @Pointcut("execution(int dao.BookDao.select())")
    private void entryPoint2() { }

    //通知,绑定切入点与通知关系,并指定通知添加到原始连接点的具体执行位置
    //@Before("entryPoint1()")
    public void method01() {
        System.out.println("before advice");
    }

    //@After("entryPoint1()")
    public void method02() {
        System.out.println("after advice");
    }

    @Around("entryPoint1()")
    public void aroundUpdate(ProceedingJoinPoint proceedingJoinPoint) {
        //原始操作前的操作
        System.out.println("around before advice");
        //表示对原始操作的使用
        try {
            proceedingJoinPoint.proceed();
        } catch (Throwable throwable) {
            System.out.println(throwable.getMessage());
        }
        //原始操作后的操作
        System.out.println("around after advice");
    }

    //@Around("entryPoint2()")
    public Object aroundSelect(ProceedingJoinPoint proceedingJoinPoint) throws Throwable {
        //原始操作前的操作
        System.out.println("around before advice");
        //表示对原始操作的使用
        Object result = proceedingJoinPoint.proceed();
        //原始操作后的操作
        System.out.println("around after advice");
        return result;
    }

    //当执行切入点时不出现异常后执行
    @AfterReturning("entryPoint2()")
    public void afterReturningSelect() {
        System.out.println("afterReturning advice");
    }

    @AfterThrowing("entryPoint2()")
    public void afterThrowingSelect() {
        System.out.println("afterThrowing advice");
    }
}
4、注意事项

(1)环绕通知必须依赖形参ProceedingJoinPoint才可实现对原始方法的调用,进而实现原始方法调用前后同时添加通知
(2)通知中若未使用ProceedingJoinPoint对原始方法进行调用将跳过原始方法的执行
(3)对原始方法的调用可不接收返回值,通知方法设置为void即可,若接收返回值必须设定为Object类型
(4)原始方法的返回值若是void类型,通知方法的返回值类型可设置为void,也可设置为Object
(5)由于无法预知原始方法运行后是否会抛出异常,因此环绕通知方法必须抛出Throwable对象
AOP案例（重要！！）
1、需求

测量业务层接口执行效率
2、导入依赖包

<dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjweaver</artifactId>
        <version>1.9.9</version>
    </dependency>
</dependencies>
3、Service接口

public interface BookService {
    void save();
}
4、Service接口实现类

/**
 * @Service:组件注册注解
 */
@Service
public class BookServiceImplement implements BookService {
    @Override
    public void save() {
        System.out.println("");
    }
}
5、开启AOP逻辑

/**
 * @Component:标注Spring管理的Bean,使用@Component注解在一个类上,表示将此类标记为Spring容器中的一个Bean。
 * @Aspect:将当前类标识为一个切面供容器读取
 */
@Component
@Aspect
public class MyAdvice {

    @Pointcut("execution(void service.BookService.save())")
    private void ServiceEntryPoint() { }

    @Around("ServiceEntryPoint()")
    public void advice01(ProceedingJoinPoint proceedingJoinPoint) throws Throwable {
        Signature signature = proceedingJoinPoint.getSignature();
        String className = signature.getDeclaringTypeName();
        String methodName = signature.getName();

        long start = System.currentTimeMillis();
        for (int i = 0; i < 10000; i++) {
            proceedingJoinPoint.proceed();
        }
        long stop = System.currentTimeMillis();
        System.out.println("万次执行" + className + "." + methodName + "花费" + (stop - start) + "ms");
    }
}
6、Spring配置类

/**
 * @Configuration:将该类作为spring的xml配置文件中的<beans>,配置spring容器
 * @ComponentScan:从约定的扫描路径中,识别标注了组件注册注解的类,并将这些类自动注册到Spring IoC容器中,这些类就是我们通常所言的bean。
 * @EnableAspectJAutoProxy:Spring AOP开启的标志,在启动类标记此注解,即可加载对应的切面类逻辑
 */
@Configuration
@ComponentScan({"service","aop"})
@EnableAspectJAutoProxy
public class SpringConfig {
}
7、测试类

public class BookServiceTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        BookService bean = applicationContext.getBean(BookService.class);
        bean.save();
    }
}
AOP通知获取数据
1、获取数据

(1)获取切入点方法的参数
	JoinPoint:适用于前置、后置、返回后、抛出异常后通知
	ProceedingJoinPoint:适用于环绕通知
(2)获取切入点方法返回值:返回后通知、环绕通知
(3)获取切入点方法运行异常信息:抛出异常后通知、环绕通知
2、导入依赖包

<dependencies>
    <dependency>
        <groupId>org.springframework</groupId>
        <artifactId>spring-context</artifactId>
        <version>5.2.10.RELEASE</version>
    </dependency>

    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjweaver</artifactId>
        <version>1.9.9</version>
    </dependency>
</dependencies>
3、Dao接口

public interface BookDao {
    String findName(int id);
}
4、Dao接口实现类

@Component
@Repository
public class BookDaoImplement implements BookDao {
    @Override
    public String findName(int id) {
        System.out.println(id);
        return "jxs";
    }
}
5、开启AOP逻辑

@Component
@Aspect
public class MyAdvice {
    @Pointcut("execution(* dao.BookDao.findName(..))")
    private void entryPoint01() {}

    //@Before("entryPoint01()")
    public void beforePoint(JoinPoint joinPoint) {
        //取参
        Object[] args = joinPoint.getArgs();
        System.out.println(Arrays.toString(args));

        System.out.println("before advice");
    }

    //@After("entryPoint01()")
    public void afterPoint(JoinPoint joinPoint) {
        //取参
        Object[] args = joinPoint.getArgs();
        System.out.println(Arrays.toString(args));

        System.out.println("after advice");
    }

    //@Around("entryPoint01()")
    public Object aroundPoint(ProceedingJoinPoint proceedingJoinPoint) throws Throwable {
        //取参
        Object[] args = proceedingJoinPoint.getArgs();
        System.out.println(Arrays.toString(args));
        //改参
        args[0] = 666;
        Object proceed = proceedingJoinPoint.proceed(args);
        return proceed;
    }

    /**
     * @param returnResult 取出返回值赋值给returnResult
     * 参数列表中JoinPoint joinPoint与Object returnResult位置不可颠倒
     */
    @AfterReturning(value = "entryPoint01()",returning = "returnResult")
    public void afterReturningPoint(JoinPoint joinPoint,Object returnResult) {
        //取参
        Object[] args = joinPoint.getArgs();
        System.out.println(Arrays.toString(args));

        System.out.println("afterReturning advice" + returnResult);
    }

    @AfterThrowing(value = "entryPoint01()",throwing = "throwable")
    public void afterThrowingPoint(Throwable throwable) {
        System.out.println("afterThrowing advice" + throwable);
    }
}
6、Spring配置类

@Configuration
@ComponentScan({"dao","aop"})
@EnableAspectJAutoProxy
public class SpringConfig {
}
7、测试类

public class BookDaoTest {
    public static void main(String[] args) {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        BookDao bookDao = applicationContext.getBean(BookDao.class);
        System.out.println(bookDao.findName(1000));
    }
}
事务
1、Spring事务简介

(1)事务作用:在数据层保障一系列的数据库操作同成功同失败
(2)Spring事务作用:在数据层或业务层保障一系列的数据库操作同成功同失败
事务案例之转账业务
案例分析
1、案例需求

(1)需求:实现任意两个账户间转账操作
(2)需求分析:
	①数据层提供基础操作,指定用户减钱、指定用户加钱
	②业务层提供转账操作,调用减钱加钱操作
	③提供两个账号和操作金额执行转账操作
	④基于Spring整合MyBatis环境搭建上述操作
2、结果分析

(1)程序正常执行时,账户金额A减B加,没有问题
(2)程序执行出现异常,转账失败,但异常之前的操作成功,异常之后的操作失败,整体业务失败
案例详解
1、数据库表对应实体类

public class Account {
    private int id;
    private String name;
    private String money;

    public Account(int id, String name, String money) {
        this.id = id;
        this.name = name;
        this.money = money;
    }

    public int getId() { return id; }
    public void setId(int id) { this.id = id; }
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    public String getMoney() { return money; }
    public void setMoney(String money) { this.money = money; }

    @Override
    public String toString() {
        return "Account{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", money='" + money + '\'' +
                '}';
    }
}
2、数据层接口

public interface AccountMapper {
    @Update("update account set money = money + #{money} where name = #{name}")
    void inMoney(@Param("name") String name, @Param("money") Double money);

    @Update("update account set money = money - #{money} where name = #{name}")
    void outMoney(@Param("name") String name, @Param("money") Double money);
}
3、业务层接口

public interface AccountService {
    /**
     * 转账操作
     * @param out   转出方
     * @param in    转入方
     * @param money 金额
     */
    @Transactional
    void transaction(String out, String in, Double money);
}
4、业务层接口实现类

@Service
public class AccountServiceImplement implements AccountService {
    @Autowired
    private AccountMapper accountMapper;

    @Override
    public void transaction(String out, String in, Double money) {
        accountMapper.inMoney(in,money);
        accountMapper.outMoney(out,money);
    }
}
5、数据源配置类

public class DataSourceConfig {
    @Bean
    public DataSource getDataSource() {
        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName("com.mysql.cj.jdbc.Driver");
        druidDataSource.setUrl("jdbc:mysql://localhost:3306/spring");
        druidDataSource.setUsername("root");
        druidDataSource.setPassword("123456");
        return druidDataSource;
    }

    @Bean
    public PlatformTransactionManager getTransactionManager(DataSource dataSource) {
        DataSourceTransactionManager transactionManager = new DataSourceTransactionManager();
        transactionManager.setDataSource(dataSource);
        return transactionManager;
    }
}
6、MyBatis配置类

public class MyBatisConfig {
    @Bean
    public SqlSessionFactory getSqlSessionFactory(DataSource dataSource) throws Exception {
        SqlSessionFactoryBean sqlSessionFactoryBean = new SqlSessionFactoryBean();
        sqlSessionFactoryBean.setTypeAliasesPackage("pojo");
        sqlSessionFactoryBean.setDataSource(dataSource);
        return sqlSessionFactoryBean.getObject();
    }

    @Bean
    public MapperScannerConfigurer getMapperScannerConfigurer() {
        MapperScannerConfigurer mapperScannerConfigurer = new MapperScannerConfigurer();
        mapperScannerConfigurer.setBasePackage("dao");
        return mapperScannerConfigurer;
    }
}
7、核心配置类

@Configuration
@ComponentScan({"config","service"})
@Import({DataSourceConfig.class,MyBatisConfig.class})
@EnableTransactionManagement
public class SpringConfig {
}
8、测试类

public class AccountServiceTest {
    @Test
    public void testSpringMyBatisAnnotation() {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        AccountService bean = applicationContext.getBean(AccountService.class);
        bean.transaction("jxs","dwy",5000.0);
    }
}
添加事务管理
1、添加事务步骤

(1)业务层接口添加事务管理注解@Transactional
(2)IoC容器中设置事务管理器的bean对象
(3)Spring配置文件开启注解式事务驱动@EnableTransactionManagement
2、添加事务注意事项

(1)Spring注解式事务通常添加在业务层接口中,而不添加在业务层接口实现类中,降低耦合。
(2)注解式事务可以添加到业务方法上表示当前方法开启事务,也可添加到接口上表示当前接口所有方法开启事务。
事务角色
1、基本介绍

(1)事务管理员:发起事务方,在Spring中通常指代业务层开启事务的方法
(2)事务协调员:加入事务方,在Spring中通常指代数据层方法,也可以是业务层方法。
事务属性
1、事务相关配置

属性	作用	示例
readOnly	设置是否为只读事务	readOnly=true 只读事务
timeout	设置事务超时时间	timeout=-1 永不超时
rollbackFor	设置事务回滚异常	rollbackFor={NullPointException.class}
rollbackForClassName	设置事务回滚异常	同上格式为字符串
noRollbackFor	设置事务不回滚异常	noRollbackFor={NullPointException.class}
noRollbackForClassName	设置事务不回滚异常	同上格式为字符串
propagation	设置事务传播行为	......
2、事务回滚注意事项

(1)默认配置中,事务中抛出异常为RuntimeException或为其子类才会回滚。
事务案例之转账业务追加日志
案例分析
1、案例需求

(1)需求:A账户减钱,B账户加钱,数据库记录日志
(2)分析:
	基于转账操作案例添加日志模块,实现数据库中记录日志
	业务层转账操作,调用减钱、加钱与日志记录功能
(3)实现效果预期:无论转账操作是否成功,均进行转账操作的日志留痕
(4)存在问题:日志的记录与转账操作隶属于同一事务,同成功同失败
(5)实现效果预期改进:无论转账操作是否成功,日志必须保留
案例详解
1、数据库表对应实体类

public class Account {
    private int id;
    private String name;
    private String money;

    public Account(int id, String name, String money) {
        this.id = id;
        this.name = name;
        this.money = money;
    }

    public int getId() { return id; }
    public void setId(int id) { this.id = id; }
    public String getName() { return name; }
    public void setName(String name) { this.name = name; }
    public String getMoney() { return money; }
    public void setMoney(String money) { this.money = money; }

    @Override
    public String toString() {
        return "Account{" +
                "id=" + id +
                ", name='" + name + '\'' +
                ", money='" + money + '\'' +
                '}';
    }
}
2、数据层接口

public interface AccountMapper {
    @Update("update account set money = money + #{money} where name = #{name}")
    void inMoney(@Param("name") String name, @Param("money") Double money);

    @Update("update account set money = money - #{money} where name = #{name}")
    void outMoney(@Param("name") String name, @Param("money") Double money);
}
public interface LogMapper {
    @Insert("insert into log (info,createTime) values (#{info},now())")
    void log(@Param("info") String info);
}
3、业务层接口

public interface AccountService {
    /**
     * 转账操作
     * @param out   转出方
     * @param in    转入方
     * @param money 金额
     */
    @Transactional
    void transaction(String out, String in, Double money);
}
public interface LogService {
    @Transactional(propagation = Propagation.REQUIRES_NEW)
    void log(String out,String in,Double money);
}
4、业务层接口实现类

@Service
public class AccountServiceImplement implements AccountService {
    @Autowired
    private AccountMapper accountMapper;

    @Autowired
    private LogService logService;

    @Override
    public void transaction(String out, String in, Double money) {
        try {
            accountMapper.inMoney(in,money);
            accountMapper.outMoney(out,money);
        } finally {
            logService.log(out,in,money);
        }
    }
}
@Service
public class LogServiceImplement implements LogService {

    @Autowired
    private LogMapper logMapper;

    @Override
    public void log(String out, String in, Double money) {
        logMapper.log(out + "转账" + money + "至" + in);
    }
}
5、数据源配置类

public class DataSourceConfig {
    @Bean
    public DataSource getDataSource() {
        DruidDataSource druidDataSource = new DruidDataSource();
        druidDataSource.setDriverClassName("com.mysql.cj.jdbc.Driver");
        druidDataSource.setUrl("jdbc:mysql://localhost:3306/spring");
        druidDataSource.setUsername("root");
        druidDataSource.setPassword("123456");
        return druidDataSource;
    }

    @Bean
    public PlatformTransactionManager getTransactionManager(DataSource dataSource) {
        DataSourceTransactionManager transactionManager = new DataSourceTransactionManager();
        transactionManager.setDataSource(dataSource);
        return transactionManager;
    }
}
6、MyBatis配置类

public class MyBatisConfig {
    @Bean
    public SqlSessionFactory getSqlSessionFactory(DataSource dataSource) throws Exception {
        SqlSessionFactoryBean sqlSessionFactoryBean = new SqlSessionFactoryBean();
        sqlSessionFactoryBean.setTypeAliasesPackage("pojo");
        sqlSessionFactoryBean.setDataSource(dataSource);
        return sqlSessionFactoryBean.getObject();
    }

    @Bean
    public MapperScannerConfigurer getMapperScannerConfigurer() {
        MapperScannerConfigurer mapperScannerConfigurer = new MapperScannerConfigurer();
        mapperScannerConfigurer.setBasePackage("dao");
        return mapperScannerConfigurer;
    }
}
7、核心配置类

@Configuration
@ComponentScan({"config","service"})
@Import({DataSourceConfig.class,MyBatisConfig.class})
@EnableTransactionManagement
public class SpringConfig {
}
8、测试类

public class AccountServiceTest {
    @Test
    public void testSpringMyBatisAnnotation() {
        ApplicationContext applicationContext = new AnnotationConfigApplicationContext(SpringConfig.class);
        AccountService bean = applicationContext.getBean(AccountService.class);
        bean.transaction("jxs", "dwy", 5000.0);
    }
}
事务传播行为
1、基本介绍

(1)事务传播行为:事务协调员对事务管理员所携带事务的处理态度
2、事务传播行为相关配置



SpringMVC
SpringMVC简介
SpringMVC概述
1、基本介绍



(1)SpringMVC技术与Servlet技术功能相同,均属于Web层开发技术
(2)SpringMVC是一种基于Java实现MVC模型的轻量级Web框架
	相比于Servlet使用更加简单、开发更加便捷
SpringMVC入门案例
1、maven创建webapp项目

2、导入依赖

<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-webmvc</artifactId>
    <version>5.2.10.RELEASE</version>
</dependency>

<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
    <version>5.2.10.RELEASE</version>
</dependency>

<dependency>
    <groupId>javax.servlet</groupId>
    <artifactId>javax.servlet-api</artifactId>
    <version>3.1.0</version>
    <scope>provided</scope>
</dependency>
3、UserController

/**
 * 使用controller定义bean
 */
@Controller
public class UserController {

    /**
     * 用户发送/select请求路径执行select方法
     * @return 响应数据
     */
    @RequestMapping("/select")
    @ResponseBody
    public String select(){
        return "{'name':'jxs'}";
    }

}
4、SpringMVC配置文件，此处使用纯注解开发

@Configuration
@ComponentScan("controller")
public class SpringMVCConfig {
}
/**
 * Servlet容器启动配置类,加载SpringMVC配置
 */
public class ServletContainerInitConfig extends AbstractDispatcherServletInitializer {
    /**
     * 加载SpringMVC容器配置
     * @return
     */
    @Override
    protected WebApplicationContext createServletApplicationContext() {
        AnnotationConfigWebApplicationContext annotationConfigWebApplicationContext
                = new AnnotationConfigWebApplicationContext();
        annotationConfigWebApplicationContext.register(SpringMVCConfig.class);
        return annotationConfigWebApplicationContext;
    }

    /**
     * 设置哪些请求归属SpringMVC处理
     * @return
     */
    @Override
    protected String[] getServletMappings() {
        return new String[]{"/"};
    }

    //加载Spring容器配置
    @Override
    protected WebApplicationContext createRootApplicationContext() {
        return null;
    }
}
5、tomcat插件配置，用于启动和管理tomcat服务器

<port>80</port>指定tomcat服务器监听端口
<path>/user</path>指定应用程序的URL路径
<build>
    <plugins>
        <plugin>
            <groupId>org.apache.tomcat.maven</groupId>
            <artifactId>tomcat7-maven-plugin</artifactId>
            <version>2.1</version>
            <configuration>
                <port>80</port>
                <path>/</path>
            </configuration>
        </plugin>
    </plugins>
</build>
6、tomcat服务器启动配置



7、总结

(1)导入SpringMVC、Servlet依赖
(2)创建SpringMVC控制器类(相当于Servlet功能)
(3)初始化SpringMVC环境(同Spring环境,设定SpringMVC加载对应的bean)
(4)初始化Servlet容器,加载SpringMVC环境
SpringMVC入门案例工作流程分析
1、启动服务器初始化过程

(1)服务器启动,执行ServletContainerInitConfig类,初始化Web容器
(2)使用createServletApplicationContext()创建WebApplicationContext对象实例
	创建AnnotationConfigWebApplicationContext对象实例
	加载SpringMVCConfig
(3)执行ComponentScan加载对应bean
(4)加载UserController,每一@RequestMapping请求路径对应一个方法
(5)执行getServletMapping方法,定义所有的请求都通过SpringMVC
2、单次请求过程

(1)浏览器输入请求路径localhost/select,发送请求
(2)web容器发现所有请求都经过SpringMVC容器,将请求交给SpringMVC处理
(3)解析请求路径/select,由请求路径匹配对应方法
(4)执行方法select()
(5)若存在@ResponseBody,直接将select方法的返回值作为响应体返回给请求方
Controller加载控制
1、基本介绍

(1)SpringMVC加载表现层bean,Spring加载逻辑层、数据层bean
	如何避免Spring加载SpringMVC管理的bean:加载Spring管理的bean时排除SpringMVC管理的bean
	SpringMVC加载的bean对应的包均在controller包内
	Spring加载的bean设定扫描范围为精准扫描,比如service包、dao包;或排除controller包
	不区分Spring与SpringMVC环境,加载到同一环境中
2、总结

(1)Spring使用过滤器过滤@Controller;SpringMVC加载@Controller
(2)不区分Spring与SpringMVC环境
3、案例演示

@Configuration
/**
 * excludeFilters:过滤器
 * type = FilterType.ANNOTATION:过滤器类型
 * classes = Controller.class:过滤的注解类型为@Controller
 */
@ComponentScan(value = "com", excludeFilters = @ComponentScan.Filter(type = FilterType.ANNOTATION, classes = Controller.class))
@Import({JDBCConfig.class, MyBatisConfig.class})
@PropertySource({"database.properties"})
public class SpringConfig {
}
(1)excludeFilters:com包下排除指定bean
(2)includeFilters:com包下包含指定bean
4、bean加载控制



更简单的解决方案:继承AbstractDispatcherServletInitializer子类AbstractAnnotationConfigDispatcherServletInitializer


PostMan
1、PostMan下载地址

https://www.postman.com/downloads/
2、PostMan用户名、密码

用户名:JXSJXS123
密码:JXSJXS123
3、PostMan中文包下载地址

https://github.com/hlmd/Postman-cn/releases
4、将PostMan中文包放至PostMan安装目录的resources目录下

请求与响应（重点：传递json数据）
请求映射路径
1、Servlet容器初始化配置类

public class ServletContainerInitConfig extends AbstractAnnotationConfigDispatcherServletInitializer {
    @Override
    protected Class<?>[] getRootConfigClasses() {
        return new Class[0];
    }

    @Override
    protected Class<?>[] getServletConfigClasses() {
        return new Class[]{SpringMVCConfig.class};
    }

    @Override
    protected String[] getServletMappings() {
        return new String[]{"/"};
    }
}
2、SpringMVC配置类

@Configuration
@ComponentScan("controller")
public class SpringMVCConfig {
}
3、Controller控制器类

@Controller
@RequestMapping("/book")
public class BookController {

    @RequestMapping("/select")
    @ResponseBody
    public String select(){
        return "jxs";
    }
}
@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/select")
    @ResponseBody
    public String select(){
        return "jxs";
    }
}
4、总结

(1)@RequestMapping:请求路径,设置在类上为当前控制器方法请求访问路径前缀
请求参数
GET请求
1、GET请求传递普通参数



@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    //普通参数
    public String select(String name,int age){
        return name + age;
    }
}
前端页面url地址传递普通参数,后端使用形参(入参)接收普通参数,形参变量名与普通参数名一致
POST请求
1、POST请求传递普通参数



form表单发送POST请求,传递普通参数,后端使用形参(入参)接收普通参数,表单普通参数名与后端形参变量名一致
2、前端页面传递普通参数后端中文乱码问题：Servlet容器初始化配置类配置过滤器

/**
 * 前端页面传递普通参数中文乱码问题
 * 设置过滤器
 * @return
 */
@Override
protected Filter[] getServletFilters() {
    CharacterEncodingFilter characterEncodingFilter = new CharacterEncodingFilter();
    characterEncodingFilter.setEncoding("utf8");
    return new Filter[]{characterEncodingFilter};
}
5种类型参数传递
1、@RequestParam注解

@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    /**
     * 前端页面传递的参数name,后端使用形参username接收
     */
    public String select(@RequestParam("name") String username, int age) {
        System.out.println(username + age);
        return username + age;
    }
}
当前端传递的参数名与后端形参变量名不一致,则使用@RequestParam注解绑定
2、前端传递的参数后端使用pojo实体类接收

/**
 * 入参
 */
public class User {
    private String name;
    private String age;

    public User() {
    }

    public User(String name, String age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getAge() {
        return age;
    }

    public void setAge(String age) {
        this.age = age;
    }

    @Override
    public String toString() {
        return "User{" +
                "name='" + name + '\'' +
                ", age='" + age + '\'' +
                '}';
    }
}
@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    public User select(User user) {
        System.out.println(user);
        return user;
    }
}
3、前端传递的参数后端使用嵌套pojo实体类接收

public class Address {
    private String province;
    private String city;

    public Address() {
    }

    public Address(String province, String city) {
        this.province = province;
        this.city = city;
    }

    public String getProvince() {
        return province;
    }

    public void setProvince(String province) {
        this.province = province;
    }

    public String getCity() {
        return city;
    }

    public void setCity(String city) {
        this.city = city;
    }

    @Override
    public String toString() {
        return "Address{" +
                "province='" + province + '\'' +
                ", city='" + city + '\'' +
                '}';
    }
}
/**
 * 入参
 */
public class User {
    private String name;
    private String age;
    private Address address;

    public User() {
    }

    public User(String name, String age, Address address) {
        this.name = name;
        this.age = age;
        this.address = address;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getAge() {
        return age;
    }

    public void setAge(String age) {
        this.age = age;
    }

    public Address getAddress() {
        return address;
    }

    public void setAddress(Address address) {
        this.address = address;
    }

    @Override
    public String toString() {
        return "User{" +
                "name='" + name + '\'' +
                ", age='" + age + '\'' +
                ", address=" + address +
                '}';
    }
}


@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    /**
     * 前端页面传递的参数name,后端使用形参username接收
     */
    public User select(User user) {
        System.out.println(user);
        return user;
    }
}
4、数组参数传递



@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    /**
     * 前端页面传递的参数name,后端使用形参username接收
     */
    public String select(@RequestParam("hobby") String[] hobbies) {
        System.out.println(Arrays.toString(hobbies));
        return Arrays.toString(hobbies);
    }
}
5、集合参数传递



@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    /**
     * 前端页面传递的参数name,后端使用形参username接收
     */
    public String select(@RequestParam List<String> hobby) {
        System.out.println(hobby);
        return "list";
    }
}
请求参数（传递json数据）
数组参数
1、依赖

<dependency>
    <groupId>com.fasterxml.jackson.core</groupId>
    <artifactId>jackson-databind</artifactId>
    <version>2.9.0</version>
</dependency>
2、SpringMVC配置类

添加@EnableWebMvc注解后可将json数据转换为对象功能
3、前端页面传递json格式数据（数组参数），后端将json格式数据转换为对象



4、UserController

@Controller
@RequestMapping("/user")
public class UserController {
    @RequestMapping("/commonParameter")
    @ResponseBody
    public String select(@RequestBody List<String> list) {
        System.out.println(list);
        return null;
    }
}
pojo参数
1、前端页面传递json格式数据（pojo参数）



2、UserController

@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    public String select(@RequestBody User user) {
        System.out.println(user);
        return null;
    }
}
集合参数
1、前端页面传递json格式数据（集合参数）

[
    {"name":"jxs","age":22},
    {"name":"dwy","age":22}
]
2、UserController

@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    public String select(@RequestBody List<User> list) {
        System.out.println(list);
        return null;
    }
}
总结
(1)EnableWebMvc
	配置类注解
	SpringMVC配置类上方定义
	将json格式数据转换为对象
(2)@RequestBody
	形参注解
	SpringMVC控制器方法形参定义前
	将请求体中包含的数据传递给形参
(3)@RequestParam与@RequestBody
	@RequestParam:接收url地址传递参数以及表单传参
	@RequestBody:接收json数据为主
日期类型参数传递
1、前端页面传递日期类型参数



2、UserController

@Controller
@RequestMapping("/user")
public class UserController {

    @RequestMapping("/commonParameter")
    @ResponseBody
    public String select(Date date01,
                         @DateTimeFormat(pattern = "yyyy-MM-dd") Date date02,
                         @DateTimeFormat(pattern = "yyyy-MM-dd HH:mm:ss") Date date03) {
        System.out.println(date01);
        System.out.println(date02);
        System.out.println(date03);
        return null;
    }
}
3、总结

(1)前端传递日期类型参数时,后端根据不同的日期格式设置不同的接收方式
(2)@DateTimeFormat注解
	形参注解
	设定日期时间类型数据格式
	属性pattern:
响应
1、响应

@Controller
public class UserController {

    /**
     * @return 响应页面
     */
    @RequestMapping("/page")
    public String toPage() {
        return "index.jsp";
    }

    /**
     * @return 将index.jsp作为响应文本
     */
    @RequestMapping("/text")
    @ResponseBody
    public String toText() {
        return "index.jsp";
    }

    /**
     * @return 响应json数据
     */
    @RequestMapping("/json")
    @ResponseBody
    public User toUser() {
        User user = new User();
        user.setName("jxs");
        user.setAge(22);
        Address address = new Address();
        address.setProvince("江苏省");
        address.setCity("泰州市");
        user.setAddress(address);
        return user;
    }

    /**
     * @return 响应pojo对象集合
     */
    @RequestMapping("/jsonList")
    @ResponseBody
    public List<User> toUserList(){
        ArrayList<User> userList = new ArrayList<User>();
        User user01 = new User();
        user01.setName("jxs");
        user01.setAge(22);

        User user02 = new User();
        user02.setName("dwy");
        user02.setAge(22);

        userList.add(user01);
        userList.add(user02);
        return userList;
    }
}
2、@ResponseBody

(1)方法注解
(2)设置当前控制器返回值作为响应体
REST风格
SSM整合
SSM整合
1、SSM整合流程

(1)创建工程
(2)SSM整合
	SpringMVC
		ServletConfig
		SpringMVCConfig
	Spring
		SpringConfig
	MyBatis
		database.properties
		JDBCConfig
		MyBatisConfig
(3)功能模块
	数据库表和数据库实体类
	controller控制层(PostMan测试)
	service逻辑层(接口+实现类)
	dao数据层(接口+自动代理)
2、pom.xml文件


表现层数据封装
异常处理器
项目异常方案处理
SSM整合标准开发
拦截器
Java面试题
设计模式
单例模式
1、单例模式基本介绍

(1)类的单例模式,采取一定的方法保证在整个软件系统中,对某个类只能存在一个对象实例,并且该类只提供一个取得其对象实例的方法(静态方法)
(2)单例模式的八种方式:
饿汉式(静态常量)
饿汉式(静态代码块)
懒汉式(线程不安全)
懒汉式(线程安全,同步方法)
懒汉式(线程安全,同步代码块)
双重检查
静态内部类
枚举
饿汉式（静态常量）
1、步骤

(1)构造器私有化(防止通过new关键字创建对象)
(2)类的内部创建对象
(3)向外暴露一个获取对象的静态公共方法(getInstance)
(4)代码实现
2、代码实现

public class SingletonTest01 {
    public static void main(String[] args) {
        Singleton instance01 = Singleton.getInstance();
        Singleton instance02 = Singleton.getInstance();
        System.out.println(instance01 == instance02);
    }
}

class Singleton {
    //1.构造器私有化,Singleton类外部不可使用new关键字创建Singleton对象实例
    private Singleton() { }

    //2.Singleton类内部创建Singleton对象实例
    private final static Singleton singleton = new Singleton();

    //3.对外提供共有的静态的getInstance方法,返回实例对象
    public static Singleton getInstance() {
        return singleton;
    }
}
3、优缺点

优点:
(1)类加载时完成实例化,避免线程同步问题

缺点:
(1)类加载时完成实例化,没有达到懒加载效果。若从始至终从未使用该实例,则会造成内存浪费
(2)此方式基于类加载机制从而避免多线程同步问题。但通过new关键字创建对象实例、调用类的静态成员或静态方法、反射都会导致类加载。
4、结论

(1)该单例模式可用,可能造成内存浪费
饿汉式(静态代码块)
1、代码实现

public class SingletonTest02 {
    public static void main(String[] args) {
        Singleton instance01 = Singleton.getInstance();
        Singleton instance02 = Singleton.getInstance();
        System.out.println(instance01 == instance02);
    }
}

class Singleton {
    //1.构造器私有化,Singleton类外部不可使用new关键字创建Singleton对象实例
    private Singleton() { }

    private final static Singleton singleton;

    //2.静态代码块中创建Singleton对象实例
    static { singleton = new Singleton(); }

    //3.对外提供共有的静态的getInstance方法,返回实例对象
    public static Singleton getInstance() {
        return singleton;
    }
}
2、优缺点

(1)此方式和上面方式类似,只不过将实例化过程放在静态代码块中。类加载时执行静态代码块中的代码。优缺点和上面的方式一致。
懒汉式(线程不安全)
1、代码实现

public class SingletonTest03 {
    public static void main(String[] args) {
        Singleton instance01 = Singleton.getInstance();
        Singleton instance02 = Singleton.getInstance();
        System.out.println(instance01 == instance02);
    }
}

class Singleton {
    private static Singleton singleton;

    //构造器私有化,防止Singleton类外部通过new关键字创建Singleton对象实例
    private Singleton() { }

    //提供一个静态的的公有方法,当调用该方法时创建Singleton对象实例,懒汉式
    public static Singleton getInstance() {
        if (singleton == null) {
            singleton = new Singleton();
        }
        return singleton;
    }
}
2、优缺点

优点:
(1)懒加载效果

缺点:
(1)只可在单线程下使用
(2)若在多线程下,一个线程进入了if判断,还未来得及往下执行,另一个线程也通过了if判断语句,此时便会产生多个实例,所以多线程环境下不可使用该方式
3、总结

(1)实际开发中不要使用这种方式
懒汉式(线程安全,同步方法)
1、代码实现

public class SingletonTest04 {
    public static void main(String[] args) {
        Singleton instance01 = Singleton.getInstance();
        Singleton instance02 = Singleton.getInstance();
        System.out.println(instance01 == instance02);
    }
}

class Singleton {
    private static Singleton singleton;

    //构造器私有化,防止Singleton类外部通过new关键字创建Singleton对象实例
    private Singleton() { }

    /*
    提供一个静态的的公有方法,当调用该方法时创建Singleton对象实例,懒汉式
    加入synchronized解决线程不安全问题
     */
    public static synchronized Singleton getInstance() {
        if (singleton == null) {
            singleton = new Singleton();
        }
        return singleton;
    }
}
2、优缺点

优点:
(1)解决线程不安全问题

缺点:
(1)效率低,每个线程获取类对象实例时执行getInstance方法都需进行同步。getInstance方法只执行一次实例化代码就足够了,后面想获得类对象实例直接return即可
3、总结

(1)实际开发中不推荐使用这种方式
双重检查
1、代码实现

public class SingletonTest05 {
    public static void main(String[] args) {
        Singleton instance01 = Singleton.getInstance();
        Singleton instance02 = Singleton.getInstance();
        System.out.println(instance01 == instance02);
    }
}

class Singleton {
    /*
    (1)volatile:轻量级的synchronized
    (2)在多线程环境下,一个线程对共享变量的操作对其他线程是不可见的。
    (3)Java提供了volatile来保证变量的可见性
    (4)一个变量被volatile关键字修饰后,当一个线程修改此变量后会立即被更新到主内存中
       其他线程读取共享变量时，会直接从主内存中读取。
     */
    private static volatile Singleton singleton;

    //构造器私有化
    private Singleton() { }

    //提供静态的公有方法,加入双重检查代码,解决线程安全问题,同时解决懒加载问题
    public static synchronized Singleton getInstance() {
        /*
        (1)A线程和B线程同时进行if判断,同时进入if代码块
        (2)A线程和B线程争夺锁,假设A线程进入同步代码块
        (3)创建Singleton对象实例,并赋值给静态变量singleton
        (4)singleton变量被volatile关键字修饰,变量修改后立即更新到主内存中
         */
        if (singleton == null) {
            synchronized (Singleton.class) {
                if (singleton == null) {
                    singleton = new Singleton();
                }
            }
        }
        return singleton;
    }
}
2、优缺点

优点:
(1)进行两次if (singleton == null)判断,保证线程安全
(2)实例化代码只需执行一次,后面再次访问时,进行第一个if (singleton == null)判断时直接return实例化对象,也避免反复进行方法同步
(3)线程安全;延迟加载;效率较高
3、总结

(1)在实际开发中推荐使用这种单例模式
工厂模式
排序算法
1、如何创建一个对象

(1)使用new关键字
(2)class类newInstance()方法
   Constructor类newInstance()方法
(3)clone()方法
(4)反序列化
2、

public class ArrayListExercise {
    public static void main(String[] args) {
        String s1 = "hello";
        StringBuilder stringBuilder = new StringBuilder(s1);
        for (int i = 0; i < 100; i++) {
            stringBuilder.append(i);
        }
        System.out.println(stringBuilder);
    }
}

创建了两个对象
3、Java中怎么将byte[] bytes转换成String？

1、String(byte[] bytes,字符集)
2、使用Base64类将字节数组转换成字符串

public class ArrayListExercise {
    public static void main(String[] args) {
        byte[] bytes = new byte[8];
        try {
            //String(byte[] bytes,字符集)
            String s1 = new String(bytes, "UTF-8");
        } catch (UnsupportedEncodingException e) {
            System.out.println(e.getMessage());
        }
        //使用Base64将字节数组转换成字符串
        String s2 = Base64.getEncoder().encodeToString(bytes);
        byte[] decode = Base64.getDecoder().decode(s2);
    }
}
4、Java中"a==b"和"a.equals(b)"的区别？

equals()方法在object类比较的两个对象的地址是否相同
若其他类重写equals()的方法,则会按照重写的规则来进行比较。
比如string类中equals()方法依次取出字符串中的字符,比较是否相同。
比如Integer类中equals()方法比较的是封装的值是否相等

==
基本数据类型:值是否相同
引用数据类型:地址是否相同
5、java中重载和重写的区别是什么？

overload(两同三不同(同一个类同一方法名 形参的个数、类型、顺序不同))

override(子类重写父类的方法(父类的方法不能被final修饰))
6、java中有两个ArrayList集合A、B，如何取这两个集合的并集，同时取出重复的元素？

public class ArrayListExercise {
    public static void main(String[] args) {
        
    }
    
    public static void removeDuplicate1(List<Integer> list) {
        //List的contains方法
        List<Integer> list3 = new ArrayList<>();
        for (Integer ele : list) {
            if (!list3.contains(ele)) {
                list3.add(ele);
            }
            list.clear();
            list.addAll(list3);
        }
    }

    public static void removeDuplicate2(List<Integer> list) {
        //双重的for循环去重
        for (int i = 0; i < list.size(); i++) {
            for (int j = 0; j < list.size(); j++) {
                if (i != j && list.get(i) == list.get(j)) {
                    list.remove(list.get(j));
                }
            }
        }
    }
}
7、排序算法

public class Sort {
    public static void main(String[] args) {
        int[] array = {1, 4, 2, 3, 6, 5, 7};
        bubbleSort(array);
        selectSort(array);
        insertSort(array);
        quickSort(array,1,6);
    }

    /**
     * 冒泡排序
     *
     * @param array
     */
    public static void bubbleSort(int[] array) {
        int temp;
        //比较的轮次
        for (int i = 0; i < array.length - 1; i++) {
            //每次比较从第一个数开始,每比较一轮产生一个极值
            for (int j = 0; j < array.length - 1 - i; j++) {
                if (array[j] > array[j + i]) {
                    //相同为0,不同为1,任何二进制数与零异或都等于其本身
                    array[j] = array[j] ^ array[j + 1];
                    /*
                    array[j + 1] = array[j] ^ array[j + 1] ^ array[j + 1] = array[j] ^ 0 = array[j]
                     */
                    array[j + 1] = array[j] ^ array[j + 1];
                    array[j] = array[j] ^ array[j + 1];
                }
            }
        }
        System.out.println(Arrays.toString(array));
    }

    /**
     * 选择排序
     * 1.首先在未排序序列中找到最小（大）元素,存放到排序序列的起始位置。
     * 2.再从剩余未排序元素中继续寻找最小（大）元素,然后放到已排序序列的末尾。
     * 3.重复第二步，直到所有元素均排序完毕。
     *
     * @param array
     */
    public static void selectSort(int[] array) {
        for (int i = 0; i < array.length - 1; i++) {
            int minIndex = i;
            for (int j = i + 1; j < array.length; j++) {
                if (array[minIndex] > array[j]) {
                    array[minIndex] = array[minIndex] ^ array[j];
                    /*
                    array[j] = array[minIndex] ^ array[j] ^ array[j] = array[minIndex] ^ 0 = array[minIndex]
                     */
                    array[j] = array[minIndex] ^ array[j];
                    array[minIndex] = array[minIndex] ^ array[j];
                }
            }
        }
        System.out.println(Arrays.toString(array));
    }

    /**
     * 插入排序
     * 1.将第一待排序序列第一个元素看做一个有序序列，把第二个元素到最后一个元素当成是未排序序列。
     * 2.从头到尾依次扫描未排序序列，将扫描到的每个元素插入有序序列的适当位置。
     * 3.如果待插入的元素与有序序列中的某个元素相等，则将待插入元素插入到相等元素的后面。
     */
    public static void insertSort(int[] array) {
        /*
        ① 从第一个元素开始，该元素可以认为已经被排序
        ② 取出下一个元素，在已经排序的元素序列中从后向前扫描
        ③如果该元素（已排序）大于新元素，将该元素移到下一位置
        ④ 重复步骤③，直到找到已排序的元素小于或者等于新元素的位置
        ⑤将新元素插入到该位置后
        ⑥ 重复步骤②~⑤
         */
        for (int i = 1; i < array.length; i++) {
            //插入的数据
            int temp = array[i];
            int j;
            for (j = i - 1; j >= 0; j--) {
                if (array[j] > temp) {
                    array[j + 1] = array[j];
                } else {
                    break;
                }
            }
            array[j + 1] = temp;
        }
        System.out.println(Arrays.toString(array));
    }

    /**
     * 快速排序
     * 1.在序列中随机选择一个数作为基准数,通常以第一个数作为基准数。
     * 2.从两端开始"探测"
     * 3.先从右往左找一个小于基准数的数,再从左往右找一个大于基准数的数,然后交换他们。
     * 4.第一轮"探测"结束
     * 5.此时以基准数为分界点,左边的数都小于等于基准数,右边的数都大于等于基准数
     * 6.左右两边各进行"探测",分别选择左右两边第一个数为基准数
     *
     * @param array
     * @param begin
     * @param end
     */
    public static void quickSort(int[] array, int begin, int end) {
        if (begin > end)
            return;
        int tmp = array[begin];
        int i = begin;
        int j = end;
        while (i != j) {
            while (array[j] >= tmp && j > i)
                j--;
            while (array[i] <= tmp && j > i)
                i++;
            if (j > i) {
                int t = array[i];
                array[i] = array[j];
                array[j] = t;
            }
        }

        array[begin] = array[i];
        array[i] = tmp;
        quickSort(array, begin, i - 1);
        quickSort(array, i + 1, end);
    }
}
8、二分查找（binarySearch）

public class Search {
    public static void main(String[] args) {
        int[] array = {1, 3, 5, 7, 9, 11, 13, 15, 17};
        System.out.println(binarySearch(array, 17));
    }

    /**
     * 初始状态下,将整个序列作为搜索区域(假设为 [begin, end])
     * 找到搜索区域内的中间元素(假设所在位置为middle)
     * 将中间元素与目标元素进行对比
     * 若相等,则搜索成功
     * 若中间元素大于目标元素,表明目标元素位于中间元素的左侧,将[begin,middle-1]作为新的搜素区域
     * 若中间元素小于目标元素,表明目标元素位于中间元素的右侧,将[middle+1,end]作为新的搜素区域
     * 重复执行,直至找到目标元素。
     * 若搜索区域无法再缩小,且区域内不包含任何元素,表明整个序列中没有目标元素,查找失败。
     *
     * @param array
     * @param key
     * @return
     */
    public static int binarySearch(int[] array, int key) {
        int low = 0;
        int high = array.length - 1;

        while (low <= high) {
            int middle = (low + high) / 2;
            if (array[middle] == key) {
                return middle;
            }
            if (array[middle] < key) {
                low = middle + 1;
            }
            if (array[middle] > key) {
                high = middle - 1;
            }
        }
        return -1;
    }
}
