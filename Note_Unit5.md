# Note——Unit5

-1.ClassLoader:ClassLoader是JVM实现的一部分，ClassLoader包括bootstrap classloader。ClassLoader在JVM运行的时候夹在Java核心的API,其中还包括用户定义的CLassLoader。用户定义的ClassLoader指ExtClassLoader(用于加载/lib/ext中的类)和AppClassLoader(用于加载用户机器上CLASSPATH设置目录中的类，用户自定义的类)。  

-
-2.面向字节的IO(不做编码转换)和面向字符的IO(做编码转换)，Java中的所有字符都是使用Unicode。

-
-3.i++

static语句块，会在类被加载的时候执行且仅会被执行一次，一般用来初始化静态变量和调用静态方法。  
i=0; i = i++ + ++i;  可以得到i = 2。

-
-4.类型的转换

包装类(Boolean,Character,Integer,Long,Float,Double).

Character.getNumericValue(char c); ...等等方法

-
-5.程序结构   
assert(断言)用于验证传递给私有方法的参数  
main函数必须是public属性的

-
-6.运算符

((a < 5)? 10.9:9) 此时9会自动转换为double类型=>9.0   
两个表达式有一个是常量表达式时,另外一个类型是T,而常量表达式可以被T表示时,输出结果就是T类型的。  
&&和||是短路运算，&和|是非短路运算。  
\>>位移运算:(num >> 32) == (num >> 0) 因为右边的参数要先进行模的32运算。  

-
-7.异常  
一个合理的应用程序不应该捕捉运行时异常。  
运行错误可以分为两类(错误和异常),错误有死循环,内存泄漏(程序运行时本身无法解决，可以通过其他程序干预),异常常见的有数组下标越界,算法溢出,除数为零(程序运行时不可解决)。  
...关于Java异常参考书

-
-8.final/finally/finalize  
final可以用于控制成员、方法或者是一个类能否被覆写或继承。  
finally关键字是Java异常处理模型的最佳补充。  
finalize用来释放资源。  
详见书本。  

-
-9.反射   

 


