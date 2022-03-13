# 数组复制

```java
 int a[] = new int[] { 18, 62, 68, 82, 65, 9 };
// copyOfRange(int[] original, int from, int to)
// 第一个参数表示源数组
// 第二个参数表示开始位置(取得到)
// 第三个参数表示结束位置(取不到)
int[] b = Arrays.copyOfRange(a, 0, 3);
```

# 转换为字符串

```java
int a[] = new int[] { 18, 62, 68, 82, 65, 9 };
System.out.println(Arrays.toString(a));
```

# 排序

```java
int a[] = new int[] { 18, 62, 68, 82, 65, 9 };
Arrays.sort(a);//排序
System.out.println(Arrays.toString(a));//将数组转换为字符串输出
```

# 搜索

```java
int a[] = new int[] { 18, 62, 68, 82, 65, 9 };
Arrays.sort(a);
//使用binarySearch之前，必须先使用sort进行排序
Arrays.binarySearch(a, 62)//在a数组的第62位
```

查询元素出现的位置

# 判断是否相同

```java
int a[] = new int[] { 18, 62, 68, 82, 65, 9 };
int b[] = new int[] { 18, 62, 68, 82, 65, 8 };
System.out.println(Arrays.equals(a, b));
```

比较两个数组的内容是否一样

# 填充

```java
Arrays.fill(a, 5);//（填充数组，填充的值）
```

使用同一个值，填充整个数组

# ArrayList

```java
ArrayList<String> a=new ArrayList<>();
ArrayList<String> b=new ArrayList<String>();//使用字符串类型数组
```

使用ArrayList这个工具