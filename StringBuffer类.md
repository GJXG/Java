StringBuffer是可变长的字符串

```Java
String str = "let there ";
StringBuffer s=new StringBuffer(str);//创建一个StringBuffer对象
```

# append追加

```java
s.append("fly");//在最后追加
```

# delete 删除

```java
s.delete(9,10);//删除9-10之间的字符
```

# insert 插入

```java
s.insert(9," ");//在9处插入字符
```

# reverse 反转

```java
s.reverse();//反转字符串
```

# 长度

```java
 System.out.println(str.length());//内容长度
```

# 容量

```java
System.out.println(str.capacity());//总空间
```

