+++
date = '2024-12-08T18:05:53+08:00'
title = 'My First Post'
categories = ["Java基础"]
tags = ["Java基础", "八股文"]

+++

## String、StringBuffer、StringBuilder区别
### 1.String
* **性质：不可变（Immutable）**
	
	* 一旦创建，字符串的内容无法改变。每次对String对象进行修改都会创建一个新的对象。
* **适用场景**
	* 字符串内容很少变化的场景，如字符串操作。
* **优点**
	
	* 线程安全，字符串常量池优化性能
	* 使用时简单直观
* **缺点**
	* 每次修改都会创建新对象，占用更多内存，性能较低。
* **示例**
	
	```java
	String str = "Hello";
	str += " World"; // 创建了新的字符串对象
	```
* **常用方法**
	1. **length()：**返回字符串的长度。
	2. **charAt(int index)：**返回指定索引位置的字符。
	3. **concat(String str)：**将指定的字符串连接到原字符串的末尾。
	4. **equals(Object obj)：**判断字符串是否与指定对象相等。
	5. **equalsIgnoreCase(String str)：**忽略大小写比较字符串是否相等。
	6. **isEmpty()：**判断字符串是否为空。
	7. **contains(CharSequence sequence)：**判断字符串是否包含指定的字符序列。
	8. **indexOf(String str)：**返回指定字符串在原字符串中第一次出现的位置索引。
	9. **lastIndexOf(String str)：**返回指定字符串在原字符串中最后一次出现的位置索引。
	10. **substring(int beginIndex)：**截取从指定索引开始到字符串末尾的子字符串。
	11. **substring(int beginIndex, int endIndex)：**截取指定索引范围的子字符串。
	12. **toLowerCase()：**将字符串转换为小写。
	13. **toUpperCase()：**将字符串转换为大写。
	14. **trim()：**去除字符串两端的空白字符。
	15. **split(String regex)：**根据指定的正则表达式将字符串拆分为字符串数组。
	16. **replace(char oldChar, char newChar)：**替换字符串中的字符。
	17. **startsWith(String prefix)：**判断字符串是否以指定的前缀开始。
	18. **endsWith(String suffix)：**判断字符串是否以指定的后缀结尾。



![image-20241212222045708](/three-feture.png)