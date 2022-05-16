1、String 是基本数据类型吗？

String 不是基本数据类型。

2、String 是可变的话？

String 是 final 类型的，不可变。

3、怎么比较两个字符串的值一样，怎么比较两个字符串是否同一对象？

比较字符串的值是否相同用 equals,比较字符串对象是否同一个用==。

4、switch 中可以使用 String 吗？

jdk7+中的 switch 可以使用 String 类型。

5、String str = new String("abc");创建了几个对象，为什么？

创建了两个，"abc"本身创建在常量池，通过 new 又创建在堆中。

6、String、StringBuffer、StringBuilder 有什么区别？

String、StringBuffer、StringBuilder 最大的不同是 String 不可变，后者可变。StringBuffer 是线程安全的，StringBuilder 线程不安全速度较快。

7、String.trim()方法去掉的是哪些字符？

trim 去掉字符串首尾的空白字符。

8、String 可以被子类继承吗？

既然 String 是 final 的，所以不能被继承。

9、可以自定义 java.lang.String 类并使用吗？

可以自定义 java.lang.String 类并编译成功，但不能被加载使用，具体请学习类加载机制。

10、String 与 byte[]两者相互之间如何转换？

String > byte[] 通过 String 类的 getBytes 方法；byte[] > String 通过 new String(byte[])构造器。
