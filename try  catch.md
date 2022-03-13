1.将可能抛出FileNotFoundException **文件不存在异常**的代码放在try里
2.如果文件存在，就会顺序往下执行，并且不执行catch块中的代码
\3. 如果文件不存在，try 里的代码会立即终止，程序流程会运行到对应的catch块中
\4. e.printStackTrace(); 会打印出方法的调用痕迹，如此例，会打印出异常开始于TestException的第16行，这样就便于定位和分析到底哪里出了异常

error类异常 大多数与编写者无关

Runtime Exception(运行时异常)

```java
File f=new File("E://CF"); 
try {
       new FileInputStream(f);
        }catch (FileNotFoundException e){
e.printStackTrace();
        }
```

FileNotFoundException是Exception的子类，

使用Exception也可以catch住FileNotFoundException

# 单一异常处理

```java
 try{
      System.out.println("试图打开 d:/LOL.exe");
      new FileInputStream(f);
     System.out.println("成功打开");
    }
    
    catch(Exception e){
  System.out.println("d:/LOL.exe不存在");
      e.printStackTrace();
    }
```

# 多异常捕捉办法1

分别进行catch

```java
//new FileInputStream(f);
//Date d = sdf.parse("2016-06-03");
//会抛出 文件不存在异常 FileNotFoundException 和 解析异常ParseException
 try{ System.out.println("试图打开 d:/LOL.exe");
new FileInputStream(f);
System.out.println("成功打开");
SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd");
Date d = sdf.parse("2016-06-03");
}catch (FileNotFoundException e) {
    System.out.println("d:/LOL.exe不存在");
    e.printStackTrace();
} catch (ParseException e) {
    System.out.println("日期格式解析错误");
    e.printStackTrace();
}
```

# 多异常捕捉办法2

放在一个catch里统一捕捉

```java
 try{ System.out.println("试图打开 d:/LOL.exe");
new FileInputStream(f);
System.out.println("成功打开");
SimpleDateFormat sdf = new SimpleDateFormat("yyyy-MM-dd");
Date d = sdf.parse("2016-06-03");
}catch (FileNotFoundException | ParseException e) {
            if (e instanceof FileNotFoundException)
                System.out.println("d:/LOL.exe不存在");
            if (e instanceof ParseException)
                System.out.println("日期格式解析错误");
 
            e.printStackTrace();
}
 
```

# finally

无论是否出现异常，finally中的代码都会被执行

```java
finally{
            System.out.println("无论文件是否存在， 都会执行的代码");
        }
```

# throws

```java
public static void main(String[] args) {
		method1();
	}
	private static void method1() {
		try {
			method2();
		} catch (FileNotFoundException e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
	}
	private static void method2() throws FileNotFoundException {
		File f = new File("d:/LOL.exe");
		System.out.println("试图打开 d:/LOL.exe");
		new FileInputStream(f);
		System.out.println("成功打开");
	}
```

主方法调用method1
method1调用method2
method2中打开文件

method2中需要进行异常处理

那么method1就会**接到该异常**。 处理办法也是两种，要么是try catch处理掉，要么也是**抛出去**。
method1选择本地try catch住 一旦try catch住了，就相当于把这个异常消化掉了，主方法在调用method1的时候，就不需要进行异常处理了