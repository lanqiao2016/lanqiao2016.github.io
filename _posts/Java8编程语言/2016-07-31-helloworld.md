---
layout: post
title: 第一个Java应用程序
category: Java8编程语言
tags: Java 入门
keywords: 蓝桥 lanqiao 教程 java Java8 开发环境
description: 
author: 付天有
importance: 4
order: 3
---

# 第一个Java应用程序：HelloWorld

开发并运行一个Java程序主要有三步：

- **编写**Java的源代码文件，以.java结尾，**源代码文件默认是不能被机器执行的**。

`特别注意，在windows上新建文本文件默认会得到一个.txt文件，需要将其改为.java后缀；如果文件名显示设置中隐藏了文件后缀，新建一个文本文件看不到后缀，但事实上有.txt后缀，如果此时仅把文件命名为***.java实际得到的文件是***.java.txt。这将导致下一个步骤的编译错误`

- 使用编译器（也就是javac命令），对源代码文件进行**编译**。把它编译成字节码文件，字节码文件是以.class结尾。它与平台无关，也就是说无论你是windows还是linux，字节码文件都是这样的一个文件，这跟系统没有关系。

- **运行**应用程序（使用java命令），在控制台我们可以看到程序运行出的结果。


看看打印单词 Hello World 的简单代码。

    public class MyFirstJavaProgram {
    
    	/* This is my first java program.  
    	 * This will print 'Hello World' as the output
    	 */
    	public static void main(String []args) {
    		System.out.println("Hello World"); // prints Hello World
    	}
    } 

看下面是如何保存文件，编译并运行该程序。请按照以下步骤进行：


- 打开记事本，并添加如上面的代码。

- 将文件另存为：MyFirstJavaProgram.java。

- 打开命令提示符窗口，然后去进入保存类的目录。假设它是C：。

- 输入'javac MyFirstJavaProgram.java“，然后按回车来编译代码。如果代码中没有错误，在命令提示符下将到下一行（假设：路径变量设置）。

- 现在，输入“java MyFirstJavaProgram'来运行程序。

- 将可以看到 ' Hello World ' 印在窗口上。

	    C : > javac MyFirstJavaProgram.java
	    C : > java MyFirstJavaProgram 
	    Hello World